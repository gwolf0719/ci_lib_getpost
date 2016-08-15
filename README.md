# ci_lib_getpost
php codeIgniter 簡化處理 getpost 外掛
---
# 功能介紹
## 將指定的 $_GET 或是 $_POST 值設定為陣列並驗證必填欄位。  
$data     輸入要被處理的陣列 key 會自動去把對應的 $_GET 或是 $_POST 放入回傳值  
$requred  必填欄位，如果有必填欄位但是沒有值就會直接回傳 false 

``  
getpost_array($data,$requred = array())  
``
## 確認是哪個欄位沒有填寫  
延續 getpost_array 這個 function 將必填欄位丟進來，會去回傳是空值的項目塞入陣列中。
$data     輸入要被處理的陣列 key ,  
ex: 輸入的 $data = array("id","pwd",'name');  
如果只有id有值，就會回傳 array("pwd",'name');  
``  
report_requred($data)
``

---
# 安裝方式
放在 application/libraries/  
---
# 呼叫方式
$this->load->library('getpost');  

