# Cyprian Birthday Website

A responsive birthday landing page for Cyprian, born 19 October 2005. It includes:
- Modern navy/charcoal design with restrained gold accents
- Personal birthday message (photo placeholders removed)
- Gift button linking to https://cyprian.courtneytech.space
- Birthday-wish form design that does not publicly display submitted messages

## Important: connect the message form before publishing

The page is currently a static design. The message form does not deliver messages yet. This is intentional: it should not claim to send messages when no receiving service is configured.

### Easiest no-code option: Formspree
1. Create an account at https://formspree.io/ and create a new form.
2. Copy the form endpoint (it looks like `https://formspree.io/f/xxxxxxxx`).
3. Open `index.html` and replace the current `wishForm` submit handler script near the bottom with a real `fetch()` submission to that endpoint, or use Formspree's supplied HTML form integration.
4. Test a submission and confirm it arrives in your email/Formspree dashboard.
5. In Formspree settings, keep submissions private and enable spam protection.

Do not publish a form that merely shows a success message unless the backend confirms successful delivery.

## Publish with GitHub Pages
1. Create or open a repository.
2. Upload `index.html` to the repository root.
3. Open Settings → Pages.
4. Select deploy from branch, choose `main` and `/ (root)`, and save.
5. Wait for GitHub Pages to publish the URL.

For private messages, ensure your form provider sends submissions only to your account and never add private API keys to frontend HTML.
