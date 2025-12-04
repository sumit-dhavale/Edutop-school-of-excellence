# Backend Implementation for School Website

## Information Gathered
- Current project is a static HTML/CSS/JS school website with pages like index.html, enquiry.html, gallery.html, etc.
- Enquiry form exists but is static (no backend submission).
- Gallery has hardcoded images; needs dynamic photo uploads.
- No backend or database yet.
- No admin panel or authentication.
- No notices system.

## Plan
- Set up Node.js/Express backend with MongoDB.
- Create models for Enquiries, Notices, and Photos.
- Implement authentication (JWT-based) for admin login.
- Build admin dashboard with routes for managing notices (add/edit/delete) and uploading photos.
- Update enquiry form to submit to backend and store in DB.
- Modify gallery to fetch photos from DB.
- Add a notices page/section to the public website to display notices.
- Ensure public website fetches data dynamically via API calls.

## Dependent Files to be edited
- New backend files: server.js, models/, routes/, middleware/, public/admin/ (for admin panel HTML).
- enquiry.html: Update form action to backend endpoint.
- gallery.html: Modify to load images from API.
- Add new public pages: notices.html.
- script.js: Add fetch calls for dynamic content.

## TODO Steps
- [ ] Install Node.js and npm if not present
- [ ] Initialize npm project and install dependencies (express, mongoose, multer, bcrypt, jsonwebtoken, cors, dotenv)
- [ ] Set up MongoDB connection
- [ ] Create server.js with basic Express setup
- [ ] Create models: Enquiry.js, Notice.js, Photo.js, Admin.js
- [ ] Create middleware: auth.js for JWT authentication
- [ ] Create routes: enquiries.js, notices.js, photos.js, auth.js
- [ ] Implement admin login/authentication
- [ ] Build admin dashboard HTML (public/admin/dashboard.html)
- [ ] Add CRUD routes for notices (add/edit/delete)
- [ ] Add photo upload route with multer
- [ ] Update enquiry.html form to submit via fetch to backend
- [ ] Modify gallery.html to fetch and display photos from API
- [ ] Create notices.html page for public website
- [ ] Update script.js with fetch calls for notices and gallery
- [ ] Test backend endpoints locally
- [ ] Verify admin panel functionality
- [ ] Verify public website dynamic content

## Followup Steps
- Deploy locally and test full integration.
- Add error handling and validation.
- Implement security measures (rate limiting, input sanitization).
- If needed, add email notifications for enquiries.
