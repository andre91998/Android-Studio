# Building your First User Interface

## Important Concepts

* The user interface (UI) for an Android app is built as a hierarchy of layouts and widgets:

  * **Layouts** are **ViewGroup objects** (containers that control how their child views are positioned on the screen)

  * **Widgets** are **View objects** (UI components such as buttons and text boxes)
  
  * **ConstraintLayout** is a layout that defines the position for each view based on constraints to sibling views and the parent layout. In  this way, you can create both simple and complex layouts with a flat view hierarchy. This type of layout avoids the need for nested layouts. A nested layout, which is a layout inside a layout, as shown in figure 2, can increase the time required to draw the UI.

* Android Studio UIs are defined in XML files, which can be written or automatically generated with Android Studio's Layout Editor (used in this tutorial)

## The Idea

For our first User Interface, we're going to build a simple app that accepts a message, has a button to send the message, and displays the message that is sent.

## The Layout Editor Sections

* The **Palette** panel at on the top left presents the available default objects that can be easily placed in your *blueprint* by dragging and dropping

* The **Component Tree** panel on the bottom left shows the layout's *hierarchy* of views. In this case, the root view is a **ConstraintLayout** (see in important concepts), which contains just one **TextView** object.

* The **Attributes** panel on the right shows all the attributes of the selected object in the editor.

* The **Design Editor** in the center is where things can be easily edited. At the top of this section you have a *toolbar* which presents the following sections:
  * Top Row:
    * **Select Design Surface**: for selecting whether you want to view the *blueprint* (for editing position and constraints), the *design* (for previewing the app), or both.
    * **Orientation for Preview**: for selecting whether you are working with *portrait*, *landscape*, or both.
    * **Device for Preview**: for selecting screen configurations based on the device you are using for testing.
    * **API Version for Preview**: for setting the API you want to use (will probably be automatically set to the best possible API).
  * Bottom Row:
    * **View Options**
    * **Autoconnection to Parent**: When turned on, it automatically creates two or more constraints for each view as you add them to the layout, but only when appropriate to constrain the view to the parent layout.
    * **Default Margins**: for defining the margin between the edge of the device screen and your views

## App Layout (Part 1)

First, lets set the Layout Editor to the desired configurations:

1. In the Project window, open app > res > layout > activity_main.xml.
2. If your editor shows the XML source, click the Design tab at the bottom of the window.
3. Click **Select Design Surface** and **select Blueprint**.
4. Click **Show**  in the Layout Editor toolbar and make sure that **Show All Constraints** is checked.
5. Make sure **Autoconnect** is **off**. A tooltip in the toolbar displays **Enable Autoconnection to Parent**  when Autoconnect is off.
6. Click **Default Margins**  in the toolbar and select **16**. If needed, you can adjust the margins for each view later.
7. Click **Device for Preview**  in the toolbar and select **5.5, 1440 × 2560, 560 dpi (Pixel XL)**.

Now, lets design the Main Activity (your app's home page):

1. Add a **Text Box**:
   1. First, you need to remove what's already in the layout. Click **TextView** in the **Component Tree panel** and then press the *Delete* key.
   2. In the **Palette panel**, click **Text** to show the available text controls.
   3. Drag the **Plain Text** into the **design editor** and drop it near the top of the layout. This is an EditText widget that accepts plain text input.
   4. Click the view in the design editor. You can now see the *square handles* to *resize the view* on each corner, and the *circular constraint anchors* on each side. For better control, you might want to zoom in on the editor. To do so, use the Zoom buttons in the Layout Editor toolbar.
   5. Click and hold the anchor on the top side, drag it up until it snaps to the top of the layout, and then release it. That's a contraint: it constrains the view within the default margin that was set. In this case, you set it to 16 dp from the top of the layout.
   6. Use the same process to create a constraint from the left side of the view to the left side of the layout.

2. Add a **Button**
   1. In the **Palette panel**, click Buttons.
   2. Drag the **Button widget** into the design editor and drop it near the right side.
   3. Create a *constraint* from the left side of the button to the right side of the text box.
   4. To constrain the views in a horizontal alignment, create a constraint between the text baselines. To do so, right click the *button component* in the **Component Tree panel** and select *Show Baseline*. The baseline anchor appears inside the button. Click and hold this anchor, and then drag it to the baseline anchor that appears in the text box.

## App Functionality (Part 1)

## App Layout (Part 2)

## App Functionality (Part2)
