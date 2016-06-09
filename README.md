# ttwwiitt
hihi
buildscript {
  repositories {
    mavenCentral()
    maven { url 'https://maven.fabric.io/public' }
  }
  dependencies {
    classpath 'io.fabric.tools:gradle:1.+'
  }
}

apply plugin: 'io.fabric'

repositories {
  mavenCentral()
  maven { url 'https://maven.fabric.io/public' }
}

dependencies {
  compile('com.twitter.sdk.android:twitter:1.13.2@aar') {
    transitive = true
  }
}
