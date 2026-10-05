# Kaam Ka Saboot — APK banane ka sabse aasaan tarika

Is package mein GitHub Actions workflow diya gaya hai. Iska kaam Android project banana aur APK automatically compile karna hai.

## Phone se karne ke steps

1. GitHub par ek naya **private repository** banaiye, naam: `kaam-ka-saboot`.
2. Is ZIP ko extract karke **andar ki saari files/folders** repository mein upload kijiye.
3. GitHub mein **Actions** tab kholiye.
4. `Build Kaam Ka Saboot APK` workflow select kijiye.
5. **Run workflow** dabaiye.
6. Build complete hone ke baad workflow ke **Artifacts** section mein `Kaam-Ka-Saboot-APK` milega.
7. Us artifact ko download karke ZIP kholiye. Andar `app-debug.apk` milega.
8. Android phone mein APK install kijiye.

## Important

- Firebase project/config already web app mein included hai.
- Firebase rules ko Firebase Console mein deploy karna alag step hai.
- Proof file ka binary upload abhi implemented nahi hai; current version proof metadata save karta hai.
- Debug APK testing ke liye hai. Play Store ke liye baad mein signed release/AAB banana hoga.
