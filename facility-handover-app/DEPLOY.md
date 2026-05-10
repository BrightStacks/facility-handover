# Facility Handover Firebase Deploy

Open Command Prompt in this folder:

```bat
C:\Users\dylan\Documents\New project\facility-handover-app
```

Then run:

```bat
firebase login
firebase deploy --only firestore:rules
firebase deploy --only storage
firebase deploy --only hosting
```

Expected Hosting URL:

```text
https://facility-handover-cfc-bha.web.app
```

If Firebase says the hosting site does not exist yet, create the Hosting site
`facility-handover-cfc-bha` in the Firebase Console, then run deploy again.

Cloud Storage is now used for private PDF storage. Export uploads the PDF,
saves Firestore metadata, then signs the user out after successful export.
