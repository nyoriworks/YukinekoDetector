# YukinekoDetector Support

YukinekoDetector provides on-device AI image analysis through its Safari Web Extension and Share extension on iPhone, iPad, and Mac.

## Contact Support

To ask a question, report a problem, or request a feature, open a new ticket on the [YukinekoDetector support page](https://github.com/nyoriworks/YukinekoDetector/issues/new).

When reporting a problem, please include:

- Your device model and operating system version.
- The YukinekoDetector app version.
- Whether the problem occurs in Safari or the Share extension.
- The steps that reproduce the problem.
- A screenshot, if it does not contain private information.

Do not attach private or sensitive images. A substitute image that reproduces the problem is sufficient.

## Enable the Safari Extension

### iPhone and iPad

1. Install and open YukinekoDetector once.
2. Open the Safari extension settings in the Settings app.
3. Enable YukinekoDetector and allow it on the websites where you want to use it.
4. Return to Safari and reload the page.

### Mac

1. Install and open YukinekoDetector once.
2. In Safari, open **Settings > Extensions**.
3. Enable YukinekoDetector and grant access to the websites where you want to use it.
4. Reload the page.

## Common Questions

### Badges do not appear in Safari

- Open the YukinekoDetector toolbar panel and confirm that **Auto-Scan** is enabled.
- Confirm that at least one of the A or N badge options is enabled.
- Grant the extension access to the current website.
- Reload the page or select **Rescan Current Page Now**.

Some protected, temporary, or cross-origin media cannot be read by a browser extension. In that case, try sharing or selecting the original image directly.

### YukinekoDetector is missing from the Share sheet

Open the Share sheet, choose the option for editing extensions or actions, and enable YukinekoDetector. The exact label can vary by operating system version.

### A shared link cannot be read

Some apps share only text, a temporary link, or content that requires an authenticated session. If YukinekoDetector cannot retrieve an image from the link, save or share the original image directly.

### Results differ between images or devices

The score can change when a service supplies a resized, compressed, or cropped version of an image. For the most comparable result, analyze the same original image file on each device.

### Is a detection result definitive?

No. AI-likely and Non-AI-likely are estimates from an on-device model. They do not prove how an image was created and can be incorrect.

## Privacy

Analysis runs on the device. See the [YukinekoDetector Privacy Policy](Privacy.md) for details.

**Last updated: September 10, 2026**
