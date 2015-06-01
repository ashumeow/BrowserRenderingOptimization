```
View Types:-

1. Select View
2. Style View
3. Position View
```
```
These three views are seen in,
-- Text view
-- Image view
-- Button view
```
```xml
Text view:

<TextView
android:text="Happy Birthday!"
android:background="@android:color/darker_gray"
android:layout_width="150dp"
android:layout_height="75dp" />

My observations: (Pop-quiz)
android:text => display text
android:background => display background
@android:color => color
android:layout_width => width measurement
android:layout_height => height measurement

Teacher's observations:
-- weird angle brackets
-- Don't know what "android.text" means
-- Says Happy Birthday, which appears on phone
-- Has height and width
```
```xml
Explaining the XML syntax:
<TextView
android:text="Happy Birthday!"
android:background="@android:color/darker_gray"
android:layout_width="150dp"
android:layout_height="75dp" />

Element:
<TextView /> => self-closing tag
<TextView></TextView> => separate opening/closing tags

Attributes (View names/attribute names) of the TextView element:
android:text
android:background
android:layout_width
android:layout_height

Attribute values:
"Happy Birthday!"
"@android:color/darker_gray"
"150dp"
"75dp"
```
```xml
Example:-

<LinearLayout
android:layout_width="wrap_content"
android:layout_height="wrap_content"
android:orientation="vertical">

<TextView
android:text="Happy Birthday"
android:layout_width="wrap_content"
android:layout_height="wrap_content" />

<TextView
android:text="You're the best!"
android:layout_width="wrap_content"
android:layout_height="wrap_content" />

</LinearLayout>

<LinearLayout> is the parent element of 2 <TextView> tags,
where the 2 <TextView> tags are the children.
```
```
XML Visualizer

(github src: https://github.com/udacity/android-layout/tree/gh-pages)
(github view: http://udacity.github.io/android-layout)

"150dp" => dp = Density Independent Pixels

Why dp??

Take screen types in devices,
-- Medium Resolution device
-- High resolution device
-- Extra high resolution device

In different devices,
The pixel size varies where the users needs to be able to tap the button.
```
