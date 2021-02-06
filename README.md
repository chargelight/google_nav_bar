# google_nav_bar


<img src="https://forthebadge.com/images/badges/built-with-love.svg" height="28px" />&nbsp;&nbsp;<img src="https://img.shields.io/badge/license-MIT-green?style=for-the-badge" height="28px" />&nbsp;&nbsp;<a href="https://pub.dev/packages/google_nav_bar"><img src="https://img.shields.io/pub/v/google_nav_bar.svg?style=for-the-badge" height="28px" /></a>

A modern google style nav bar for flutter.

![demo](https://user-images.githubusercontent.com/13378059/90664650-7df1a800-e27d-11ea-8c41-0fd79bc8de07.gif)

![google_nav_bar](https://user-images.githubusercontent.com/13378059/107119103-f0038b00-68b7-11eb-980a-66880c7d8c36.gif)


GoogleNavBar is a Flutter widget designed by [Aurelien Salomon](https://dribbble.com/shots/5925052-Google-Bottom-Bar-Navigation-Pattern/) and developed by [sooxt98](https://www.instagram.com/sooxt98/).


## Getting Started

Add this to your package's `pubspec.yaml` file:
```
...
dependencies:
  google_nav_bar: ^4.0.0
  
```

Now in your Dart code, you can use:
```
import 'package:google_nav_bar/google_nav_bar.dart';
```

## Usage

Style your tab globally with GNav's attribute, if you wish to style tab separately, use GButton's attribute

``` dart
GNav(
  tabBorderRadius: 15, 
  tabActiveBorder: Border.all(color: Colors.black, width: 1), // tab button border
  tabBorder: Border.all(color: Colors.grey, width: 1), // tab button border
  tabShadow: [BoxShadow(color: Colors.grey.withOpacity(0.5), blurRadius: 8)], // tab button shadow
  curve: Curves.easeOutExpo, // tab animation curves
  duration: Duration(milliseconds: 900), // tab animation duration
  gap: 8, // the tab button gap between icon and text 
  color: Colors.grey[800], // unselected icon color
  activeColor: Colors.purple, // selected icon and text color
  iconSize: 24, // tab button icon size
  tabBackgroundColor: Colors.purple.withOpacity(0.1), // selected tab background color
  padding: EdgeInsets.symmetric(horizontal: 20, vertical: 5), // navigation bar padding
  tabs: [
    GButton(
      icon: LineIcons.home,
      text: 'Home',
    ),
    GButton(
      icon: LineIcons.heart_o,
      text: 'Likes',
    ),
    GButton(
      icon: LineIcons.search,
      text: 'Search',
    ),
    GButton(
      icon: LineIcons.user,
      text: 'Profile',
    )
  ]
)
```

View the example folder

There are 4 different use case included in the /example directory, go try it out!