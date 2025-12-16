# TODO: Implement Secure Order Creation with Payment Status

## Tasks
- [ ] Update AccountController.cs login method to generate and return JWT token
- [ ] Modify CheckoutView.vue to store JWT token and send Authorization header in API requests
- [ ] Add payment method selection in CheckoutView.vue and send PaymentStatus in order data
- [ ] Update OrderController.cs PlaceOrder method to require authentication, get UserId from claims, fetch user for FullName, and handle PaymentStatus
- [ ] Test order placement functionality

## Notes
- Ensure PaymentStatus is sent from frontend (e.g., "Cash", "Card", etc.)
- Default PaymentStatus to "Pending" if not provided
- Use JWT for secure authentication
