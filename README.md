# sourcegraph

Sourcegraph makes it easy to read, write, and fix code—even in big, complex codebases.

- Code search: Search all of your repositories across all branches and all code hosts.
- Code intelligence: Navigate code, find references, see code owners, trace history, and more.
- Fix and refactor: Roll out large-scale changes to many repositories at once and track big migrations.

## Install

Install from the [Official Site](https://docs.sourcegraph.com/cli/explanations/versioning#installation-linux). **OR**

### Script installation(Recommendation)

```
git clone https://github.com/ShubhamKumar89/sourcegraph
cd sourcegraph/
chmod 777 sourcegraph
./sourcegraph
```

Opens at [localhost:3080](http://localhost:3080/).

## Github Template(Basic)

```
{
  "url": "https://github.com",
  "token": "<personal access token>",
  "orgs": ["organisation"],
  "repos": [
    "organisation/repository"
  ]
}
```

** Example**

```
{
  "url": "https://github.com",
  "token": "ACCESS_TOKEN",
  "orgs": ["kubernetes"],
  "repos": [
    "kubernetes/kubernetes"
  ]
}
```

`repos` - A list of repositories in owner/name format. The order determines the order in which we sync repository metadata and is safe to change.

`orgs` - A list of organizations (every repository belonging to the organization will be cloned).
