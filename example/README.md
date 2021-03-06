# Amplify Analytics Example

This project contains a simple JavaScript website using the Amplify library which sends test events to an AWS Pinpoint application, such as the one created by the `nuage:aws:Analytics` component.

To run this example you will need node.js version 12 or higher.  You will also need the AWS CLI (with correctly configured credentials) and the [Amplify CLI](https://aws-amplify.github.io/docs/).

To launch the website:

* Run the Pulumi program in the root of this project, such that it presents a list of outputs.
* Update the configuration in `app.js` to use your Pinpoint appliction and the Identity Pool created in the last step.
* Run `npm install`
* Run `npm start` and visit `localhost:8080` in your web browser.  Click the button to generate an event.

Note that events will take a minute or so to appear in Pinpoint, and will take 5 minutes to appear in S3.
