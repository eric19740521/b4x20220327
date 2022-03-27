# b4x20220327
B4X實驗: APP如何連線到資料庫服務器JRDC(中間層),並示範讀取資料(B4J)

B4X實驗: APP如何連線到資料庫服務器JRDC(中間層),並示範讀取資料(B4J)
參考資料:
https://www.b4x.com/android/forum/threads/b4x-jrdc2-b4j-implementation-of-rdc-remote-database-connector.61801/#content
https://andy6804tw.github.io/2019/01/29/ubuntu-mysql-setting/


0.jRDC 服務器?? Web+RDC Server
它（jRDC 服務器）基於完整版的 jetty(jServer lib) 和 JDBC(jSQL lib) ，這在 android 上不可用。
它被設計為客戶端（Android、iOS、B4J 應用程序）和數據庫之間的中間件。這個中間件可以讓你的數據庫更安全、更容易訪問。



1.Linux MYSQL安裝(這部分.還沒測試好)
https://andy6804tw.github.io/2019/01/29/ubuntu-mysql-setting/

Win10 XAMPP(暫時用這個) 雲

2.演示一下程式運作


3.JRDC Server,驅動
mysql-connector-java-5.1.47-bin.jar
https://www.dropbox.com/sh/q2h7qmiwrparzru/AACmjXllUKcYF1XhNOrYkGh3a?dl=0


查看指定端口的佔用情況 C:\>netstat -aon|findstr "51042"
查看PID對應的進程 C:\>tasklist|findstr "2016"
結束該進程 C:\>taskkill /f /t /im java.exe


程式解說(部分解說)
會用到的LIB
參數檔解說


4.JRDC Client,
LIB
程式解說


https://github.com/eric19740521/b4x20220327







