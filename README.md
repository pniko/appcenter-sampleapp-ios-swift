# First 48 Developer Hackathon

## Requirements:
1. Developer machine
2. (if iOS) Apple Developer Account and an iOS Device 
3. Source Code- [aka.ms/first48](aka.ms/first48])
4. VS Code (For Azure Functions work)
5. Azure Subscription
6. Optional- Headphones for videos/focused work

## Introduction

Let’s imagine that you work for Contoso, Inc. and you have been tasked to develop an app that interacts with your companies’ new website. This is a companion app to bring a native mobile experience to the functionality offered by the website already. You're collaborating with 3 other developers to build this iOS companion app and the team has decided to use Visual Studio App Center to automate the iOS application lifecycle.

The dev team has decided to use Visual Studio App Center automate the iOS application lifecycle. You’ve read that App Center can connect to your repository in minutes, build in the cloud, test on thousands of devices, distribute to beta testers and app stores, and monitor real-world usage with crash and analytics data.

For the next two days you’re going to put App Center to the test to see if it delivers on those promises.

## Challenge 1- CI-CD
*Est. Time to Complete: 60 min*

### 1.1 Setting up Your CI/CD Pipeline (35 min)

**Scenario:** You have your code on your local machine, but as you collaborate with your team, you want to ensure nobody is breaking the build as they all commit their updates. You want an autonomous solution to build this all for you, without hardware to manage and configure. Additionally, you want to have these new builds verified and automatically distributed to an internal alpha test group.

**Challenge:** Connect your code to App Center, configure a continuous build whenever code is submitted that includes a launch test and automatic distribution to a beta test group. Verify everything builds and is distributed

### 1.2 Distribution Management (15 min)

**Scenario:** Now that you have your general build pipeline established, your QA team needs a build delivered to them on a regular basis. Additionally, you want to start sharing your app to external groups, so you will need an additional public test group as well

**Challenge:** Setup and distribute both an internal beta distribution group using the existing build from 1.1, as well as a public test group. Test and confirm.

## Challenge 2- Test
*Est. Time to Complete: 3 hours*

### 2.1 Building your Test Suite (60 min)

**Scenario:** You have added new functionality to your application, and you need to verify it works. Part of your sign-off process is to integrate new automation scripts into your code that can be run on a regular basis to test for any regressions in the future

**Challenge:** Write some automation scripts that will run through and test the functionality of the application.

### 2.2 Uploading and Running your Tests (60 min)

**Scenario:** Once you have written functionality, it can be difficult to ensure your app works on the devices your users are using.

**Challenge:** Create a targeted set of devices in App Center, then upload your app and tests and run them on the device set you created.

### 2.3 CI Revisited (60 min)

**Scenario:** Add Test to your Build process

**Challenge:** Integrate your testing as part of your CI/CD process, where tests will launch after Build is completed. (HINT: App Center lacks the ability to toggle a setting for integration of Build->Test but this can be done in other ways)

## Challenge 3- Monitoring/Learning from your application
*Est. Time to Complete: 120 min*

### 3.1 Crash Reporting and Bug Tracking (60 min)

**Scenario:** Your app is tested, verified and successfully published, but now you are getting reports of crashes from the users. You need better metrics and insight on when these crashes take place, and as much detail about them as possible. Additionally you want to have it integrated into your own bug tracking process to ensure proper workflow and signoff when issues are resolved.

**Challenge:** Add crash reporting to your application, and connect it to the GitHub bug tracker (in your forked repo). Trigger a couple of crashes within your app, and ensure the workflow has been established.

### Challenge 3.2 Event Tracking (60 min)

**Scenario:** With your recently launched app, you want to understand how your app is being used, and if functionality is begin discovered. Additionally you would like greater insight on device usage trends and general session information

**Challenge:** Enable analytics and add manual event tracking to your application, and track the results after a few use cases. Include some additional properties of information for extra detail. (identifiable measurable goals for manual event tracking). Use Log Flow to look at your new events coming in.

## Challenge 4- Azure App Insights
*Est Time to Complete: 90 min*

**Scenario:** You have had your application running for a while now, and have been gathering a great deal of analytics and data. Your teams product lead would like some additional reports on how the application is doing and you are tasked with proving some visual representations of the data.

**Challenge:** Connect your app to Azure Application Insights, set up a data export, then within App Insights create a chart from some of the exported data. Take bucketed events and put it into a graph that can be measured. (Hint: You may need to run the app after setting up export and generate new events to get it to show up in App Insights)

## Challenge 5- Azure Functions
*Est Time to Complete: 60 min*

**Scenario:** After establishing a delivery pipeline and pool of quality testers you feel confident in you can move on to a more automated approach. With all the great analytics and crash data at your fingertips, rather than relying on manual analysis you would like to automatically interpret this data and redistribute a release to a larger public group of testers.

**Challenge:** Setup and debug the sample Azure Function project locally to validate you are able to achieve the desired automation. Follow it up by configuring this Function to run automatically in the cloud every minute by directly hooking up your repository to Azure.

## Challenge 6- Push
*Est Time to Complete: 45 min*

**Scenario:** You have noticed some general usage trends with your application, and want to send a targeted push notification that includes a thank you to your active users, as well as a promo for an upcoming event. You need to create some segmented messaging based on your audiences.

**Challenge:** Set up push notifications for your application, create a push campaign and send the notification. Send a push, send an event when acknowledged.

---

## Bonus 1- Tools Integration
*Est Time to Complete: 30 min*

**Scenario:** My team likes to be notified when new crashes come in, and has some of their own tools as part of the developer process. You would like to integrate App Center into these workflows you already have in place.

**Challenge:** Use webhooks to set up a notification to a third party service you use (Slack, Teams, etc)

## App Center Documentation
Begin with the [Getting Started](https://docs.microsoft.com/en-us/mobile-center/quickstarts/ios/getting-started) tutorial. After you've completed that, you can do the rest in the order below, or choose a specific tutorial to follow.

| Tutorial | Description |
|:-|:-|
| [Getting Started](https://docs.microsoft.com/en-us/appcenter/quickstarts/ios/getting-started) | Set up the app |
| [Build](https://docs.microsoft.com/en-us/appcenter/quickstarts/ios/build) | Build the app |
| [Test](https://docs.microsoft.com/en-us/appcenter/quickstarts/ios/test) | Run automated UI tests on real devices |
| [Distribute](https://docs.microsoft.com/en-us/appcenter/quickstarts/ios/distribute)| Distribute application to a group of users |
| [Crashes](https://docs.microsoft.com/en-us/appcenter/quickstarts/ios/crashes) | Monitor application crashes |
| [Analytics](https://docs.microsoft.com/en-us/appcenter/quickstarts/ios/analytics) | View user analytics |
| [Push](https://docs.microsoft.com/en-us/appcenter/quickstarts/ios/push) | Send push notifications to your app users |

