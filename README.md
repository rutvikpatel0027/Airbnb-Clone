# Airbnb Clone Console Application

A premium, high-efficiency React and Tailwind CSS Airbnb clone complete with client search feeds, booking managers, and a live isolated Admin Dashboard Console.

---

## 🔑 Admin Console Credentials

Access the Admin Panel at `/admin` (or via the profile dropdown) using the following credentials:
* **Username / ID:** `admin`
* **Password:** `admin`

*(An auto-fill button is also available on the Admin Login page for quick testing).*

---

## 🔄 Application Workflow

### 1. Client Home Feed
* **Feed Browse**: Users can view property listings dynamically sorted by categories (Beach, Cabins, Islands, etc.).
* **Grid vs Map Views**: Toggle between the custom Grid listing cards and the interactive Leaflet Map view via the floating button at the bottom center.
* **Search & Filters**: Search stays by popular destinations, check-in/out dates, and guest counts. Refine results via the Advanced Filters modal (max price, bed/bath specs, amenities checklist).

### 2. User Authentication
* **Seamless Sign-in**: Log in or Sign up via the profile menu dropdown. You can also click "Continue as Guest" for instant access.
* **Live Admin Sync**: Once a new user creates an account, their name, email, and join date are automatically synced and registered under the global directory in the Admin Dashboard.

### 3. Reservations & "My Trips"
* **Bookings**: Select any listing, view properties, specifications, and host info. Select dates, input guests, and click **Reserve Stay** to confirm a booking.
* **Trips Panel**: Access booked stays directly via the "My Trips" shortcut on the navigation header. Normal trips reflect the dynamically updated payment status. If an admin cancels a booking, it displays a status message stating `"Admin cancelled the booking"`.

### 4. Admin Dashboard Console
* **Overview Tab**: Live KPI dashboard displaying earnings, occupancy rates, listing category distributions (donut chart), and weekly check-in graphs.
* **Listings Tab**: Directory listing of properties, allowing admins to modify details (via Edit Drawer) or remove listings (auto-cancelling related bookings). *Property addition is disabled throughout the application.*
* **Bookings Tab**: Unified order logs showing checks, guests, dates, and status. Admins can:
  * **Rotate Payment Status**: Click the payment badge to toggle status (`Paid` -> `Pending` -> `Refunded`). Updates are reflected on the client's Trips page.
  * **Update Booking Status**: Cancel or reconfirm reservations.
* **Hosts & Users Tab**: Database directory of all users. Highlights status (Active/Suspended), dynamic bookings counts, and total transaction costs spent. Suspended users are greyed out and can be reactivated by the admin.

---

## 🛠️ Tech Stack & Scripts

* **Frontend Framework**: React 18, Vite
* **Styling**: Tailwind CSS
* **Animations**: Framer Motion
* **Charts & Analytics**: Recharts
* **Icons**: Lucide React

### Running Locally
1. Install dependencies:
   ```bash
   npm install
   ```
2. Start local development server:
   ```bash
   npm run dev
   ```
3. Build production bundle:
   ```bash
   npm run build
   ```
