
### Additional Features
- **KHQR Payment Integration** - Cambodian QR code payment system
- **Groq AI Chatbot** - AI-powered customer assistance
- **Email OTP** - Secure password reset functionality
- **Role-based Access Control** - Admin, Manager, and Staff permissions

##  Key Features

### 🛒 Point of Sale (POS)
- Real-time sales processing
- Customer search and management during checkout
- Multiple payment methods (Cash, Card, KHQR)
- Receipt generation and printing
- Order history tracking
- Customer debt management

###  Inventory Management
- Product catalog with categories
- Stock level monitoring
- Low stock alerts and reorder points
- Inventory adjustments and history
- Product attributes (variants)

###  Customer Management
- Customer database with contact information
- Purchase history tracking
- Credit/debt management
- Customer search and filtering

### Supplier & Purchasing
- Supplier management
- Purchase order processing
- Stock replenishment tracking

###  Financial Management
- Sales reporting
- Expense tracking
- Payment processing
- Profit/loss analysis

###  User Management
- Multi-user support with role-based permissions
- User authentication and authorization
- Profile management
- Password reset with OTP

### AI Integration
- Groq-powered chatbot for customer support
- Intelligent product recommendations

## System Architecture

The application follows Laravel's MVC architecture:

- **Models**: Business logic and database interactions
  - Product, Category, Customer, Order, Inventory, etc.
- **Views**: Blade templates for server-side rendering
- **Controllers**: Handle HTTP requests and responses
- **Routes**: Define application endpoints
- **Middleware**: Authentication, authorization, and request filtering

##  Database Schema

Key tables include:
- `users` - System users with roles
- `products` - Product catalog
- `categories` - Product categories
- `customers` - Customer information
- `orders` - Sales transactions
- `order_details` - Order line items
- `inventory` - Stock levels
- `suppliers` - Supplier information
- `purchases` - Purchase orders
- `payments` - Payment records
- `expenses` - Business expenses
- ......

##  Installation & Setup

### Prerequisites
- PHP 8.2 or higher
- Composer
- Node.js & npm
- MySQL database
- Git

### Installation Steps

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd pos_pc_project
   ```

2. **Install PHP dependencies**
   ```bash
   composer install
   ```

3. **Install Node.js dependencies**
   ```bash
   npm install
   ```

4. **Environment configuration**
   ```bash
   cp .env.example .env
   php artisan key:generate
   ```

5. **Database setup**
   - Create a MySQL database
   - Update `.env` with database credentials
   ```bash
   php artisan migrate
   php artisan db:seed
   ```

6. **Build assets**
   ```bash
   npm run build
   ```

7. **Storage link**
   ```bash
   php artisan storage:link
   ```

8. **Start the application**
   ```bash
   php artisan serve
   ```

## Usage

### For Sales Staff
1. Login to the POS interface
2. Search and add products to cart
3. Process customer information
4. Select payment method
5. Generate receipt

### For Administrators
1. Access dashboard for overview
2. Manage products, categories, and inventory
3. Handle customer and supplier relationships
4. Generate reports and analytics
5. Configure system settings

## 🔧 Configuration

### Payment Integration
- Configure KHQR API credentials in `.env`
- Set up payment processing endpoints

### AI Chatbot
- Configure Groq API key for chatbot functionality
- Customize chatbot responses and behavior

### Email Settings
- Configure SMTP settings for OTP emails
- Set up email templates



