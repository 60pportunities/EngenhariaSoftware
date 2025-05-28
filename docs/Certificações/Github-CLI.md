- [ ] gh api graphql -H X-Github-Next-Global-ID:1 -f query=' query { viewer { login name bio } } '
gh api graphql -H X-Github-Next-Global-ID:1 -f query=' query($owner:String!, $repo:String!) { repository(owner:$owner, name:$repo) { name description id stargazerCount forkCount issues(states:OPEN) { totalCount } } } ' -F owner=horaciovasconcellos -F repo=estudo-actions
gh api graphql -f query='
{
  user(login: "horaciovasconcellos") {
    repositories(first: 100, orderBy: {field: NAME, direction: ASC}) {
      nodes {
        name
      }
    }
  }
}'

gh api graphql -f query='
{
  user(login: "horaciovasconcellos") {
    repositories(first: 100) {
      nodes {
        id
        name
        nameWithOwner
        url
        description
        createdAt
        updatedAt
        pushedAt
        stargazerCount
        watchers {
          totalCount
        }
        primaryLanguage {
          name
        }
        forkCount
        issues(states: OPEN) {
          totalCount
        }
        licenseInfo {
          name
        }
        defaultBranchRef {
          name
        }
        owner {
          login
          avatarUrl
        }
      }
    }
  }
}'


gh api graphql -H X-Github-Next-Global-ID:1 -f query='
  mutation($repositoryId:ID!, $title:String!, $body:String) {
    createIssue(input:{repositoryId:$repositoryId, title:$title, body:$body}) {
      issue {
        url
        number
        title
        body
        state
      }
    }
  }
' -F repositoryId="R_kgDOABPHjQ" -F title="Creating issue with GraphQL" -F body="Issue body created via GraphQL\!"

gh api graphql -H X-Github-Next-Global-ID:1 -f query=' query($owner:String!, $repo:String!) { repository(owner:$owner, name:$repo) { issues(first:3, states:OPEN) { nodes { number title url } } } } ' -F owner=horaciovasconcellos -F repo=estudo-action —jq '.data.repository.issues.nodes[]'

 -F repo=estudo-actions

gh api graphql --paginate -H X-Github-Next-Global-ID:1 -f query=' query($owner:String!, $repo:String!, $endCursor:String) { repository(owner:$owner, name:$repo) { issues(first:100, after:$endCursor, states:OPEN, orderBy:{field:CREATED_AT, direction:DESC}) { pageInfo { hasNextPage endCursor } nodes { number title createdAt } } } } ' -F owner=horaciovasconcellos -F repo=estudo-actions

https://cli.github.com/manual/gh_api
