# Show & Hide elements on click

* Login to Webflow > Dashboard > New Project > Blank Site
* Add element > section | height: 300px; background-color: beige
* Add element > container within section

## How to make one element trigger another element's animation
* Add element > div block | width: 100px; height: 50px; border: 1px solid black
* Add element > paragraph | width: 500px; 
* Select the div block > Interactions tab > Add Element Trigger > Mouse Click
* On 1st Click > Start an Animation > Add Timed Animation > Name it 'move'
* Add Timed Action > Move > 
* OOPS! Moved wrong element, don't worry, we can fix that
* Under Timed Action - 0:00, right click div, select 'Change target' > Click the paragraph
* Move x 
* Preview by pressing Play



## Recreate tabbed example from uxdesign.cc/good-to-great-ui-animation-tips-7850805c12e5
* Change layout view to tablet portrait 
* Add element > section | height: 100vh
* Add a container within section | height: 100%

## Add tabs
* Add element > div | width: 50%; height: 50px; background-color: royalblue; display: inline-block;
* Add element > div | width: 50%; height: 50px; background-color: skyblue; display: inline-block;

## Add tab content
* Add element > div which sits below tabs (so it's same hierarchy)
* Add element > paragraph | padding: 10px; height: 300px; border: 3px solid royalblue; border-radius: 25px;
* Add paragraph again right after 1st paragraph for 2nd tab's content but make border skyblue

## Animate Tab 1
* Select Tab 1 so it's active > Interactions > Add Element Trigger > Mouse Click
* On 1st Click > Start an animation > Add Timed Animation > name it tab1move
* Select Tab1's paragraph block so it's active
* Add Timed action 0:00 > Set initial state > Move x:-1000px
* Select Tab2's paragraph block so it's active
* Add Timed action 0:00 > Set initial state > Move y:-310px
* (2nd paragraph) Add Timed action end > Move x: 1000px
* (1st paragraph) Add Timed action end > Move x: 0px



## Animate Tab 2
* Select Tab 2 so it's active > Interactions > Add Element Trigger > Mouse Click
* On 1st Click > Start an animation > Add Timed Animation > name it tab2move
* Select Tab1's paragraph > Set initial state > Move x:0px
* Select Tab2's paragraph > Set initial state > Move y: -310px; x: 1000px
* (2nd paragraph) Add Timed action end > Move x: 0px
* (1st paragraph) Add Timed action end > Move x: -1000px









