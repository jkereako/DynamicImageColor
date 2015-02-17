# Dynamic image color
This is a simple app which demonstrates how to use Core Image filters.

Specifically, this app loads an image and applies the filter [`CIHueAdjust`](https://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIHueAdjust) which, as the name implies, adjusts the hue. The app presents the user with an image and a [`UISlider`](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UISlider_Class/index.html). When the user touches the `UISlider`, the new value reflects in the image as a change in hue.

## Demonstration
<img src="https://github.com/jkereako/dynamic-image-color/raw/master/demo.gif" alt="Dynamic image color demo" width="320" height="568" />

# Some considerations
- Rendering an image can take a while, so make sure you render images asynchronously
- The larger the image, the more resource expensive applying the filters will be. Keep this in mind when designing your application.

# Further reading
- [Core Image Programming Guide](https://developer.apple.com/library/ios/documentation/GraphicsImaging/Conceptual/CoreImaging/ci_intro/ci_intro.html)
- [Drawing and Printing Guide for iOS](https://developer.apple.com/library/ios/documentation/2DDrawing/Conceptual/DrawingPrintingiOS/GraphicsDrawingOverview/GraphicsDrawingOverview.html)
- [Quartz 2D Programming Guide](https://developer.apple.com/library/ios/documentation/GraphicsImaging/Conceptual/drawingwithquartz2d/Introduction/Introduction.html)
