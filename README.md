# Next.js and GraphQL Server

## Available Scripts

**Start for Development**

```sh
npm run dev
```

**Start Next.js Server(Production)**

```sh
npm start
```

**Build pages for Production**

```sh
npm run build
```

---

## GraphQL API available at

```
http://localhost:3000/api/graphql
```

```graphql
query AllUsers {
  getUsers {
    id
    login
    avatar_url
  }
}

# Set `name` variable in Playground
query UserByName($name: String!) {
  getUser(name: $name) {
    login
    id
    avatar_url
  }
}
```
