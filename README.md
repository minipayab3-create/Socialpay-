# SocialPay v8.0

## What's New in v8

### 1. Bank Details System
- Permanent save — stored once, auto-reused in all withdrawals
- No re-entry required on withdrawal
- Dropdown list of all Nigerian banks + wallets
- Manual account name entry (no API required)
- No user editing — contact support to change
- Admin can edit / delete bank details
- Duplicate account number blocked across all accounts

### 2. Super Admin
- Can view password hash and PIN hash for any user
- Full account data with no restrictions

### 3. Forgot Password
- Login page: "Forgot Password" → Telegram with pre-filled email
- Profile page: option with User ID pre-filled

### 4. Image Upload Progress Bar
- Real-time 0%→100% progress bar
- Replaces "Processing…" text
- Works for task screenshots, admin messages, broadcasts

### 5. Transfer Controls (Admin Settings)
- Enable / Disable transfers globally
- Minimum transfer amount
- Maximum transfer amount
- Daily transfer limit per user

### 6. Admin Messaging
- Send text + image to individual users
- Dedicated /admin/messages page
- Dashboard shows alert banner for unread messages
- Notifications page shows admin messages + images separately

### 7. Broadcast
- Image attachment support
- Live preview before sending
- Styled by type (info/success/warning/error)
- No formatting restrictions

### 8. Daily Login Reward
- Manual click to claim (never automatic)
- Clearer UI

### 9. Network Failure Handling
- Never freezes the app
- Red banner: "No internet connection. Please check your network."
- Retry button; auto-dismisses on reconnection

### 10. Spin
- Result pre-calculated and saved to DB before animation
- Reward credited even if user closes app or loses connection

### 11. User Tracking (Super Admin)
- IP address, country, city, device info captured on every login
- Last 5 logins shown in user detail
- Full tracking log at /admin/tracking

### 12. Security
- Login attempt limits (default 5), configurable in settings
- 15-minute lockout after too many failures
- Configurable Telegram support username

### 13. Activity Logs
- Expanded to 200 records
- Covers all key actions

### 14. Transaction Filters
- Filter by type (credit/debit) and date on balance page

---

## Setup
```
pip install flask werkzeug pillow
python app.py
```
Admin: socialpay.app.ng@gmail.com / @ Ahmerdee4622

## Environment Variables
- SECRET_KEY, ADMIN_EMAIL, ADMIN_PASSWORD, FLASK_ENV=production
