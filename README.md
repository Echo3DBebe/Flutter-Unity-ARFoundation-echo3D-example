# Unity-Flutter-echo3D-example
Starter project to build Android apps using Flutter & Unity with echo3D.

## Setup
* Built with Unity 2020.3.25.  _(Note: The echo3D Unity SDK is supported in 2020.3.25 and higher.)_
* Register for FREE at [echo3D](https://console.echo3D.co/#/auth/register).
* [Add the Unity SDK](https://medium.com/r/?url=https%3A%2F%2Fdocs.echo3d.co%2Funity%2Finstallation). Troubleshoot [here](https://docs.echo3d.com/unity/troubleshooting#im-getting-a-newtonsoft.json.dll-error-in-unity).
* Clone this repo. 

## Steps
1. In your flutter project folder, create a new Unity project or clone our [Unity-ARFoundation-echo3D-example](https://github.com/echo3Dco/Unity-ARFoundation-echo3D-example) and jump to step 4.
2. [Install the echo3D Unity SDK](https://docs.echo3D.co/unity/installation).
3. Open the sample scence under `echo3D/Examples/Sample.unity`.
4 [Set the API key](https://docs.echo3d.co/quickstart/access-the-console) and Entry IDs for those same models in the Inspector. <br>
![APIKeyandEntryId](https://user-images.githubusercontent.com/99516371/195749269-f7a43477-b67a-49e8-a212-6abdb9c948fd.png)<br>
![NEWAPIKeyandEntryID](https://user-images.githubusercontent.com/99516371/205407613-b746840f-8e8a-4ec8-b056-a680395dfab4.png)<br>
5. [Type your Secret Key](https://docs.echo3d.co/web-console/deliver-pages/security-page#secret-key) as the value for the parameter secKey in the file Packages/co.echo3D.unity/Runtime/Echo3DHologram.cs. _(Note: Secret Key only matters if you have the Security Key enabled). You can turn it off in the Security options in your echo3D console._
![NEWSecKey2](https://user-images.githubusercontent.com/99516371/195749308-b2349a3b-7e43-4d3c-8f09-fbfa9d3cb0be.png).<br>
* (Recommended) To move, resize or edit the assets live in your Scene view, check the boxes for “Editor Preview” and “Ignore Model Transforms”. To enable this, click Echo3D > Load Editor Holograms in your Unity toolbar. <br>
![EditorPreviewAndIgnoreModelTransforms](https://user-images.githubusercontent.com/99516371/195749348-dc0b06ad-efa6-4dbd-962f-0119b5c33ea0.png).<br>
![LoadHolograms](https://user-images.githubusercontent.com/99516371/195749354-b2295183-f877-444a-af22-ed87ffb17705.png). <br>

## Flutter Fonfiguration
* Import the project dependecies by running `flutter pub get` from your terminal

## Unity Project Build Settings
* Follow the instructions for the [flutter_unity](https://pub.dev/packages/flutter_unity#-readme-tab-) plugin.

## Run
* Open your `main.dart` file
* Find and replace the value `<YOUR-PROJECT-KEY>` with your API key and uncomment the code line
* Find and replace the value `<YOUR-ENTRY-ID>` with your model's entry ID and uncomment the code line
* Save the file and run the project on an andorid phone

## Learn more
Refer to our [documentation](https://docs.echo3D.co/unity/) to learn more about how to use Unity and echo3D.

This project uses a [third party library](https://pub.dev/packages/flutter_unity#-readme-tab-).

## Support
Feel free to reach out at [support@echo3D.co](mailto:support@echo3D.co) or join our [support channel on Slack](https://go.echo3D.co/join).

## Screenshots
![Flutter with Unity scene screenshot](/images/Flutter%20with%20Unity.jpg)
![echo3D console screenshot](/images/Console.jpg)
