footer: © Fyber GmbH, 2014
slidenumbers: true

# Analyzing Crash Reports

---
```
Incident Identifier: E44AD7C2-4F93-47A8-A1D7-CB619425EFB1
CrashReporter Key:   5f34f05ff9130504d107ebb1aadfe546e55af43c
Hardware Model:      iPhone7,2
Process:             Crashy [8364]
Path:                /private/var/mobile/Containers/Bundle/Application/83FB728B-ACE7-4D2B-9CB2-D24901F83FFB/Crashy.app/Crashy
Identifier:          com.fyber.Crashy
Version:             1 (1.0)
Code Type:           ARM-64 (Native)
Parent Process:      launchd [1]

Date/Time:           2015-03-01 08:18:47.887 +0100
Launch Time:         2015-03-01 08:18:46.159 +0100
OS Version:          iOS 8.1.3 (12B466)
Report Version:      105

Exception Type:  EXC_CRASH (SIGABRT)
Exception Codes: 0x0000000000000000, 0x0000000000000000
Triggered by Thread:  0

Last Exception Backtrace:
0   CoreFoundation                	0x1883aa59c __exceptionPreprocess + 132
1   libobjc.A.dylib               	0x198af40e4 objc_exception_throw + 60
2   CoreFoundation                	0x188292d40 -[__NSPlaceholderArray initWithObjects:count:] + 412
3   CoreFoundation                	0x18829eff8 +[NSArray arrayWithObjects:count:] + 60
4   Crashy                        	0x100052d10 0x10004c000 + 27920
5   UIKit                         	0x18cb8d418 -[UIApplication sendAction:to:from:forEvent:] + 96
6   UIKit                         	0x18cb7652c -[UIControl _sendActionsForEvents:withEvent:] + 612
7   UIKit                         	0x18cb8cdb4 -[UIControl touchesEnded:withEvent:] + 592
8   UIKit                         	0x18cb8ca40 -[UIWindow _sendTouchesForEvent:] + 700
9   UIKit                         	0x18cb85f94 -[UIWindow sendEvent:] + 684
10  UIKit                         	0x18cb5968c -[UIApplication sendEvent:] + 264
11  UIKit                         	0x18cdf860c _UIApplicationHandleEventFromQueueEvent + 14992
12  UIKit                         	0x18cb57bf4 _UIApplicationHandleEventQueue + 1616
13  CoreFoundation                	0x1883629ec __CFRUNLOOP_IS_CALLING_OUT_TO_A_SOURCE0_PERFORM_FUNCTION__ + 24
14  CoreFoundation                	0x188361c90 __CFRunLoopDoSources0 + 264
15  CoreFoundation                	0x18835fd40 __CFRunLoopRun + 712
16  CoreFoundation                	0x18828d0a4 CFRunLoopRunSpecific + 396
17  GraphicsServices              	0x1914275a4 GSEventRunModal + 168
18  UIKit                         	0x18cbbeaa4 UIApplicationMain + 1488
19  Crashy                        	0x100052e14 0x10004c000 + 28180
20  libdyld.dylib                 	0x199162a08 start + 4


Thread 0 name:  Dispatch queue: com.apple.main-thread
Thread 0 Crashed:
0   libsystem_kernel.dylib        	0x000000019927b270 __pthread_kill + 8
1   libsystem_pthread.dylib       	0x0000000199319224 pthread_kill + 108
2   libsystem_c.dylib             	0x00000001991f2b14 abort + 108
3   libc++abi.dylib               	0x00000001982c5414 abort_message + 112
4   libc++abi.dylib               	0x00000001982e4b88 default_terminate_handler() + 300
5   libobjc.A.dylib               	0x0000000198af43bc _objc_terminate() + 124
6   libc++abi.dylib               	0x00000001982e1bb0 std::__terminate(void (*)()) + 12
7   libc++abi.dylib               	0x00000001982e1738 __cxa_rethrow + 140
8   libobjc.A.dylib               	0x0000000198af4290 objc_exception_rethrow + 40
9   CoreFoundation                	0x000000018828d150 CFRunLoopRunSpecific + 568
10  GraphicsServices              	0x00000001914275a0 GSEventRunModal + 164
11  UIKit                         	0x000000018cbbeaa0 UIApplicationMain + 1484
12  Crashy                        	0x0000000100052e10 0x10004c000 + 28176
13  libdyld.dylib                 	0x0000000199162a04 start + 0

Thread 1 name:  Dispatch queue: com.apple.libdispatch-manager
Thread 1:
0   libsystem_kernel.dylib        	0x0000000199260c94 kevent64 + 8
1   libdispatch.dylib             	0x000000019914897c _dispatch_mgr_invoke + 272
2   libdispatch.dylib             	0x000000019913b3b0 _dispatch_mgr_thread + 48

Thread 2:
0   libsystem_kernel.dylib        	0x000000019927bc78 __workq_kernreturn + 8
1   libsystem_pthread.dylib       	0x0000000199315390 _pthread_wqthread + 988
2   libsystem_pthread.dylib       	0x0000000199314fa4 start_wqthread + 0

Thread 3:
0   libsystem_kernel.dylib        	0x000000019927bc78 __workq_kernreturn + 8
1   libsystem_pthread.dylib       	0x0000000199315390 _pthread_wqthread + 988
2   libsystem_pthread.dylib       	0x0000000199314fa4 start_wqthread + 0

Thread 4:
0   libsystem_kernel.dylib        	0x000000019927bc78 __workq_kernreturn + 8
1   libsystem_pthread.dylib       	0x0000000199315390 _pthread_wqthread + 988
2   libsystem_pthread.dylib       	0x0000000199314fa4 start_wqthread + 0

Thread 0 crashed with ARM Thread State (64-bit):
    x0: 0x0000000000000000   x1: 0x0000000000000000   x2: 0x0000000000000000   x3: 0x00000001740f6ab7
    x4: 0x00000001982e5dfd   x5: 0x000000016fdb3410   x6: 0x000000000000006e   x7: 0x0000000000000f80
    x8: 0x0000000008000000   x9: 0x0000000004000000  x10: 0x0000000000000200  x11: 0x0000000000000000
   x12: 0x0000000000000000  x13: 0x0000000000000000  x14: 0x0000000000000002  x15: 0x0000000000000000
   x16: 0x0000000000000148  x17: 0x0000000000000000  x18: 0x0000000000000000  x19: 0x0000000000000006
   x20: 0x000000019ce0f310  x21: 0x000000019cdf7ce8  x22: 0x000000017415aa50  x23: 0x0000000199777c80
   x24: 0x0000000000000001  x25: 0x000000017415aa40  x26: 0x000000019cdf60a8  x27: 0x0000000000000001
   x28: 0x0000000000000000  fp: 0x000000016fdb3370   lr: 0x0000000199319228
    sp: 0x000000016fdb3350   pc: 0x000000019927b270 cpsr: 0x00000000

Binary Images:
0x10004c000 - 0x100053fff Crashy arm64  <8dc879259bb03b8eb2b7a85480d7f1a9> /var/mobile/Containers/Bundle/Application/83FB728B-ACE7-4D2B-9CB2-D24901F83FFB/Crashy.app/Crashy
0x1200a8000 - 0x1200cffff dyld arm64  <21c893f791653e989e1c3e15446d772b> /usr/lib/dyld
0x186b84000 - 0x186d17fff AVFoundation arm64  <c9cd60a62cfb3e77be72db6cd3062a09> /System/Library/Frameworks/AVFoundation.framework/AVFoundation
0x186d18000 - 0x186d7cfff libAVFAudio.dylib arm64  <017d90360b443ae788ef31cfd73d17f6> /System/Library/Frameworks/AVFoundation.framework/libAVFAudio.dylib
0x186dc0000 - 0x186dc0fff Accelerate arm64  <e9ba7838f51634a7b59ed392be50e86f> /System/Library/Frameworks/Accelerate.framework/Accelerate
0x186dd8000 - 0x186ff7fff vImage arm64  <da44067fc79931c7aef1b7e88bf82a83> /System/Library/Frameworks/Accelerate.framework/Frameworks/vImage.framework/vImage
0x186ff8000 - 0x18709ffff libBLAS.dylib arm64  <e5276e7784ef34a4baca480264978ea0> /System/Library/Frameworks/Accelerate.framework/Frameworks/vecLib.framework/libBLAS.dylib
0x1870a0000 - 0x18741afff libLAPACK.dylib arm64  <165b05f9f75736d5ae8f5f39293bd6e7> /System/Library/Frameworks/Accelerate.framework/Frameworks/vecLib.framework/libLAPACK.dylib
0x18741c000 - 0x187431fff libLinearAlgebra.dylib arm64  <5574ec3bd4e537e1b662d38a63aec58b> /System/Library/Frameworks/Accelerate.framework/Frameworks/vecLib.framework/libLinearAlgebra.dylib
0x187434000 - 0x18749cfff libvDSP.dylib arm64  <004f5668574139bc906c5fa4fdced3b1> /System/Library/Frameworks/Accelerate.framework/Frameworks/vecLib.framework/libvDSP.dylib
0x1874a0000 - 0x1874c3fff libvMisc.dylib arm64  <5790e7ace143367ea6f2428852be384e> /System/Library/Frameworks/Accelerate.framework/Frameworks/vecLib.framework/libvMisc.dylib
0x1874c4000 - 0x1874c4fff vecLib arm64  <211d7711a6e93fe8ae6d6b42585cad2d> /System/Library/Frameworks/Accelerate.framework/Frameworks/vecLib.framework/vecLib
0x1874c8000 - 0x1874f6fff Accounts arm64  <2508d336b9893176ad4e1bc67ff04188> /System/Library/Frameworks/Accounts.framework/Accounts
0x1874fc000 - 0x18757efff AddressBook arm64  <09e2e24ef5e23fb8a62ae209466a64bd> /System/Library/Frameworks/AddressBook.framework/AddressBook
0x187898000 - 0x187b55fff AudioToolbox arm64  <f0b739a395993b808d66e85e1a6e9f18> /System/Library/Frameworks/AudioToolbox.framework/AudioToolbox
0x187cf4000 - 0x187efffff CFNetwork arm64  <68adcebf440d30769bd2d67adc7932a2> /System/Library/Frameworks/CFNetwork.framework/CFNetwork
0x187f98000 - 0x187ffdfff CoreAudio arm64  <10aae62ba1c43dd29bc678fbf0f985ef> /System/Library/Frameworks/CoreAudio.framework/CoreAudio
0x188020000 - 0x188041fff CoreBluetooth arm64  <b30de1ce792a318aa125a84b06e8a95d> /System/Library/Frameworks/CoreBluetooth.framework/CoreBluetooth
0x188044000 - 0x188282fff CoreData arm64  <33c0d795a45e35c9affed5cf9d83a8a1> /System/Library/Frameworks/CoreData.framework/CoreData
0x188284000 - 0x1885e0fff CoreFoundation arm64  <83a9627362333366a8543e8c2d28166e> /System/Library/Frameworks/CoreFoundation.framework/CoreFoundation
0x1885e4000 - 0x188746fff CoreGraphics arm64  <7a02a2d0b69f3706b3cb91726db6f8af> /System/Library/Frameworks/CoreGraphics.framework/CoreGraphics
0x18879c000 - 0x18879efff libCGXType.A.dylib arm64  <73accc252e3f3efc84a84cce0504b5f7> /System/Library/Frameworks/CoreGraphics.framework/Resources/libCGXType.A.dylib
0x1887a0000 - 0x1887abfff libCMSBuiltin.A.dylib arm64  <fc4d017ca3403b21ad1e97eba9080873> /System/Library/Frameworks/CoreGraphics.framework/Resources/libCMSBuiltin.A.dylib
0x1889a0000 - 0x1889befff libRIP.A.dylib arm64  <5b43ca11f0b836798cc44159e62af17d> /System/Library/Frameworks/CoreGraphics.framework/Resources/libRIP.A.dylib
0x1889c0000 - 0x188aedfff CoreImage arm64  <444c44b06f533bad9c1b030edd486b49> /System/Library/Frameworks/CoreImage.framework/CoreImage
0x188b88000 - 0x188c46fff CoreMedia arm64  <f090b302cad23151b3aef050d50be152> /System/Library/Frameworks/CoreMedia.framework/CoreMedia
0x188c48000 - 0x188d16fff CoreMotion arm64  <0b3890116c60302980d4c0c3a0c14453> /System/Library/Frameworks/CoreMotion.framework/CoreMotion
0x188d18000 - 0x188d89fff CoreTelephony arm64  <f99cf601387938d3808c32e97a9a30cf> /System/Library/Frameworks/CoreTelephony.framework/CoreTelephony
0x188d8c000 - 0x188e8efff CoreText arm64  <e46b1730715c339a82db3f67eee4fe84> /System/Library/Frameworks/CoreText.framework/CoreText
0x188e90000 - 0x188eacfff CoreVideo arm64  <402f868dbba63d59a3b2e738982b9d71> /System/Library/Frameworks/CoreVideo.framework/CoreVideo
0x189188000 - 0x1893dcfff Foundation arm64  <e596bd80bcc83f15aca36a7ef014f457> /System/Library/Frameworks/Foundation.framework/Foundation
0x1894f4000 - 0x189560fff IOKit arm64  <1cd3da5151d03be5a0ba0c30c19228ea> /System/Library/Frameworks/IOKit.framework/Versions/A/IOKit
0x189564000 - 0x1897fefff ImageIO arm64  <10491d236e813eb6bb07d792047a7475> /System/Library/Frameworks/ImageIO.framework/ImageIO
0x189800000 - 0x189ca0fff JavaScriptCore arm64  <9d8bd2cbb97c33c59376cf656634704a> /System/Library/Frameworks/JavaScriptCore.framework/JavaScriptCore
0x18a514000 - 0x18a51afff MediaAccessibility arm64  <5dc0d8bda3593b9cb00a8703b21953fd> /System/Library/Frameworks/MediaAccessibility.framework/MediaAccessibility
0x18a738000 - 0x18ab52fff MediaToolbox arm64  <dbda28de74cd3fcca10622bbf00809b9> /System/Library/Frameworks/MediaToolbox.framework/MediaToolbox
0x18ac28000 - 0x18ac9bfff Metal arm64  <69e3d92ae3ec3375a550022b7ac4a184> /System/Library/Frameworks/Metal.framework/Metal
0x18ac9c000 - 0x18ad48fff MobileCoreServices arm64  <21a27692c6393c00a8f8f2bbd3ccb23c> /System/Library/Frameworks/MobileCoreServices.framework/MobileCoreServices
0x18becc000 - 0x18bed6fff OpenGLES arm64  <b707e102e4553f26994bfef0579c9f52> /System/Library/Frameworks/OpenGLES.framework/OpenGLES
0x18bedc000 - 0x18beddfff libCVMSPluginSupport.dylib arm64  <7e1f08d7776b37efb6ff01f6486afcde> /System/Library/Frameworks/OpenGLES.framework/libCVMSPluginSupport.dylib
0x18bee0000 - 0x18bee3fff libCoreFSCache.dylib arm64  <5888d3587c633af2ac7cf57ac15ab5e4> /System/Library/Frameworks/OpenGLES.framework/libCoreFSCache.dylib
0x18bee4000 - 0x18bee8fff libCoreVMClient.dylib arm64  <291806c545fe3219b844a93e2fb682b4> /System/Library/Frameworks/OpenGLES.framework/libCoreVMClient.dylib
0x18beec000 - 0x18bef6fff libGFXShared.dylib arm64  <f5e5cfc1d6673d469f25b3fa77fa995b> /System/Library/Frameworks/OpenGLES.framework/libGFXShared.dylib
0x18bef8000 - 0x18bf43fff libGLImage.dylib arm64  <4e284cf07fe23789b94c9f204f7aa52e> /System/Library/Frameworks/OpenGLES.framework/libGLImage.dylib
0x18c4a0000 - 0x18c624fff QuartzCore arm64  <313aba56d17e30d1b68b2fdfda1820f8> /System/Library/Frameworks/QuartzCore.framework/QuartzCore
0x18c8b8000 - 0x18c90afff Security arm64  <cb64d037f82a3f0a92ab63708334c938> /System/Library/Frameworks/Security.framework/Security
0x18cad0000 - 0x18cb43fff SystemConfiguration arm64  <cbcb5237ab8637aebf0cb493aaa4af92> /System/Library/Frameworks/SystemConfiguration.framework/SystemConfiguration
0x18cb48000 - 0x18d4bdfff UIKit arm64  <a1283daa6f5a33048ab9d29d91f62c09> /System/Library/Frameworks/UIKit.framework/UIKit
0x18d4c0000 - 0x18d539fff VideoToolbox arm64  <13a05b41cd0136239ef94de508febe1d> /System/Library/Frameworks/VideoToolbox.framework/VideoToolbox
0x18dde0000 - 0x18dde5fff AggregateDictionary arm64  <2f9120e6400835f08bd7bfd2d4ada020> /System/Library/PrivateFrameworks/AggregateDictionary.framework/AggregateDictionary
0x18dfe4000 - 0x18e018fff AirPlaySupport arm64  <442269677a2e302ea3bf68c54f1ff539> /System/Library/PrivateFrameworks/AirPlaySupport.framework/AirPlaySupport
0x18e264000 - 0x18e2aefff AppSupport arm64  <f35ee13bec64354d9044e2a5ea519640> /System/Library/PrivateFrameworks/AppSupport.framework/AppSupport
0x18e40c000 - 0x18e454fff AppleJPEG arm64  <8377453201ad3862b7b6182be4ac4342> /System/Library/PrivateFrameworks/AppleJPEG.framework/AppleJPEG
0x18e480000 - 0x18e489fff AppleSRP arm64  <7a5d169c15b83573a29f1c018c8ecbb8> /System/Library/PrivateFrameworks/AppleSRP.framework/AppleSRP
0x18e49c000 - 0x18e4a7fff AssertionServices arm64  <52d911832bf9382d802961ea9d1614f9> /System/Library/PrivateFrameworks/AssertionServices.framework/AssertionServices
0x18e4a8000 - 0x18e4c3fff AssetsLibraryServices arm64  <1b0a20bfd23a3295aec6d82c8b7a2f24> /System/Library/PrivateFrameworks/AssetsLibraryServices.framework/AssetsLibraryServices
0x18e528000 - 0x18e52cfff BTLEAudioController arm64  <8539b6078e1b3c739d412842418188ed> /System/Library/PrivateFrameworks/BTLEAudioController.framework/BTLEAudioController
0x18e530000 - 0x18e54cfff BackBoardServices arm64  <62bf606fae3b3231b48d5ec35a552aa5> /System/Library/PrivateFrameworks/BackBoardServices.framework/BackBoardServices
0x18e554000 - 0x18e591fff BaseBoard arm64  <62044bafc2293567aec7797b25708b48> /System/Library/PrivateFrameworks/BaseBoard.framework/BaseBoard
0x18e5ac000 - 0x18e5b3fff BluetoothManager arm64  <afd2bca7997434f08d4723c3005ca0f9> /System/Library/PrivateFrameworks/BluetoothManager.framework/BluetoothManager
0x18e844000 - 0x18e84efff CaptiveNetwork arm64  <8ba9d547383b3a7fba9a31cc361fc06a> /System/Library/PrivateFrameworks/CaptiveNetwork.framework/CaptiveNetwork
0x18e850000 - 0x18e99afff Celestial arm64  <48f92eb00d0636808c583028f766d983> /System/Library/PrivateFrameworks/Celestial.framework/Celestial
0x18f098000 - 0x18f0aafff CommonUtilities arm64  <1cb495ce473a3127bb291cc541762fb3> /System/Library/PrivateFrameworks/CommonUtilities.framework/CommonUtilities
0x18f0ac000 - 0x18f0b0fff CommunicationsFilter arm64  <836ffdf2d1bf38948dc8ce6c2f8179e1> /System/Library/PrivateFrameworks/CommunicationsFilter.framework/CommunicationsFilter
0x18f138000 - 0x18f13dfff ConstantClasses arm64  <855d1ee3980637a1b48a47adf5327c35> /System/Library/PrivateFrameworks/ConstantClasses.framework/ConstantClasses
0x18f180000 - 0x18f184fff CoreAUC arm64  <bf359bb9dcc837f78745ec21c2983ad2> /System/Library/PrivateFrameworks/CoreAUC.framework/CoreAUC
0x18f21c000 - 0x18f23bfff CoreDuet arm64  <ee7872f60256383a96f35468fb7a3dc5> /System/Library/PrivateFrameworks/CoreDuet.framework/CoreDuet
0x18f240000 - 0x18f252fff CoreDuetDaemonProtocol arm64  <aa7ade578b203db19f39ea32a0e1829a> /System/Library/PrivateFrameworks/CoreDuetDaemonProtocol.framework/CoreDuetDaemonProtocol
0x18f25c000 - 0x18f25efff CoreDuetDebugLogging arm64  <ec769c1bea803724880716f71249ba1c> /System/Library/PrivateFrameworks/CoreDuetDebugLogging.framework/CoreDuetDebugLogging
0x18f960000 - 0x18f9f2fff CoreUI arm64  <01dbaf25ff893847ba41f2ff92b411a8> /System/Library/PrivateFrameworks/CoreUI.framework/CoreUI
0x18f9f4000 - 0x18fa70fff CoreUtils arm64  <a30cc6baffe8324aaa50865c52d59141> /System/Library/PrivateFrameworks/CoreUtils.framework/CoreUtils
0x18fa74000 - 0x18fa7afff CrashReporterSupport arm64  <ba2801fd567a305da540a0b276dc7537> /System/Library/PrivateFrameworks/CrashReporterSupport.framework/CrashReporterSupport
0x18fd3c000 - 0x18fd62fff DataAccessExpress arm64  <50d5ab9c38ee3e69bd4da116bc7bd4f8> /System/Library/PrivateFrameworks/DataAccessExpress.framework/DataAccessExpress
0x18fdb4000 - 0x18fdbbfff DataMigration arm64  <e0c839ae4aed387887ea9853c6c25682> /System/Library/PrivateFrameworks/DataMigration.framework/DataMigration
0x18fdc4000 - 0x18fdc5fff DiagnosticLogCollection arm64  <fa41e1d5be703f8e80e8ff3316a49e3d> /System/Library/PrivateFrameworks/DiagnosticLogCollection.framework/DiagnosticLogCollection
0x18fdc8000 - 0x18fde8fff DictionaryServices arm64  <d4d267ee319135ccb3a6679497243088> /System/Library/PrivateFrameworks/DictionaryServices.framework/DictionaryServices
0x18fe10000 - 0x18fe36fff EAP8021X arm64  <c99ae63150f83cd5b9dd00d12ac1e9f8> /System/Library/PrivateFrameworks/EAP8021X.framework/EAP8021X
0x18ff98000 - 0x1903c5fff FaceCore arm64  <a0f71a06ddb83c77b3b59257e4002445> /System/Library/PrivateFrameworks/FaceCore.framework/FaceCore
0x1903f8000 - 0x1903f8fff FontServices arm64  <c7cd675f737e346db28b52c37065163f> /System/Library/PrivateFrameworks/FontServices.framework/FontServices
0x1903fc000 - 0x1904dbfff libFontParser.dylib arm64  <48edcd60e46e3b9f9dffab1ae9283706> /System/Library/PrivateFrameworks/FontServices.framework/libFontParser.dylib
0x1904dc000 - 0x1904e8fff libGSFontCache.dylib arm64  <0c92c17ccfd03da88fd356e758e17497> /System/Library/PrivateFrameworks/FontServices.framework/libGSFontCache.dylib
0x1905f8000 - 0x190618fff FrontBoardServices arm64  <17de7a3c55253f02a2d676919d73ccb6> /System/Library/PrivateFrameworks/FrontBoardServices.framework/FrontBoardServices
0x19141c000 - 0x19142ffff GraphicsServices arm64  <b5078b39bd36372190e4ad5e7d991f68> /System/Library/PrivateFrameworks/GraphicsServices.framework/GraphicsServices
0x191708000 - 0x19176afff IDS arm64  <c3ab13565e513311805a3813291b9c27> /System/Library/PrivateFrameworks/IDS.framework/IDS
0x19176c000 - 0x191790fff IDSFoundation arm64  <5a05fb27e5083d09b5f289d7560edbee> /System/Library/PrivateFrameworks/IDSFoundation.framework/IDSFoundation
0x19196c000 - 0x1919dcfff IMFoundation arm64  <c8aa1eec15b63d05831678746a299da0> /System/Library/PrivateFrameworks/IMFoundation.framework/IMFoundation
0x1919e8000 - 0x1919ebfff IOAccelerator arm64  <ec8452ce495a3f1088b1c6024e027167> /System/Library/PrivateFrameworks/IOAccelerator.framework/IOAccelerator
0x1919f0000 - 0x1919f7fff IOMobileFramebuffer arm64  <c1f736ec9ad732728480d64c59a86f5f> /System/Library/PrivateFrameworks/IOMobileFramebuffer.framework/IOMobileFramebuffer
0x1919f8000 - 0x1919fefff IOSurface arm64  <719f179613ae37b688ee169eb5ed46fc> /System/Library/PrivateFrameworks/IOSurface.framework/IOSurface
0x191a00000 - 0x191a02fff IOSurfaceAccelerator arm64  <3fb692bcaed8321db9c674cf00c5f719> /System/Library/PrivateFrameworks/IOSurfaceAccelerator.framework/IOSurfaceAccelerator
0x191ac4000 - 0x191b06fff LanguageModeling arm64  <0f8255591fef33cdb8a91f460e678ccb> /System/Library/PrivateFrameworks/LanguageModeling.framework/LanguageModeling
0x191cf0000 - 0x191daefff ManagedConfiguration arm64  <43215fab0090325d976c63af94aa02b5> /System/Library/PrivateFrameworks/ManagedConfiguration.framework/ManagedConfiguration
0x191dbc000 - 0x191dbdfff Marco arm64  <374e233c50c2373a8dc5ca0a817b12a4> /System/Library/PrivateFrameworks/Marco.framework/Marco
0x191dc0000 - 0x191e46fff MediaControlSender arm64  <8042568e5afa3775a7b165d138a799ae> /System/Library/PrivateFrameworks/MediaControlSender.framework/MediaControlSender
0x191efc000 - 0x191f11fff MediaRemote arm64  <b54d94f44dcf3147ab669748e7fd1f19> /System/Library/PrivateFrameworks/MediaRemote.framework/MediaRemote
0x191f14000 - 0x191f25fff MediaServices arm64  <46469813721c3f6193bbd7fbb4e0a5eb> /System/Library/PrivateFrameworks/MediaServices.framework/MediaServices
0x1920dc000 - 0x1920ebfff MobileAsset arm64  <9164537c500e345abf5970138aa9b1dd> /System/Library/PrivateFrameworks/MobileAsset.framework/MobileAsset
0x192118000 - 0x192124fff MobileBluetooth arm64  <d698ec87311e3132b0de7ce0ddcd8fbb> /System/Library/PrivateFrameworks/MobileBluetooth.framework/MobileBluetooth
0x192158000 - 0x192161fff MobileInstallation arm64  <6a17b4f0b6aa363ba2decf9b6c8167b1> /System/Library/PrivateFrameworks/MobileInstallation.framework/MobileInstallation
0x192164000 - 0x192173fff MobileKeyBag arm64  <77b5fa7d33ef319299072ec85128fe37> /System/Library/PrivateFrameworks/MobileKeyBag.framework/MobileKeyBag
0x1921b0000 - 0x1921b3fff MobileSystemServices arm64  <9b2bbc93fbb231baa08b41c6aee209ed> /System/Library/PrivateFrameworks/MobileSystemServices.framework/MobileSystemServices
0x1921dc000 - 0x1921edfff MobileWiFi arm64  <79c784a6040b35d1b09e97c60b0def58> /System/Library/PrivateFrameworks/MobileWiFi.framework/MobileWiFi
0x1924e4000 - 0x1924eafff Netrb arm64  <b58a090c9a12346a9f4af0d22626f6f3> /System/Library/PrivateFrameworks/Netrb.framework/Netrb
0x1924ec000 - 0x1924f3fff NetworkStatistics arm64  <8d818200ba99385bbd69dad9dda0319d> /System/Library/PrivateFrameworks/NetworkStatistics.framework/NetworkStatistics
0x192520000 - 0x192523fff OAuth arm64  <3049cf937f053793a4b97aa26375f1cb> /System/Library/PrivateFrameworks/OAuth.framework/OAuth
0x192cf8000 - 0x192d46fff OpenCL arm64  <7350f5063e4232a1a3cc921e47de6ef5> /System/Library/PrivateFrameworks/OpenCL.framework/OpenCL
0x192e64000 - 0x192e8cfff PersistentConnection arm64  <b7044531bbf73fcf9b586269283bfb50> /System/Library/PrivateFrameworks/PersistentConnection.framework/PersistentConnection
0x1932d4000 - 0x193321fff PhysicsKit arm64  <625733e02bc3372ca473ac973020e32e> /System/Library/PrivateFrameworks/PhysicsKit.framework/PhysicsKit
0x193324000 - 0x19333efff PlugInKit arm64  <cc8ba22bd61e32a5a80b083d5e0dd86e> /System/Library/PrivateFrameworks/PlugInKit.framework/PlugInKit
0x193340000 - 0x193348fff PowerLog arm64  <506bca8a5af033a68bbd5958c9f995a7> /System/Library/PrivateFrameworks/PowerLog.framework/PowerLog
0x19365c000 - 0x1936a3fff PrintKit arm64  <2181399ad0d331e8934c69d4220f7bcc> /System/Library/PrivateFrameworks/PrintKit.framework/PrintKit
0x1936a8000 - 0x193767fff ProofReader arm64  <377a2b68fdcf3fe3be30455084083eb5> /System/Library/PrivateFrameworks/ProofReader.framework/ProofReader
0x1937c8000 - 0x193846fff Quagga arm64  <a0e7e7857a69346ab1f5c4e065491469> /System/Library/PrivateFrameworks/Quagga.framework/Quagga
0x193cf8000 - 0x193d17fff SpringBoardServices arm64  <118627bb068a3a82b87ba8c62583e7a8> /System/Library/PrivateFrameworks/SpringBoardServices.framework/SpringBoardServices
0x19410c000 - 0x194253fff StoreServices arm64  <8c5dfc1c4baf3eaca6420c6af360bf5e> /System/Library/PrivateFrameworks/StoreServices.framework/StoreServices
0x194344000 - 0x194347fff TCC arm64  <0dc32625c39b3087893e5da6ff7dd7b4> /System/Library/PrivateFrameworks/TCC.framework/TCC
0x194398000 - 0x1943dbfff TelephonyUtilities arm64  <1cb4e1e61c2e3d5580283cd1e3039be4> /System/Library/PrivateFrameworks/TelephonyUtilities.framework/TelephonyUtilities
0x1951bc000 - 0x1951eafff TextInput arm64  <b19843fb56343a97b9e0dd0014231115> /System/Library/PrivateFrameworks/TextInput.framework/TextInput
0x1952c0000 - 0x195399fff UIFoundation arm64  <402e5079593a32a8b49d604f4a1eedeb> /System/Library/PrivateFrameworks/UIFoundation.framework/UIFoundation
0x1953c0000 - 0x1953c3fff UserFS arm64  <da16ebc138783ad7a4a1ed8d0b09bda7> /System/Library/PrivateFrameworks/UserFS.framework/UserFS
0x195d24000 - 0x196c4bfff WebCore arm64  <42110cbe7d7e3f899dc1bd4015282fcc> /System/Library/PrivateFrameworks/WebCore.framework/WebCore
0x196c4c000 - 0x196d1efff WebKitLegacy arm64  <23c78a31ba4b39cd9286e376281b0e66> /System/Library/PrivateFrameworks/WebKitLegacy.framework/WebKitLegacy
0x197b3c000 - 0x197b45fff libAccessibility.dylib arm64  <aa09cdc041b53a05b0161253d121621d> /usr/lib/libAccessibility.dylib
0x197dd8000 - 0x197df3fff libCRFSuite.dylib arm64  <a41a2f95f1ff30d9a4ab2d6145480db2> /usr/lib/libCRFSuite.dylib
0x197e34000 - 0x197f6bfff libFosl_dynamic.dylib arm64  <3013ac9596c03e458767997983ac758f> /usr/lib/libFosl_dynamic.dylib
0x197f90000 - 0x197faafff libMobileGestalt.dylib arm64  <f625ec0e13bf3a2f8ba8571b9546444d> /usr/lib/libMobileGestalt.dylib
0x197fdc000 - 0x197fddfff libSystem.B.dylib arm64  <882b19bba06d348d97fcdaf545163f47> /usr/lib/libSystem.B.dylib
0x198060000 - 0x1980aefff libTelephonyUtilDynamic.dylib arm64  <a84c6f652ea63a52921b96b6185c531c> /usr/lib/libTelephonyUtilDynamic.dylib
0x1981d8000 - 0x198202fff libarchive.2.dylib arm64  <6e7ce417e487309c8acc744b1b6b523f> /usr/lib/libarchive.2.dylib
0x198244000 - 0x198254fff libbsm.0.dylib arm64  <6651c9abc7b6353c8343d7f0f4e09a23> /usr/lib/libbsm.0.dylib
0x198258000 - 0x198268fff libbz2.1.0.dylib arm64  <f6ec1b6a4719369aa059ee3269823a2d> /usr/lib/libbz2.1.0.dylib
0x19826c000 - 0x1982c2fff libc++.1.dylib arm64  <c8e65982941e374c95463384e600181d> /usr/lib/libc++.1.dylib
0x1982c4000 - 0x1982e6fff libc++abi.dylib arm64  <fd49f85cb61d31b582895366ea6c2d01> /usr/lib/libc++abi.dylib
0x1982ec000 - 0x1982fdfff libcmph.dylib arm64  <dca2c6c0bd65352b947d537395e23ab9> /usr/lib/libcmph.dylib
0x198344000 - 0x198360fff libextension.dylib arm64  <e8ead22587533875b26071dda1330ce1> /usr/lib/libextension.dylib
0x198398000 - 0x19848bfff libiconv.2.dylib arm64  <3ebb30c258f43c0294bcdeebb48b3fc1> /usr/lib/libiconv.2.dylib
0x19848c000 - 0x198673fff libicucore.A.dylib arm64  <02e9eb5b92473df89af04da09371417a> /usr/lib/libicucore.A.dylib
0x198688000 - 0x198689fff liblangid.dylib arm64  <80e626200785352a8d5e98a061ca19b8> /usr/lib/liblangid.dylib
0x19868c000 - 0x198698fff liblockdown.dylib arm64  <f53a3d2ac76330f7bd299be0a9206109> /usr/lib/liblockdown.dylib
0x19869c000 - 0x1986b5fff liblzma.5.dylib arm64  <ac6807960fbd34d9939a070cf6ecf081> /usr/lib/liblzma.5.dylib
0x198a8c000 - 0x198aa3fff libmis.dylib arm64  <130d691e68403ec2882abd44479e9891> /usr/lib/libmis.dylib
0x198aec000 - 0x198ce8fff libobjc.A.dylib arm64  <e6224d745a023588af8e5bb67498139a> /usr/lib/libobjc.A.dylib
0x198dd0000 - 0x198dedfff libresolv.9.dylib arm64  <fd78cddab3e43bd9a7a6440273b15059> /usr/lib/libresolv.9.dylib
0x198e20000 - 0x198ef1fff libsqlite3.dylib arm64  <286839512b673f7c938aa79ac70bde15> /usr/lib/libsqlite3.dylib
0x198f48000 - 0x198f7afff libtidy.A.dylib arm64  <2b69233bafd53bdaafa6d9b1767bbad5> /usr/lib/libtidy.A.dylib
0x198f8c000 - 0x19907afff libxml2.2.dylib arm64  <dbcfe4d423bb3ae48174394f298ad244> /usr/lib/libxml2.2.dylib
0x19907c000 - 0x1990a5fff libxslt.1.dylib arm64  <f3770c5f8ac3313bbe4ef1258ebf5733> /usr/lib/libxslt.1.dylib
0x1990a8000 - 0x1990b9fff libz.1.dylib arm64  <2a347410b967358289e8256c913714de> /usr/lib/libz.1.dylib
0x1990bc000 - 0x1990c0fff libcache.dylib arm64  <d322f485769b3fd5a11bc2aff7265fdf> /usr/lib/system/libcache.dylib
0x1990c4000 - 0x1990d0fff libcommonCrypto.dylib arm64  <2aa56db3851c3b24b7eb849f0e289140> /usr/lib/system/libcommonCrypto.dylib
0x1990d4000 - 0x1990d7fff libcompiler_rt.dylib arm64  <65f2a15e126435769154e2a7b44b942e> /usr/lib/system/libcompiler_rt.dylib
0x1990d8000 - 0x1990dffff libcopyfile.dylib arm64  <1f428d2df193398e9e72250952f08953> /usr/lib/system/libcopyfile.dylib
0x1990e0000 - 0x199135fff libcorecrypto.dylib arm64  <4a97f227130a3cbaa0a8c5b561e97314> /usr/lib/system/libcorecrypto.dylib
0x199138000 - 0x19915efff libdispatch.dylib arm64  <e19d74563485344485b6d4457a93e89d> /usr/lib/system/libdispatch.dylib
0x199160000 - 0x199162fff libdyld.dylib arm64  <d5ebc6da536338f5be9bb4c3be2f7716> /usr/lib/system/libdyld.dylib
0x199164000 - 0x199164fff liblaunch.dylib arm64  <da357dcde300321685d77140a4f82e6c> /usr/lib/system/liblaunch.dylib
0x199168000 - 0x19916dfff libmacho.dylib arm64  <cddfd20412643baeb9023095eb2cf29f> /usr/lib/system/libmacho.dylib
0x199170000 - 0x199171fff libremovefile.dylib arm64  <e8124da88b1131f2ac005b75d8559ca7> /usr/lib/system/libremovefile.dylib
0x199174000 - 0x199189fff libsystem_asl.dylib arm64  <17448aec6f7d3498aebcabc8a1598c9a> /usr/lib/system/libsystem_asl.dylib
0x19918c000 - 0x19918dfff libsystem_blocks.dylib arm64  <f38b7145bed330d98d8d79b8362b03de> /usr/lib/system/libsystem_blocks.dylib
0x199190000 - 0x199210fff libsystem_c.dylib arm64  <71df87643ff839bdb9559e4e50bb6eea> /usr/lib/system/libsystem_c.dylib
0x199214000 - 0x199216fff libsystem_configuration.dylib arm64  <37655cc87bb3391b946955b0fbc4384a> /usr/lib/system/libsystem_configuration.dylib
0x199218000 - 0x199219fff libsystem_coreservices.dylib arm64  <a8e2019df4123295bf71800fa1bd73be> /usr/lib/system/libsystem_coreservices.dylib
0x19921c000 - 0x19922cfff libsystem_coretls.dylib arm64  <e837369c4d623fc7adb19a892b03aba8> /usr/lib/system/libsystem_coretls.dylib
0x199230000 - 0x199238fff libsystem_dnssd.dylib arm64  <18b39491d06c3fa18c810118f03143ee> /usr/lib/system/libsystem_dnssd.dylib
0x19923c000 - 0x19925dfff libsystem_info.dylib arm64  <72514f76b03335729f18da536331df97> /usr/lib/system/libsystem_info.dylib
0x199260000 - 0x199280fff libsystem_kernel.dylib arm64  <ccacc11311c23f8f8fa58f58ce96be0f> /usr/lib/system/libsystem_kernel.dylib
0x199284000 - 0x1992a0fff libsystem_m.dylib arm64  <e25dbaa110a03706a8ea7e0709ec385a> /usr/lib/system/libsystem_m.dylib
0x1992a4000 - 0x1992bdfff libsystem_malloc.dylib arm64  <bb0250acb085340ea6689a755edc5515> /usr/lib/system/libsystem_malloc.dylib
0x1992c0000 - 0x1992f7fff libsystem_network.dylib arm64  <d7b99c2b98ff3affbe5a8743121419d2> /usr/lib/system/libsystem_network.dylib
0x1992f8000 - 0x1992fefff libsystem_networkextension.dylib arm64  <8248d7bdf0bd3e0b9d2a5ba10b238921> /usr/lib/system/libsystem_networkextension.dylib
0x199300000 - 0x19930afff libsystem_notify.dylib arm64  <4a9bcea2df8d351f987d0e9f84406427> /usr/lib/system/libsystem_notify.dylib
0x19930c000 - 0x199310fff libsystem_platform.dylib arm64  <03902be9733b35d2b193cf8724a8d95a> /usr/lib/system/libsystem_platform.dylib
0x199314000 - 0x19931cfff libsystem_pthread.dylib arm64  <ffbb6452a3e531969e9571cd95896210> /usr/lib/system/libsystem_pthread.dylib
0x199320000 - 0x199322fff libsystem_sandbox.dylib arm64  <b8d755b4fc043ad791277d6a8cf0b4b6> /usr/lib/system/libsystem_sandbox.dylib
0x199324000 - 0x199327fff libsystem_stats.dylib arm64  <e2b3982965873f27b542a1a81f212b5b> /usr/lib/system/libsystem_stats.dylib
0x199328000 - 0x19932efff libsystem_trace.dylib arm64  <122df0fd03b43a8f82ed69916c95524a> /usr/lib/system/libsystem_trace.dylib
0x199330000 - 0x199335fff libunwind.dylib arm64  <0c07617876a43cacbde6104a2b75f4f2> /usr/lib/system/libunwind.dylib
0x199338000 - 0x19935bfff libxpc.dylib arm64  <2a02e77c431732e292fbe37af8747b2e> /usr/lib/system/libxpc.dylib 
```

