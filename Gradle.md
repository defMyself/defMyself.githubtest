# Gradle

使用条件：

* jdk 8+



```kotlin
plugins {
    id('com.android.application') version '4.2.0-beta03'
}

repositories {
    google()
    mavenCentral()
}

android {
    compileSdkVersion 30
    defaultConfig {
        applicationId 'org.gradle.samples'
        minSdkVersion 30
        versionCode 1
        versionName '1.0'
        testInstrumentationRunner 'andrdoix.test.runner.AndroidJUnitRunner'
    }
    buildTypes {
        release {
            minifyEnabled false
            proguardFiles getDefaultProguardFile('proguard-android-optimize.txt'),  'proguard-rules.pro'
        }
    }
}

dependencies {
    implementation 'android.appcompat:appcompat:1.2.0'
    implementation 'com.google.android.material:material:1.2.0'
    implementation 'android.constraintlayout:constraintlayout:2.0.4'
    testImplementation 'junit:junit:4.13.1'
    androidTestImplementation 'android.test.ext:junit:1.1.2'
    androidTestImplementation 'android.test.espresso:espresso-core:3.3.0'
}
```

```shell
./gradlew build
```

构建Java应用程序

```shell
mkdir demo
cd demo
gradle init

```

gradle 选项

build script

* Groovy

* Kotlin



test framework

* JUnit 4
* TestNG
* Spock
* JUnit Jupiter



![image-20210505201809862](C:\Users\anxin\AppData\Roaming\Typora\typora-user-images\image-20210505201809862.png)





