# WebView for Flutter (Developers Preview)

[![pub package](https://img.shields.io/pub/v/webview_flutter.svg)](https://pub.dartlang.org/packages/webview_flutter)

A Flutter plugin that provides a WebView widget.

On iOS the WebView widget is backed by a [WKWebView](https://developer.apple.com/documentation/webkit/wkwebview);
On Android the WebView widget is backed by a [WebView](https://developer.android.com/reference/android/webkit/WebView).

## Developers Preview Status
The plugin relies on Flutter's new mechanism for embedding Android and iOS views.
As that mechanism is currently in a developers preview, this plugin should also be
considered a developers preview.

Known issues are tagged with the [platform-views](https://github.com/flutter/flutter/labels/a%3A%20platform-views) and/or [webview](https://github.com/flutter/flutter/labels/p%3A%20webview) labels.

To use this plugin on iOS you need to opt-in for the embedded views preview by
adding a boolean property to the app's `Info.plist` file, with the key `io.flutter.embedded_views_preview`
and the value `YES`.

Keyboard support within webviews is also experimental. The above tags also
surface known issues with keyboard input. Some currently known keyboard issues,
as of `webview_flutter` version `0.3.10+4`:
* [Keyboard persists after tapping outside text
  field](https://github.com/flutter/flutter/issues/36478)
* [WebView's text selection dialog is not responding to touch
  events](https://github.com/flutter/flutter/issues/24585)
## Setup

### iOS
Opt-in to the embedded views preview by adding a boolean property to the app's `Info.plist` file
with the key `io.flutter.embedded_views_preview` and the value `YES`.

## Usage
Add `webview_flutter` as a [dependency in your pubspec.yaml file](https://flutter.io/platform-plugins/).

You can now include a WebView widget in your widget tree.
See the WebView widget's Dartdoc for more details on how to use the widget.
