# RoomDataLib
[![](https://jitpack.io/v/dolevd2012/RoomDataLib.svg)](https://jitpack.io/#dolevd2012/RoomDataLib)

# Database Columns

![readme md](https://user-images.githubusercontent.com/74798510/99882821-da24e900-2c2b-11eb-8632-d46deb37b8d3.png)

## Requirement 
```minSdkVersion 23```



## Repository
Add this in your root build.gradle file (not your module build.gradle file):
```
allprojects {
	repositories {
		...
		maven { url "https://jitpack.io" }
	}
}
```

## Dependency
Add this to your module's build.gradle file (Note: version should match the jitpack badge above)
```
dependencies {
	implementation 'com.github.dolevd2012:RoomDataLib:1.00.01'
}
```
## Usage
Get the instance of RoomData:
```
RoomDB database;
database = RoomDB.getInstance(this);
```
