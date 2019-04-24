# Xamarin.Forms UI Challenge

Initial bootstrap repository used to start Xamarin.Forms UI Challenges that we do here @ [Lambda3](https://lambda3.com.br/). It comes with [HotReload](https://github.com/AndreiMisiukevich/HotReload) included with [Cake](https://cakebuild.net).

## Running HotReload 🔥

The app is configured to listen on port `4290` for Android and port `4291` for iOS.

To activate HotReload for XAML pages, just run this **after** your iOS Simulator and Android Emulator are running. You don't have to be debugging your app, it just needs to be open, you should be able to see the changes simultaneously on iOS and Android.

Running the Cake task on Windows 💻:

```bash
./build.ps1 -Target HotReload
```

Running the Cake task on Mac 👩‍💻:

```bash
./build.sh -Target=HotReload
```