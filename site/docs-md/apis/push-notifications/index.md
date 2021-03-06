<plugin-platforms platforms="ios,android"></plugin-platforms>

# Push Notifications

The Push Notifications API provides methods for registering a device to receive notifications from a server, along with processing received notifications and responding to them. In contrast, the [Local Notifications](../local-notifications) API provides means for offline, local notification scheduling and processing.

## Enabling Push Notifications Capabilites

On iOS it's required to enable Push Notifications Capabilities in your project to make Push Notifications plugin work. To do so, go to the `Capabilities` section of your app and switch the `Push Notifications` button from `OFF` to `ON` possition.

That will add the push capabilites to your app and will create an entitlements file.

![Enabling Push Notifications Capabilities](./img/enable-push-capabilities.png)

## Disabling Push Notifications plugin

If you are not using Push Notifications in your project, when you submit the app to iTunes Connect, Apple will send you an email saying it has issues because of `Missing Push Notification Entitlement`. That happens because Capacitor includes the code for registering for push notifications and getting the token.

Apple sends that mail just to make sure you didn't make a mistake and forgot to enable Push Notifications Capabilities in your app, but can safely ignore it if you are not using the Push Notifications plugin.

In case you don't want to receive the mail, you can disable the Push Notifications plugin by removing `USE_PUSH` from `Active Compilation Conditions` in your project's Build Settings section.

![Disable Push Notifications](./img/disable-push-plugin.png)


<plugin-api index="true" name="push-notifications"></plugin-api>


## Example

## API

<plugin-api name="push-notifications"></plugin-api>