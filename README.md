# tuya-api-device-control-v1

This project is developed using Tuya SDK, which enables you to quickly  develop smart devices, branded APP, cloud development project, etc.

For more information, please check Tuya Developer Click and Connect      Challenge: https://pages.tuya.com/develop/ClickAndConnect_TuyaDeveloper?_source=e9684c7ca6b31e7221c8420f5af94631
# What would you need for this project?
Materials required: A Tuya IoT Platform Account, Any Tuya compatible smart device (I've used a smart plug), A desktop or laptop with active internet connection.
# Introduction
I've used Tuya's OpenAPI to control my smart device. It is extremely easy and anyone with some basic understanding of technology will be able to do it.
##  Register yourself with Tuya IoT Platform:
* Go to https://pages.tuya.com/develop/Develop_with_Tuya_Mobile?_source=c172143906c877fb833a1f188736b33d&gclid=CjwKCAjww-CGBhALEiwAQzWxOqSJqq0VcQ1uhGDTJEoUzHI-HUHpfT_wv7eYkrXS1G6Kjp1c8nYG8RoC5qsQAvD_BwE and register yourself with the Tuya IoT cloud Platform. It is free and all the materials required are provided by Tuya.
* You should be able to see this dashboard:

![GitHub](/Tuya-img1.png)

## Create a Cloud Project
* Go to Cloud > Create a new Cloud Project
* Click on the Free Trial Button.
* This will open a new tab. Fill in all the details as required.
* Head back to the IoT Dashboard and click on Subscribe.
* Now, you'll be able to create Cloud projects. You should see something like this.
![Cloud Platform Dashboard](/Tuya-img2.png)

* Click on Create. You should see a menu popping up, similar to this:

![GitHub](/Screenshot.png)

* Type in your project details like Project name and description. You can use any name and description.
* Now, select 'Smart Home' for the industry and choose 'Smart Home PaaS' for the development method. You should see something like this:

![GitHub](/Tuya-img4.png)

## Linking your smart Device with Tuya Cloud Platform
* Head over to your smartphone and download the Tuya Smart App.
* Register yourself with the app by providing appropriate details like Email ID and new password.
* Note: You'll need your email ID for verification.
* After loging in, you should be able to see a screen like this:

![GitHub](/Tuya-img5.png)

* Click on the plus button in the right hand corner, and click on the scan icon next to the Auto Scan button.
* Note: Connect your device with the smartplug through WiFi or bluetooth or any other mode of communication.
* After following the onscreen instructions, You should see your homescreen with one device connected to your account. I've already done mine.

* If you have any problems regarding this, contact the Tuya support team.
* Now, head back to your desktop.
* Go to Link Devices:

![GitHub Logo](/Tuya-img7.png)

* And go to Link devices by Account. Now, you should be able to link your account with the Tuya Developer account. 
* Click on 'Add App Account', and scan the QR Code with the Tuya Smart App. Go to '+', Click on the scan button and scan the QR Code.
* Allow all the prompts. You should be able to see your account under the linked accounts section, similar to this:

![GitHub](/Tuya-img8.png)

* Go to Device List and copy the code [Device ID] under the Name of the device.

## Control your device remotely within your desktop
* Now, click on the API Explorer in the left navigation menu.
* You should see a Dashboard similar to this:

![GitHub Logo](/Tuya-img9.png)

* Go to Device Control > Get the instruction set support and paste the device id into the device-id textbox. Then, click on submit request.
* You should see a response window, similar to this:

![GitHub Logo](/Tuya-img10.png)

* Now, from the above response, we'll use the <code>"name": "switch 1"</code> function, and use the True or False values for the input.
* The reason why we use True/False here is that, the function only accepts these values, or simply Boolean values (Data type). Boolean values are basically Yes or No, or True or False.
* Now, go to Device Control > Control Device. 
* Enter your device id and paste the following code on commands textbox:
<code>[{"code":"switch_1","value":true}]</code>
* This may be applicable only for Smart Plugs. For other devices, it may vary accordingly. 
* What this does is that, it switches on your smart device. In my case, it did.
* You should have a response similar to this:

<code>{
  "result": true,
  "success": true,
  "t": 1624808513836
}</code>

* Congratulations, you have successfully controlled your smart device remotely from your desktop. You can do than this. For other info, visit Tuya's documentation for more details.







