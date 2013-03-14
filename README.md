# Android Accessibility

Things to find out:

1. Set a trait such as selected
2. Move focus to an element
3. Group content description on a container
4. Use a list so that a user knows how many items there are
5. How to use the D-pad



## Notes

* Explore by touch was added in Android 4.0


## Techniques

### Adding an accessibility label to an element


To add some text for an image, button or view set the android:contentDescription to the relevant view in your layout xml file

	android:contentDescription="@string/logo_alt"

There is also a method for doing this

	public void setContentDescription (CharSequence contentDescription)


If you have some furniture which doesn't require some text use @null so you don't get an error in link

	android:contentDescription="@null"

* [android:contentDescription](http://developer.android.com/reference/android/view/View.html#attr_android:contentDescription)
* [setContentDescription](http://developer.android.com/reference/android/view/View.html#setContentDescription(java.lang.CharSequence)
* [Android Accessibility Solution in 30 Seconds](http://www.youtube.com/watch?v=OtwCe-YlD5k) - video by Ted Drake showing how to use contentDescription attribute

### Making a view focusable

If a view is not focusable by default you can make it focusable from the XML layout file by setting the android:focusable attribute to "true"

	android:focusable="true"

There are also a methods for doing this

	setFocusable(boolean)
	setFocusableInTouchMode(boolean)
	
* [android:focusable](http://developer.android.com/reference/android/view/View.html#attr_android:focusable)
* [setFocusable](http://developer.android.com/reference/android/view/View.html#setFocusable%28boolean%29)
* [attr_android:focusableInTouchMode](http://developer.android.com/reference/android/view/View.html#attr_android:focusableInTouchMode)
* [setFocusableInTouchMode](http://developer.android.com/reference/android/view/View.html#setFocusableInTouchMode(boolean))

### Controlling focus order

You can provide explicit overrides to the ordering using the following XML attributes in the layout file

* android:nextFocusDown - Defines the next view to receive focus when the user navigates down.
* android:nextFocusLeft - Defines the next view to receive focus when the user navigates left.
* android:nextFocusRight - Defines the next view to receive focus when the user navigates right.
* android:nextFocusUp - Defines the next view to receive focus when the user navigates up.

For more detail see: [Controlling focus order](http://developer.vodafone.com/smartaccess2012/designing_for_accessibility/#FocusOrder)



## Resources

### Google Documentation
* [Accessibility | Patterns](http://developer.android.com/design/patterns/accessibility.html)
* [Accessibility | developer.android.com](http://developer.android.com/guide/topics/ui/accessibility/index.html)
	* [Making Applications Accessible](http://developer.android.com/guide/topics/ui/accessibility/apps.html) 
	* [Accessibility Developer Checklist](http://developer.android.com/guide/topics/ui/accessibility/checklist.html)
	* [Building Accessibility Services](http://developer.android.com/guide/topics/ui/accessibility/services.html)
* [Implementing Accessibility | Training](http://developer.android.com/training/accessibility/index.html)
	* [Developing Accessible Applications](http://developer.android.com/training/accessibility/accessible-app.html)
	* [Developing an Accessibility Service](http://developer.android.com/training/accessibility/service.html)
* [android.view.accessibility](http://developer.android.com/reference/android/view/accessibility/package-summary.html)
* [AccessibilityEvent ](http://developer.android.com/reference/android/view/accessibility/AccessibilityEvent.html)
* [AccessibilityEventSource](http://developer.android.com/reference/android/view/accessibility/AccessibilityEventSource.html)

### Forums
* [eyes-free](https://groups.google.com/forum/?fromgroups#!forum/eyes-free)

### Articles
* [Take These Steps to Make your Android App Accessible](http://www.grokkingandroid.com/steps-to-making-android-app-accessible/)
* [Vodaphone Developers Blog: Designing for Accessibility (Android)](http://developer.vodafone.com/smartaccess2012/designing_for_accessibility/)
* [Making Android apps voice output accessible](http://www.netmagazine.com/tutorials/making-android-apps-voice-output-accessible) - by Henny Swan
* [Android Developers Blog: Accessibility: Are You Serving All Your Users?](http://android-developers.blogspot.co.uk/2012/04/accessibility-are-you-serving-all-your.html)
* [Implementing Accessibility on Android](http://www.apps4android.org/?p=3628)
* [Top 7 Android Accessibility Features](http://www.developer.com/ws/android/development-tools/top-7-android-accessibility-features.html)

### Blogs
* [Android developers blog - tag:accessibility](http://android-developers.blogspot.co.uk/search/label/accessibility)
* [Henny Swan bog - tag:android](http://www.iheni.com/tag/android)
* [Eyes-Free Android](http://eyes-free.blogspot.co.uk/)

### Presentations / Slides
* [TalkBack & Magnification Accessibility in Android 4.2+](http://pauljadam.com/androida11y/)
* [Leveraging Android Accessibility APIs To Create An Accessible Experience](http://static.googleusercontent.com/external_content/untrusted_dlcp/www.google.com/en//events/io/2011/static/notesfiles/LeveragingAndroidAccessibilityAPIsToCreateAnAccessibleExperience.pdf)

### Videos
* [YouTube Channel: EyesFreeAndriod](http://www.youtube.com/user/EyesFreeAndroid?feature=watch)
* [Google I/O 2011: Leveraging Android Accessibility APIs To Create An Accessible Experience](http://www.youtube.com/watch?v=BPXqsPeCneA)
* [Google I/O 2012 - Making Android Apps Accessible](http://www.youtube.com/watch?v=q3HliaMjL38)
* [Developing with Accessibility - 2 day event](http://www.fcc.gov/events/developing-accessibility)

### Misc
* [Android Accessibility | http://eyes-free.googlecode.com/](http://eyes-free.googlecode.com/svn/trunk/documentation/android_access/index.html)
* [apps4android](http://www.apps4android.org/)








