


# 💼 BillForge – Multi-Tenant Invoicing Platform

**BillForge** is a full-stack, secure, and scalable invoicing platform designed for modern organizations. Built using Next.js 15, it supports user and organization-based billing, robust authentication, payment integration, and real-time transactional workflows — all with a focus on clean backend architecture.

---

## 🚀 Tech Stack

- **Frontend**: Next.js 15, React 19, Tailwind CSS, shadcn/ui  
- **Backend**: Server Actions, Drizzle ORM, Xata  
- **Auth**: Clerk (Passkeys, MFA, Social Login)  
- **Payments**: Stripe (Subscriptions, One-Time, Webhooks)  
- **Emails**: Resend (Transactional Email API)  

---

## ✨ Features

- 🔐 Passwordless Auth, Multi-Factor Authentication (MFA), and Role-Based Access
- 🧾 Create, view, and manage invoices per organization
- 💳 Stripe integration with Checkout sessions and billing portals
- 📧 Transactional emails on invoice events (created, updated, paid) using Resend
- 📊 Modern, accessible UI with shadcn/ui and Tailwind CSS
- ⚡ Server Actions for secure backend operations


---

## 🛠️ Setup Instructions

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/billforge.git
cd billforge
````

### 2. Install Dependencies

```bash
npm install
```

### 3. Configure Environment Variables

Create a `.env.local` file and add:

```env
CLERK_PUBLISHABLE_KEY=
CLERK_SECRET_KEY=
XATA_API_KEY=
XATA_BRANCH=
STRIPE_SECRET_KEY=
STRIPE_WEBHOOK_SECRET=
RESEND_API_KEY=
NEXT_PUBLIC_CLERK_SIGN_IN_URL=/login
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/signup
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/dashboard
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/dashboard
```

### 4. Set Up Xata & Drizzle ORM

```bash
npx xata init
npx drizzle-kit push
```

---

## 🧪 Key Functionalities

### 🔐 Authentication with Clerk

* Social login, email/password, MFA (TOTP), passkeys
* Route protection and server actions security
* Organization & user-level access separation

### 🧾 Invoice Management

* Create, edit, delete invoices with progressive forms
* Table view with filtering and sorting (DataTable)
* Join customer & invoice tables for relational insights

### 💳 Payments via Stripe

* One-time and subscription payments
* Webhooks to handle status updates
* Public payment page with status handling

### 📧 Email Notifications (Resend)

* Custom email templates built with React
* Triggered on invoice creation and updates
* Fully managed email delivery via Resend

---

## 👤 Author

**Gollapalli Abhiram**
🔗 [LinkedIn](https://www.linkedin.com/in/abhiramgollapalli/)
🔗 [GitHub](https://github.com/gollapalliabhiram)


