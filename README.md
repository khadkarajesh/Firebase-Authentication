# firebase-auth [![](https://jitpack.io/v/khadkarajesh/firebase-auth.svg)](https://jitpack.io/#khadkarajesh/firebase-auth)
Library contains the following features:
1. Authentication using email
2. Authentication using social media(facebook, gmail)
3. Forgot password
4. User logout

# To get a Git project into your build:

Step 1.
Add it in your root build.gradle at the end of repositories:
```gradle
   allprojects {
    repositories {
        maven { url 'https://jitpack.io' }
    }
   }
```
Step 2.
Add the dependency
```gradle
   implementation 'com.github.khadkarajesh:firebase-auth:v0.1.0-alpha'
```
Step 3.
```kotlin
   class App : Application(){
    override fun onCreate() {
        super.onCreate()
        Auth.init(this, "Web client ID from firebase console")
    }
}
```
Step 4.
Keep google-services.json in app/ directory

Step 5. 
dependencies {
        classpath 'com.google.gms:google-services:4.0.1'
 }
 
Step 6.
in app level build.gradle
```kotlin
   dependencies {}
   apply plugin: 'com.google.gms.google-services'
```
 
