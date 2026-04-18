# RuralDoc-Connect
  This web platform helps farmers and cattle owners in remote areas find nearby doctors by entering their village and location, ensuring quick access to essential healthcare even where network is poor.
📁 File Structure
go_raksha/
├── lib/
│   ├── main.dart                    # App entry + MaterialApp + green theme
│   ├── models/
│   │   ├── doctor_model.dart        # Doctor class + Firestore deserialization
│   │   ├── scheme_model.dart        # GovtScheme + 4 sample Kannada schemes
│   │   └── first_aid_model.dart     # 5 first aid tips in Kannada
│   └── screens/
│       ├── home_screen.dart         # Dashboard with 4 menu tiles + emergency banner
│       ├── doctor_list_screen.dart  # Search + filter + Call Now button
│       ├── schemes_screen.dart      # Expandable scheme cards with "How to Apply"
│       └── first_aid_screen.dart    # Numbered steps with warning banners
├── pubspec.yaml                     # Firebase + url_launcher dependencies
└── FIREBASE_SETUP.md                # Step-by-step Firebase + calling setup guide

🚀 Quick Start
1. Install dependencies:
bashflutter pub get
2. Connect Firebase (see FIREBASE_SETUP.md):
bashflutterfire configure --project=your-project-id
3. Enable phone calls — add to AndroidManifest.xml:
xml<queries>
  <intent><action android:name="android.intent.action.DIAL"/>
  <data android:scheme="tel"/></intent>
</queries>
4. Run:
bashflutter run

✅ Key Features Included
FeatureDetails🏠 Home ScreenGreen gradient header, 4 menu tiles, emergency 1962 helpline banner👨‍⚕️ Doctor LocatorLive search by village/taluk, Govt/Private filter chips, "ಈಗ ಕರೆ ಮಾಡಿ" button🏛️ Govt Schemes4 schemes (Lumpy relief, free vaccine, KCC, livestock insurance) with expandable "How to Apply" steps🩹 First Aid5 tips with numbered steps, color-coded by category, warning banners📴 Offline ReadySample data works without Firebase for demosMainCode · DART OpenHome screenCode · DART OpenDoctor list screenCode · DART OpenSchemes screenCode · DART OpenFirst aid screenCode · DART OpenDoctor modelCode · DART OpenScheme modelCode · DART OpenFirst aid modelCode · DART OpenPubspecYAML OpenFirebase setupDocument · MD OpenDownload all
        @keyframes bannerSlideUp {
          from {
            opacity: 0;
            transform: translateY(8px);
          }
          to {
            opacity: 1;
            transform: translateY(0);
          }
        }
      Next time, try this in CoworkHand off complex tasks for Claude to handle independently. Come back to finished results.Upgrade to tryUpgrade to try
