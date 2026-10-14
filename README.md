FOS — Multi-Vendor Employee Cafeteria Ordering System
A responsive, browser-based demonstration of an employee cafeteria ordering workflow. Employees choose a cafeteria outlet, browse a time-based menu, place an order, and receive a pickup token. Vendors prepare orders and call tokens on an LED-style display; employees pay at the counter when collecting their food.
Independent portfolio project. This is an original demonstration and is not an Infosys product, deployment, or reproduction of any employer's internal code or designs.

Live demo
Open FOS
Features
Employee portal
- Choose from active cafeteria outlets, such as Sip & Bite, Tangy Tadka, Chai Wala, and Amul Ice Cream.
- Browse the selected vendor's menu for breakfast, lunch, or dinner.
- See meal service hours and item availability.
- Add items to a cart and generate a pickup token; no online payment is required.
- Check the LED-style token display to know when food is ready.
- Each order is associated with one vendor.
Vendor portal
- Select a registered outlet in the demo and view that outlet's orders.
- Add menu items, set prices, select meal categories, and enter stock quantities.
- Configure low-stock thresholds; see low-stock and sold-out indicators.
- Update inventory and enable or disable menu availability.
- Process orders through Placed → Preparing → Ready → Served; payment is collected at the counter.
Admin portal
- Register and manage cafeteria vendors; active outlets appear in the employee portal.
- Configure breakfast, lunch, and dinner service windows.
- Review order information and overview statistics.
LED-style pickup screen
- Displays tokens marked ready for collection, with their vendor outlet.
- Helps employees identify the appropriate counter for pickup and payment.
Example ordering flow
1. Admin registers a vendor and configures meal timings.
2. Vendor adds food items and available quantities.
3. Employee selects the vendor and an available meal window.
4. Employee places an order and receives a token.
5. Vendor prepares the order and marks it Ready.
6. The token appears on the pickup display.
7. Employee pays at the counter and collects the order; vendor marks it Served.
Demo access
The role selection screen offers Employee, Vendor, and Admin demo views. Enter any non-empty display name and ID to explore them. These are not authenticated accounts.
Role	Example name	Example ID
Employee	Priya Sharma	EMP1024
Vendor	Rahul Caterers	VEN001
Admin	Facility Admin	ADM001


The sample credentials are illustrative only. When meal ordering is closed, use the application's demo preview option to test the ordering flow.
Tech stack
- HTML5, CSS3, and vanilla JavaScript
- Browser localStorage for demonstration data
- Static site hosting on Netlify
Note: This published demo is not an Angular application and does not currently use a backend.
Run locally
Download or clone the repository and open index.html in a browser. No dependency installation or build step is required.
To deploy, upload the folder containing index.html to Netlify Drop.
Current limitations
This is a frontend-only portfolio prototype, not a production cafeteria platform:
- Role selection is simulated; there is no password verification or server-side authorization.
- Menu, inventory, and order data are stored in the current browser, not in a shared database.
- Multiple devices will not see the same orders or inventory. Browser tabs on the same origin can share local storage.
- Inventory changes are not transaction-safe across concurrent real users.
- The LED display is a browser view, not an integration with physical LED hardware.
- No online payment processing or verified counter payment integration is implemented.
A production version would require secure role-based login, a backend API, database, server-side inventory validation, real-time token updates, and audit trails.
Portfolio focus
This project demonstrates multi-role UX design, vendor-specific data flows, time-based menus, inventory status, and token-based counter pickup. It is suitable for showcasing frontend product thinking and interface development.
Live demo: https://sabra-food-ordering-system.netlify.app/
