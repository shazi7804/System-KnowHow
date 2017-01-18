# 伺服器管理規範

## 權限 (permission)

權限是在**安全已不可信任**後的第二道防線，即使是系統管理員也必須 Login user 後再提供 sudo >權限。

> Default not allow root !!
>
> Web Service：special user not login with only read (400)
>
> Data service：special user not login with write (600)
