# Code Lou QA Project
## Test outline for https://www.polygon.com/pages/newsletter

This test outline is for functionality of Polygon.com's new email subscription sign up interface. These tests below will cover the email entry field for the subscription function, as well as several features associated with the subcription emails, user settings in regards to these subscriptions, and sharing the subscription function over social media.

**Feature to Test**
1. Enter Email Field

***Test Type: Critical Path***

*-preconditions:* direct to URL to access the subscription field 

* Test steps: enter a valid, correct Email address in the subscription field

* **Expected outcome:** Subscription submission Successful, Follow-up email will be sent to confirm subscription

2. Enter Email Field

***Test Type: Critical Path***

*-preconditions:* direct to URL to access the subscription field 

* Test steps: enter an invalid, unregistered Email address in the subscription field

* **Expected Outcome:** Display Error Message - Invalid Email, prompt user to try again

3. Terms Agreement hyperlink under submission form

***Test Type: Integration Test***

*-preconditions:* direct to URL to access the subscription field

* Test Steps: Click on the "Terms" link bellow the subscription field

* **Expected Outcome:** Open new broswer window, directed to Terms of Use page

4. Share to Twitter Link

***Test Type: API Test***

*-preconditions:* direct to URL to access the subscription field

* Test Steps: Click on the Twitter Icon in the top left, above the subscription field 

* **Expected Outcome:** Open new broswer window, prompting to log into Twitter to access profile permissions

5. Enter Email Field

***Test Type: Critical Path Test***

*-preconditions:* direct to URL to access the subscription field

* Test Steps: Enter an invalid email format into the subscription field. Enter without an "@" or .com ending

* **Expected Outcome:** Display Error Message - Invalid Email, prompt user to try again

6. Subscription Email Message

***Test Type: Integration Test***

*-preconditions:* Enter a valid email into the subscription field, successfully prompting a confirmation email

* Test Steps: Clink the "unsubscribe" link inside the confirmation email, or an email generated from the subscription list

* **Expected Outcome:** Open new browser window with email address reference and "unsubscribe" confirmation

7. Subscription Email Message

***Test Type: Critical Path Test***

*-preconditions:* receive a confirmation email for the Subscription 

* Test Steps: Click the "Confirm Subscription" Button link in the confirmation email 

* **Expected Outcome:** Open new broswer window. Confirmation message displayed - Email address added to subscription list

8. Email Delivery Time

***Test Type: System Test***

*-preconditions:* direct to URL to access the subscription field 

* Test Steps: Successfully Enter a viable email address, triggering a confirmation email to be sent - time delivery time for confirmation email to arrive in inbox

* **Expected Outcome:** Confirmation email should be delivered in <2 minutes

9. Subscription Reminder Service

***Test Type: Integration Test***

*-preconditions:* successfully enter valid email address, prompting confirmation email. 

* Test Steps: **Do Not Confirm Email**

* **Expected Outcome:** A follow up, reminder email should be sent to the inbox after 2 days

10. Unsubscribe options menu

***Test Type: Critical Path Test***

*-preconditions:* Click on "unsubscribe" link within confirmation email

* Test Steps: click on "manage your email preferences here" on the unsubscribe page 

* **Expected Outcome:** direct user to page with check boxes, allowing specific topics to be unsubscribed from
