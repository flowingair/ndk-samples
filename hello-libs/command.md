
03/14 15:03:02: Launching 'app' on Google Pixel 2.
Install successfully finished in 449 ms.
$ adb shell am start -n "com.example.hellolibs/com.example.hellolibs.MainActivity" -a android.intent.action.MAIN -c android.intent.category.LAUNCHER -D
Waiting for application to come online: com.example.hellolibs.test | com.example.hellolibs
Waiting for application to come online: com.example.hellolibs.test | com.example.hellolibs
Connected to process 9640 on device 'google-pixel_2-HT79F1A05312'.
Capturing and displaying logcat messages from application. This behavior can be disabled in the "Logcat output" section of the "Debugger" settings page.
W/ActivityThread: Application com.example.hellolibs is waiting for the debugger on port 8100...
I/System.out: Sending WAIT chunk
Waiting for application to come online: com.example.hellolibs.test | com.example.hellolibs
Connecting to com.example.hellolibs
Now Launching Native Debug Session
$ adb shell cat /data/local/tmp/lldb-server | run-as com.example.hellolibs sh -c 'cat > /data/data/com.example.hellolibs/lldb/bin/lldb-server && chmod 700 /data/data/com.example.hellolibs/lldb/bin/lldb-server'
$ adb shell cat /data/local/tmp/start_lldb_server.sh | run-as com.example.hellolibs sh -c 'cat > /data/data/com.example.hellolibs/lldb/bin/start_lldb_server.sh && chmod 700 /data/data/com.example.hellolibs/lldb/bin/start_lldb_server.sh'
Starting LLDB server: /data/data/com.example.hellolibs/lldb/bin/start_lldb_server.sh /data/data/com.example.hellolibs/lldb unix-abstract /com.example.hellolibs-0 platform-1615705384604.sock "lldb process:gdb-remote packets"
Debugger attached to process 9640
