# ArticleInsight – Multi-Category Article Submission Website

This package is a complete static frontend for GitHub Pages with Firebase Authentication, Cloud Firestore and Firebase Storage.

## Firebase setup
1. Open Firebase Console for `articleinsight-e4f09`.
2. Authentication → Sign-in method → enable Email/Password.
3. Firestore Database → create database.
4. Storage → Get started.
5. Deploy `firestore.rules`, `storage.rules`, and `firestore.indexes.json` using Firebase CLI, or copy the rules in the Firebase Console.
6. Authentication → Settings → Authorized domains → add `articleinsight.github.io`.

## Make an admin
1. Register on the website.
2. In Firestore, open `users/{your-user-uid}`.
3. Change `role` from `author` to `admin`.
4. Log out and log back in.

## GitHub Pages
Upload all files to the repository root. In Settings → Pages, choose Deploy from branch, `main`, root folder.

## Important
The Firebase web API key is public by design. Security comes from the included Firestore and Storage rules. Never add service-account private keys to this repository.
