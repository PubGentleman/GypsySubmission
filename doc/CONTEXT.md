# Project Context

## Property Submission Form

The project includes a property submission form (`property-form.html`) that allows users to submit property listings. The form features:

### Features
- Modern, responsive UI using Tailwind CSS
- Form validation for required fields
- Support for multiple photo uploads
- Success message feedback
- Form data submission via FormData API
- Zelle payment integration
- Multiple posting options with different pricing tiers

### Form Fields
- Name
- Email
- Phone Number
- Property Address
- Property Type (Apartment/House/Condo)
- Price
- Description
- Photo Uploads (multiple)
- Zelle Payment Screenshot
- Post Type Selection
- Boost Options

### Posting Options
1. Basic Listing Post ($25)
   - One-time IG story or single post
2. Premium Post ($50)
   - Multi-platform: IG, TikTok, Facebook Group
3. Featured Post ($100)
   - Pinned for 48-72 hours
4. Featured Post with Paid Ads ($150)
5. Video Walkthrough/Custom Ad Creation ($250)

### Boost Options
- None
- Instagram Boost ($50)
- Facebook Boost ($50)
- TikTok Boost ($50)
- All Platforms Boost ($120)

### Technical Details
- Uses Tailwind CSS via CDN for styling
- Form submission handled via fetch API
- Endpoint: `/submit-property`
- Supports multipart/form-data for file uploads
- Zelle payment integration (number: 3473612229)

### Backend Requirements
The form expects a backend endpoint at `/submit-property` that can handle:
- POST requests
- Multipart form data
- File uploads (photos and payment proof)
- JSON response for success/failure
- Payment verification
- Post type and boost option processing
