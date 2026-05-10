# Facility Handover App

Single-file Firebase-hosted Facility Handover web app for authenticated staff and admin-backed record review.

## Live App

https://facility-handover-cfc-bha.web.app

## Firebase Project

- Project ID: `facility-handover-8e0fc`
- Hosting site: `facility-handover-cfc-bha`

## Important Files

- `public/index.html` - app UI, auth gate, PDF export, Storage upload, and admin dashboard
- `public/assets/cfc-logo.jpg` - CFC logo used in the PDF report
- `firestore.rules` - Firestore access control
- `storage.rules` - private PDF Storage access control
- `firebase.json` - Firebase Hosting, Firestore, and Storage config

## Deploy

```bat
firebase deploy --only storage
firebase deploy --only firestore:rules
firebase deploy --only hosting
```

## Security Notes

Firebase browser config is public by design. Do not add service account keys, admin credentials, staff passwords, or API secrets to this repository.
