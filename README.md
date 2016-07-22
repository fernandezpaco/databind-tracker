# databind-tracker


It tracks data binding events and populates a timestamped list with this events

Up to 4 properties can be tracked

Returns an array with all the events.

In the following example every time that you click on the video, an screenshot will be generated. The databind tracker will mantain a list like this:

timestamp 		p0

1469190369888	data:image/png;base64,iVBOR....

1469190435503	data:image/png;base64,1fji3....

```html
<video-camera screenshot="{{sc}}"></video-camera>
<databind-tracker p0="{{sc}}" data={{eventsarray}}></databind-tracker>
``