# Mini Nature Museum AR

A beginner WebAR learning example based on the supplied lecture Step 5. Point a camera at the Hiro marker to see a miniature nature museum. Understand and personalise this example with your group before submitting it.

## Group details

Group number: ADD YOUR MODULE GROUP NUMBER

Members: ADD YOUR GROUP MEMBERS AND STUDENT IDS

Public repository URL: ADD AFTER CREATING YOUR REPOSITORY

Live HTTPS URL: ADD AFTER ENABLING GITHUB PAGES

## Assessment requirements

| Requirement | Implementation |
| --- | --- |
| Hiro marker | `a-marker preset="hiro"` |
| At least four objects and two primitive types | Ground plane, pedestal cylinder, bouncing sphere, green box, tree trunk cylinder, tree canopy cone |
| At least one a-text label | Museum title and exhibit label |
| Two animated objects using different properties | Avocado rotates; sphere changes position |
| One glTF or GLB model other than the duck | `models/Avocado.glb` |
| Workshop ball colour interaction | `color-changer` component on the sphere |
| New tappable object and custom component | `grow-toggle` on the green box |
| Status text and colour change | `marker-status` handles `markerFound` and `markerLost` |
| HTTPS and phone test | Complete deployment and the real device checks below |

## Software

- Visual Studio Code: https://code.visualstudio.com/
- Live Server by Ritwick Dey: https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer
- Chrome or Edge on a computer with a webcam.
- A smartphone for the required final test.
- GitHub account: https://github.com/

This static app uses HTML, CSS, JavaScript, A-Frame 1.3.0 and AR.js 3.4.5, matching the lecture's library versions. There is no database, npm install, Unity or Android Studio step. Internet is needed for the library scripts and A-Frame's default text font assets; the model is included locally.

## Run locally

1. Extract the ZIP before opening it.
2. In VS Code, use File > Open Folder and choose the folder containing index.html.
3. Install Live Server by Ritwick Dey.
4. Right-click index.html > Open with Live Server.
5. Use http://localhost:5500/ or the local 127.0.0.1 address shown by Live Server. The port may differ.
6. Allow camera access. Print markers/hiro.png or show it on a second device.
7. Show the complete marker and its white margin, flat and well lit, to the webcam.
8. Click the bouncing ball and green box; then hide and show the marker.

Do not run by double-clicking the HTML file. A phone opening an ordinary HTTP address such as http://192.168.1.5:5500 does not have the same secure-origin exception as localhost. Use the HTTPS published site for phone testing.

## Publish with GitHub Pages

1. Sign into GitHub and create a new public repository, e.g. ar-nature-museum.
2. Upload the CONTENTS of this folder, keeping index.html at the repository root. Include models, markers, credits and README.md. Do not upload only the ZIP.
3. Commit the files to main.
4. Settings > Pages > Build and deployment > Source > Deploy from a branch.
5. Select main and /(root), then Save.
6. Wait for deployment; it may take up to about 10 minutes. Use the Visit site link in Pages settings.
7. Check HTTPS and open the live URL on your phone. A typical URL is https://YOUR-USERNAME.github.io/ar-nature-museum/.
8. Allow camera access and point the rear camera at the marker displayed on a laptop or printed paper.

## Real device test record

The source and JavaScript interactions were checked while preparing this example. This does not replace a real camera or phone test. The example has not been published into your GitHub account.

Phone make and model: TO BE COMPLETED

Browser and version: TO BE COMPLETED

Test date: TO BE COMPLETED

| Test | Expected result | Actual result |
| --- | --- | --- |
| Open HTTPS site and allow camera | Live camera view | NOT YET TESTED |
| Marker not visible | Red looking/lost banner | NOT YET TESTED |
| Show Hiro marker | Scene appears; banner becomes green | NOT YET TESTED |
| Watch exhibit | Avocado spins; ball bounces | NOT YET TESTED |
| Tap ball repeatedly | Colour cycles | NOT YET TESTED |
| Tap green box twice | Grows, then returns to original size | NOT YET TESTED |
| Cover marker | Scene hides; banner turns red and says LOST | NOT YET TESTED |
| Show marker again | Scene reappears; banner says FOUND | NOT YET TESTED |

Replace the actual results only after doing each test. Optional screenshots or a short demonstration video are useful evidence but are not explicitly required by the supplied assignment sheet.

## Model attribution and licence

- Model: Avocado.
- Creator credit in the source README: Microsoft for Everything.
- Source: KhronosGroup glTF Sample Assets.
- Source README: https://github.com/KhronosGroup/glTF-Sample-Assets/blob/main/Models/Avocado/README.md
- Original GLB: https://raw.githubusercontent.com/KhronosGroup/glTF-Sample-Assets/main/Models/Avocado/glTF-Binary/Avocado.glb
- Licence: Creative Commons Zero v1.0 Universal (CC0-1.0).
- Licence URL: https://creativecommons.org/publicdomain/zero/1.0/
- Original notice: Copyright 2017, Public.
- Modification in this example: embedded textures resized to a maximum of 512 pixels per side for a smaller mobile download; geometry unchanged.
- The original model README is preserved in credits/Avocado-source.md.

The model was downloaded and its licence notice checked on 6 November 2026. It is not the workshop duck. The coursework explicitly asks for a model credit in this README, even though CC0 does not require attribution.

Hiro marker source: https://github.com/AR-js-org/AR.js/blob/master/data/images/hiro.png. AR.js is MIT licensed: https://github.com/AR-js-org/AR.js/blob/master/LICENSE. The marker is included for this AR.js exercise; its source is credited here. A-Frame is MIT licensed: https://github.com/aframevr/aframe/blob/v1.3.0/LICENSE.

## Submission

The supplied AR Activity document requires a GROUP assignment, one submission per group, a PUBLIC GitHub repository, and a Word document containing the repository link. Name the Word document with your actual module group number, e.g. 12.docx if your group number is 12. The supplied documents do not state the group number or deadline.

Suggested Word content:

AR Group Assignment

Group Number: [your module group number]

Project Title: Mini Nature Museum AR

GitHub Repository: [your actual public repository URL]

Live HTTPS Application: [your actual live URL]

Group Members: [names and student IDs]

The live URL and members are useful additions; the repository URL is explicitly required. Submit the repository link, not only the live site link. The optional challenge levels in the lecture guide do not make a second marker, custom marker or video mandatory in this assignment.

## Troubleshooting

| Problem | Check |
| --- | --- |
| No camera | Camera permission, OS camera privacy setting, HTTPS or localhost, another app using camera |
| Camera works but no objects | Whole correct marker visible, white margin intact, no glare, good light |
| Model invisible | models/Avocado.glb uploaded, exact filename and letter case, model request not 404 |
| AFRAME is not defined | Internet and library loading; A-Frame script must be first |
| Tap does nothing | clickable class, custom component, camera cursor and raycaster still present |
| Changes do not appear | Save, refresh, and wait for Pages deployment |
| Phone cannot access camera on local Wi-Fi link | Use the deployed HTTPS URL |
| Labels seem backward or invisible | View the marker from the opposite edge; text has a front-facing orientation |

Press F12 > Console for JavaScript errors and Network for missing files.

## Learning support

This is an AI-assisted learning example prepared for the student, not a statement that the group has already completed deployment or device testing. Follow your course's rules for using and declaring assistance. See LEARN-Sinhala.md for the Sinhala and English walkthrough and the lecture's ten understanding questions with answers.
