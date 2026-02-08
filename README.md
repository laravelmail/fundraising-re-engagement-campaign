# Fundraising Re Engagement Campaign

A professional email template for a fundraising re-engagement campaign aimed at current and potential donors of a non-profit organization.

![Thumbnail](./thumbnail.png)

## Template Details

- **Industries:** Non-Profit
- **Message Type:** Fundraising
- **Tags:** donation, support, re engagement

## Files
- `index.html`: The improved, localized, and branded HTML template.
- `template.blade.php`: Ready-to-use Laravel Blade template with `asset()` helpers.
- `assets/`: Directory containing localized images and styles used in the template.

## Usage in Laravel

### 1. Store the Template
Place the `index.html` content in a Blade view (e.g., `resources/views/emails/fundraising-re-engagement-campaign.blade.php`).

### 2. Handle Assets
Move the content of `assets/` to your public directory (e.g., `public/vendor/mail-templates/fundraising-re-engagement-campaign/`) and update the paths in the HTML to use the `asset()` helper.

### 3. Send Email
```php
Mail::to($user)->send(new \App\Mail\GenericEmail([
    'view' => 'emails.fundraising-re-engagement-campaign',
    'data' => [
        // Your dynamic data here
    ]
]));
```

---
*Created with ❤️ by **[LaravelMail.com](https://laravelmail.com)** - Your source for professional email templates.*
