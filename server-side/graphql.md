# GraphQL



* * * [Architecture](https://hasura.io/learn/graphql/nextjs-fullstack-serverless/intro-to-graphql/1-architecture/)
    * [Fetching data - Queries](https://hasura.io/learn/graphql/nextjs-fullstack-serverless/intro-to-graphql/2-fetching-data-queries/)
    * [Writing data - Mutations](https://hasura.io/learn/graphql/nextjs-fullstack-serverless/intro-to-graphql/3-writing-data-mutations/)
    * [Watching data - Subscriptions](https://hasura.io/learn/graphql/nextjs-fullstack-serverless/intro-to-graphql/4-watching-data-subscriptions/)
  * [Hasura Backend Setup](https://hasura.io/learn/graphql/nextjs-fullstack-serverless/hasura-backend/)
  * [Auth0 Setup](https://hasura.io/learn/graphql/nextjs-fullstack-serverless/auth0-setup/)
    * [Custom Claims in Auth0 Rules](https://hasura.io/learn/graphql/nextjs-fullstack-serverless/auth0-setup/1-custom-claims/)
    * [Connect Hasura with Auth0](https://hasura.io/learn/graphql/nextjs-fullstack-serverless/auth0-setup/2-connect-hasura-auth0/)
    * [Sync Users with Rules](https://hasura.io/learn/graphql/nextjs-fullstack-serverless/auth0-setup/3-user-sync-rule/)
  * [Next.js Boilerplate Setup](https://hasura.io/learn/graphql/nextjs-fullstack-serverless/setup/)
  * [Configure Apollo Client with Next.js](https://hasura.io/learn/graphql/nextjs-fullstack-serverless/apollo-client/)
  * [Queries](https://hasura.io/learn/graphql/nextjs-fullstack-serverless/queries/)
    * [Fetch todos - query](https://hasura.io/learn/graphql/nextjs-fullstack-serverless/queries/1-fetch-todos-query/)
    * [useQuery hook](https://hasura.io/learn/graphql/nextjs-fullstack-serverless/queries/2-create-query/)
    * [Handle loading/errors](https://hasura.io/learn/graphql/nextjs-fullstack-serverless/queries/3-handle-errors/)
  * [Mutations & Query variables](https://hasura.io/learn/graphql/nextjs-fullstack-serverless/mutations-variables/)
    * [Create todos - mutation](https://hasura.io/learn/graphql/nextjs-fullstack-serverless/mutations-variables/1-create-todo/)
    * [Query Variables](https://hasura.io/learn/graphql/nextjs-fullstack-serverless/mutations-variables/2-query-variables/)
    * [useMutation Hook, Update Cache](https://hasura.io/learn/graphql/nextjs-fullstack-serverless/mutations-variables/3-create-mutation/)
  * [Optimistic UI](https://hasura.io/learn/graphql/nextjs-fullstack-serverless/optimistic-update-mutations/)
    * [Update todos - mutation](https://hasura.io/learn/graphql/nextjs-fullstack-serverless/optimistic-update-mutations/1-update-todos/)
    * [Mutation and update cache](https://hasura.io/learn/graphql/nextjs-fullstack-serverless/optimistic-update-mutations/2-mutation-cache/)
    * [Remove todos - mutation](https://hasura.io/learn/graphql/nextjs-fullstack-serverless/optimistic-update-mutations/3-remove-todos/)
    * [Mutation and update cache](https://hasura.io/learn/graphql/nextjs-fullstack-serverless/optimistic-update-mutations/3.1-mutation-update-cache/)
    * [Bulk delete todos - mutation](https://hasura.io/learn/graphql/nextjs-fullstack-serverless/optimistic-update-mutations/3.2-bulk-delete-mutation/)
    * [Mutation and update cache](https://hasura.io/learn/graphql/nextjs-fullstack-serverless/optimistic-update-mutations/3.3-clear-completed/)
  * [Subscriptions to show online users](https://hasura.io/learn/graphql/nextjs-fullstack-serverless/subscriptions/)
    * [Apollo useSubscription React hook](https://hasura.io/learn/graphql/nextjs-fullstack-serverless/subscriptions/1-apollo-subscription/)
    * [Create Subscription and Render Result](https://hasura.io/learn/graphql/nextjs-fullstack-serverless/subscriptions/2-create-subscription/)
  * [Realtime Feed](https://hasura.io/learn/graphql/nextjs-fullstack-serverless/realtime-feed/)
    * [Fetch public todos - subscription](https://hasura.io/learn/graphql/nextjs-fullstack-serverless/realtime-feed/1-fetch-public/)
    * [Sync new todos](https://hasura.io/learn/graphql/nextjs-fullstack-serverless/realtime-feed/2-sync-todo/)
  * [Deployment](https://hasura.io/learn/graphql/nextjs-fullstack-serverless/deployment/)
  * [What next?](https://hasura.io/learn/graphql/nextjs-fullstack-serverless/what-next/)
* * [Hasura Docs](https://hasura.io/docs/latest/graphql/core/index.html)
* [GraphQL API](https://hasura.io/graphql/)

## Intro to GraphQL

[![Github logo](data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0idXRmLTgiPz4NCjwhLS0gR2VuZXJhdG9yOiBBZG9iZSBJbGx1c3RyYXRvciAyMi4xLjAsIFNWRyBFeHBvcnQgUGx1Zy1JbiAuIFNWRyBWZXJzaW9uOiA2LjAwIEJ1aWxkIDApICAtLT4NCjxzdmcgdmVyc2lvbj0iMS4yIiBiYXNlUHJvZmlsZT0idGlueSIgaWQ9IkxheWVyXzEiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyIgeG1sbnM6eGxpbms9Imh0dHA6Ly93d3cudzMub3JnLzE5OTkveGxpbmsiDQoJIHg9IjBweCIgeT0iMHB4IiB2aWV3Qm94PSIwIDAgMjM1MCAyMzE0LjgiIHhtbDpzcGFjZT0icHJlc2VydmUiPg0KPHBhdGggZD0iTTExNzUsMEM1MjUuOCwwLDAsNTI1LjgsMCwxMTc1YzAsNTUyLjIsMzc4LjksMTAxMC41LDg5MC4xLDExMzkuN2MtNS45LTE0LjctOC44LTM1LjMtOC44LTU1Ljh2LTE5OS44SDczNC40DQoJYy03OS4zLDAtMTUyLjgtMzUuMi0xODUuMS05OS45Yy0zOC4yLTcwLjUtNDQuMS0xNzkuMi0xNDEtMjQ2LjhjLTI5LjQtMjMuNS01LjktNDcsMjYuNC00NC4xYzYxLjcsMTcuNiwxMTEuNiw1OC44LDE1OC42LDEyMC40DQoJYzQ3LDYxLjcsNjcuNiw3Ni40LDE1NS43LDc2LjRjNDEuMSwwLDEwNS43LTIuOSwxNjQuNS0xMS44YzMyLjMtODIuMyw4OC4xLTE1NS43LDE1NS43LTE5MC45Yy0zOTMuNi00Ny01ODEuNi0yNDAuOS01ODEuNi01MDUuMw0KCWMwLTExNC42LDQ5LjktMjIzLjMsMTMyLjItMzE3LjNjLTI2LjQtOTEuMS02MS43LTI3OS4xLDExLjgtMzUyLjVjMTc2LjMsMCwyODIsMTE0LjYsMzA4LjQsMTQzLjljODguMS0yOS40LDE4NS4xLTQ3LDI4NC45LTQ3DQoJYzEwMi44LDAsMTk2LjgsMTcuNiwyODQuOSw0N2MyNi40LTI5LjQsMTMyLjItMTQzLjksMzA4LjQtMTQzLjljNzAuNSw3MC41LDM4LjIsMjYxLjQsOC44LDM1Mi41YzgyLjMsOTEuMSwxMjkuMywyMDIuNywxMjkuMywzMTcuMw0KCWMwLDI2NC40LTE4NS4xLDQ1OC4zLTU3NS43LDQ5OS40YzEwOC43LDU1LjgsMTg1LjEsMjE0LjQsMTg1LjEsMzMxLjlWMjI1NmMwLDguOC0yLjksMTcuNi0yLjksMjYuNA0KCUMyMDIxLDIxMjMuOCwyMzUwLDE2ODkuMSwyMzUwLDExNzVDMjM1MCw1MjUuOCwxODI0LjIsMCwxMTc1LDBMMTE3NSwweiIvPg0KPC9zdmc+DQo=)Edit on GitHub](https://github.com/hasura/learn-graphql/tree/master/tutorials/frontend/nextjs/tutorial-site/content/intro-to-graphql.md)

### What is GraphQL? <a id="whatisgraphql?"></a>

GraphQL is a specification for how to talk to an API. It's typically used over HTTP where the key idea is to `POST` a "query" to an HTTP endpoint, instead of hitting different HTTP endpoints for different resources.

GraphQL is designed for developers of web/mobile apps \(HTTP clients\) to be able to make API calls to fetch the data they need from their backend APIs conveniently.

### GraphQL vs REST: an example <a id="graphqlvsrest:anexample"></a>

Let's say you have an API to fetch a user's profile and their address. In a typical REST scenario, this is what the request/response would look like:

![GraphQL API example](https://graphql-engine-cdn.hasura.io/learn-hasura/assets/graphql-react/rest-api.png)

If your API server was a GraphQL server instead, this is what your API calls would look like:

![GraphQL API example](https://graphql-engine-cdn.hasura.io/learn-hasura/assets/graphql-react/graphql-api.gif)

You can see that the response JSON is different for different "queries" sent by the client.

```text
Request1:         |  Response1:query {           |  {  user (id: 1) {  |    "user": {    id            |       "id": 1  }               |     }}                 |  }----------------------------------------Request2:         |   Response2:query {           |   {  user (id: 1) {  |     "user": {    id            |       "id": 1    name          |       "name": "Elmo"  }               |     }}                 |   }
```

### Thinking in GraphQL <a id="thinkingingraphql"></a>

We're changing the way we think about API calls. Instead of making different API calls to different URLs to fetch data, we're making ad-hoc queries to a "single URL endpoint" that returns data based on the query.

* Instead of 'GET'ing a resource you 'POST' a query that describes what data you want.
* You think of the data your API returns as a "graph", this allows you to make queries to fetch "related" pieces of data in a single shot. In the example above, you fetch the user and the user's address \(as a nested JSON object\) in the same API call, as opposed to making 2 API calls.
* The "query" you send as data in the POST request has a structure and a syntax. This "language" is called GraphQL.

As you can see in the example above, GraphQL queries look very neat and easy to read! This is because the query is the "shape" of the final JSON data you desire. This is one of the key-reasons that makes GraphQL a joy to work with!

### GraphQL benefits <a id="graphqlbenefits"></a>

* **Avoid over-fetching**: You avoid fetching more data than you need because you can specify the exact **fields** you need.
* **Prevent multiple API calls**: In case you need more data, you can also avoid making multiple calls to your API. In the case above, you don't need to make 2 API calls to fetch `user` and `address` separately.
* **Lesser communication with API developers**: Sometimes to fetch the exact data you need, especially if you need to fetch more data and want to avoid multiple API calls, you will need to ask your API developers to build a new API. With GraphQL, your work is _independent_ of the API team! This allows you to work faster on your app.
* **Self-documenting**: Every GraphQL API conforms to a "schema" which is the graph data model and what kinds of queries a client can make. This allows the community to build lots of cool tools to explore & visualise your API or create IDE plugins that autocomplete your GraphQL queries and even do "codegen". We'll understand this in more detail later!

Here's a quick chart to show you the GraphQL analogs of typical REST-ish terms:

| Requirement | REST | GraphQL |
| :--- | :--- | :--- |
| Fetching data objects | GET | query |
| Writing data | POST | mutation |
| Updating/deleting data | PUT/PATCH/DELETE | mutation |
| Watching/subscribing to data | - | subscription |







## Architecture

[![Github logo](data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0idXRmLTgiPz4NCjwhLS0gR2VuZXJhdG9yOiBBZG9iZSBJbGx1c3RyYXRvciAyMi4xLjAsIFNWRyBFeHBvcnQgUGx1Zy1JbiAuIFNWRyBWZXJzaW9uOiA2LjAwIEJ1aWxkIDApICAtLT4NCjxzdmcgdmVyc2lvbj0iMS4yIiBiYXNlUHJvZmlsZT0idGlueSIgaWQ9IkxheWVyXzEiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyIgeG1sbnM6eGxpbms9Imh0dHA6Ly93d3cudzMub3JnLzE5OTkveGxpbmsiDQoJIHg9IjBweCIgeT0iMHB4IiB2aWV3Qm94PSIwIDAgMjM1MCAyMzE0LjgiIHhtbDpzcGFjZT0icHJlc2VydmUiPg0KPHBhdGggZD0iTTExNzUsMEM1MjUuOCwwLDAsNTI1LjgsMCwxMTc1YzAsNTUyLjIsMzc4LjksMTAxMC41LDg5MC4xLDExMzkuN2MtNS45LTE0LjctOC44LTM1LjMtOC44LTU1Ljh2LTE5OS44SDczNC40DQoJYy03OS4zLDAtMTUyLjgtMzUuMi0xODUuMS05OS45Yy0zOC4yLTcwLjUtNDQuMS0xNzkuMi0xNDEtMjQ2LjhjLTI5LjQtMjMuNS01LjktNDcsMjYuNC00NC4xYzYxLjcsMTcuNiwxMTEuNiw1OC44LDE1OC42LDEyMC40DQoJYzQ3LDYxLjcsNjcuNiw3Ni40LDE1NS43LDc2LjRjNDEuMSwwLDEwNS43LTIuOSwxNjQuNS0xMS44YzMyLjMtODIuMyw4OC4xLTE1NS43LDE1NS43LTE5MC45Yy0zOTMuNi00Ny01ODEuNi0yNDAuOS01ODEuNi01MDUuMw0KCWMwLTExNC42LDQ5LjktMjIzLjMsMTMyLjItMzE3LjNjLTI2LjQtOTEuMS02MS43LTI3OS4xLDExLjgtMzUyLjVjMTc2LjMsMCwyODIsMTE0LjYsMzA4LjQsMTQzLjljODguMS0yOS40LDE4NS4xLTQ3LDI4NC45LTQ3DQoJYzEwMi44LDAsMTk2LjgsMTcuNiwyODQuOSw0N2MyNi40LTI5LjQsMTMyLjItMTQzLjksMzA4LjQtMTQzLjljNzAuNSw3MC41LDM4LjIsMjYxLjQsOC44LDM1Mi41YzgyLjMsOTEuMSwxMjkuMywyMDIuNywxMjkuMywzMTcuMw0KCWMwLDI2NC40LTE4NS4xLDQ1OC4zLTU3NS43LDQ5OS40YzEwOC43LDU1LjgsMTg1LjEsMjE0LjQsMTg1LjEsMzMxLjlWMjI1NmMwLDguOC0yLjksMTcuNi0yLjksMjYuNA0KCUMyMDIxLDIxMjMuOCwyMzUwLDE2ODkuMSwyMzUwLDExNzVDMjM1MCw1MjUuOCwxODI0LjIsMCwxMTc1LDBMMTE3NSwweiIvPg0KPC9zdmc+DQo=)](https://github.com/hasura/learn-graphql/tree/master/tutorials/frontend/nextjs/tutorial-site/content/intro-to-graphql/1-architecture.md)Before going further in understanding GraphQL, it's useful to get a sense of how GraphQL is actually used in an HTTP client \(typically a web/mobile app\).

### GraphQL over HTTP <a id="graphqloverhttp"></a>

Check out the diagram below, to get a sense of how GraphQL is typically used in your stack:

![GraphQL over HTTP](https://graphql-engine-cdn.hasura.io/learn-hasura/assets/graphql-react/graphql-on-http.png)

#### GraphQL client-server flow: <a id="graphqlclient-serverflow:"></a>

1. Note that the GraphQL query is not really JSON; it looks like the shape of the JSON you _want_. So when we make a 'POST' request to send our GraphQL query to the server, it is sent as a "string" by the client.
2. The server gets the JSON object and extracts the query string. As per the GraphQL syntax and the graph data model \(GraphQL schema\), the server processes and validates the GraphQL query.
3. Just like a typical API server, the GraphQL API server then makes calls to a database or other services to fetch the data that the client requested.
4. The server then takes the data and returns it to the client in a JSON object.

#### Example GraphQL client setup: <a id="examplegraphqlclientsetup:"></a>

In your day to day work, you don't actually need to worry about the underlying HTTP requests & responses.

Just like when you work with a REST API and use a HTTP client to reduce the boilerplate in making API calls and handling responses, you can choose a GraphQL client to make writing GraphQL queries, sending them and handling responses much easier.

In fact, the mechanism of how you send the GraphQL query and accept the GraphQL response has become standard. This makes working with GraphQL very easy on the client.

Here's what a typical GraphQL client setup and making a query would look like:

```text
// Setup a GraphQL client to use the endpointconst client = new client("https://myapi.com/graphql");// Now, send your query as a string (Note that ` is used to create a multi-line// string in javascript).client.query(`  query {    user {      id      name    }  }`);
```

