# System Manage Policy (Linux)
一台 Server 的建立除了建立的 **目的性** 以外，還需要許多的規範讓開發者、管理者去遵守才不會讓系統雜亂無章的存在，造能管理上的困難。

## 定位 (Type)

在建立一台 Server 之前必須先定位好這台 Server 的定位類型。
> Web、Application、Database、Streaming、Proxy ... etc

## 系統 (OS)
決定 OS 的版本，這個 OS 的版本必須考慮到整體系統管理的統一性、長期支援、穩性性、常用第三方套件支援(Apache, PHP, Nginx ..etc)
> RedHat、CentOS、Ubuntu、Debian、OpenSUSE、OpenWrt ... etc

## 硬體資源 (Resource)
必須從 **目的性**、**定位** 去確認這台伺服器可能需要的硬體資源，並且考量 resource 的擴充彈性以滿足可能持續擴張的管理需求，除了功能性的縱向擴充，硬體資源的橫向擴充更是避免**移機**的關鍵。
> CPU core、Memory、Disk io、NetWork Speed ... etc

## 應用程式 (Application)
一台伺服器應該避免存在多種相同性質的 Application 如 Java, PHP, Python ..

應用程式的版本選擇也是重大的關鍵，Library 的支援、支援長期 bugfix、以及大環境的支援(ex: ssl chip、flash)
> LNMP、LAMP、Tomcat、Node.js ... etc

## 安全 (Security)
安全是伺服器的罩門，務必做好 Policy 管理，關閉不必要的服務端口、僅允許系統人員管理、定期 scan CVE。

> Access service：http(80)，https(443)
>
> Debug mode service：http(8080)，https(8443)
>
> Manager service：ssh(22)，
>
> Data service：ftp(21)，samba(137~139,445)
>
> Important service：SQL(3306,1433,1521)

除了 Access service 以外皆不可對外開放，

## 權限 (permission)

權限是在**安全已不可信任**後的第二道防線，即使是系統管理員也必須 Login user 後再提供 sudo 權限。

> Default not allow root !!
>
> Web Service：special user not login with only read (400)
>
> Data service：special user not login with write (600)
> 
> 

## 可用性 (Availability)

必須





