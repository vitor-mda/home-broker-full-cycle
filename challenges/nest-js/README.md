# 🐱 Challenge: Nest.js

> Using Docker Compose, create a Nest.js app with Prisma for ORM and Mongo (image: bitnami/mongodb:5.0.17) for persistency. It should run on port 3000.
> 
> It needs to expose the following REST routes:
> - GET `/api/assets` - View assets
> - POST `/api/assets` - Create assets
> - GET `/api/orders` - View orders
> - POST `/api/orders` - Create orders
>
> An asset has the following data:
> - `id` (user supplied)
> - `symbol`
>
> An order has the following data:
> - `id` (autogenerated)
> - `asset_id`
> - `price`
> - `status` (`'open'`, `'pending'`, and `'closed'`. Can't be user supplied)
>
> Create an api.http file for the HTTP API calls. When Running `docker compose up`, the application should be served.