Icons
==================
2016-11-23


Add svg icons to your website.



This library helps you integrating svg icons in your website.
It works best (only?) if all icons have same size, such as when they all come from the same icons library.


I created this helper to work mainly with [material icons](https://material.io/icons/)



How does it work?
-------------------

1. Include the Icons.php file and the IconsFactory.php file in your application

2. Configure IconsFactory.php (look in the script sections to generate the Factory from a simple svg file)

3. Css pass

If you are sure that your icons will always have the same characteristics, you can define them in css, like this for instance:


```css
.icon{
	width: 48px;
	height: 48px;
}		
```


4. Prepare your layout

Put this php code at the bottom of each html page that you generate.

```php
IconsFactory::printIconsDefinitions();
```


5. Use the icons when you want.

Now you're ready.

Whenever you need an icon, type the following in your html code:

```html
<?php Icons::printIcon('add'); ?>
```

You can change the color on the fly with the second argument:

```html
<?php Icons::printIcon('add', 'blue'); ?>
```

You can also change the size on the fly with the third argument:

```html
<?php Icons::printIcon('add', null, 48); ?>
```





 
 
History Log
------------------
    
- 1.0.0 -- 2016-12-24

    - separated IconsFactory from Icons

- ??? -- ???
	- initial commit    
