Test case 1: Verify face and ID match
Position: Onboarding
Steps:

User initiates eKYC process
User uploads a photo of their government-issued ID
User takes a live photo of their face
System verifies that the face in the live photo matches the face on the ID
Expectation: System should confirm that the face and ID match
Acceptance criteria: System should display a success message and proceed to the next step of the eKYC process.
Test case 2: Detect spoofed face
Position: Onboarding
Steps:

User initiates eKYC process
User uploads a photo of a government-issued ID
User shows a printed photo of someone else's face to the camera
System detects the spoofed face and rejects the attempt
Expectation: System should detect that the face is not live and reject the attempt
Acceptance criteria: System should display an error message and not proceed to the next step of the eKYC process.
Test case 3: Verify document authenticity
Position: Onboarding
Steps:

User initiates eKYC process
User uploads a photo of their government-issued ID
System checks that the document is valid and has not been tampered with
Expectation: System should confirm that the document is authentic and has not been tampered with
Acceptance criteria: System should display a success message and proceed to the next step of the eKYC process.
Test case 4: Detect fraudulent ID
Position: Onboarding
Steps:

User initiates eKYC process
User uploads a photo of a government-issued ID that has been tampered with or is fraudulent
System detects the fraudulent document and rejects the attempt
Expectation: System should detect that the document is fraudulent and reject the attempt
Acceptance criteria: System should display an error message and not proceed to the next step of the eKYC process.
Test case 5: Verify live face
Position: Onboarding
Steps:

User initiates eKYC process
User takes a live photo of their face
System checks that the face is live and not a photo or video playback
Expectation: System should confirm that the face is live and not a photo or video playback
Acceptance criteria: System should display a success message and proceed to the next step of the eKYC process.
Test case 6: Verify ID matches user information
Position: Onboarding
Steps:

User initiates eKYC process
User uploads a photo of their government-issued ID
System verifies that the ID matches the user's information provided during registration
Expectation: System should confirm that the ID matches the user's information provided during registration
Acceptance criteria: System should display a success message and proceed to the next step of the eKYC process.

Test Case 6: Invalid ID, Invalid Selfie

Description:
This test case is used to check the system's ability to detect invalid ID and selfie inputs.

Pre-Condition:

User has an invalid or expired ID document.
User has a selfie that does not match their true identity.
Test Steps:

User enters their invalid or expired ID document.
User takes a selfie that does not match their true identity.
System detects that both the ID document and selfie inputs are invalid and prompts the user to try again.
User enters a valid ID document.
User retakes a selfie that matches their true identity.
System successfully verifies the user's identity.
Expected Result:
System should detect that both the ID document and selfie inputs are invalid and prompt the user to try again. After the user enters a valid ID document and takes a selfie that matches their true identity, the system should successfully verify the user's identity.

Verification with altered image:
Position: User
Step:
Provide a valid ID card.
Take a photo of yourself holding the ID card.
Alter the photo by changing the lighting or angle of the image.
Submit the altered photo and ID card photo for verification.
Expectation: The system should reject the altered image and display an error message asking the user to retake the photo.
Acceptance Criteria: The system should correctly detect that the image has been altered and prevent the verification process from proceeding.
Verification with fake ID:
Position: User
Step:
Provide a fake ID card.
Take a photo of yourself holding the fake ID card.
Submit the fake ID card photo and user photo for verification.
Expectation: The system should reject the fake ID and display an error message asking the user to provide a valid ID card.
Acceptance Criteria: The system should correctly detect that the ID card is fake and prevent the verification process from proceeding.
Verification with blurry image:
Position: User
Step:
Provide a valid ID card.
Take a photo of yourself holding the ID card with a blurry image.
Submit the blurry image and ID card photo for verification.
Expectation: The system should reject the blurry image and display an error message asking the user to retake the photo.
Acceptance Criteria: The system should correctly detect that the image is blurry and prevent the verification process from proceeding.
Verification with low-resolution image:
Position: User
Step:
Provide a valid ID card.
Take a photo of yourself holding the ID card with a low-resolution camera.
Submit the low-resolution image and ID card photo for verification.
Expectation: The system should reject the low-resolution image and display an error message asking the user to retake the photo.
Acceptance Criteria: The system should correctly detect that the image is low-resolution and prevent the verification process from proceeding.
Verification with mismatched ID card information:
Position: User
Step:
Provide a valid ID card.
Take a photo of yourself holding the ID card.
Alter the information on the ID card (e.g. name, date of birth).
Submit the altered ID card photo and user photo for verification.
Expectation: The system should reject the mismatched ID card and display an error message asking the user to provide a valid ID card.
Acceptance Criteria: The system should correctly detect that the information on the ID card does not match the submitted user photo and prevent the verification process from proceeding.