---
#Identifier

```
Incident Identifier: E44AD7C2-4F93-47A8-A1D7-CB619425EFB1
CrashReporter Key:   5f34f05ff9130504d107ebb1aadfe546e55af43c
Hardware Model:      iPhone7,2
Process:             Crashy [8364]
Path:                /private/var/mobile/Containers/Bundle/Application/83FB728B-ACE7-4D2B-9CB2-D24901F83FFB/Crashy.app/Crashy
Identifier:          com.fyber.Crashy
Version:             1 (1.0)
Code Type:           ARM-64 (Native)
Parent Process:      launchd [1]

Date/Time:           2015-03-01 08:18:47.887 +0100
Launch Time:         2015-03-01 08:18:46.159 +0100
OS Version:          iOS 8.1.3 (12B466)
Report Version:      105

```
---
#What Happened

```
Exception Type:  EXC_CRASH (SIGABRT)
Exception Codes: 0x0000000000000000, 0x0000000000000000
Triggered by Thread:  0
```

---

#BackTraces

```
Last Exception Backtrace:
0   CoreFoundation                	0x1883aa59c __exceptionPreprocess + 132
1   libobjc.A.dylib               	0x198af40e4 objc_exception_throw + 60
2   CoreFoundation                	0x188292d40 -[__NSPlaceholderArray initWithObjects:count:] + 412
3   CoreFoundation                	0x18829eff8 +[NSArray arrayWithObjects:count:] + 60
4   Crashy                        	0x10004eacc 0x100048000 + 27340
5   Crashy                        	0x10004ea44 0x100048000 + 27204
6   Crashy                        	0x10004e9e8 0x100048000 + 27112
7   Crashy                        	0x10004e980 0x100048000 + 27008
8   UIKit                         	0x18cb8d418 -[UIApplication sendAction:to:from:forEvent:] + 96
9   UIKit                         	0x18cb7652c -[UIControl _sendActionsForEvents:withEvent:] + 612
10  UIKit                         	0x18cb8cdb4 -[UIControl touchesEnded:withEvent:] + 592
11  UIKit                         	0x18cb8ca40 -[UIWindow _sendTouchesForEvent:] + 700
12  UIKit                         	0x18cb85f94 -[UIWindow sendEvent:] + 684
13  UIKit                         	0x18cb5968c -[UIApplication sendEvent:] + 264
14  UIKit                         	0x18cdf860c _UIApplicationHandleEventFromQueueEvent + 14992
15  UIKit                         	0x18cb57bf4 _UIApplicationHandleEventQueue + 1616
16  CoreFoundation                	0x1883629ec __CFRUNLOOP_IS_CALLING_OUT_TO_A_SOURCE0_PERFORM_FUNCTION__ + 24
17  CoreFoundation                	0x188361c90 __CFRunLoopDoSources0 + 264
18  CoreFoundation                	0x18835fd40 __CFRunLoopRun + 712
19  CoreFoundation                	0x18828d0a4 CFRunLoopRunSpecific + 396
20  GraphicsServices              	0x1914275a4 GSEventRunModal + 168
21  UIKit                         	0x18cbbeaa4 UIApplicationMain + 1488
22  Crashy                        	0x10004ee30 0x100048000 + 28208
23  libdyld.dylib                 	0x199162a08 start + 4


Thread 0 name:  Dispatch queue: com.apple.main-thread
Thread 0 Crashed:
0   libsystem_kernel.dylib        	0x000000019927b270 __pthread_kill + 8
1   libsystem_pthread.dylib       	0x0000000199319224 pthread_kill + 108
2   libsystem_c.dylib             	0x00000001991f2b14 abort + 108
3   libc++abi.dylib               	0x00000001982c5414 abort_message + 112
....
```

