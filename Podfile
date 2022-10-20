source "https://cdn.cocoapods.org/"
platform :ios, 14.0
use_frameworks!
inhibit_all_warnings!
plugin 'cocoapods-binary'

target 'PodsBinaryFixture' do
  pod 'SwiftLint', :binary => true

  pod "Firebase", :binary => true
  pod 'FirebaseAuth', :binary => true
  pod 'FirebaseCore', :binary => true
  pod 'FirebaseCoreDiagnostics', :binary => true
  pod 'FirebaseCoreExtension', :binary => true
  pod 'FirebaseCoreInternal', :binary => true
  pod 'FirebaseDatabase', :binary => true
  pod 'FirebaseDynamicLinks', :binary => true
  pod 'FirebaseFirestore', :binary => true
  pod 'FirebaseFunctions', :binary => true
  pod 'FirebasePerformance', :binary => true
  pod 'FirebaseStorage', :binary => true
  pod 'Firebase/Messaging', :binary => true
  pod "Firebase/Analytics", :binary => true
  pod "Firebase/Performance", :binary => true
  pod "Firebase/Crashlytics", :binary => true
  pod 'FirebaseRemoteConfig', :binary => true

  pod "FBSDKCoreKit", :binary => true
  pod "FBSDKLoginKit", :binary => true

  pod 'GoogleAnalytics', :binary => true
  pod "GoogleSignIn", :binary => true
end

post_install do |installer|
  installer.pods_project.targets.each do |target|
    target.build_configurations.each do |config|
      config.build_settings['IPHONEOS_DEPLOYMENT_TARGET'] = '14.0'
    end
  end
end
