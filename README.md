# Merged Manifest Bug

This project illustrates the bug in Android Studio where Merged Manifest doesn't show contributions
from transitive dependencies.

The `app` module depends on `mylibrary` which in turn depends on Work Manager. Work Manager has
several components added to the `AndroidManifest.xml` file including permissions, Content Providers,
Services and Broadcast Receivers. However, as seen in the screenshot, none of those are visible in
the merged manifest view for the app's `AndroidManifest.xml`.

![Screenshot](ScreenShot.png)
