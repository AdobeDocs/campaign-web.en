---
audience: end-user
title: Design a push notification delivery
description: Learn how to design a push notification delivery with Adobe Campaign Web
badge: label="Alpha" type="Positive"
---
# Design a push delivery {#content-push}

## Message {#push-message}

>[!BEGINTABS]

>[!TAB Android]

With Firebase Cloud Messaging, you can choose between two types of messages:

* The **Data message**, handled by the client app. Messages are sent directly to the mobile application which will generate and display the android notification to the device. Data messages contain only your custom application variables.
    
    Click the **[!UICONTROL Message]** field and use the Expression editor to define content, personalize data and add dynamic content.

* The Notification message, handled automatically by the FCM SDK. FCM automatically displays the message on your users’ devices on behalf of the client app. Notification messages contain a predefined set of parameters and options but can still be further personalized with custom application variables.

    To compose your message, click the **[!UICONTROL Title]** and **[!UICONTROL Body]** fields. Use the Expression editor to define content, personalize data and add dynamic content.
    
    To further personalize your push notification, you can choose an image to add to your push notification, the notification’s icon to display on your profiles’ devices and its color.

>[!BEGINTABS]

>[!TAB iOS]

To compose your message, click the **[!UICONTROL Title]** and **[!UICONTROL Body]** fields. Use the Expression editor to define content, personalize data and add dynamic content.

You can add a **[!UICONTROL Subtitle]**, value of the subtitle parameter of the iOS notification payload. Refer to the this section.

The Silent Push mode allows a “silent” notification to be sent to a mobile application. The user is not made aware of the notification’s arrival. It is transferred directly to the application.

>[!ENDTABS]

## Advanced settings {#push-advanced}

>[!BEGINTABS]


* **[!UICONTROL Sound]**: Set the sound to play when the device receives your notification.

* **[!UICONTROL Notification Count]**: Set the number of new unread information to display directly on the application icon.

* **[!UICONTROL Channel ID]**: Set your notification’s channel ID. The app must create a channel with this channel ID before any notification with this channel ID is received.

* **[!UICONTROL Click action]**: Set the action associated with a user click on your notification.

* **[!UICONTROL Tag]**: Set the identifier used to replace existing notifications in the notification drawer.

* **[!UICONTROL Priority]**: Set the priority levels of your notification to default, minimum, low or high. For more on this, refer to FCM documentation.

* **[!UICONTROL Visibility]**: Set the visibility levels of your notification to public, private or secret. For more on this, refer to FCM documentation.

* **[!UICONTROL Sticky]**: If deactivated, the notification is automatically dismissed when the user clicks it. If activated, the notification is still displayed even when the user clicks it.

>[!BEGINTABS]

>[!TAB iOS]

* **[!UICONTROL Critical alert mode]**: enable this option to add sound to your notification even the user’s phone is set on focus mode or if the iPhone is muted.

* **[!UICONTROL Clean Badge]**: enable this options to refresh the badge value.

* **[!UICONTROL Notification count]**: set a number which will be used to display directly on the application icon the number of new unread information.

* **[!UICONTROL Volume]**: volume of your sound from 0 to 100.

* **[!UICONTROL Mutable content]** (iOS only): Sends the mutable-content flag in the push payload and will allow the push notification content to be modified by a notification service application extension provided in iOS SDK. For more on this, refer to [Apple developer documentation](https://developer.apple.com/library/content/documentation/NetworkingInternet/Conceptual/RemoteNotificationsPG/ModifyingNotifications.html). enable this option to allow the mobile application to download media content.

* **[!UICONTROL Relevance score]**: set a relevance score from 0 to 100. The system uses this to sort the notifications in the notification summary.

* **[!UICONTROL Interruption level]**:

    * **[!UICONTROL Active]**: Set by default, the system presents the notification immediately, lights up the screen, and can play a sound. Notifications do not break through Focus modes.

    * **[!UICONTROL Passive]**: The system adds the notification to the notification list without lighting up the screen or playing a sound. Notifications do not break through Focus modes.

    * **[!UICONTROL Time sensitive]**: The system presents the notification immediately, lights up the screen, can play a sound and break through Focus modes. This level does not require a special permission from Apple.

    * **[!UICONTROL Critical]**: The system presents the notification immediately, lights up the screen, and bypasses the mute switch or focus modes. Note that this level requires a special permission from Apple.

* **[!UICONTROL Thread-id]**: identifier used to group related notifications together.

* **[!UICONTROL Category]**: name of your category ID which will display action buttons. These notifications give the user a faster way to perform different tasks in response to a notification without opening or navigating in the application.

* **[!UICONTROL Target content ID]**: identifier used to target which application window to brought forward when the notification is opened.

* **[!UICONTROL Launch image]**: name of the launch image file to display. If the user chooses to launch your application, the selected image will displayed instead of your application’s launch screen.

>[!ENDTABS]

<!--Sounds must be included in the application and defined when the service is created. Refer to this section.-->



