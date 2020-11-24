# RoomDataLib
[![](https://jitpack.io/v/dolevd2012/RoomDataLib.svg)](https://jitpack.io/#dolevd2012/RoomDataLib)
![](https://img.shields.io/github/license/dolevd2012/RoomDataLib?color=blue)
![](https://img.shields.io/github/issues/dolevd2012/RoomDataLib?color=purple)


# DESCRIPTION
1.This lib makes it easy to transfer data in our activities using database unlike sharedPref that requires coding in each activity

2.Easy way to store huge amount of data


# Database Columns

![MainData](https://user-images.githubusercontent.com/74798510/100033073-13af4d00-2e02-11eb-8bb2-a93f07936503.png))

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
	implementation 'com.github.dolevd2012:RoomDataLib:1.01.01'
}
```
## Usage
Get the instance of RoomData:
```
RoomDB database;
database = RoomDB.getInstance(this);
```
## Creating class + adding attributes
```
MainData data = new MainData();
data.setString("Any String you want"); 
```
Default value is empty String

```
MainData data = new MainData();
data.setNumber("Any int you want"); 
```
Default value is -1

```
MainData data = new MainData();
data.setID("Any int you want"); 
```
i do not recommend doing that because you may 
override another MainData in your database

## Adding the MainData to the database
```
database.mainDao().insert(data);
```
# Queries we can use 
![query](https://user-images.githubusercontent.com/74798510/100033111-2cb7fe00-2e02-11eb-83e0-60f0a6598eff.png)
