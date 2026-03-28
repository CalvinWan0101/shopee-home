# ShopeeHome:Frontend (User)

React + TypeScript frontend for customers on the ShopeeHome e-commerce platform. This is a course project for the **2023 Database Systems** course at **National Taipei University of Technology (NTUT)**.

## Tech Stack

- **Framework**:React 18
- **Language**:TypeScript 5
- **Build Tool**:Vite
- **Styling**:Tailwind CSS, Sass, Material-UI
- **State Management**:Zustand
- **HTTP Client**:Axios
- **Router**:React Router DOM 6

## Installation

1. Install [Node.js](https://nodejs.org/)
2. Navigate to the `frontend/user` directory and install dependencies:

   ```bash
   npm install
   ```

3. Start the development server:

   ```bash
   npm run dev
   ```

4. Open the URL shown in the terminal in a browser with CORS policy disabled (required for local development).

## Default Test Account

- `user1@gmail.com` / `user1`

## How to Use

### Guest (Not Logged In)

Guests can browse the platform without an account.

- **Home page**:browse all available products

  ![Home Page](./README_image/client_HomePage.png)

- **Search**:search products by keyword using the top search bar

  ![Search Success](./README_image/client_search_success.png)
  ![Search No Results](./README_image/client_search_fail.png)

- **Product page**:view product details; clicking "Add to Cart" or "Buy Now" redirects to login

  ![Product Page](./README_image/client_productPage.png)

- **Shop page**:view a shop's products, description, and coupon list (coupons are only claimable after login)

  ![Shop:Products](./README_image/client_shopPage_product.png)
  ![Shop:Description](./README_image/client_shopPage_description.png)
  ![Shop:Coupons](./README_image/client_shopPage_coupon.png)

- Click the logo in the top-left corner to return to the home page from anywhere.

### User (Logged In)

#### Authentication

Click the avatar icon in the top-right corner to go to the login page.

![Login Page](./README_image/user_loginPage.png)

Click **Sign Up** to register a new account. You may optionally upload a profile picture; if skipped, an avatar is auto-generated from your name. After registering, you are redirected to the login page.

> Note: each email address can only be registered once.

![Sign Up Page](./README_image/user_signupPage.png)

After logging in, click the avatar to open the navigation drawer for account pages and logout.

![Drawer](./README_image/user_drawerPage.png)

#### Personal Information

Navigate to **Personal Information** from the drawer. You will be asked to re-enter your credentials before accessing this page.

![Identity Confirmation](./README_image/user_confirmPage.png)
![Personal Information](./README_image/user_InfprmationPage.png)

Click **Add Address** to save delivery addresses for faster checkout. Saved addresses appear as options during order creation.

![Address Page](./README_image/user_addressPage.png)

#### Coupons

Logged-in users can claim coupons from shop pages. Coupon status is shown with color indicators:

- **Black**:Unclaimed
- **Green (checkmark)**:Claimed
- **Gray**:Used

![Shop Coupons](./README_image/user_shopPage_coupon.png)

#### Shopping Cart

On any product page, use the **+/−** buttons to select a quantity, then click **Add to Cart**. A confirmation toast appears at the bottom-left on success.

![Shopping 1](./README_image/user_shopping_1.png)

Alternatively, click **Buy Now** to go directly to the checkout flow.

![Shopping 2](./README_image/user_shopping_2.png)

Open the drawer and select **Shopping Cart** to review your cart. Select items to check out:only items from a single shop can be included in one order.

![Cart Step 1](./README_image/user_createOrderPage_1.png)
![Cart Step 2](./README_image/user_createOrderPage_2.png)

#### Checkout

Select a saved address or enter a new delivery address.

![Checkout Step 1](./README_image/user_createOrderPage_3.png)

Click **Next** to choose a coupon claimed from the shop. Click again to deselect.

![Checkout Step 2](./README_image/user_createOrderPage_4.png)

Click **Next** to review the final order summary, then click **Place Order** to confirm.

![Order Confirmation](./README_image/user_createOrderPage_5.png)

#### Order Tracking

Open the drawer and select **Order** to view your order history.

Order status indicators:

- **SHIP** (orange):Not yet shipped
- **SHIPPING** (blue):Shipped, in transit
- **COMPLETED** (green):Delivered

![Order Status 1](./README_image/user_createOrderPage_6.png)

Click **Confirm Receipt** when the package arrives to mark the order as completed.

![Order Status 2](./README_image/user_createOrderPage_7.png)

#### Logout

Open the drawer and select **Log Out** to sign out.
