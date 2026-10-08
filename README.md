# Aurevia Marketplace

A clean, separate full-stack marketplace for **Cars, Furnished Houses and Plots**.

## What is included
- New MySQL database: `aurevia_marketplace`
- Separate admin authentication and dashboard
- Category-specific listing forms
- Up to 12 images per listing
- Public client pages read directly from the same database/API as admin
- Customer registration with required WhatsApp number
- Booking workflow with stored lead + full WhatsApp message + image references
- Click-to-WhatsApp integration; Cloud API credentials can be added later
- Working local/demo booking-fee payment flow; Stripe environment hooks are provided for live payment integration
- Professional responsive marketplace UI
- Real-estate hero uses the requested image URL
- Separate sample data: one car, one furnished house, one plot, each with multiple images

## Admin
URL: `http://localhost:5173/admin/login`
Email: `admin@aurevia.local`
Password: `Admin@123`

## Environment
Copy `server/.env.example` to `server/.env` and set MySQL credentials plus a long `JWT_SECRET`.

## Run
1. Start XAMPP MySQL.
2. From this folder run `npm install`.
3. Run `npm run install:all`.
4. Run `npm run dev`.
5. Open `http://localhost:5173`.

The server creates `aurevia_marketplace` automatically if the MySQL user has permission. You may also import `database/schema.sql` manually.
