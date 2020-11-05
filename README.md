# Welcome 👋

## What's this?

Developers write better apps when they can [read the source](https://blog.codinghorror.com/learn-to-read-the-source-luke/). Unfortunately, the sources for the Android framework and various Google Android libraries are scattered all over the web.

This pages helps Android developers find the sources they're looking for.

## Can I help? 

You can improve this page and help the Android community by opening [an issue](https://github.com/pyricau/androidsrc/issues/new) or [a pull request](https://github.com/pyricau/androidsrc/edit/main/README.md) 🙏.

# Libraries

## Jetpack

* Most Jetpack libraries have sources available [on cs.android.com](https://cs.android.com/androidx/platform/frameworks/support) in the _androidx_ subproject.
  * [androidx.activity](https://cs.android.com/androidx/platform/frameworks/support/+/androidx-master-dev:activity/)
  * [Startup](https://cs.android.com/androidx/platform/frameworks/support/+/androidx-master-dev:startup/)
  * [Compose](https://cs.android.com/androidx/platform/frameworks/support/+/androidx-master-dev:compose/)
  * There's way more entries to add here.
* Jetpack libraries are also available on Github: [androidx/androidx](https://github.com/androidx/androidx)
  * Github contributions workflow is still experimental. See [contribution guide](https://github.com/androidx/androidx#contribution-guide)

## ConstraintLayout / MotionLayout

* Developed directly [on GitHub](https://github.com/androidx/constraintlayout), browsable on [cs.android.com](https://cs.android.com/androidx/constraintlayout/+/main:constraintlayout/).
  * The git history starts at 2.0.0, 1.x sources are available [here](https://cs.android.com/androidx/constraintlayout/+/main:constraintlayout/constraintlayout/src/main/java/androidx/constraintlayout/widget/ConstraintLayout.java).

## Espresso / Android Test

* Developed directly [on GitHub](https://github.com/android/android-test).

## Data Binding

* Available [on cs.android.com](https://cs.android.com/android/platform/superproject/+/studio-master-dev:tools/data-binding/extensions/library/src/main/java/androidx/databinding/) on the `studio-master-dev` branch and [on android.googlesource.com](https://android.googlesource.com/platform/frameworks/data-binding/+/refs/heads/mirror-goog-studio-master-dev/extensions/library/src/main/java/androidx/databinding) on the `mirror-goog-studio-master-dev` branch.
  * 👎🔎 Not searchable online: the `studio-master-dev` branch is not indexed.

## Dagger 2

* Developed directly [on GitHub](https://github.com/google/dagger).

# The Android Framework

* Available [on cs.android.com](https://cs.android.com/android/platform/superproject)
* View internals? See [View.java](https://cs.android.com/android/platform/superproject/+/master:frameworks/base/core/java/android/view/View.java).
* Activity lifecycle? See [ActivityThread.java](https://cs.android.com/android/platform/superproject/+/master:frameworks/base/core/java/android/app/ActivityThread.java).
* Art Runtime? See [class.cc](https://cs.android.com/android/platform/superproject/+/master:art/runtime/mirror/class.cc).

## What if it's a new version, sources not available yet?

* Start an emulator for the latest version.
* Run `adb pull /system/framework/framework.jar`.
* Unzip `framework.jar` (contains dexes).
* Use dex2jar to turn dexes into jars.
* Explore with [jd-gui](http://java-decompiler.github.io/) or IntelliJ (hack: add as a dependency)

# Android Studio

* Available [on cs.android.com](https://cs.android.com/android/platform/superproject/+/studio-master-dev:tools/adt/idea/) on the `studio-master-dev` branch.
  * 👎🔎 Not searchable online: the `studio-master-dev` branch is not indexed.

# Android Gradle Plugin (AGP)

* Available [on android.googlesource.com](https://android.googlesource.com/platform/tools/base/+/refs/heads/mirror-goog-studio-master-dev/build-system/) on the `mirror-goog-studio-master-dev` branch.
* [@jrodbx](https://github.com/jrodbx) dumped the sources for each release [on github](https://github.com/jrodbx/agp-sources).

# Kotlin

* Sources for the Kotlin compiler and standard lib are [on GitHub](https://github.com/JetBrains/kotlin)

# Firebase

* A subset of Firebase Android libraries have sources available [on GitHub](https://github.com/firebase/firebase-android-sdk), also browsable [on cs.opensource.google](https://cs.opensource.google/firebase-sdk/firebase-android-sdk).

# Google Play Services

* Play Services is not open source. I added this entry because people keep asking about it 😅.

# Android Open Source Project Code Review Tool

* A web-based code review system for projects that use Git. Available [on android-review.googlesource.com](https://android-review.googlesource.com/q/status:open+-is:wip)