---

#Loaded binaries

```
Binary Images:
0x100048000 - 0x10004ffff Crashy arm64  <8263f02cc044325b9a2133bb6d04389e> /var/mobile/Containers/Bundle/Application/53C61964-285F-4932-84A6-2E2FD76A5016/Crashy.app/Crashy
0x1200b0000 - 0x1200d7fff dyld arm64  <21c893f791653e989e1c3e15446d772b> /usr/lib/dyld
0x186b84000 - 0x186d17fff AVFoundation arm64  <c9cd60a62cfb3e77be72db6cd3062a09> /System/Library/Frameworks/AVFoundation.framework/AVFoundation
0x186d18000 - 0x186d7cfff libAVFAudio.dylib arm64  <017d90360b443ae788ef31cfd73d17f6> /System/Library/Frameworks/AVFoundation.framework/libAVFAudio.dylib
0x186dc0000 - 0x186dc0fff Accelerate arm64  <e9ba7838f51634a7b59ed392be50e86f> /System/Library/Frameworks/Accelerate.framework/Accelerate
0x186dd8000 - 0x186ff7fff vImage arm64  <da44067fc79931c7aef1b7e88bf82a83> /System/Library/Frameworks/Accelerate.framework/Frameworks/vImage.framework/vImage
0x186ff8000 - 0x18709ffff libBLAS.dylib arm64  <e5276e7784ef34a4baca480264978ea0> /System/Library/Frameworks/Accelerate.framework/Frameworks/vecLib.framework/libBLAS.dylib
0x1870a0000 - 0x18741afff libLAPACK.dylib arm64  <165b05f9f75736d5ae8f5f39293bd6e7> /System/Library/Frameworks/Accelerate.framework/Frameworks/vecLib.framework/libLAPACK.dylib
0x18741c000 - 0x187431fff libLinearAlgebra.dylib arm64  <5574ec3bd4e537e1b662d38a63aec58b> /System/Library/Frameworks/Accelerate.framework/Frameworks/vecLib.framework/libLinearAlgebra.dylib
0x187434000 - 0x18749cfff libvDSP.dylib arm64  <004f5668574139bc906c5fa4fdced3b1> /System/Library/Frameworks/Accelerate.framework/Frameworks/vecLib.framework/libvDSP.dylib
....
```

