Mukhi House Website
A static landing page for Mukhi House, a restored 1920 haveli museum in Hyderabad, Sindh. This page highlights the house’s history, gallery, virtual tour, and ticket booking options with both local and foreign pricing.

Features
Hero section with heritage-style branding and strong visitor CTA
About section with house history and restoration story
Gallery showcasing Mukhi House architecture and interiors
Embedded virtual tour iframe for remote visitors
Ticket booking form with:
Local visitor price: Rs 50 per person
Foreigner price: Rs 1000 per person
EmailJS integration for booking requests
mailto fallback when EmailJS is unavailable
Responsive design for desktop and mobile screens
Page Structure
mukhi-house-website.html: main single-page site with inline CSS and JavaScript
Gallery images are loaded through HTML and optional JavaScript overrides
Booking form uses client-side logic to calculate totals and send reservations
How to Use
Open mukhi-house-website.html in a browser.
Use the top navigation links to jump to About, Gallery, Virtual Tour, Visit, or Contact.
Fill in the booking form with your name, phone, email, visit date, visitor type, and ticket quantity.
Submit to send a reservation request.
Booking Rules
Local visitor tickets: Rs 50 each
Foreigner tickets: Rs 1000 each
Total is calculated immediately on the page
Reservation is sent by EmailJS if configured
If EmailJS fails or isn’t configured, a mailto draft opens addressed to esportsnexus233@gmail.com
EmailJS Setup
Create an EmailJS account at https://www.emailjs.com/
Add a service and template
Replace the placeholder IDs in the page script:
emailjs.init('YOUR_USER_ID')
EMAILJS_SERVICE_ID
EMAILJS_TEMPLATE_ID
Test the form to confirm email delivery
Customization
Change text content in the hero, about, and footer sections
Replace gallery image URLs directly in the HTML
Update the virtual tour URL if needed
Adjust ticket pricing values in the JavaScript logic if rules change
Notes
This is a client-side static page; no backend server is required
Browser cache may need a hard refresh after edits
The current email fallback ensures bookings can still be sent even without EmailJS configured
