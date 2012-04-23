#ArcMenu

An android custom view which looks like the menu in [Path 2.0](https://path.com/) (for iOS).
Originally done by [daCapricorn](https://github.com/daCapricorn/ArcMenu).

![Preview](https://dl.dropbox.com/u/11369687/preview0.png)
![Preview](https://dl.dropbox.com/u/11369687/preview1.png)

##About

The user experience in [Path 2.0](https://path.com/) (for iOS) is amazing, but the android version miss much.

Just for fun, I try to realize the amazing menu for android, which could be equal to the iOS version's.

##Usage

To setup the menu:

``` java
ArcMenu menu = (ArcMenu) findViewById(R.id.arc_menu);

final int itemCount = ITEM_DRAWABLES.length;
for (int i = 0; i < itemCount; i++) {
     ImageView item = new ImageView(this);
     item.setImageResource(ITEM_DRAWABLES[i]);
     menu.addItem(item, null);// Add a menu item
}
```

If you want to change the default appearence:

in arc_menu.xml

    custom:childSize="50px"
    custom:fromDegrees="0.0"
    custom:toDegrees="300.0"

or in ArcMenu.java

``` java    
arcLayout.setChildSize(50);
arcLayout.setArc(0.0f, 300.0f);    
```

##Origin & More
**Original author: [Capricorn](https://github.com/daCapricorn/ArcMenu)**

**Forker: MrBuBBLs**

[GitHub](https://github.com/MrBuBBLs)
[Twitter](https://twitter.com/#!/MrBuBBLs)
[Google+](https://plus.google.com/111952807180188983777)





