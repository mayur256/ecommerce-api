# API Documentation

## Preferred Technologies

- **API Framework**: FastAPI / Flask  
- **Database**: PostgreSQL  
- **Payment Gateway**: Any (e.g., Stripe, PayPal)  
- **ORM**: SQLAlchemy (best compatible with both Flask and FastAPI)  
- **Architecture**: MVC (Model-View-Controller)  
- **Code Standards**: Follow PEP8, RESTful API principles, and use type hints, dependency injection, and modular code structure for maintainability and scalability.

---

## API Endpoints

### Authentication & User Management

- `POST /auth/register` – User registration  
- `POST /auth/login` – User authentication  
- `POST /auth/refresh` – Token refresh  
- `POST /auth/logout` – User logout  
- `GET /users/profile` – User profile retrieval  
- `PUT /users/profile` – User profile update  
- `POST /auth/forgot-password` – Password reset request  
- `POST /auth/reset-password` – Password reset confirmation  

### Product & Catalog Management

- `GET /products` – Product listing with pagination and filtering  
- `GET /products/:id` – Product details retrieval  
- `POST /products` – Product creation (admin)  
- `PUT /products/:id` – Product update (admin)  
- `DELETE /products/:id` – Product deletion (admin)  
- `GET /categories` – Category listing  
- `GET /products/search` – Product search functionality  

### Shopping Cart & Orders

- `GET /cart` – Shopping cart retrieval  
- `POST /cart/items` – Add item to cart  
- `PUT /cart/items/:id` – Update cart item  
- `DELETE /cart/items/:id` – Remove item from cart  
- `POST /orders` – Order creation  
- `GET /orders` – Order history  
- `GET /orders/:id` – Order details  
- `PUT /orders/:id/status` – Order status update (admin)  
