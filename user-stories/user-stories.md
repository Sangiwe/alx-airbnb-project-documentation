# Airbnb Clone - User Stories

## 1. User Registration
**Title**: Account Registration  
**As a** guest or host, **I want to** register using email/password or OAuth (Google/Facebook), **so that** I can access the platform.  
**Acceptance Criteria**:  
- [ ] Email validation prevents duplicate accounts.  
- [ ] OAuth login redirects correctly and creates a user profile.  
- [ ] Password strength is enforced (min 8 chars, special characters).  

## 2. Property Listing Creation  
**Title**: Publish a Property Listing  
**As a** host, **I want to** add property details (title, description, price, amenities), **so that** guests can discover my property.  
**Acceptance Criteria**:  
- [ ] Photos upload successfully to AWS S3.  
- [ ] Price field rejects negative values.  
- [ ] Amenities are selectable from a predefined list.  

## 3. Property Booking  
**Title**: Book a Property  
**As a** guest, **I want to** select check-in/check-out dates and book a property, **so that** I can reserve my stay.  
**Acceptance Criteria**:  
- [ ] Calendar shows real-time availability.  
- [ ] System prevents double-booking for the same dates.  
- [ ] Total price calculates automatically (price × nights).  

## 4. Payment Processing  
**Title**: Secure Payment  
**As a** guest, **I want to** pay via Stripe/PayPal, **so that** my booking is confirmed.  
**Acceptance Criteria**:  
- [ ] Payment gateway redirects to a secure checkout page.  
- [ ] Receipt is emailed to the guest after successful payment.  
- [ ] Failed payments trigger a booking cancellation.  

## 5. Review Submission  
**Title**: Leave a Review  
**As a** guest, **I want to** rate and review a property after checkout, **so that** future guests can make informed decisions.  
**Acceptance Criteria**:  
- [ ] Reviews require a completed booking.  
- [ ] Rating is limited to 1-5 stars.  
- [ ] Hosts can respond to reviews.  

## 6. Booking Cancellation  
**Title**: Cancel a Booking  
**As a** guest or host, **I want to** cancel a booking according to the cancellation policy, **so that** I can manage my reservations.  
**Acceptance Criteria**:  
- [ ] Cancellation policy (e.g., "50% refund if canceled ≥7 days prior") is enforced.  
- [ ] Automated refunds process via the original payment method.  