plugins {
    id 'com.android.application'
}

android {
    namespace 'com.ghostwars.game'
    compileSdk 33

    defaultConfig {
        applicationId "com.ghostwars.game"
        minSdk 21
        targetSdk 33
        versionCode 1
        versionName "1.0"
    }
    buildTypes {
        release {
            minifyEnabled false
            proguardFiles getDefaultProguardFile('proguard-android-optimize.txt'), 'proguard-rules.pro'
        }
    }
}

dependencies {
    implementation 'androidx.appcompat:appcompat:1.5.1'
}<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:background="#121212"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:padding="20dp">

    <TextView
        android:id="@+id/gameTitle"
        android:text="حرب الأشباح - Ghost Wars"
        android:textColor="#FFFFFF"
        android:textSize="24sp"
        android:layout_centerHorizontal="true"
        android:layout_marginTop="10dp" />

    <TextView
        android:id="@+id/tvCoins"
        android:text="العملات: 0"
        android:textColor="#FFFFFF"
        android:textSize="18sp"
        android:layout_below="@id/gameTitle"
        android:layout_marginTop="30dp"
        android:layout_centerHorizontal="true" />

    <Button
        android:id="@+id/btnWatchAd"
        android:text="شاهد إعلان +10 عملات"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_below="@id/tvCoins"
        android:layout_centerHorizontal="true"
        android:layout_marginTop="30dp" />

    <Button
        android:id="@+id/btnDailyReward"
        android:text="مكافأة يومية +50 عملة"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_below="@id/btnWatchAd"
        android:layout_centerHorizontal="true"
        android:layout_marginTop="20dp" />

    <Button
        android:id="@+id/btnOpenShop"
        android:text="فتح متجر الأسلحة"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_below="@id/btnDailyReward"
        android:layout_centerHorizontal="true"
        android:layout_marginTop="20dp" />

</RelativeLayout>
