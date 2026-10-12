# SmartMove Transport — front-end learning prototype

## Pages
- `index.html` redirects to `login.html`.
- `login.html` provides a demo sign-in page with a role selector.
- `register.html` registers passenger demo accounts in this browser only.
- `customer.html` is the passenger portal (overview, booking, tickets, reviews, help).
- `admin.html` is the admin workspace (fleet, drivers, routes, trips, maintenance, passengers, booking records, reviews and reports).

## Demo credentials
- Admin: `admin@smartmove.demo` / `Admin123!`
- Passenger: `customer@smartmove.demo` / `Passenger123!`

Open `index.html` or `login.html` in a modern browser. No server is required for this static prototype.

## Important limitations
This is a front-end-only learning prototype. Login role checks and registered demo accounts use browser storage and are **not secure authentication**. Do not use real passwords or personal data. Demo data is held in JavaScript memory and resets on page reload; registered demo accounts persist in the current browser's local storage. There is no payment processing, database connection, Oracle SQL, PL/SQL, or MongoDB code. The database components must be implemented and tested separately for the coursework.

## Recent front-end updates
- Passenger reviews now include a rating selector and optional image attachment (image files up to 3 MB). Photos appear alongside the review in the current page session.
- Admin reports now let you choose a dataset, select the fields to include, filter rows by a keyword, generate a preview, and export the selected result as CSV.
- These features use only sample data in the front-end; reviews, photos, and generated reports are not persisted to Oracle or MongoDB.

## Review form fix
- Fixed the review button action dispatch so `add-review` opens the review form instead of being treated as an admin add-record action.
