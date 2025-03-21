# The Veras Website
Public details for the private client- and server-side repositories for https://the-veras.web.app/

The client-side repository was templated off of my other public repo [Reusable Site Template](https://github.com/aorlanes/Reusable-Site-Template). These projects were used to create the client- and server- side repositories for my wedding/engagement [website](https://the-veras.web.app). This project consists of a multi-page dynamic website that communicates to a server for read and write operations. The server-side project is in a separate repository. Both client- and server-side repositories are private. If you would like to see those repos, please contact me directly.

## Architecture

### Client:
The client architecture is organized by site main pages, custom reusable components, assets, firebase utilities, entities (Typescript purposes) and custom hooks. Within the main page folders should be modules associated with the respective page. Controlled environment variables are also used for dev and prod.

### Server:
The server caters to a RESTful and CRUD architectural style. Because the project uses Google Cloud Functions, the whole project sits within the `functions` folder. The rest of the project is organized by controller and respective services. Controlled environment variables are also used for dev and prod.

## Future Goals

A lot more goals for this project, in terms of efficiencies and exploring/learning supplemental services. The only limitation is costs ($), as this is a personal project that has no intention of targeting a large audience. Most services used are free or have a free tier.

## Tech Stacks, Services, and Dependencies Used

### Client:
- Typescript
- [React](https://react.dev/), with use of hooks
- [Firebase tools](https://firebase.google.com/) (client-side)
  - Google Analytics
  - Hosting
- [Axios](https://axios-http.com/) (HTTP requests)
- [Material UI](https://mui.com/material-ui/)
- [Add to Calendar](https://add-to-calendar-button.com/)
- [Webpack](https://webpack.js.org/) (module bundler)
- [Stripe](https://stripe.com/) (payments handler)
- Local browser storage (technically not a service since its apart of the Javasript window, but still an important utility that's used)

### Server:
- Javascript
- [Node.js](https://nodejs.org/en/)
- [Express](https://expressjs.com/) (API handling and Node framework)
- [Cors](https://www.npmjs.com/package/cors) (Origin handling)
- [Dotenvx](https://dotenvx.com/) ("dotenv but better", environment and encrytpion handling)
- [Firebase tools](https://firebase.google.com/) (server-side)
  - Firestore
  - Cloud Functions
