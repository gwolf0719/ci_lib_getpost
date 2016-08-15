# ci_lib_getpost
php codeIgniter 簡化處理 getpost 外掛

# 功能介紹
將指定的 $_GET 或是 $_POST 值設定為陣列並驗證必填欄位。  
$data 輸入要被處理的陣列 key 會自動去把對應的 $_GET 或是 $_POST 放入回傳值
``
getpost_array($data,$requred = array())  
``


# 安裝方式
放在 application/libraries/  
# 呼叫方式
$this->load->library('getpost');  

