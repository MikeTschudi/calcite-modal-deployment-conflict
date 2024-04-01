#### solution-deployment-app doesn't display calcite-modals correctly

On Androids and in Google Chrome's mobile emulator set for a mobile display, a calcite-modal is wider than the screen.
![image](https://github.com/MikeTschudi/calcite-modal-deployment-conflict/assets/2125181/8de41919-dd5d-495d-99f2-aea4b361e69b)
instead of
![image](https://github.com/MikeTschudi/calcite-modal-deployment-conflict/assets/2125181/e4a3f3e9-d1ec-4e4d-b3c2-ead64d2a271a)

Examples:
* modalE9d2.html has a modal that is wider than the screen (left image)
* modalE9d3.html has a modal that fits the screen (right image)

The difference between the two is that modalE9d2 has a modal atop a "gallery" containing an image that's 400px wide, while modalE9d3's gallery's image is only 200px wide.

If the example is changed to use calcite-components 1.11.0 instead of 2.x (modalE9d2a.html), the modal fits the screen even with 400px images.
