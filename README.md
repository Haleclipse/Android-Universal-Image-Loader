# ![Logo](https://github.com/nostra13/Android-Universal-Image-Loader/raw/master/sample/src/main/res/drawable-mdpi/ic_launcher.png) Universal Image Loader

Sadly UIL no longer updated by it's author. I made some changes based on requirements for my own project.

Add JitPack repository to root `build.gradle`
```Gradle
allprojects {
    repositories {
        maven { url "https://jitpack.io" }
    }
}
```
Add the dependency
```Gradle
dependencies {
    compile 'com.github.danimahardhika:Android-Universal-Image-Loader:056f384091@aar'
}
```

### 21/04/2017
* Fixed bitmap still in use get recycled

### 16/04/2017 
* Code cleanup
* Updated dependency
* Updated gradle, target sdk, compile sdk
* Added new scheme for `package://` to load installed app icon from package name
* DisplayImageOptions.showImageOnLoading(), DisplayImageOptions.showImageForEmptyUri(), and DisplayImageOptions.showImageOnFail() supports vector drawable
* Changed min sdk to API 9

## Acceptable URIs examples
```java
"http://site.com/image.png" // from Web
"file:///mnt/sdcard/image.png" // from SD card
"file:///mnt/sdcard/video.mp4" // from SD card (video thumbnail)
"content://media/external/images/media/13" // from content provider
"content://media/external/video/media/13" // from content provider (video thumbnail)
"assets://image.png" // from assets
"drawable://" + R.drawable.img // from drawables (non-9patch images)
"package://com.app.package.name" // from installed package name
```

## Donation
You can support the project and thank the author for his hard work :)

<a href='https://pledgie.com/campaigns/19144'><img alt='Click here to lend your support to: Universal Image Loader for Android and make a donation at pledgie.com !' src='https://pledgie.com/campaigns/19144.png?skin_name=chrome' border='0' ></a> <a href="http://flattr.com/thing/1110177/nostra13Android-Universal-Image-Loader-on-GitHub" target="_blank"><img src="http://api.flattr.com/button/flattr-badge-large.png" alt="Flattr this" title="Flattr this" border="0" /></a>
* **PayPal** - nostra.uil[at]gmail[dot]com

## License

    Copyright 2011-2015 Sergey Tarasevich

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
