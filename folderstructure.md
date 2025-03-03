ecommerce-microfrontends/
├── shell-app/                     # Container App (Angular 19 + Module Federation)
│   ├── src/
│   │   ├── app/
│   │   │   ├── app.module.ts
│   │   │   ├── app.component.ts
│   │   │   ├── app-routing.module.ts
│   │   │   ├── mfe-loader.service.ts  # Micro-frontend loader service
│   │   │   ├── navbar.component.ts
│   │   ├── assets/
│   │   ├── environments/
│   ├── webpack.config.js
│   ├── webpack.prod.config.js
│   ├── angular.json
│   ├── package.json
│   ├── Dockerfile
│   ├── docker-compose.yml
│   ├── nginx.conf
│
├── product-catalog/               # Micro-frontend 1: Product Listing
│   ├── src/
│   │   ├── app/
│   │   │   ├── product.module.ts
│   │   │   ├── product-list.component.ts
│   │   │   ├── product-details.component.ts
│   │   │   ├── redux/
│   │   │   │   ├── product.actions.ts
│   │   │   │   ├── product.reducer.ts
│   │   │   │   ├── product.selectors.ts
│   │   ├── assets/
│   ├── webpack.config.js
│   ├── angular.json
│   ├── package.json
│   ├── Dockerfile
│
├── cart-checkout/                 # Micro-frontend 2: Cart and Checkout
│   ├── src/
│   │   ├── app/
│   │   │   ├── cart.module.ts
│   │   │   ├── cart.component.ts
│   │   │   ├── checkout.component.ts
│   │   │   ├── redux/
│   │   │   │   ├── cart.actions.ts
│   │   │   │   ├── cart.reducer.ts
│   │   │   │   ├── cart.selectors.ts
│   ├── webpack.config.js
│   ├── angular.json
│   ├── package.json
│   ├── Dockerfile
│
├── user-auth/                     # Micro-frontend 3: Authentication
│   ├── src/
│   │   ├── app/
│   │   │   ├── auth.module.ts
│   │   │   ├── login.component.ts
│   │   │   ├── register.component.ts
│   │   │   ├── redux/
│   │   │   │   ├── auth.actions.ts
│   │   │   │   ├── auth.reducer.ts
│   │   │   │   ├── auth.selectors.ts
│   ├── webpack.config.js
│   ├── angular.json
│   ├── package.json
│   ├── Dockerfile
│
├── order-management/               # Micro-frontend 4: Order History and Admin
│   ├── src/
│   │   ├── app/
│   │   │   ├── order.module.ts
│   │   │   ├── order-list.component.ts
│   │   │   ├── order-details.component.ts
│   │   │   ├── redux/
│   │   │   │   ├── order.actions.ts
│   │   │   │   ├── order.reducer.ts
│   │   │   │   ├── order.selectors.ts
│   ├── webpack.config.js
│   ├── angular.json
│   ├── package.json
│   ├── Dockerfile
│
├── docker-compose.yml               # Docker Compose to run all micro-frontends
├── nginx.conf                        # Nginx reverse proxy for routing