---

# Can you see the root cause?

```
3   CoreFoundation                	0x18829eff8 +[NSArray arrayWithObjects:count:] + 60
4   Crashy                        	0x10004eacc 0x100048000 + 27340
5   Crashy                        	0x10004ea44 0x100048000 + 27204
6   Crashy                        	0x10004e9e8 0x100048000 + 27112
7   Crashy                        	0x10004e980 0x100048000 + 27008
8   UIKit                         	0x18cb8d418 -[UIApplication sendAction:to:from:forEvent:] + 96
```
---

#WAT?

---

# Symbolication


- Restores the binary addresses to readable method names
- Requires
  - The ipa that caused the crash
  - The dSYM file (that contain the information about the symbols)
  - The crash report

---
  
# IPA, dSYM and Crash Report must match

---
# Symbolication, the quick way

- Create a new folder
- Copy the ipa, dSYM and crash report
- Unzip the ipa
- Unzip (if needed the dSYM)
- Run symbolicatecrash

---

# Running symbolicatecrash


DEVELOPER\_DIR=\`xcode-select -print-path\` /Applications/Xcode.app/Contents/SharedFrameworks/DTDeviceKitBase.framework/Versions/A/Resources/symbolicatecrash -o <output_file> <input_crash_file>

(aliases are your friend)


---
# What does it do?

- Matches the crash, ipa and crash report
- Runs `otool` to verify the correct base address
- Run `lipo` to make sure the arch slice is present
- Run `atos` to perform the symbolication
- It's a perl script. Read it if you dare :)

---
#Ouput

```
3   CoreFoundation                	0x18829eff8 +[NSArray arrayWithObjects:count:] + 60
4   Crashy                        	0x10004eacc -[ViewController method3] (ViewController.m:49)
5   Crashy                        	0x10004ea44 -[ViewController method2] (ViewController.m:42)
6   Crashy                        	0x10004e9e8 -[ViewController method1] (ViewController.m:36)
7   Crashy                        	0x10004e980 -[ViewController crash:] (ViewController.m:30)
8   UIKit                         	0x18cb8d418 -[UIApplication sendAction:to:from:forEvent:] + 96
```
---

#BEAUTIFUL

---
#Questions?