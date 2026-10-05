# Firebase setup

Project: kaam-ka-saboot

The web app already contains the Firebase Web SDK configuration shown in the Firebase console screenshot.

Enabled providers:
- Email/Password
- Phone (OTP)

Firestore:
- Standard edition
- asia-south1 (Mumbai)
- Production mode

Required rules are in `firestore.rules`.

Important: the current UI stores proof metadata in Firestore. Actual photo/PDF/audio binary uploads require Firebase Storage to be enabled and its rules deployed. Do not put service-account private keys in the app.

For admin access, create an authenticated Firebase user for the admin and manually create `/admins/{uid}` in Firestore. Client-side password checks are intentionally not used.
