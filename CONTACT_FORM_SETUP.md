# Portfolio Contact Form Setup

The portfolio Contact Me section is powered by [FormSubmit](https://formsubmit.co/), replacing the previous Google Apps Script. It works with the existing GitHub Pages static hosting.

## One-time activation (required)

1. Once GitHub Pages deploys the updated site, open https://prabinr2004.github.io/#contact.
2. Fill out the form with a short test message using a sender email you can access.
3. Check **prabinroka2004@gmail.com** for a FormSubmit activation/confirmation email. Check spam if needed.
4. Click the **Activate/Confirm** link in that email. Only the mailbox owner can authorize the destination.
5. Submit a second test and verify it is actually received in the inbox.

**Important:** Until email confirmation is completed, mail delivery is not active. A visible thank-you page is not evidence that the destination inbox received the message.

## How it works

- HTML form POSTs to `https://formsubmit.co/prabinroka2004@gmail.com`.
- A hidden `_honey` field adds spam protection; FormSubmit's default CAPTCHA has **not** been disabled.
- The `_next` field redirects successful submissions to `thanks.html` on this same site.
- Visitors can also click the direct email link.
- No Google Apps Script, JavaScript fetch, API key, or separate backend is needed.

## If delivery stops

- Make sure the original FormSubmit activation link was confirmed.
- Check spam or promotions folders and test a new message.
- Verify that the `action` target and `_next` address in `index.html` are still accurate.
- See [FormSubmit help](https://formsubmit.co/help).
