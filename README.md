 <!--
This README describes the package. If you publish this package to pub.dev,
this README's contents appear on the landing page for your package.

For information about how to write a good package README, see the guide for
[writing package pages](https://dart.dev/guides/libraries/writing-package-pages).

For general information about developing packages, see the Dart guide for
[creating packages](https://dart.dev/guides/libraries/create-library-packages)
and the Flutter guide for
[developing packages and plugins](https://flutter.dev/developing-packages).
-->
 
## _Bottom_ _Navigation_ _Bar_ 

The botton_nav_bar library is a custom implementation of the bottom navigation bar in Flutter. The library provides a customizable bottom navigation bar widget that allows users to navigate between different screens in an application. It is built to be flexible and can be adapted to fit any app's design

The botton_nav_bar library includes two main classes:

BottomBarItem: A model class that represents a single item in the bottom navigation bar. The BottomBarItem class has several parameters, including the screen to be displayed when the item is selected, the icon to be displayed when the item is not selected, the selected icon to be displayed when the item is selected, and the label to be displayed for the item.

BottomNavBar: A stateful widget that represents the bottom navigation bar. The BottomNavBar widget takes a list of BottomBarItem objects as input and displays them as a row of items. The widget also includes a floating action button that can be customized with an icon, label, and color.

The BottomNavBar widget allows users to customize several aspects of the bottom navigation bar, including the size and color of the icons and labels, the location of the floating action button, and the font weight of the item label

## _BottomBarItem_ _Parameters_
The BottomBarItem class has the following parameters:

screen: A Widget representing the screen that should be displayed when this item is selected.
icon: A Widget representing the unselected icon for this item.
label: A String representing the label to be displayed below this item.
selectedIcon: An IconData representing the selected icon for this item.

centerDockedTitle: A String representing the title to be displayed in the center of the bottom navigation bar.

bottomItemSelectedColor: A Color representing the color of the selected item in the bottom navigation bar

bottomItemUnSelectedColor: A Color representing the color of the unselected items in the bottom navigation bar

bottomItems: A list of BottomBarItem objects that are used to define the items in the bottom navigation bar.

fabChild: A widget that represents the label of the floating action button (FAB).

fabBackGroundColor: The background color of the FAB.

bottomNavBarColor: The background color of the bottom navigation bar.

floatingActionButtonLocation: The location of the FAB on the screen.

fabIcon: The icon that represents the FAB.

fabElevation: The elevation of the FAB.

fabHeight: The height of the FAB.

fabWidth: The width of the FAB.

bottomNavItemSelectedIconSize: The size of the icon when a bottom navigation bar item is selected.

bottomNavItemunSelectedIconSize: The size of the icon when a bottom navigation bar item is unselected.

bottomNavItemSelectedLabelSize: The font size of the label when a bottom navigation bar item is selected.

bottomNavItemLabelHeight: The height of the label of a bottom navigation bar item.

bottomNavItemIconHeight: The height of the icon of a bottom navigation bar item.

bottomNavItemunSelectedLabelSize: The font size of the label when a bottom navigation bar item is unselected.

bottomNavItemHeight: The height of a bottom navigation bar item.

bottomItemLabelFontWeight: The font weight of the label of a bottom navigation bar item.

onPressFAB: A function that is called when the FAB is pressed.

These parameters can be used to customize and configure the bottom navigation bar and FAB for a package in Dart.
 

 
## _Features_
. Customizable bottom navigation bar.
. Supports floating action button.
. Easy to implement.
. Comes with a demo application.

 
## _Getting_ _started_
```dart
dependencies:
  botton_nav_bar: ^0.1.1
```
 

## _Package_ _Implementation_
```dart
import 'package:bottom_navy_bar/bottom_navy_bar.dart';

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) => Scaffold(
        drawer: const DrawerWidget(),
        body: BottomNavBar(
          bottomItems: <BottomBarItem>[
            BottomBarItem(
              selectedColor: Colors.green,
              label: 'Screen 1',
              screen: const HomeScreen(),
              selectedIcon: Icons.collections_bookmark_outlined,
            ),
            BottomBarItem(
              selectedColor: Colors.red,
              label: 'Screen 2',
              screen: const SearchScreen(),
              selectedIcon: Icons.search_rounded,
            ),
            BottomBarItem(
              selectedColor: Colors.amber,
              label: 'Screen 3',
              selectedIcon: Icons.menu_open_rounded,
              screen: const Screen3(),
            ),
            BottomBarItem(
              selectedColor: Colors.grey,
              label: 'Screen 4',
              screen: const Screen4(),
              selectedIcon: Icons.notifications_active,
            )
          ],
        ),
      );}
```
  


 
## _Additional_ _information_
For more information, check out the botton_nav_bar package on pub.dev.

In this example, the BottomNavBar widget includes four items:  When the user selects an item, the corresponding screen is displayed.

Overall, the botton_nav_bar library provides a convenient and customizable way to implement a bottom navigation bar in a Flutter application.



 

 
