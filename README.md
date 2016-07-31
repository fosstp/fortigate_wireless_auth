# fortigate_wireless_auth
Fortigate firewall wireless authentication template  
<因預設參數問題，此檔案僅適用於Fortigate防火牆>  
<若要於其他平台認證，請自行替換圖片與帳號密碼之參數>  

設定說明：  
1. 請先選定貴校所需認證類型，只有校內或教育局Radius認證請使用「SigninFlatBlue」，若需結合Google認證請選用「GoogleSignin」。  
2. 製作貴校logo，並修改html檔案內的「title」、「img」、「placehoder」（需修改的地方皆有中文提示，請同時修改一般頁面與error頁面）。  
3. 在Fortigate新增4個FQDN位址物件，目的為在還沒認證前成功前正確載入css&js與學術網路規範網頁。  
	(a) maxcdn.bootstrapcdn.com  
	(b) code.jquery.com  
	(c) oss.maxcdn.com  
	(d) edu.law.moe.gov.tw  
4. 到Fortigate的「網路」→「介面」中選取wifi介面，於Exempt Destination/Services新增剛剛的4個FQDN位址物件。  
5. 到Fortigate的「系統管理」→「置換訊息」→「登入頁面」貼入html中的內容（登入失敗頁面貼入error的html內容）。
