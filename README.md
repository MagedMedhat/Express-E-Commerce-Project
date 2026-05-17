# Node.js Project

A complete Node.js guide project featuring Express, MongoDB, authentication, file uploads, and more.

## Features

- RESTful API with Express
- MongoDB integration via Mongoose
- User authentication (signup, login, logout)
- Session management with express-session and connect-mongodb-session
- CSRF protection
- File uploads with Multer
- Form validation with express-validator
- Flash messages with connect-flash
- Password hashing with bcryptjs
- Email sending with Nodemailer and Sendgrid
- PDF generation with PDFKit
- Payment processing with Stripe
- Admin and shop routes
- Image serving

## Prerequisites

- Node.js (>=14)
- npm or yarn
- MongoDB Atlas (or local MongoDB instance)
- Sendgrid account (for emails)
- Stripe account (for payments)

## Setup

1. **Clone the repository**

   ```bash
   git clone https://github.com/your-username/node-js-project.git
   cd node-js-project
   ```

2. **Install dependencies**

   ```bash
   npm install
   ```

3. **Configure environment variables**

   Create a `.env` file in the project root based on the example below:

   ```env
   MONGODB_URI=mongodb+srv://<username>:<password>@cluster0.example.mongodb.net/shop?appName=Cluster0
   SESSION_SECRET=your_super_secret_string
   SENDGRID_API_KEY=your_sendgrid_api_key
   EMAIL_FROM=your_email@example.com
   STRIPE_KEY=your_stripe_secret_key
   ```

   > **Important:** Never commit your `.env` file. It is already ignored by `.gitignore`.

4. **Start the development server**

   ```bash
   npm run start
   # or
   npm start
   ```

   The app will be available at `http://localhost:3000`.

## Available Scripts

- `npm start` – Start the server with Node
- `npm run start-server` – Alternative start command
- `npm test` – Placeholder for tests

## Project Structure

```
node-js-project/
├─ controllers/      # Route handlers (admin, shop, auth)
├─ models/           # Mongoose models (User, Product, Order, etc.)
├─ routes/           # Express route definitions
├─ views/            # EJS templates
├─ public/           # Static assets (CSS, JS, images)
├─ images/           # Uploaded images (created at runtime)
├─ app.js            # Entry point: Express app setup and MongoDB connection
├─ package.json      # Dependencies and scripts
└─ .env              # Environment variables (not tracked)
```

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/awesome-feature`)
3. Commit your changes (`git commit -am 'Add awesome feature'`)
4. Push to the branch (`git push origin feature/awesome-feature`)
5. Open a pull request

## License

This project is licensed under the ISC License.