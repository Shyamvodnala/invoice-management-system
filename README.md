# Invoice Management System

A Django-based invoice management system for cloth business with multi-user support (Admin & User), party-based taxation, payment tracking, and transportation management.

## Features

- **User Roles**: Admin and Regular User
- **Invoice Management**: Create, Edit, Delete (before approval), Approve/Reject
- **Multi-Product Support**: Support for quantity and meters in single invoice
- **Party-Based Taxation**: CGST+SGST, GST, or Zero GST
- **Invoice-Level Discount**: Fixed amount or percentage
- **Payment Tracking**: Track partial payments with dates and methods
- **Transportation Details**: Track shipping with delivery status
- **PDF Generation**: Generate invoice PDFs
- **Email Notifications**: Notify users on invoice approval/rejection

## Tech Stack

- Python 3.8+
- Django 4.2+
- PostgreSQL
- HTML/CSS/Bootstrap 5

## Quick Start

1. Clone repository: `git clone https://github.com/Shyamvodnala/invoice-management-system.git`
2. Create virtual environment: `python -m venv venv`
3. Activate: `source venv/bin/activate`
4. Install: `pip install -r requirements.txt`
5. Copy `.env.example` to `.env` and configure PostgreSQL
6. Run migrations: `python manage.py migrate`
7. Create admin: `python manage.py createsuperuser`
8. Start server: `python manage.py runserver`
9. Access: http://localhost:8000

## Database Schema

- **Users**: User authentication and roles
- **Parties**: Customer/Party information with tax settings
- **Products**: Product catalog
- **ProductPricing**: Product pricing by party
- **Invoices**: Invoice headers
- **InvoiceItems**: Invoice line items
- **InvoiceApprovals**: Approval workflow
- **Payments**: Payment tracking
- **Transportation**: Shipping details
