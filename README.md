# Post Video Stabilization

This is a demo project that allows users to stabilize video using JavaCV Library.

## Getting Started

To run this project, insert video into device's external directory
```
Take hippo.mp4 from the project folder
```

### Prerequisites

This project requires Android Studio and a mobile phone to be able to run, running on emulator(x86) does not work as it only runs on environment android-arm & android-arm64.

### Dependencies needed

```
implementation 'com.android.support:multidex:1.0.3'
```
```
implementation group: 'org.bytedeco', name: 'javacv', version: '1.4.3'
```
```
implementation group: 'org.bytedeco.javacpp-presets', name: 'ffmpeg', version: '4.1-1.4.4', classifier: 'android-arm'
implementation group: 'org.bytedeco.javacpp-presets', name: 'ffmpeg', version: '4.1-1.4.4', classifier: 'android-arm64'
```
```
implementation group: 'org.bytedeco.javacpp-presets', name: 'opencv', version: '4.0.1-1.4.4', classifier: 'android-arm'
implementation group: 'org.bytedeco.javacpp-presets', name: 'opencv', version: '4.0.1-1.4.4', classifier: 'android-arm64'
```

### Limitations

Currently only able to post proccess videos with no audio frames as frames does not have image data to stabilize.
