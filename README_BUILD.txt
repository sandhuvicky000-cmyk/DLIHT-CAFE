D’LIGHT CAFE — ANDROID STUDIO WRAPPER PROJECT

BUILD APK
1. Extract the ZIP to a normal folder (not inside Downloads ZIP preview).
2. Open Android Studio.
3. Choose File > Open and select the extracted DLightCafe folder (the folder containing settings.gradle.kts).
4. Wait for Gradle Sync. If prompted, install Android SDK Platform 35 and use JDK 17.
5. Connect an Android phone with USB debugging enabled, or use an emulator.
6. For a test APK: Build > Build Bundle(s) / APK(s) > Build APK(s).
7. When the build finishes, click "locate" in the notification. APK is usually app/build/outputs/apk/debug/app-debug.apk.
8. Transfer app-debug.apk to your Android phone and install it. Allow installing unknown apps if Android asks.

INCLUDED
- Web menu, cart, checkout, special notes, location attachment, UPI intent, WhatsApp order flow.
- App label and native WebView shell.
- UPI ID configured in app.js: 9023020046@ybl.
- QR image is not included.

IMPORTANT TESTS / LIMITATIONS
- UPI payment is launched using a UPI intent. This app does not verify payment automatically.
- The customer must complete payment in their UPI app and the cafe must verify receipt independently.
- WhatsApp order text is prefilled; the customer must press Send.
- GPS requires user permission and device location enabled.
- Product photos and Google Fonts use internet, so first launch needs internet.
- Before public distribution, verify menu prices, delivery area/charge, coupon rules, WhatsApp number and UPI ID.
- This project builds a debug APK for testing. For Play Store/public release, create a signed release build.


LATEST UPDATE
- Increased top header spacing and enabled Android system-bar inset handling so the logo is not covered by status icons.
- Added a gentle original instrumental loop at low volume with an on-screen music toggle. Android WebView is configured for autoplay; some device/browser policies may still require the first tap on the music button.
- Added business address: Vijay Kumar, Near Civil Hospital, Sherpur. Delivery address is prefilled with Near Civil Hospital, Sherpur; customer can edit it.
- Rebuild the APK after opening this updated project and allowing Gradle Sync.


PREPAID UPI ORDER FLOW UPDATE
- Paid orders must complete the UPI payment step before WhatsApp order submission is enabled.
- UPI ID: 9023020046@ybl. The app launches a UPI payment intent with the exact payable amount and order reference.
- Customer returns to the app and enters the UPI transaction reference (UTR); only then does the app open WhatsApp with the order details and UTR.
- The VICKY coupon makes the order total ₹0 and skips payment. SANDHU46 remains free delivery on eligible orders.
- Static app cannot verify UPI settlement automatically. Cafe staff must verify the UTR/payment in the merchant bank/UPI app before preparing the order. Never ask customers for UPI PIN/OTP.


CHECKOUT UPDATE
- Removed all online payment / UPI / QR / UTR checkout options.
- Checkout now uses Cash on Delivery (COD) only. Order details open in WhatsApp after the customer submits.
- Removed the prefilled delivery address; the address field starts blank for the customer to enter.
