# EmailJS Setup Instructions

EmailJS allows you to send emails directly from client-side JavaScript without a backend.

## Steps:

1. Sign up at https://www.emailjs.com/
2. Create a service (Gmail, Outlook, etc.)
3. Create an email template
4. Get your Service ID, Template ID, and Public Key

## HTML Addition:
Add EmailJS script before closing body tag:
```html
<script src="https://cdn.jsdelivr.net/npm/@emailjs/browser@3/dist/email.min.js"></script>
```

## JavaScript Implementation:
Replace the simulateFormSubmission method with EmailJS integration.

Example template variables for EmailJS:
- {{from_name}} - sender's name
- {{from_email}} - sender's email  
- {{subject}} - message subject
- {{message}} - message content
- {{to_email}} - your email (jimueleligio@gmail.com)
