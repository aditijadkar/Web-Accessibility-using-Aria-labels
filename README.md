# Web-Accessibility-using-Aria-labels

## ✅ ARIA Roles

ARIA roles define the semantic role of an element to assistive technologies, improving accessibility for users relying on screen readers.

| Role              | Purpose                                                                      |
|-------------------|------------------------------------------------------------------------------|
| `role="navigation"` | Used in the navbar for the main navigation section                         |
| `role="dialog"`     | Used in login, register, payment, and product modals                       |
| `role="tooltip"`    | Used in the popup description for each product                             |
| `role="button"`     | Used for each product card container to indicate interactivity             |

---

## ✅ ARIA Attributes

### 1. `aria-label`
Provides accessible names for elements not described by visible text.

- **Navigation**
  - `aria-label="Main navigation"`

- **Product Section Labels**
  - `aria-label="All Products Section"`
  - `aria-label="Fashion Section"`
  - `aria-label="Electronics Section"`
  - `aria-label="Stationery Section"`
  - `aria-label="My Cart Section"`
  - `aria-label="My Orders Section"`
  - `aria-label="About Us Section"`

- **Product Elements (Dynamically Generated)**
  - `aria-label="Product: {name}, Price: ${price}, Rating: {rating} out of 5, Delivery in {delivery} days"`

- **Inputs & Buttons**
  - `aria-label="Quantity for {name}"`
  - `aria-label="Update quantity for {item.name}"`
  - `aria-label="Remove {item.name} from cart"`
  - `aria-label="Cancel Login"`
  - `aria-label="Cancel Registration"`
  - `aria-label="Cancel Payment"`
  - `aria-label="Close Product Details"`

---

### 2. `aria-labelledby`
Associates modals with their corresponding titles for better screen reader navigation.

- **Login Modal**: `aria-labelledby="login-modal-title"`
- **Register Modal**: `aria-labelledby="register-modal-title"`
- **Payment Modal**: `aria-labelledby="payment-modal-title"`
- **Product Modal**: `aria-labelledby="product-modal-title"`

---

### 3. `aria-modal="true"`
Used in modals to indicate that the user must interact with the modal before returning to the main content.

---

### 4. `aria-live="polite"`
Announces updates (like cart changes) to screen readers without interrupting the user.

### 5. aria-hidden="true" / "false"
Controls visibility of elements for assistive technologies (e.g., tooltips or modals).
