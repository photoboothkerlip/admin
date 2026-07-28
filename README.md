# admin
# Kerlip Photobooth Booking

## Firebase setup

1. In Firebase Console, open **Authentication > Sign-in method** and enable **Email/Password**.
2. Open **Authentication > Users** and create the admin account(s). Do not add public sign-up to this app.
3. Deploy the Firestore rules with `firebase deploy --only firestore:rules`, or paste `firestore.rules` into **Firestore Database > Rules** and publish it.

The app only permits signed-in Firebase Authentication users to access `kerlipApp/mainData`; all other Firestore paths are denied.
