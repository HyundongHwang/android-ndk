<!-- TOC -->

- [apk 파일 다운로드](#apk-%ED%8C%8C%EC%9D%BC-%EB%8B%A4%EC%9A%B4%EB%A1%9C%EB%93%9C)
- [빌드](#%EB%B9%8C%EB%93%9C)
    - [빌드환경](#%EB%B9%8C%EB%93%9C%ED%99%98%EA%B2%BD)
    - [전체빌드, 설치 스크립트](#%EC%A0%84%EC%B2%B4%EB%B9%8C%EB%93%9C-%EC%84%A4%EC%B9%98-%EC%8A%A4%ED%81%AC%EB%A6%BD%ED%8A%B8)
    - [전체빌드 로그파일](#%EC%A0%84%EC%B2%B4%EB%B9%8C%EB%93%9C-%EB%A1%9C%EA%B7%B8%ED%8C%8C%EC%9D%BC)
- [original README.md](#original-readmemd)
    - [Build Steps](#build-steps)
    - [Debugging](#debugging)
    - [Support](#support)
    - [License](#license)

<!-- /TOC -->

<br>
<br>
<br>

# apk 파일 다운로드

- [/audio-echo/app/build/outputs/apk/release/app-release.apk](https://github.com/HyundongHwang/android-ndk/raw/master/audio-echo/app/build/outputs/apk/release/app-release.apk)
- [/bitmap-plasma/app/build/outputs/apk/release/app-release.apk](https://github.com/HyundongHwang/android-ndk/raw/master/bitmap-plasma/app/build/outputs/apk/release/app-release.apk)
- [/camera/basic/build/outputs/apk/release/basic-release.apk](https://github.com/HyundongHwang/android-ndk/raw/master/camera/basic/build/outputs/apk/release/basic-release.apk)
- [/camera/texture-view/build/outputs/apk/release/texture-view-release.apk](https://github.com/HyundongHwang/android-ndk/raw/master/camera/texture-view/build/outputs/apk/release/texture-view-release.apk)
- [/display-p3/image-view/build/outputs/apk/release/image-view-release.apk](https://github.com/HyundongHwang/android-ndk/raw/master/display-p3/image-view/build/outputs/apk/release/image-view-release.apk)
- [/endless-tunnel/app/build/outputs/apk/release/app-release.apk](https://github.com/HyundongHwang/android-ndk/raw/master/endless-tunnel/app/build/outputs/apk/release/app-release.apk)
- [/gles3jni/app/build/outputs/apk/release/app-release.apk](https://github.com/HyundongHwang/android-ndk/raw/master/gles3jni/app/build/outputs/apk/release/app-release.apk)
- [/hello-gl2/app/build/outputs/apk/release/app-release.apk](https://github.com/HyundongHwang/android-ndk/raw/master/hello-gl2/app/build/outputs/apk/release/app-release.apk)
- [/hello-jni/app/build/outputs/apk/arm/release/app-arm-release.apk](https://github.com/HyundongHwang/android-ndk/raw/master/hello-jni/app/build/outputs/apk/arm/release/app-arm-release.apk)
- [/hello-jni/app/build/outputs/apk/arm7/release/app-arm7-release.apk](https://github.com/HyundongHwang/android-ndk/raw/master/hello-jni/app/build/outputs/apk/arm7/release/app-arm7-release.apk)
- [/hello-jni/app/build/outputs/apk/arm8/release/app-arm8-release.apk](https://github.com/HyundongHwang/android-ndk/raw/master/hello-jni/app/build/outputs/apk/arm8/release/app-arm8-release.apk)
- [/hello-jni/app/build/outputs/apk/mips/release/app-mips-release.apk](https://github.com/HyundongHwang/android-ndk/raw/master/hello-jni/app/build/outputs/apk/mips/release/app-mips-release.apk)
- [/hello-jni/app/build/outputs/apk/universal/release/app-universal-release.apk](https://github.com/HyundongHwang/android-ndk/raw/master/hello-jni/app/build/outputs/apk/universal/release/app-universal-release.apk)
- [/hello-jni/app/build/outputs/apk/x86/release/app-x86-release.apk](https://github.com/HyundongHwang/android-ndk/raw/master/hello-jni/app/build/outputs/apk/x86/release/app-x86-release.apk)
- [/hello-jni/app/build/outputs/apk/x86_64/release/app-x86_64-release.apk](https://github.com/HyundongHwang/android-ndk/raw/master/hello-jni/app/build/outputs/apk/x86_64/release/app-x86_64-release.apk)
- [/hello-jniCallback/app/build/outputs/apk/release/app-release.apk](https://github.com/HyundongHwang/android-ndk/raw/master/hello-jniCallback/app/build/outputs/apk/release/app-release.apk)
- [/hello-libs/app/build/outputs/apk/release/app-release.apk](https://github.com/HyundongHwang/android-ndk/raw/master/hello-libs/app/build/outputs/apk/release/app-release.apk)
- [/hello-neon/app/build/outputs/apk/release/app-release.apk](https://github.com/HyundongHwang/android-ndk/raw/master/hello-neon/app/build/outputs/apk/release/app-release.apk)
- [/native-activity/app/build/outputs/apk/release/app-release.apk](https://github.com/HyundongHwang/android-ndk/raw/master/native-activity/app/build/outputs/apk/release/app-release.apk)
- [/native-audio/app/build/outputs/apk/release/app-release.apk](https://github.com/HyundongHwang/android-ndk/raw/master/native-audio/app/build/outputs/apk/release/app-release.apk)
- [/native-codec/app/build/outputs/apk/release/app-release.apk](https://github.com/HyundongHwang/android-ndk/raw/master/native-codec/app/build/outputs/apk/release/app-release.apk)
- [/native-media/app/build/outputs/apk/release/app-release.apk](https://github.com/HyundongHwang/android-ndk/raw/master/native-media/app/build/outputs/apk/release/app-release.apk)
- [/native-plasma/app/build/outputs/apk/release/app-release.apk](https://github.com/HyundongHwang/android-ndk/raw/master/native-plasma/app/build/outputs/apk/release/app-release.apk)
- [/san-angeles/app/build/outputs/apk/release/app-arm64-v8a-release.apk](https://github.com/HyundongHwang/android-ndk/raw/master/san-angeles/app/build/outputs/apk/release/app-arm64-v8a-release.apk)
- [/san-angeles/app/build/outputs/apk/release/app-armeabi-v7a-release.apk](https://github.com/HyundongHwang/android-ndk/raw/master/san-angeles/app/build/outputs/apk/release/app-armeabi-v7a-release.apk)
- [/san-angeles/app/build/outputs/apk/release/app-mips-release.apk](https://github.com/HyundongHwang/android-ndk/raw/master/san-angeles/app/build/outputs/apk/release/app-mips-release.apk)
- [/san-angeles/app/build/outputs/apk/release/app-x86-release.apk](https://github.com/HyundongHwang/android-ndk/raw/master/san-angeles/app/build/outputs/apk/release/app-x86-release.apk)
- [/teapots/choreographer-30fps/build/outputs/apk/release/choreographer-30fps-release.apk](https://github.com/HyundongHwang/android-ndk/raw/master/teapots/choreographer-30fps/build/outputs/apk/release/choreographer-30fps-release.apk)
- [/teapots/classic-teapot/build/outputs/apk/release/classic-teapot-release.apk](https://github.com/HyundongHwang/android-ndk/raw/master/teapots/classic-teapot/build/outputs/apk/release/classic-teapot-release.apk)
- [/teapots/more-teapots/build/outputs/apk/release/more-teapots-release.apk](https://github.com/HyundongHwang/android-ndk/raw/master/teapots/more-teapots/build/outputs/apk/release/more-teapots-release.apk)
- [/webp/view/build/outputs/apk/release/view-release.apk](https://github.com/HyundongHwang/android-ndk/raw/master/webp/view/build/outputs/apk/release/view-release.apk)


<br>
<br>
<br>


# 빌드

## 빌드환경
- Windows 10 64bit
- Gradle 4.4
- CMake	3.6.4111459
- lldb 3.0
- android

```groovy
android {
    compileSdkVersion 27
    buildToolsVersion "27.0.1"

    defaultConfig {
 		...       
 		minSdkVersion 19
        targetSdkVersion 27
		...
    }
    signingConfigs {
        release {
            storeFile file('../../debug.keystore')
            storePassword "android"
            keyAlias "androiddebugkey"
            keyPassword "android"
        }
    }
    buildTypes {
        release {
			...            
			signingConfig signingConfigs.release
        }
    }
	...
}
```

## 전체빌드, 설치 스크립트

```powershell
ls -Directory -Exclude ".*" | 
foreach { 
	write "`n`n`n`n`n`n`n`n`n`n"
	write "PROJECT DIR : $($_.FullName)"
	write "`n`n`n"
	cd $_.FullName
	./gradlew clean
	./gradlew assembleRelease --daemon --stacktrace
	
	ls "*-release.apk" -Recurse | 
	foreach { 
		write "`n`n`n"
		write "APK FILE PATH : $($_.FullName )"
		write "adb install ..."
		write "`n`n`n"
		adb install -r $_.FullName 
	}

	cd ..
} | tee -FilePath build.log
```

## 전체빌드 로그파일
- [/blob/master/build.log](https://github.com/HyundongHwang/android-ndk/blob/master/build.log)


<br>
<br>
<br>


# original README.md


NDK Samples
- NDK Samples [![Build Status](https://travis-ci.org/googlesamples/android-ndk.svg?branch=master)]
- (https://travis-ci.org/googlesamples/android-ndk) [![Build status](https://ci.appveyor.com/api/projects/status/48tbtqwg4heytmnq?svg=true)](https://ci.appveyor.com/project/proppy/android-ndk)

===========

This repository contains [Android NDK][0] samples with Android Studio [C++ integration](https://www.youtube.com/watch?v=f7ihSQ44WO0&feature=youtu.be).

These samples uses the new [CMake Android plugin](https://developer.android.com/studio/projects/add-native-code.html) with C++ support.

Samples could also be built with other build systems:
- for ndk-build with Android Studio, refer to directory [other-builds/ndkbuild](https://github.com/googlesamples/android-ndk/tree/master/other-builds/ndkbuild)
- for gradle-experimental plugin, refer to directory other-builds/experimental. Note that gradle-experiemental could not work with unified headers yet: use NDK version up to r15 and Android Studio up to version 2.3

Additional Android Studio samples:    
- [Google Play Game Samples with Android Studio](https://github.com/playgameservices/cpp-android-basic-samples)
- [Google Android Vulkan Tutorials](https://github.com/googlesamples/android-vulkan-tutorials)
- [Android Vulkan API Basic Samples](https://github.com/googlesamples/vulkan-basic-samples)
- [Android High Performance Audio](https://github.com/googlesamples/android-audio-high-performance)	

Documentation
- [Add Native Code to Your Project](https://developer.android.com/studio/projects/add-native-code.html)
- [CMake for NDK](https://developer.android.com/ndk/guides/cmake.html)
- [Hello-CMake Codelab](https://codelabs.developers.google.com/codelabs/android-studio-cmake/index.html)

Known Issues
- Some are documented at [Android Studio](http://tools.android.com/knownissues) page

For samples using `Android.mk` build system with `ndk-build` see the [android-mk](https://github.com/googlesamples/android-ndk/tree/android-mk) branch.

Build Steps
----------
- With Android Studio: use "Import Project(Eclipse ADT, Gradle, etc)" or "File" > "Import Project" option
- On Command Line/Terminal:  make sure set up ANDROID_HOME and ANDROID_NDK_HOME to local installation of SDK and NDK, then go to individual sample dir, and use "gradlew assembleDebug"

Debugging
---------
- [References](REFERENCE.md)
 
Support
-------

- [Google+ Community](https://plus.google.com/communities/105153134372062985968)
- [Stack Overflow](http://stackoverflow.com/questions/tagged/android)

If you've found an error in these samples, please [file an issue](https://github.com/googlesamples/android-ndk/issues/new).

Patches and new samples are encouraged, and may be submitted by [forking this project](https://github.com/googlesamples/android-ndk/fork) and
submitting a pull request through GitHub. Please see [CONTRIBUTING.md](CONTRIBUTING.md) for more details.

License
-------

Copyright 2015 The Android Open Source Project, Inc.

Licensed to the Apache Software Foundation (ASF) under one or more contributor
license agreements.  See the NOTICE file distributed with this work for
additional information regarding copyright ownership.  The ASF licenses this
file to you under the Apache License, Version 2.0 (the "License"); you may not
use this file except in compliance with the License.  You may obtain a copy of
the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.  See the
License for the specific language governing permissions and limitations under
the License.

[LICENSE](LICENSE)

[0]: https://developer.android.com/ndk
