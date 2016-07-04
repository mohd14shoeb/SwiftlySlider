# SwiftlySlider

Simple iOS slider control.

![alt tag](https://raw.github.com/maximbilan/SwiftlySlider/master/img/1.png)

## Installation
<b>CocoaPods</b>:
<pre>
pod 'SwiftlySlider'
</pre>
<b>Manual</b>:
<pre>
Just copy the <i>SwiftlySlider.swift</i> into your project.
</pre>

## Using

You can create from <i>Storyboard</i> or <i>XIB</i>. Or create manually:
<pre>
let slider = SwiftlySlider()
</pre>

For handling changing of values you should implement protocol <i>SwiftlySliderDelegate</i>:

<pre>
slider.delegate = self

func swiftlySliderValueChanged(value: Int) {
}
</pre>

Direction:
<pre>
picker.direction = SwiftlySlider.PickerDirection.Horizontal // Vertical, Horizontal
</pre>

Also you can change current value, maximum value or minimum value, for example:
<pre>
picker.currentValue = 0
picker.maxValue     = 30
picker.minValue     = 1
</pre>

Slider settings:

<pre>
sliderImage       // Custom image of the slider
sliderImageOffset // Offset of custom slider position
sliderSize        // Size of custom slider position
</pre>

Normal indicator:

<pre>
useNormalIndicator  // Use normal indicator
normalValue         // Normal value
</pre>

Color settings:
<pre>
labelFontColor        // Font color of the moving label
labelBackgroundColor  // Background color of the moving label
labelFont             // Font of the moving label
bgColor               // Background color
</pre>

You can easily found example in this repository.

## License

SwiftlySlider is available under the MIT license. See the LICENSE file for more info.
