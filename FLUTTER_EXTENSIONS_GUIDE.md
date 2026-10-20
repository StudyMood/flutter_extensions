# 🚀 Antigravity Flutter & Dart Extensions - The Ultimate Productivity Guide

> **लक्ष्य (Goal):** Flutter और Dart App Development में आपकी कोडिंग स्पीड को **10x** बढ़ाना!  
> इस गाइड में Antigravity IDE (Open VSX / VS Code आधारित) में उपलब्ध सबसे शक्तिशाली Flutter एक्सटेंशन्स की पूरी जानकारी, उनके उपयोग, शॉर्टकट्स, और प्रैक्टिकल उदाहरण (Before/After) दिए गए हैं।

---

## 📌 विषय सूची (Table of Contents)
1. [Core & Must-Have Extensions (अनिवार्य एक्सटेंशन)](#1-core--must-have-extensions)
   - [Flutter & Dart (Dart-Code)](#1-flutter--dart-by-dart-code)
   - [Pubspec Assist](#2-pubspec-assist-by-jeroen-meijer)
2. [UI, Widgets & Snippet Boosters (डिज़ाइन और कोडिंग स्पीड)](#2-ui-widgets--snippet-boosters)
   - [Awesome Flutter Snippets](#3-awesome-flutter-snippets)
   - [Flutter Widget Wrapper](#4-flutter-widget-wrapper-)
   - [Flutter Color](#5-flutter-color)
3. [Asset & Code Generation Tools (इमेज और मॉडल्स)](#3-asset--code-generation-tools)
   - [Flutter Assets Generator](#6-flutter-assets-generator)
   - [Dart Data Class Generator / Paste JSON as Code](#7-dart-data-class-generator)
4. [State Management & Architecture Helpers (स्टेट मैनेजमेंट)](#4-state-management-helpers)
   - [Bloc (by Felix Angelov)](#8-bloc-by-felix-angelov)
   - [Flutter Riverpod Snippets](#9-flutter-riverpod-snippets)
5. [Testing, Quality & Platform Compatibility (क्वालिटी और टेस्टिंग)](#5-testing-quality--platform)
   - [Flutter Widget Test Preview](#10-flutter-widget-test-preview)
   - [Pubspec Platform](#11-pubspec-platform)
   - [Error Lens](#12-error-lens)
6. [Extension Packs (ऑल-इन-वन बंडल)](#6-extension-packs)
   - [02 Mr Chetan Flutter Extension Pack / Eazy Flutter](#13-extension-packs)
7. [⚡ Ultimate Flutter Keyboard Shortcuts Cheat Sheet](#-ultimate-flutter-keyboard-shortcuts-cheat-sheet)
8. [⚙️ Supercharge Antigravity: Recommended `settings.json`](#-supercharge-antigravity-recommended-settingsjson)

---

## 1. Core & Must-Have Extensions

### 1. Flutter & Dart (by Dart-Code)
* **ID:** `Dart-Code.flutter`, `Dart-Code.dart-code`
* **क्या काम करता है:** यह Flutter डेवलपमेंट की जान है। यह सिंटैक्स हाइलाइटिंग, हॉट रीलोड (Hot Reload), हॉट रीस्टार्ट (Hot Restart), विजेट इंस्पेक्टर (Widget Inspector), डिबगिंग और कोड रिफैक्टरिंग प्रोवाइड करता है।

#### 💡 मुख्य फीचर्स और यूज़ेज:
1. **Quick Fix / Refactor Menu:** `Alt + Enter` या `Ctrl + .` दबाकर किसी भी विजेट को तुरंत:
   - `Wrap with widget...` (किसी भी विजेट से लपेटें)
   - `Wrap with Padding`
   - `Wrap with Center`
   - `Wrap with Row / Column`
   - `Extract Widget` (बड़ा विजेट अलग क्लास में निकालें)
   - `Convert to StatefulWidget / StatelessWidget`
2. **Hot Reload & Hot Restart:**
   - Hot Reload: `r` (टर्मिनल में) या `Ctrl + F5`
   - Hot Restart: `R` या `Ctrl + Shift + F5`
3. **Flutter Doctor Run:** `Ctrl + Shift + P` दबाएं और टाइप करें `Flutter: Run Flutter Doctor`.

#### 💻 प्रैक्टिकल उदाहरण:
```dart
// Before: साधारण Text विजेट
Text("Hello Flutter")

// Shortcut: Cursor 'Text' पर रखें और Alt + Enter दबाकर "Wrap with Padding" चुनें
// After (1 सेकंड में तैयार):
Padding(
  padding: const EdgeInsets.all(8.0),
  child: Text("Hello Flutter"),
)
```

---

### 2. Pubspec Assist (by jeroen-meijer)
* **ID:** `jeroen-meijer.pubspec-assist`
* **क्या काम करता है:** जब भी आपको कोई पैकेज (जैसे `http`, `provider`, `shared_preferences`, `dio`) अपने प्रोजेक्ट में जोड़ना होता है, तो बार-बार pub.dev वेबसाइट पर जाने और लेटेस्ट वर्जन कॉपी करने की ज़रूरत नहीं है।

#### 💡 कैसे यूज़ करें:
1. `Ctrl + Shift + P` दबाएं।
2. टाइप करें: `Pubspec Assist: Add/update dependency`
3. पैकेज का नाम लिखें (जैसे `dio, provider, google_fonts` - कॉमा लगाकर एक साथ कई पैकेज भी लिख सकते हैं)।
4. यह अपने-आप `pubspec.yaml` में सबसे लेटेस्ट कम्पैटिबल वर्जन जोड़ देगा और `flutter pub get` चला देगा!

#### 💻 प्रैक्टिकल उदाहरण:
* **बिना एक्सटेंशन के:** ब्राउज़र खोलो -> pub.dev सर्च करो -> पैकेज ढूंढो -> `dependencies:` में सही इंडेंटेशन के साथ पेस्ट करो। (समय: ~2 मिनट)
* **Pubspec Assist के साथ:** `Ctrl+Shift+P` -> `dio` -> Enter. (समय: 3 सेकंड!)

---

## 2. UI, Widgets & Snippet Boosters

### 3. Awesome Flutter Snippets
* **ID:** `Nash.awesome-flutter-snippets`
* **क्या काम करता है:** बड़े-बड़े बॉइलरप्लेट कोड को केवल 2-4 अक्षरों का शॉर्टकट टाइप करके तुरंत जनरेट कर देता है।

#### 💡 सबसे लोकप्रिय स्निपेट्स (Shortcut Triggers):
| शॉर्टकट ट्रिगर | क्या जनरेट होता है |
| :--- | :--- |
| `stless` | पूरा `StatelessWidget` क्लास स्ट्रक्चर |
| `stful` | पूरा `StatefulWidget` विथ State क्लास स्ट्रक्चर |
| `stanim` | AnimationController के साथ `StatefulWidget` विथ `SingleTickerProviderStateMixin` |
| `initS` | `initState()` मेथड |
| `dis` | `dispose()` मेथड |
| `bldr` | `Builder` विजेट |
| `listv` | `ListView.builder` विथ `itemCount` और `itemBuilder` |

#### 💻 प्रैक्टिकल उदाहरण:
खाली फाइल में केवल `stless` लिखें और `Tab` या `Enter` दबाएं:
```dart
class MyWidget extends StatelessWidget {
  const MyWidget({super.key});

  @override
  Widget build(BuildContext context) {
    return const Placeholder();
  }
}
```

---

### 4. Flutter Widget Wrapper 🚀
* **ID:** `tahadarwish.flutter-widget-wrapper`
* **क्या काम करता है:** विजेट्स को तेज़ी से रैप (Wrap) करने के लिए शॉर्टकट और डेडिकेटेड कमांड्स देता है। (जैसे Container, Expanded, SizedBox, Visibility, Builder, StreamBuilder, आदि)।

#### 💡 कैसे यूज़ करें:
- कोड में विजेट सेलेक्ट करें और राइट-क्लिक करें या शॉर्टकट से सीधे रैप करें:
  - Wrap with `Expanded`
  - Wrap with `SizedBox`
  - Wrap with `Positioned`
  - Wrap with `Visibility`
  - Wrap with `Flexible`

---

### 5. Flutter Color
* **ID:** `circlecodesolution.fluttercolor`
* **क्या काम करता है:** कोड में लिखे कलर कोड्स (जैसे `Color(0xFF2196F3)` या `Colors.blue`) को एडिटर में ही लाइव कलर बॉक्स की तरह दिखाता है।

#### 💡 फायदा:
- बिना ऐप रन किए पता चल जाता है कि कौन सा हेक्स कोड किस शेड का है।
- कलर बॉक्स पर क्लिक करके आप डायरेक्ट कलर पिकर (Color Picker) से नया कलर भी सेलेक्ट कर सकते हैं।

#### 💻 प्रैक्टिकल उदाहरण:
```dart
// एडिटर में इसके बगल में एक नीला कलर बॉक्स दिखेगा:
Color brandPrimary = const Color(0xFF1E88E5); 
```

---

## 3. Asset & Code Generation Tools

### 6. Flutter Assets Generator
* **ID:** `ramgopal.flutter-assets-generator`
* **क्या काम करता है:** इमेजेस और आइकन्स के पाथ (Path) में गलत स्पेलिंग की वजह से आने वाले **"Asset not found"** एरर को हमेशा के लिए खत्म करता है। यह आपके `assets/` फोल्डर को स्कैन करके एक टाइप-सेफ डार्ट क्लास (जैसे `Assets.imagesLogo`) बना देता है।

#### 💡 कैसे यूज़ करें:
1. अपनी इमेजेज को `assets/images/` फोल्डर में रखें।
2. एक्सटेंशन रन करें (`Ctrl + Shift + P` -> `Generate Flutter Assets`).
3. यह तुरंत `assets.dart` या `constants.dart` फाइल बना देगा।

#### 💻 प्रैक्टिकल उदाहरण:
```dart
// ❌ पुराना तरीका (स्पेलिंग गलती होने का भारी खतरा):
Image.asset('assets/images/user_prfile_banner.png') // Crash! 'profile' ki spelling galat hai

// ✅ नए तरीके से (Type-safe & Auto-complete):
Image.asset(Assets.imagesUserProfileBanner) // Code completion se select karein!
```

---

### 7. Dart Data Class Generator / Paste JSON as Code
* **ID:** `brapifra.phparchitect` (Dart Data Class) या `quicktype.quicktype`
* **क्या काम करता है:** API इंटीग्रेशन के समय JSON रेस्पॉन्स को हाथ से मॉडल क्लास में लिखने में घंटों बर्बाद होते हैं। यह एक्सटेंशन 2 सेकंड में JSON से पूरी Dart Model क्लास तैयार कर देता है।

#### 💡 क्या-क्या जनरेट करता है:
- `Constructor`
- `fromJson(Map<String, dynamic> json)`
- `toJson()`
- `copyWith()`
- `toString()`
- `==` और `hashCode`

#### 💻 प्रैक्टिकल उदाहरण:
मान लीजिए API से यह JSON मिला:
```json
{
  "id": 101,
  "name": "Rahul Sharma",
  "email": "rahul@example.com",
  "is_active": true
}
```
**Quicktype / Dart Data Class Generator** इसे 1 सेकंड में इस क्लास में बदल देगा:
```dart
class UserModel {
  final int id;
  final String name;
  final String email;
  final bool isActive;

  UserModel({required this.id, required this.name, required this.email, required this.isActive});

  factory UserModel.fromJson(Map<String, dynamic> json) => UserModel(
    id: json['id'],
    name: json['name'],
    email: json['email'],
    isActive: json['is_active'],
  );

  Map<String, dynamic> toJson() => {
    'id': id,
    'name': name,
    'email': email,
    'is_active': isActive,
  };
}
```

---

## 4. State Management Helpers

### 8. Bloc (by Felix Angelov)
* **ID:** `FelixAngelov.bloc`
* **क्या काम करता है:** यदि आप **BLoC** या **Cubit** स्टेट मैनेजमेंट यूज़ करते हैं, तो यह एक्सटेंशन मस्ट-हैव है।

#### 💡 मुख्य फीचर्स:
- **New Bloc / Cubit in 1-Click:** किसी भी फोल्डर पर राइट-क्लिक करें -> **"Bloc: New Bloc"** या **"Bloc: New Cubit"** चुनें।
  - यह अपने-आप `auth_bloc.dart`, `auth_event.dart`, और `auth_state.dart` फाइलें जनरेट कर देगा।
- **Wrap with Bloc:** किसी विजेट पर `Alt + Enter` दबाएं:
  - `Wrap with BlocBuilder`
  - `Wrap with BlocConsumer`
  - `Wrap with BlocProvider`
  - `Wrap with BlocListener`

---

### 9. Flutter Riverpod Snippets
* **ID:** `carlos-menezes.riverpod-snippets`
* **क्या काम करता है:** Riverpod 2.x के सभी प्रोवाइडर्स और कंज्यूमर्स के लिए रेडीमेड स्निपेट्स।

#### 💡 स्निपेट्स:
- `consumer` -> `ConsumerWidget`
- `stfulconsumer` -> `ConsumerStatefulWidget`
- `prov` -> `Provider((ref) => ...)`
- `notifprov` -> `NotifierProvider`
- `refw` -> `ref.watch(...)`

---

## 5. Testing, Quality & Platform

### 10. Flutter Widget Test Preview (by FelipeFontes)
* **ID:** `FelipeFontes.flutter-widget-test-preview`
* **क्या काम करता है:** Flutter में जब हम विजेट टेस्ट (`testWidgets`) लिखते हैं, तो स्क्रीन दिखती नहीं है। यह एक्सटेंशन आपके टेस्ट रन करते समय साइडबार में लाइव विजेट रेंडर करके विज़ुअली दिखा देता है!
* **AI & MCP Tools:** इसमें AI असिस्टेंट्स के साथ लाइव विजेट इंस्पेक्ट करने की क्षमता भी होती है।

---

### 11. Pubspec Platform (by ygorazambuja)
* **ID:** `ygorazambuja.pubspec-platform`
* **क्या काम करता है:** जब आप कोई पैकेज `pubspec.yaml` में डालते हैं, तो कई बार वह पैकेज केवल Android या iOS सपोर्ट करता है (Web, Windows या macOS नहीं)।
- यह एक्सटेंशन `pubspec.yaml` में पैकेज के नाम के ठीक ऊपर दिखाता है कि यह पैकेज किन-किन प्लेटफॉर्म्स (`Android`, `iOS`, `Web`, `Windows`, `macOS`, `Linux`) पर सपोर्टेड है।
- इससे प्रोडक्शन में ऐप क्रैश होने से बच जाता है।

---

### 12. Error Lens (by usernamehw)
* **ID:** `usernamehw.errorlens`
* **क्या काम करता है:** सामान्यतः एरर देखने के लिए नीचे दिए "Problems" टैब में जाना पड़ता है। Error Lens किसी भी सिंटैक्स एरर या वॉर्निंग को कोड की लाइन के अंत में लाल/पीले रंग में टेक्स्ट के साथ तुरंत दिखा देता है।

---

## 6. Extension Packs

### 13. 02 Mr Chetan Flutter Extension Pack / Eazy Flutter
* **Mr Chetan Flutter Extension Pack:** यदि आप एक-एक करके 10 एक्सटेंशन डाउनलोड नहीं करना चाहते, तो यह बंडल पैक एक क्लिक में लोकप्रिय Flutter टूल्स, स्निपेट्स और थीमिंग को इंस्टॉल कर देता है।
* **Eazy Flutter:** क्विक एक्शन्स, ऑटो-इम्पोर्ट और प्रोजेक्ट सेटअप कमांड्स को आसान बनाता है।

---

## ⚡ Ultimate Flutter Keyboard Shortcuts Cheat Sheet

| शॉर्टकट (Windows) | एक्शन / काम |
| :--- | :--- |
| `Alt + Enter` या `Ctrl + .` | **Quick Fix:** Wrap with Widget, Extract Widget, Remove Widget |
| `F5` | Start Debugging (ऐप चालू करें) |
| `Ctrl + F5` | Run Without Debugging |
| `Shift + F5` | Stop Debugging (ऐप बंद करें) |
| `Ctrl + Shift + F5` | Hot Restart (पूरी ऐप रीलोड करें) |
| `r` (इन टर्मिनल) | Hot Reload (सिर्फ UI चेंज तुरंत देखें) |
| `Ctrl + Shift + P` | Command Palette (Flutter Doctor, New Project, Pubspec Assist) |
| `Shift + Alt + F` | Auto Format Code (कोड को सुंदर और इंडेंट करें) |
| `Ctrl + P` | Go to File (नाम लिखकर तुरंत फाइल खोलें) |

---

## ⚙️ Supercharge Antigravity: Recommended `settings.json`

Antigravity IDE में Flutter की परफॉर्मेंस और ऑटोमेशन को और तेज़ करने के लिए `Ctrl + Shift + P` दबाएं, **"Preferences: Open User Settings (JSON)"** खोलें, और ये सेटिंग्स जोड़ें:

```json
{
  // हर बार सेव करने पर कोड अपने आप फॉर्मेट होगा और कॉमा के अनुसार सही स्ट्रक्चर बन जाएगा
  "editor.formatOnSave": true,
  "editor.codeActionsOnSave": {
    "source.fixAll": "explicit",
    "source.organizeImports": "explicit"
  },

  // Flutter UI Guides (पेरेंट और चाइल्ड विजेट्स के बीच गाइड लाइन दिखेगी)
  "dart.previewFlutterUiGuides": true,
  
  // कोड के आखिरी क्लोजिंग ब्रैकेट के पास विजेट का नाम दिखेगा (Closing Labels)
  "dart.closingLabels": true,

  // ऑटोमैटिक ब्रैकेट कलर पेयरिंग
  "editor.bracketPairColorization.enabled": true,
  "editor.guides.bracketPairs": "active"
}
```

---

## 🎯 सारांश (Summary) - आपकी कोडिंग स्पीड कैसे 10x होगी?

1. **बॉइलरप्लेट कोड के लिए:** `Awesome Flutter Snippets` (`stless`, `stful`).
2. **पैकेज जोड़ने के लिए:** `Pubspec Assist` (`Ctrl + Shift + P`).
3. **विजेट्स मॉडिफाई करने के लिए:** `Alt + Enter` (Dart-Code Quick Fix) और `Flutter Widget Wrapper`.
4. **API और JSON के लिए:** `Dart Data Class Generator / Quicktype`.
5. **एसेट्स एरर से बचने के लिए:** `Flutter Assets Generator`.
6. **कलर और एरर तुरंत पकड़ने के लिए:** `Flutter Color` और `Error Lens`.

*इस फाइल को अपने प्रोजेक्ट में बुकमार्क रखें या टीम के साथ शेयर करें ताकि पूरी टीम की प्रोडक्टिविटी दोगुनी हो सके!* 🚀
