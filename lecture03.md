# 第3回課題提出
## APサーバー
- 名前:Puma
- バージョン：5.6.5  

## DBサーバー
- 名前：MySQL
- バージョン：？  
　→確認したところ、raisetech-live8-sample-app内のdatabase.ymlでは5.5.8であったが、  
![バージョン確認①](/RaiseTech/DBver.check01.png)
`mysql -u root -p`で起動したmysql内で確認したところ8.0.34と記載があった。  
![バージョン確認②](/RaiseTech/DBver.check02.png)  
どちらを確認すればよいか分からなかった。  

## Rails構成管理ツール
→ Gem
## 今回の課題から学んだこと
　ひとつのアプリケーションを動かすためにWebサーバー、APサーバー、DBサーバーを動かさなければならないことを知った。  
　また、アプリケーションを起動させていく過程で様々なコマンドがあることを知った。それぞれがRubyのコマンドなのか、gitコマンドなのか等々まだ混同してしまうため覚えていきたい。  
　
## 疑問点
　DBを起動していく際に、database.ymlをコピーしてdatabase.yml.sampleを作成していたが、それは何故か？  
実際自分で進めた際は、手順の通り進めても`Can't connect to local MySQL server through socket '/tmp/mysql.sock' (2)`と出て先に進めなかったが、元々あったdatabase.ymlのpassword,socketを埋めると起動できた。  
