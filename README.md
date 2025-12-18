# 💳 Payment Gateway Demo (Laravel)

This project demonstrates **secure payment gateway integration** in Laravel using **Razorpay and PhonePe**.  
It focuses on real-world implementation patterns such as order creation, callback handling, and webhook verification.

---

## 🚀 Features

- Razorpay payment integration
- PhonePe payment integration
- Order creation & payment initiation
- Secure payment verification
- Webhook handling
- Environment-based configuration
- Proper error handling & logging

---

## 🛠️ Tech Stack

- Laravel (9/10/11 compatible)
- PHP
- MySQL
- REST APIs
- Webhooks
- Blade / Bootstrap (basic UI)

---

## 🧩 Payment Flow

1. User initiates payment
2. Backend creates order with gateway
3. Payment page opens
4. Gateway redirects callback
5. Server verifies signature / checksum
6. Payment status stored in database

---

## 📂 Key Modules

- `PaymentController`
- `WebhookController`
- Order & Transaction Models
- Service-based payment handling
- `.env` based credentials management

---

## 🔐 Security Practices Used

- Signature / checksum verification
- Server-side amount validation
- Secure webhook endpoints
- No sensitive keys exposed in frontend

---

## ⚙️ Installation

```bash
git clone https://github.com/shivm1987/payment-gateway-demo.git
cd payment-gateway-demo
composer install
cp .env.example .env
php artisan key:generate
php artisan migrate
