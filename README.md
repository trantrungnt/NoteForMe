# Note For Me
##Chú ý
+ Thư viện Exo Player đã thay MediaPlayer trong hình kiến trúc hệ điều hành Android
+ Máy ảo ART đã thay Máy ảo Dalvik
+ Apk là viết tắt của Android Application Package
+ Máy ảo ART và Máy ảo Dalvik đều chạy file thực thi .dex
+ Khi gõ nhầm tên Package, muốn thay đổi thì: refactor trong Android studio (tạo pakage với tên mới), sau đó tìm thư mục tạo package và lấy các file .java trong package cũ và cho vào package có tên mới. sau đó, đổi tên package trong các file java sử dụng tên package mới. Ngoài ra, trong file Manifest ta cũng điền tên Pakcage mới. Cuối cùng, ta Build lại project là được
+ [Sandbox in Android](http://www.androidauthority.com/secure-android-90523/) and [Sandbox](http://researchcenter.paloaltonetworks.com/2014/08/insecure-internal-storage-android/)
+ [Sandbox - Security Tips](https://developer.android.com/training/articles/security-tips.html)
+ [Difference between onCreate and onStart](http://stackoverflow.com/questions/6812003/difference-between-oncreate-and-onstart)
+ [Eclipse Code Formatter Plugin for Android Studio](http://stackoverflow.com/questions/16710367/android-code-style-in-intellij-idea-android-studio)
+ [Android Broad Cast Receiver for screen on and Screen Off](http://stackoverflow.com/questions/9477922/android-broadcast-receiver-for-screen-on-and-screen-off) or [Handing Screeen On](https://thinkandroid.wordpress.com/2010/01/24/handling-screen-off-and-screen-on-intents/)
+ [Start Application knowing package name](http://stackoverflow.com/questions/3422758/start-application-knowing-package-name)
+ [Differences between Intent and Pending Intent](http://stackoverflow.com/questions/24257247/differences-between-intent-and-pendingintent)
+ [How to launch Pending Intent](http://iserveandroid.blogspot.com/2011/03/how-to-launch-pending-intent.html)
+ [Phân biệt foregroudn life time avaf visible life time] (https://duythanhcse.wordpress.com/2013/03/27/bai-tap-6-phan-biet-foreground-lifetime-va-visible-lifetime/)
+ [ví dụ về Pending Intent](http://www.programcreek.com/java-api-examples/android.app.PendingIntent)
+ [Gợi ý chỉnh lại chế độ gới ý tự dộng  tính và code trong Android Studio khi bị lỗi](http://stackoverflow.com/questions/18370599/android-studio-auto-complete-and-other-features-not-working) 
Cách sửa:
```
  Go File > Invalidate Caches / Restart... > Click at Invalidate and Restart
```
+ [Android BroadcastReceiver - Tutorial](http://www.vogella.com/tutorials/AndroidBroadcastReceiver/article.html#pending-intent)
+ [Understanding Android Broadcast Receivers](http://codetheory.in/android-broadcast-receivers/) or [Broad cast Receiver](http://www.tutorialspoint.com/android/android_broadcast_receivers.htm)
+ [Launch application after phone boot or screen unlock in Android using BroadcastReceiver](http://findnerd.com/list/view/Launch-application-after-phone-boot-or-screen-unlock-in-Android-using-BroadcastReceiver/98/) or [autor start custom Android Application](http://www.digi.com/resources/documentation/digidocs/90001945-13/task/android/t_faq_autostart_custom_android_applications.htm) or [Android broad cast receiver for screen on and screen off](http://stackoverflow.com/questions/9477922/android-broadcast-receiver-for-screen-on-and-screen-off) or [Expland: Android Broad Cast Receiver for Scrren on and Screen Off](https://codedump.io/share/svQs8bwGaeGj/1/android-broadcast-receiver-for-screen-on-and-screen-off)
+ [Fragment in Android - VietJack](http://vietjack.com/android/fragment_trong_android.jsp)
+ [Broad Cast Receiver - VietJack](http://vietjack.com/android/broadcast_receiver_trong_android.jsp)
+ [Service - VietJack](http://vietjack.com/android/service_trong_android.jsp)
+ Chú ý: khi đăng ký ở đâu thì hủy tương ứng với nó
(onResume - onPause; onStart - onStop; onCreate - onDestroy)
+ 1 Component Name bao gồm: PakageName + ClassName
+ Explicit Intent (tường minh) thì: biết rõ Component
+ 1 Intent có thể actived: Activity, BroadCast Recevier, Servce
+ onNewIntent ==> để kiểm tra xem: khi tạo 1 Activity mới (A mở B, B mở C, sau đó C mở lại A) thì: Single Top để duy nhất Activity cũ là A được giữ lại, đồng thời xóa các Activity ở Top của Stack
+ [Inflate](http://stackoverflow.com/questions/4448779/how-to-inflate-xml-layout-file-correctly-inside-custom-viewgroup) có thể ép XML thành đối tượng và sử dụng bình thường
+ Mặc định: khi load View trong setContentView thì: Activity đã có sẵn 1 View, khi setContentView thì nó add vào View đó
+ Pending Intent dùng cho trường hợp: đến thời điểm nào đó cần start activity, notifiication ... thì ta mới dùng Pending Intent
+ Không nên dùng Log.d và Log.v khi hiển thị lỗi trong App (để khách hàng nhìn thấy)
+ state-lít có nhiều trạng thái: pressed, select, focus, hover, enable, actived, checkable (=true cho kiểu chọn List các món ăn), che
+ [Android Navigation Drawer Example](https://www.codeofaninja.com/2014/02/android-navigation-drawer-example.html)
+ [Android Navigation drawer ](http://www.journaldev.com/9958/android-navigation-drawer-example-tutorial)
+ [144 Android Navigation Drawer Tutorial Part 1 | coursetro.com](https://www.youtube.com/watch?v=K8hSIP2ha-g)
+ [Config: Android Studio Gradle Could not reserve enough space for object heap](http://stackoverflow.com/questions/30045417/android-studio-gradle-could-not-reserve-enough-space-for-object-heap)
+ [Install Plugin Genymotion in Android Stuido](http://stackoverflow.com/questions/36142055/genymotion-device-doesnt-appear-on-device-chooser-android-studio) or [here](http://stackoverflow.com/questions/27261474/android-studio-doesnt-see-genymotion)
+ Path Default for Android Studio install temp
```
 C:\Users\TEMP\AppData\Local\Android\Sdk
 C:\Users\TrungNT\AppData\Local\Temp //delete cache in my computer
```

+ Coding Convention in Android Studio (use format of Eclip)
```
 File -> Settings -> Plugins.
 click 'Browse repositories' button, enter 'Eclipse Code Formatter' in the search field and install the plugin.
 Restart Android Studio.
```
+ [Life Cycle Fragment](http://www.journaldev.com/9266/android-fragment-example-tutorial-lifecycle)
+ [Use an illeaglArgumentException](http://stackoverflow.com/questions/10344187/is-this-the-correct-way-to-use-an-illegalargumentexception)
+ [View Holder for ListView](https://www.codeofaninja.com/2013/09/android-viewholder-pattern-example.html)
+ [Code app for Tablets and Handsets](https://developer.android.com/guide/practices/tablets-and-handsets.html)
+ [Android app for Phone and Tablets](http://stackoverflow.com/questions/7468049/android-app-for-phone-and-tablet-1-or-2-apps)
+ [Example of an app with PHone and Tablets](https://www.b4x.com/android/forum/threads/example-of-an-app-with-a-phone-and-tablet-layouts.22999/)
+ [Create layout folder for tablet](http://android-er.blogspot.com/2013/04/create-layout-folder-for-tablet.html)
+ [Create layout change Phone - Tablet Android](http://www.coderzheaven.com/2013/02/17/create-layouts-change-phone-tablet-android-fragments/)
+ [Handle different layout for Phone and Tablet](http://android-er.blogspot.com/2013/04/handle-different-layout-for-phone-and.html)
+ [Fragment](https://developer.android.com/training/basics/fragments/index.html)
+ [Creating and Using Fragments](https://guides.codepath.com/android/Creating-and-Using-Fragments)
+ [Full exammple of using fragment](http://www.easyinfogeek.com/2013/07/full-example-of-using-fragment-in.html)
+ [comunuicate fragments](https://developer.android.com/training/basics/fragments/communicating.html)
+ [Activity passing data to fragment throught call backs](http://stackoverflow.com/questions/20040024/activity-passing-data-to-fragment-through-callbacks)
+ [Intorduction to Android - Fragments Tutorial](https://www.raywenderlich.com/117838/introduction-to-android-fragments-tutorial)
+ [How to comunicate between fragments and activities](http://simpledeveloper.com/how-to-communicate-between-fragments-and-activities/)
+ [data sharing between fragments and activity in Android](http://stackoverflow.com/questions/13445594/data-sharing-between-fragments-and-activity-in-android)
+ [Add files to android media library using the media scanner](http://www.grokkingandroid.com/adding-files-to-androids-media-library-using-the-mediascanner/)
+ [Scan media files in Android](http://droidyue.com/blog/2014/01/19/scan-media-files-in-android/)
+ [Android how to check if media scanner](http://sudarnimalan.blogspot.com/2012/05/android-how-to-check-if-media-scanner.html)
+ [Android saving files on internal and external storage](http://codetheory.in/android-saving-files-on-internal-and-external-storage/)
+ [How to Make a Simple Media Player for Android](http://hubpages.com/technology/How-to-Make-a-Simple-Media-Player-for-Android)
+ [Audio Service](https://gettysburg.wccnet.edu/aa/web/chasselb/cps251W12/Web/Contents/Class_Content/AudioService.htm)
+ [Android saving a sound file to sd from resource and setting as ringstone](http://www.stealthcopter.com/blog/2010/01/android-saving-a-sound-file-to-sd-from-resource-and-setting-as-ringtone/)
+ [Meida Scanner - example](http://alvinalexander.com/java/jwarehouse/android/media/java/android/media/MediaScanner.java.shtml)
+ [Refactoring](https://refactoring.guru/refactorings/refactorings)
+ [xposed.mediascanneroptimizer](http://repo.xposed.info/module/com.thomashofmann.xposed.mediascanneroptimizer)
+ [Android Parcelable Example](http://prasanta-paul.blogspot.com/2010/06/android-parcelable-example.html)
+ [Content Provider tutorial in Android with Example](http://www.compiletimeerror.com/2013/12/content-provider-in-android.html#.V7RSQJCg-Va)
+ [Use Content Provider to manage App data](https://www.sitepoint.com/using-androids-content-providers-manage-app-data/)
