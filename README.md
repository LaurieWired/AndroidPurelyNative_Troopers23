![Picture1](https://github.com/LaurieWired/AndroidPurelyNative_Troopers23/assets/123765654/d71f554e-6fa0-49ed-a604-3c1967462716)

# Beyond Java: Obfuscating Android Apps with Purely Native Code
During this talk I demonstrate how to use purely native code as an obfuscation technique in Android. Together, we rewrite a standard Android Java applicaiton in C++ and remove all traces of the entrypoint. We even mask our Android framework API calls by using direct Binder invocations and messages.

## Tools
- [JADX](https://github.com/skylot/jadx)
- [Android Studio](https://developer.android.com/studio)
  - Make sure the NDK is installed [Install and configure the NDK and CMake](https://developer.android.com/studio/projects/install-ndk)
- [Ghidra](https://ghidra-sre.org/)

## Link References
- Android samples soure code
  - https://github.com/vxunderground/MalwareSourceCode/tree/main/Android\

### Java Native Interface (JNI)
- [JNI Functions](https://docs.oracle.com/javase/7/docs/technotes/guides/jni/spec/functions.html)
- [JNI Types and Signatures](https://docs.oracle.com/javase/8/docs/technotes/guides/jni/spec/types.html#type_signatures)

### NativeActivity
- Android framework NativeActivity class
  - https://android.googlesource.com/platform/frameworks/base.git/+/master/core/java/android/app/NativeActivity.java 
- Rawdrawandroid
  - https://github.com/cnlohr/rawdrawandroid

### Android Source Code
- Binder
  - https://cs.android.com/android/kernel/superproject/+/common-android-mainline:common/drivers/android/binder.c 
- ServiceManager
  - https://cs.android.com/android/platform/superproject/+/master:frameworks/base/core/java/android/os/ServiceManager.java
