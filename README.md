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
