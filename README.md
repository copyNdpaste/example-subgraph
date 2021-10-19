# init
* login to thegraph, create subgraph
* `yarn global add @graphprotocol/graph-cli`
* `graph init --from-example copyNdpaste/example-subgraph` on root dir
* `graph auth` enter deploy key

# setup
* `cd example-subgraph`
* `graph codegen && graph build`
* `graph deploy --studio gravatar`

* query on https://thegraph.com/studio/subgraph/gravatar/ after SYNCING
```
{
  gravatars(first: 5) {
    id
    owner
    displayName
    imageUrl
  }
}
```
