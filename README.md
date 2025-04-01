### rhis moved to here: https://github.com/The-Poolz/InterfaceStrapi

# Poolz Data GraphQL SDK

[![NPM Version](https://img.shields.io/npm/v/poolz-data-graphql-sdk)](https://www.npmjs.com/package/poolz-data-graphql-sdk)
[![License](https://img.shields.io/npm/l/poolz-data-graphql-sdk)](LICENSE)
[![Downloads](https://img.shields.io/npm/dt/poolz-data-graphql-sdk)](https://www.npmjs.com/package/poolz-data-graphql-sdk)

A TypeScript SDK for interacting with the Poolz Finance GraphQL API.

## 🚀 Installation

```sh
npm install poolz-data-graphql-sdk
```

## 👀 Usage

```ts
import { request } from "graphql-request";
import { getSdk } from "poolz-data-graphql-sdk";

const client = getSdk((query, variables) =>
  request("https://data.poolz.finance/graphql", query, variables)
);

async function fetchData() {
  const result = await client.GetPools();
  console.log(result);
}

fetchData();
```

## 🔄 Auto-Generated Queries

This SDK provides auto-generated TypeScript functions for querying Poolz Finance's GraphQL API.  
To regenerate queries, run:

```sh
npm run codegen
```

## 🎯 Features
👉 Fully typed GraphQL requests  
👉 Easy-to-use SDK  
👉 Auto-generated queries with `graphql-codegen`  

## 📚 Links
- **NPM Package:** [poolz-data-graphql-sdk](https://www.npmjs.com/package/poolz-data-graphql-sdk)
- **GraphQL API:** [https://data.poolz.finance/graphql](https://data.poolz.finance/graphql)

## 💜 License

This project is licensed under the [MIT License](LICENSE).

