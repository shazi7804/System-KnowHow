## 權限 \(permission\)

權限是在**安全已不可信任**後的第二道防線，



### Remote Access 

即使是系統管理員也必須 Login user 後再提供 sudo 權限。

> Default not allow root !!
>
> Data service：special user not login with write \(600\)



### Web Application

通常 Web 權限都會使用特別的 User，並且權限設定為 Read Only 避免出現 Web 漏洞時被植入惡意程式

> /var/www/html：special user\(www-data\) not login with only read \(400\)



### Content Access

檔案寫入的部份通常另外處理，避免和 Web 相同伺服器，由 Content Server 擔任寫入點，一樣使用特別 User 寫入，最多給予 `600` 的權限。

























