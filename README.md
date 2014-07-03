mt-template-data-api-recent-entry-list
======================================
Data APIを使ってブログ記事の一覧を取得して表示させます。  

■Step1■  
jQueryを読み込むようにテンプレートの&lt;head&gt;内を編集します。  
例：  
&lt;script src="http://your-url/jquery.min.js"&gt;&lt;/script&gt;  

■Step2■  
mt-data-api.jsを読み込むようにテンプレートの&lt;head&gt;内を編集します。  
例：  
&lt;script type="text/javascript" src="http://your-url/mt-static/data-api/v1/js/mt-data-api.js"&gt;&lt;/script&gt;  
  
■Step3■  
「mt-template-data-api-recent-entry-list.txt」をコピーしてインデックス・テンプレートを作成し、書き出します。  
例：mt-template-data-api-recent-entry-list.js  

設定が必要なところ  
・clientId  
　　clientIdには任意の名前を設定してください。  
・blogId  
　　blogIdにはデータを取得したいブログのID番号を設定してください。  

■Step4■  
ブログ記事リストを表示させたいページに■Step3■で書き出したファイルを読み込むようにテンプレートの&lt;head&gt;内を編集します。  
例：  
「mt-template-data-api-recent-entry-list.js」というファイル名で書き出した場合。  
&lt;script type="text/javascript" src="http://your-url/mt-template-data-api-recent-entry-list.js"&gt;&lt;/script&gt;  

■Step5■  
ブログ記事のリストを表示させたいところに以下のHTMLソースを追加してください。    
&lt:ul id="recententrylist"&gt;&lt;/ul&gt;    

======================================
取得されるブログ記事の件数はデフォルトでは10件ですが、20件のブログ記事を取得するようになっています。  

取得件数を変更したい場合は、「limit: 20,」の箇所で件数を変更してください。  
