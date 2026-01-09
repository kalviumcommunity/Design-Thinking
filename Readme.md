Case Study: The App That Looked and Only Works Perfect on One Phone.
Problem Overview

The original FlexiFit UI was created with hard pixel values and fixed layouts that were made on a single device (Pixel 7). Although the design looked aesthetically flawless on that device, it did not work on smaller iPhones and larger tablets. On smaller screens, an element of a UI was clipped or overlapped with another, whereas on larger screens, it was excessively spaced and did not seem to balance with other elements. This was due to the fact that the static designs fail to adjust to the differences in the screen size, aspect ratio, and the differences in platform.

Why Static Design Failed

Layout overflow was experienced on small devices because of fixed widths and heights.

Absolute spacing created components overlaps.

Increased sizes brought about white space wastage and lack of visual hierarchy.

None of the dynamic scaling depending on the size of the screen.

Flutter-based Responsive Solution.

In order to maintain the original Figma design purpose and at the same time be responsive, the layout was recreated with Flutters adaptive widgets:

MediaQuery

Utilized to get device screen sizes, scale UI components proportionately rather than with fixed pixel values. This enabled Stable inter-spacing and sizing between devices.

Flexible & Expanded

Used in Row and Column widgets so that the components can share available space dynamically. This avoided overlapping and provided equal layouts on both small and large screens.

LayoutBuilder

Installed to identify the size of the screen and alternate layouts. The mobile devices are vertically stacked with layouts whereas the tablets are wider with grid based layout to facilitate better utilization of content.

Final Outcome

UI is user-friendly on both phones and tablets.

None of the overlapping or clipped elements on small screens.

Appropriate separation and layout on bigger gadgets.

Visual consistency to the original Figma design preserved.

More user-friendly and cross-platform compatibility.

This method changed an unresponsive UI to a responsive and adaptable Flutter application that provides a reliable and consistent user experience on all screens and platforms.