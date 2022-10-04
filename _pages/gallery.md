---
title         : "Gallery"
permalink     : /gallery

# Gallery of renders
# Images from /images/renders/
render_gallery:
  - url: /images/renders/Render1-V1.0.JPG
    image_path: /images/renders/Render1-V1.0.JPG
    alt: "Isometric render of robot"
    title: "Isometric render of full robot"
  - url: /images/renders/Render2-V1.0.JPG
    image_path: /images/renders/Render2-V1.0.JPG
    alt: "Top three-quarters render of robot"
    title: "Top 3/4 render of robot"
  - url: /images/renders/Render3-V1.0.JPG
    image_path: /images/renders/Render3-V1.0.JPG
    alt: "Bottom three-quarters render of robot"
    title: "Bottom 3/4 render of robot"

# Gallery of testing photos
# Images from /images/testing/mit-river-test/
testing_gallery:
  - url: /images/testing/mit-river-test/boat.jpeg
    image_path: /images/testing/mit-river-test/boat.jpeg
    alt: "Transporting the robot to the middle of the river"
    title: "Testing in the Charles River"
  - url: /images/testing/mit-river-test/boathouse.JPG
    image_path: /images/testing/mit-river-test/boathouse.JPG
    alt: "Testing from the MIT Sailing Pavilion"
    title: "Testing from the MIT Sailing Pavilion"
  - url: /images/testing/mit-river-test/inwater.jpeg
    image_path: /images/testing/mit-river-test/inwater.jpeg
    alt: "Initial testing off the side of the dock"
    title: "Initial dock testing"

# Gallery of studio photos
# Images from /images/studio/
studio_gallery:
  - url: /images/studio/electronics.jpg
    image_path: /images/studio/electronics.jpg
    alt: "View of the electronics tubes on the robot"
    title: "Electronics Tubes"
  - url: /images/studio/side.jpg
    image_path: /images/studio/side.jpg
    alt: "Side view of robot"
    title: "Side view"
  - url: /images/studio/top.jpg
    image_path: /images/studio/top.jpg
    alt: "Top view of robot"
    title: "Top view"
---

<!-- Adds gallery of full robot renders -->
{% include gallery id="render_gallery" caption="**Full Robot Renders**" %}

<!-- Adds gallery of testing photos -->
{% include gallery id="testing_gallery" caption="**Testing**" %}

<!-- Adds gallery of studio photos -->
{% include gallery id="studio_gallery" caption="**Studio Photos**" %}
