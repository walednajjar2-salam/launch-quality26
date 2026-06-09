[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/new?templateId=ORctok&envs=JAWDAH_HOST,JAWDAH_PORT,JAWDAH_DATA_DIR&optionalEnvs=JAWDAH_DB_PATH&JAWDAH_HOSTDefault=0.0.0.0&JAWDAH_PORTDefault=8080&JAWDAH_DATA_DIRDefault=/var/data&JAWDAH_DB_PATHDefault=/var/data/jawdah.sqlite3&repo=https://github.com/walednajjar2-salam/launch-quality26)

# Launch Quality LLC - Real Estate & Hospitality Management System

## نظام إدارة العقارات والضيافة

### Features / الميزات
- 🏠 إدارة العقارات والوحدات
- 👥 إدارة العملاء والمستأجرين
- 📑 إدارة العقود والاتفاقيات
- 🧾 نظام الفواتير والتحصيل
- 💰 الحسابات والتقارير المالية
- 🔧 طلبات الصيانة والإصلاح
- 📊 لوحة التحكم التنفيذية
- 🛡️ نظام الصلاحيات والمستخدمين

### Quick Start

```bash
# Clone the repository
git clone https://github.com/walednajjar2-salam/launch-quality26.git
cd launch-quality26

# Run with Docker
docker-compose up -d

# Or run directly
python server.py
```

### Default Credentials

**Admin:**
- Username: `admin`
- Password: `admin123`

**Accountant:**
- Username: `razan.accounting`
- Password: `Jawdeh123`

### Environment Variables

```
JAWDAH_HOST=0.0.0.0
JAWDAH_PORT=8080
JAWDAH_DATA_DIR=/var/data
JAWDAH_DB_PATH=/var/data/jawdah.sqlite3
```

### Database

SQLite database with 20+ tables:
- properties, clients, contracts, invoices, payments
- accounts, purchase_invoices, revenues, salaries
- admin_expenses, inventory_items, inventory_transactions
- bank_transactions, chart_accounts, financial_periods
- approvals, bank_reconciliations, maintenance, users, audit_log

### API Endpoints

- `POST /api/login` - User login
- `GET /api/bootstrap` - Load all data
- `GET /api/dashboard` - Dashboard KPIs
- `POST /api/invoice_from_contract` - Create invoice from contract
- `POST /api/pay_invoice` - Record payment
- `GET /api/financial_statements` - Financial reports
- `GET /api/backup` - Export backup

### Deployment

**One-Click Deploy to Railway:** Click the button at the top ☝️

**Or manually:**
- **Railway**: `python server.py`
- **Docker**: `docker-compose up`
- **Render**: See render.yaml

### License

Launch Quality LLC © 2026