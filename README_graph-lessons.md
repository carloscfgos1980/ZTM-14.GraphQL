## GraphQL

Course Source code

https://github.com/odziem/graphql-example

# Lesson 1. GraphQL Overview

https://academy.zerotomastery.io/courses/1206554/lectures/34307059

# Lesson 2. Our First GraphQL Query

https://academy.zerotomastery.io/courses/1206554/lectures/34307061

N: Practising GraphQL in a Github page

{
film(filmID: 2) {
title
producers
}
}

# Lesson 3. GraphQL Queries In Action

https://academy.zerotomastery.io/courses/1206554/lectures/34307063

# Lesson 4. GraphQL vs REST: Over-fetching & Under-fetching

https://academy.zerotomastery.io/courses/1206554/lectures/34307067

# Lesson 5. GraphQL vs REST Summary

https://academy.zerotomastery.io/courses/1206554/lectures/34309617

# Lesson 6. Exploring GraphQL Implementations

https://academy.zerotomastery.io/courses/1206554/lectures/34312873

# Lesson 7. GraphQL In Node

https://academy.zerotomastery.io/courses/1206554/lectures/34312875

npm init -y
npm install express
npm install graphql
npm install express-graphql

- This last package is already decapricated!

# Lesson 8. Working With Deprecated Packages

https://academy.zerotomastery.io/courses/1206554/lectures/49842499

# Lesson 9. Recommended: Migrating GraphQL Packages

https://academy.zerotomastery.io/courses/1206554/lectures/49842501

npm install grapjql-yoga

# Lesson 10. GraphiQL

https://academy.zerotomastery.io/courses/1206554/lectures/34357743

app.use('/graphql', createYoga({
schema: schema,
graphiql: true,
}));

N: This allow to load the tools from Graphiql in GitHub

# Lesson 11. Designing An E-Commerce Schema

https://academy.zerotomastery.io/courses/1206554/lectures/34357746

Example:
const schema = buildSchema(`
type Query {
products: [Product]
orders: [Order]
}

    type Product {
        id: ID
        description: String!
        reviews: [Review]
        price: Float
    }

    type Review {
        rating: Int!
        comment: String
    }

    type Order {
        date: String!
        Subtotal: Float!
        items: [OrderItem]
    }

    type OrderItem {
        product: Product!
        quantity: Int!
    }

`);

N: description: String! means that description is required

# Lesson 12. GraphQL Tools

https://academy.zerotomastery.io/courses/1206554/lectures/34357749

Check for tools
https://the-guild.dev/graphql/tools

# Lesson 13. Modularizing Large GraphQL Projects: Schemas

https://academy.zerotomastery.io/courses/1206554/lectures/34357750

npm install @graphql-tools/schema
npm install @graphql-tools/load-files

# Lesson 14. Resolvers

https://academy.zerotomastery.io/courses/1206554/lectures/34357752

# Lesson 15. Modularizing Large GraphQL Projects: Resolvers

https://academy.zerotomastery.io/courses/1206554/lectures/34361287

# Lesson 16. Filtering with Queries and Resolvers

https://academy.zerotomastery.io/courses/1206554/lectures/34361292

# Lesson 17. Exercise: Query Products By ID

https://academy.zerotomastery.io/courses/1206554/lectures/34369325

# Lesson 18. Implementing Mutations on the Server

https://academy.zerotomastery.io/courses/1206554/lectures/34403824

# Lesson 19. Exercise: Add New Product Review

https://academy.zerotomastery.io/courses/1206554/lectures/34403826
