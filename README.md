# Android Accessibility

Things to find out:

1. Set a trait such as selected
2. Move focus to an element
3. Group content description on a container
4. Use a list so that a user now how many items there are



## Techniques

### Adding an accessibility label to an element


To add some text for an image, button or view set the android:contentDescription for the relevant view in your layout xml file

	android:contentDescription="@string/logo_alt"


If you have some furniture which doesn't require some text use @null so you don't get an error in link

	android:contentDescription="@null"


* [android:contentDescription | developer.android.com](http://developer.android.com/reference/android/view/View.html#attr_android:contentDescription)
* [Android Accessibility Solution in 30 Seconds](http://www.youtube.com/watch?v=OtwCe-YlD5k) - video by Ted Drake showing how to use contentDescription attribute


## Resources

* [Accessibility | developer.android.com](http://developer.android.com/guide/topics/ui/accessibility/index.html)
	* [Making Applications Accessible](http://developer.android.com/guide/topics/ui/accessibility/apps.html) 
	* [Accessibility Developer Checklist](http://developer.android.com/guide/topics/ui/accessibility/checklist.html)
	* [Building Accessibility Services](http://developer.android.com/guide/topics/ui/accessibility/services.html)