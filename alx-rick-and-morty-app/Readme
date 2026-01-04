# Rick and Morty App with Next.js and Apollo Client

## Project Overview

This is a Next.js application built with TypeScript, ESLint, and Tailwind CSS that integrates with the Rick and Morty GraphQL API using Apollo Client.

## Setup Instructions

### Prerequisites
- Node.js (v18 or higher)
- npm

### Installation

1. Install dependencies:
```bash
npm install
```

2. Run the development server:
```bash
npm run dev
```

3. Open [http://localhost:3000](http://localhost:3000) in your browser to see the application.

## Project Structure

```
alx-rick-and-morty-app/
├── graphql/
│   ├── apolloClient.ts    # Apollo Client configuration
│   └── queries.ts         # GraphQL queries
├── pages/
│   ├── _app.tsx          # App wrapper with ApolloProvider
│   ├── _document.tsx     # HTML document structure
│   └── index.tsx         # Home page
├── styles/
│   └── globals.css       # Global styles with Tailwind
└── public/               # Static assets
```

## Technologies Used

- **Next.js**: React framework for production
- **TypeScript**: Static type checking
- **Apollo Client**: GraphQL client for data fetching
- **Tailwind CSS**: Utility-first CSS framework
- **ESLint**: Code linting and formatting

## GraphQL Integration

### Apollo Client Setup

The Apollo Client is configured in `graphql/apolloClient.ts` to connect to the Rick and Morty API:

```typescript
import { ApolloClient, InMemoryCache, HttpLink} from "@apollo/client"

const client = new ApolloClient({
  link: new HttpLink({
    uri: "https://rickandmortyapi.com/graphql"
  }),
  cache: new InMemoryCache()
})

export default client;
```

### Available Queries

**GET_EPISODES**: Fetches paginated episode data with filtering options

```graphql
query getEpisodes($page: Int, $filter: FilterEpisode) {
  episodes(page: $page, filter: $filter) {
    info {
      pages
      next
      prev
      count
    }
    results {
      id
      name
      air_date
      episode
    }
  }
}
```

## Development

### Running the Development Server

```bash
npm run dev
```

The application will be available at [http://localhost:3000](http://localhost:3000)

### Building for Production

```bash
npm run build
npm start
```

### Linting

```bash
npm run lint
```

## API Reference

This project uses the [Rick and Morty GraphQL API](https://rickandmortyapi.com/graphql)

## Repository

- **GitHub repository**: alx-graphql-0x01
- **Directory**: alx-rick-and-morty-app

## Key Files

- `graphql/apolloClient.ts` - Apollo Client configuration
- `graphql/queries.ts` - GraphQL query definitions
- `pages/_app.tsx` - Application wrapper with ApolloProvider

## Learn More

- [Next.js Documentation](https://nextjs.org/docs)
- [Apollo Client Documentation](https://www.apollographql.com/docs/react/)
- [Rick and Morty API](https://rickandmortyapi.com/documentation)
- [TypeScript Documentation](https://www.typescriptlang.org/docs/)
- [Tailwind CSS Documentation](https://tailwindcss.com/docs)
