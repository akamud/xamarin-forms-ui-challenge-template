# Xamarin.Forms UI Challenge Template

Project template used to start Xamarin.Forms UI Challenges that we do here @ [Lambda3](https://lambda3.com.br/). It comes with [HotReload](https://github.com/AndreiMisiukevich/HotReload) included with [Cake](https://cakebuild.net).

You can just download the `template` folder and add everything to your solution, but it is recommended to use it as a template.

## Using it as a template

1. Clone this project anywhere.

2. Download the MonoDevelop Template Creator Addin for Visual Studio for Mac  
Search for the [Template Creator](https://github.com/mrward/monodevelop-template-creator-addin) addin in the Gallery.

3. After it is installed, open the Visual Studio for Mac preferences, search for **Template > Custom Folders**. Add the directory for the `xamarin-forms-ui-challenge`.

![https://raw.githubusercontent.com/akamud/xamarin-forms-ui-challenge-template/master/preferences.png](https://raw.githubusercontent.com/akamud/xamarin-forms-ui-challenge-template/master/preferences.png)

4. Now it should come up when creating a new solution under **Multiplatform > App**:

![https://raw.githubusercontent.com/akamud/xamarin-forms-ui-challenge-template/master/new-solution.png](https://raw.githubusercontent.com/akamud/xamarin-forms-ui-challenge-template/master/new-solution.png)

## Running HotReload 🔥

The app is configured to listen on port `4290` for Android and port `4291` for iOS.

To activate HotReload for XAML pages, just run this **after** your iOS Simulator and Android Emulator are running. You don't have to be debugging your app, it just needs to be open, you should be able to see the changes simultaneously on iOS and Android.

### Running the Cake task on Windows 💻:

```bash
./build.ps1 -Target HotReload
```

### Running the Cake task on Mac 👩‍💻:

First make sure you have given permission to the `build.sh` script:

```bash
chmod +x build.sh
```

Then:

```bash
./build.sh -Target=HotReload
```

## Further Improvements

* Create an Addin to facilitate the template usage.
