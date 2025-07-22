# Netlify Forms Setup

If you're hosting on Netlify, you can use their built-in form handling:

## HTML Changes:
Replace the form tag with:
```html
<form name="contact" method="POST" data-netlify="true" netlify-honeypot="bot-field">
    <input type="hidden" name="form-name" value="contact" />
    <p style="display: none;">
        <label>Don't fill this out if you're human: <input name="bot-field" /></label>
    </p>
    <!-- rest of your form fields -->
</form>
```

## JavaScript Changes:
Update the form submission method to work with Netlify forms (no endpoint needed).
