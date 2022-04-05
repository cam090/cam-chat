# cam-chat
Fully functioning realtime chat application that uses React, Apollo, GraphQL subscriptions, web sockets, and Module Federation.

**How it works**
1) Start the server using _yarn start_
2) Go to localhost:8080
3) Type name and a message in the chat box - press enter to submit
4) Open a new tab or window and type in a new name and new message then submit
5) Now you should be able to see two users having a conversation with each other :)
6) You can even add a third user...

**Tech stack**
 - [React](https://reactjs.org/) is used to create the chat app interface.
 - [GraphQL](https://graphql.org/) is used to read and write messages.
 - [Apollo Client](https://www.apollographql.com/docs/) is used to create the React app that uses subscriptions to connect to the server. Apollo uses [WebSocket](https://developer.mozilla.org/en-US/docs/Web/API/WebSocket) to implement subscriptions. Unlike the conventional POST method, a subscription query performs the query over the WebSocket endpoint, and the subscription listens for data pushed from the server via the WebSocket. In short, updated results are pushed from the server to the subscribed clients.
 - [Module Federation](https://webpack.js.org/concepts/module-federation/) is then used to share the chat component with another application, turning the app into a 'live chat'. Module Federation allows the loading of seperately compiled applications at runtime and sharing of common dependencies. In turn, this allows sharing of common data, which in this case is the chat.
 - [graphql-yoga](https://www.graphql-yoga.com/docs/quick-start) is a GraphQL starterkit used to create the GraphQL server.
 - [Shards React](https://designrevision.com/docs/shards-react/getting-started) is a component library used.


<img width="1435" alt="Screenshot 2022-04-02 at 18 40 48" src="https://user-images.githubusercontent.com/43217221/161394796-290a2095-783a-4854-b12d-a59bf72e2eab.png">