Test Case 13: Document Verification
Position: Verification Agent
Steps:

Receive the scanned image of the customer's identity document.
Verify that the document is authentic and has not been tampered with.
Check that the document matches the customer's personal information.
Mark the document as verified in the system.
Expectation: The document should be verified and the customer's information should match the document.

Acceptance Criteria:

The document should have all necessary security features, including watermarks, holograms, and other anti-tampering measures.
The information on the document should match the customer's information as provided during the registration process.
If the document fails to pass verification, the customer should be notified and asked to submit a new document.
Test Case 14: Video Verification
Position: Verification Agent
Steps:

Connect with the customer over a video call.
Verify the customer's identity using the video feed.
Verify the customer's personal information, including name and address.
Mark the video as verified in the system.
Expectation: The customer should be verified and their personal information should match the information provided during registration.

Acceptance Criteria:

The video quality should be sufficient for verification purposes, with clear images and audio.
The customer should be clearly visible and identifiable in the video.
The customer's personal information should match the information provided during the registration process.
If the video fails to pass verification, the customer should be notified and asked to repeat the verification process.
Test Case 15: Face Recognition Verification
Position: Verification Agent
Steps:

Request the customer to submit a selfie image.
Verify that the image is an accurate representation of the customer's face.
Compare the selfie image with the customer's identity document image.
Mark the face recognition verification as successful in the system.
Expectation: The customer's face should be accurately matched with their identity document.

Acceptance Criteria:

The selfie image should clearly show the customer's face, with no obstructions or disguises.
The selfie image should match the customer's identity document image.
The system should be able to accurately recognize and match facial features, including eye and mouth positioning, nose shape, etc.
If the face recognition verification fails, the customer should be notified and asked to repeat the verification process.

Test Case 16:
Title: Rejection of Non-Live Images
Description: Verify that the system should reject non-live images during the eKYC process.

Test Steps:

Prepare a non-live image of an identity document or a selfie.
Initiate the eKYC process on the digital banking app using the non-live image.
Verify that the system should detect the non-live image and reject it.
Record the error message displayed on the app.
Repeat the process with a live image.
Verify that the live image is accepted by the system.
Record the successful message displayed on the app.
Expected Result:

The system should detect the non-live image and reject it with an appropriate error message.
The system should accept the live image and proceed with the eKYC process.
Acceptance Criteria:

The non-live image should be rejected with a clear and concise error message, indicating that only live images are accepted.
The live image should be accepted and the eKYC process should proceed smoothly.


Test Case 17: Same face recognition check

Test Description:
This test case verifies that the system is able to recognize the same face on different images captured during the eKYC process.

Precondition:

The user has successfully completed the previous steps of the eKYC process.
The user is presented with a new screen to capture another image of their face.
Test Steps:

User captures a new image of their face using the front camera.
The system compares the new image with the previous image captured during the eKYC process.
The system displays a message indicating whether the two images match or not.
Expected Result:

The system should be able to recognize that the two images are of the same face.
The system should display a message indicating that the images match.
The user should be able to proceed to the next step of the eKYC process.
Acceptance Criteria:

The system should have a matching threshold of at least 90% for this test case.
The system should have a low false-positive rate for this test case.
The test case should be performed with different lighting conditions and angles to ensure the system can accurately recognize the same face.


Test Case 18: Matching of multiple images
Description: Test whether the system can match multiple face images of a person correctly or not.

Test Steps:

Provide two or more images of the same person's face.
Submit the images to the system for matching.
Expected Result: The system should match all the images correctly and confirm the identity of the person.

Acceptance Criteria:

The system should match all the images with at least 99% accuracy.
The matching process should take no longer than 10 seconds.
Test Case 19: Poor image quality test
Description: Test whether the system can detect and reject poor quality face images.

Test Steps:

Provide a poor quality image of a person's face (e.g. low resolution, blurry, distorted).
Submit the image to the system for matching.
Expected Result: The system should reject the image and ask for a better quality image.

Acceptance Criteria:

The system should detect poor quality images with at least 95% accuracy.
The rejection message should be clear and informative.
Test Case 20: Lighting condition test
Description: Test whether the system can match face images taken under different lighting conditions.

Test Steps:

Provide two or more face images of the same person taken under different lighting conditions (e.g. bright light, low light, backlight).
Submit the images to the system for matching.
Expected Result: The system should match all the images correctly and confirm the identity of the person.

Acceptance Criteria:

The system should match all the images with at least 99% accuracy.
The matching process should take no longer than 10 seconds.
Test Case 21: Face expression test
Description: Test whether the system can match face images of the same person with different facial expressions.

Test Steps:

Provide two or more face images of the same person with different facial expressions (e.g. smiling, frowning, neutral).
Submit the images to the system for matching.
Expected Result: The system should match all the images correctly and confirm the identity of the person.

Acceptance Criteria:

The system should match all the images with at least 99% accuracy.
The matching process should take no longer than 10 seconds.
Test Case 22: Face angle test
Description: Test whether the system can match face images of the same person taken from different angles.

Test Steps:

Provide two or more face images of the same person taken from different angles (e.g. frontal view, side view, 45-degree angle).
Submit the images to the system for matching.
Expected Result: The system should match all the images correctly and confirm the identity of the person.

Acceptance Criteria:

The system should match all the images with at least 99% accuracy.
The matching process should take no longer than 10 seconds.


Matching of facial images with various attributes: This test case verifies the matching of facial images with various attributes such as age, gender, ethnicity, and other physical attributes.

Matching of facial images captured at different angles: This test case verifies that the facial recognition system is able to match facial images captured at different angles with the reference image.

Matching of facial images captured under different lighting conditions: This test case verifies that the facial recognition system is able to match facial images captured under different lighting conditions with the reference image.

Matching of facial images captured with different facial expressions: This test case verifies that the facial recognition system is able to match facial images captured with different facial expressions with the reference image.

Testing with different mobile devices: This test case verifies that the eKYC system works seamlessly with different types of mobile devices, including smartphones and tablets.

Testing with different operating systems: This test case verifies that the eKYC system works seamlessly with different operating systems, including iOS and Android.

Testing with different network speeds: This test case verifies that the eKYC system works seamlessly with different network speeds, including 3G, 4G, and Wi-Fi.

Testing with different image quality: This test case verifies that the eKYC system is able to capture and process facial images of different quality levels.

Testing with multiple languages: This test case verifies that the eKYC system is able to support multiple languages for user interface and instructions.

Testing with different types of identification documents: This test case verifies that the eKYC system is able to scan and verify different types of identification documents, including national ID cards, passports, and driver's licenses.

Testing with different countries and regions: This test case verifies that the eKYC system is able to operate in different countries and regions, including compliance with local laws and regulations.

Performance testing: This test case verifies that the eKYC system is able to handle a high volume of user requests and transactions without any performance degradation.

Security testing: This test case verifies that the eKYC system is secure and able to protect user data and information in accordance with industry standards and regulations.

Integration testing: This test case verifies that the eKYC system is able to integrate with other systems and platforms, including core banking systems and third-party service providers.

Usability testing: This test case verifies that the eKYC system is user-friendly and easy to use for all types of users, including those with different levels of technical knowledge and experience.

Accessibility testing: This test case verifies that the eKYC system is accessible to users with different types of disabilities, including visual impairment and hearing impairment.

Compatibility testing: This test case verifies that the eKYC system is compatible with different types of software and hardware, including browsers, operating systems, and devices.

Regression testing: This test case verifies that the eKYC system remains functional and stable after any software updates or changes to the system.

User acceptance testing: This test case verifies that the eKYC system meets the requirements and expectations of end-users, including ease of use, reliability, and security.

