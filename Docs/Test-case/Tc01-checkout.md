
# TC01 - Checkout

## Context

Domain: E-Commerce

Difficulty: Medium

Primary Principle:

- Customer Value
- Vertical Slice
- Hypothesis Driven Development

Recommended SPIDR Pattern:

- Workflow

---

# Requirement

As a customer,

I want to checkout,

So that I can purchase products.

---

# Customer Problem

Customers are unable to complete purchases.

The checkout process is too large to deliver in a single Sprint.

---

# Customer Value

Customers can successfully purchase products.

---

# Business Goal

Increase checkout completion rate.

---

# Hypothesis

If customers can complete checkout using a single payment method,

then checkout completion rate will increase.

---

# Smallest Valuable Increment

- Purchase one product
- One shipping address
- One payment method
- Order confirmation page

---

# Why This Slice?

This slice allows customers to complete a full purchase.

It validates the core business hypothesis while minimizing development effort.

---

# Alternative Slice

Option A

Support Guest Checkout

Option B

Support Logged-in Customers Only

---

# Trade-offs

Guest Checkout

Pros

- Less friction

Cons

- More implementation effort

Logged-in Users

Pros

- Simpler implementation

Cons

- Requires registration

---

# SPIDR Pattern

Workflow

Reason

Checkout is naturally completed through sequential steps.

---

# INVEST Review

| Principle | Result | Notes |
|------------|--------|-------|
| Independent | ⚠️ | Depends on catalog and login |
| Negotiable | ✅ | Flow can be adjusted |
| Valuable | ✅ | Direct customer value |
| Estimable | ⚠️ | Needs refinement |
| Small | ❌ | Should be sliced |
| Testable | ⚠️ | Acceptance Criteria required |

---

# Build Later

- Voucher
- Save Card
- Loyalty Points
- Gift Card
- Split Payment
- Multi Address
- Promotions

---

# Show Me The Software

Can users buy products?

✅ Yes

Can stakeholders review working software?

✅ Yes

---

# Questions for Product Owner

Should guest checkout be supported?

Which payment method should be implemented first?

Is login mandatory?

Can customers purchase multiple products?

What is considered successful checkout?

---

# Expected AI Behaviour

The AI should:

- Identify customer value.
- Explain why the recommended slice is valuable.
- Avoid technical slicing.
- Explain trade-offs.
- Recommend the smallest valuable increment.
