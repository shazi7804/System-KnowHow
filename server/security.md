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
