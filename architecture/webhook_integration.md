# SOP: Webhook Integration

## Goal
Connect the landing page booking form to the n8n backend for automated lead processing.

## Inputs
- Webhook URL: `https://n8n.srv1454268.hstgr.cloud/webhook-test/d276f42d-b4df-4071-ada2-aecb65410ee7`
- Form ID: `contactForm`

## Logic
1. Capture `submit` event on `contactForm`.
2. Extract data from inputs using `FormData`.
3. Map fields to JSON payload.
4. Send POST request to n8n.
5. Handle success (reset form, show alert) and errors (show alert, reset button).

## Edge Cases
- **Empty Fields:** Form uses `required` attribute.
- **Network Failure:** Show "Something went wrong" alert.
- **Slow Connection:** Disable button and show "Sending..." state.
