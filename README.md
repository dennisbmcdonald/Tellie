# Tellie's QA Assessment

**_[Estimated completion time: ~45 minutes]_**

Hello and welcome to Tellie&#39;s QA assessment! 👋

This will test your ability to catch visual and behavioral test case failures in real-world components. Tellie is a visually rich application, so our quality bar for aesthetics and user experience is high!

Today, we want you to assure the quality of two UI components:

1. Add/Edit Tiles ([storybook](https://tellieengineering.github.io/qa-assessment/?path=/story/composed-ui-library-set-editor-tiles--interactive) / [figma](https://www.figma.com/file/PbmqwQVTBul7CnqlRDdDC5/QA-Assessment-Design-Guide?node-id=2%3A4474))
1. Image Well ([storybook](https://tellieengineering.github.io/qa-assessment/?path=/story/core-ui-library-images-and-icons-image-well--interactive) / [figma](https://www.figma.com/file/PbmqwQVTBul7CnqlRDdDC5/QA-Assessment-Design-Guide?node-id=2%3A4474))

Tellie uses [Storybook](https://storybook.js.org/) and [Figma](https://www.figma.com) to bridge our design and development teams. You will find links to each component in their respective applications above. There are more stories in our storybook (feel free to explore!), but please only test the specific stories above (**two** **total**). Also, please also review our fonts and color scheme here.

We have purposefully introduced bugs/errors into at least one of the components above. Review the Acceptance Criteria below and manually test each component against the criteria in Chrome on Desktop (you might opt to test other browsers, but this is not required).

## Add/Edit Tiles Interactive - Acceptance Criteria

Tellie provides &quot;Tiles&quot; to users. Tiles are the main primitive with which users build their sites. There are several different Tile types, from Tiles that display an image, that display a set of links, that play media, etc. This component manages what Tiles appear on a user&#39;s site (and in what order on Mobile).

- Must match designs exactly (pixel perfect colors, spacing, fonts, etc.)
- Clicking Add Tile should show a popup with three Tile types: Image, Links, and Shop
- Clicking an item in the Add Tile popup should add that Tile type to the Tile list below
- User should not be able to add more than 10 Tiles
- Should show delete modal to confirm deleting a tile
- Message should appear when a Tile is deleted explaining the deletion and disappear after 5 seconds
- Message should appear when the max Tile limit is reached
- Tiles are ordered and dragging a Tile should reorder the Tiles
- User should be able to delete a Tile by clicking the small down arrow on the right of each Tile item and clicking &quot;Delete&quot;
- Dragging items should be ~60fps
- Text should be selectable

## Image Well Interactive - Acceptance Criteria

The Image Well allows a user to select an image from their computer and upload it to Tellie.

- Must match designs exactly (pixel perfect colors, spacing, fonts, etc.
- User can drag an image file (only image files) from their native system onto the image well and it should begin the upload process*
- User can click the image well and select an image (filtered by image type) from their native file system.
- User should see an error if trying to upload an image larger than 1200x800
- User can remove an image after it is uploaded

_* Storybook does not actually upload an image to Tellie&#39;s servers, so the uploaded image will be a placeholder._ **_This is acceptable in this case._**

# What to send us

Create a shareable online document (Google Docs, etc) and provide us a completed test plan and test case for each component. Email the document to `engineering@tell.ie` and title it `<Your Name> - QA Submission`. Also include answers to the following (500 words max for each answer):

1. What tools did you use to validate the acceptance criteria?
1. What steps would you take to eliminate future regressions?
1. How would you approach the e2e testing of these components once they graduate to the application?
1. What other questions might you have about the components?

Feel free to reach out with any questions to the same email. Good luck and thank you!
