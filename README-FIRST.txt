MEDISWIFT AI - COMPLETE FULL-STACK PROJECT

Run locally:
1) Open this folder in VS Code
2) Terminal: cd backend
3) First time: npm.cmd install
4) Start: node server.js
5) Open http://localhost:3000

Do not use Live Server or double-click index.html for full-stack testing.

Included: register/login/logout, backend cart, checkout/orders, order history, editable My Profile, phone/address/city/pincode, change password, doctor appointment booking, appointment list/cancel, mobile account menu, and the existing store/search/prescription demo/assistant UI.

Note: real payments, real video calls, SMS/OTP, real AI processing and courier GPS need external services. JSON files are suitable for this local/demo build; use a managed database for production hosting.


V3 FIX: Account/profile button visibility fixed after login. If browser has an old token, log in again once.


V4 SAVED DELIVERY DETAILS
-------------------------
- Registration now collects phone, delivery address, city and pincode.
- These details are saved to the user's backend profile.
- Checkout automatically loads the saved address, city, pincode and phone.
- If the customer changes delivery details at checkout, MediSwift saves the latest values to the profile for future orders.
- Existing older accounts can add missing details from My Profile.
