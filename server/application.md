## 應用程式 (Application)
一台伺服器應該避免存在多種相同性質的程式語言，除非因成本因素或測試否則環境盡量讓伺服器的環境單純。

> PHP、JAVA、Python、Perl、C ... etc

在 `Application` 的選擇上在這個 OpenSource 林立的時代，經常會需要抉擇其中一種做使用，這必須因環境需求來選擇最貼近的 `Application`，以 `MySQL` 為例其分支就有好幾種且分為 `MyISAM`、`InnoDB`、`XtraDB`，其 Mobile01[^1] 就是更換為 `Percona` 的 `XtraDB` 來解決大量 `Query` 的需求。

> Oracle MySQL、MariaDB、Percona、Drizzle ... 


應用程式的版本選擇也是重大的關鍵，`Library` 的支援、支援長期 `bugfix`、以及大環境的支援

> LNMP、LAMP、Tomcat、Parse ... etc






[^1]: [Mobile01 - 現在SSD硬碟可以拿來跑資料庫嗎?][mobile01-ssdb]

[mobile01-ssdb]: http://www.mobile01.com/topicdetail.php?f=506&t=2982822&p=1