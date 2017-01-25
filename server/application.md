## 應用程式 (Application)
一台伺服器應該避免存在多種相同性質的程式語言，除非因成本因素或測試否則環境盡量讓伺服器的環境單純。

> PHP、JAVA、Python、Perl、C ... etc

在 `Application` 的選擇上在這個 `Open Source` 林立的時代，經常會需要抉擇其中一種做使用，這必須因環境需求來選擇最貼近的 `Application`，以 `MySQL` 為例其分支就有好幾種且分為 `MyISAM`、`InnoDB`、`XtraDB`，其 Mobile01[^1] 就是更換為 `Percona` 的 `XtraDB` 來解決大量 `Query` 的需求。

> Oracle MySQL、MariaDB、Percona、Drizzle ... 

應用程式的版本選擇也是重大的關鍵，`Library` 的支援、支援長期 `bugfix` 以及大環境的支援，然而版本不是最新的最好，而是要能新又穩定，通常最新版本 `Release` 後的第一個版本都是白老鼠，要能穩定使用後都是在 `build` 或 `minor` 版本[^2]更新 1-2 個版本後再開始採用會比較好。  

軟體的支援程度也會是一位工程師必須思考到的，就像銀行或公家機關常會選擇商業軟體，是因為出事不需要自行維護，只需要 call 廠商，而在一家資訊公司或是工程師有能力維護的環境，就必須考慮這套軟體是否還能繼續支援、支援多久，可靠性。

現在也有許多 `Open Source` 的軟體既是第三方開源，但也擁有官方企業支援，是現在很常見的商業模式，算是時代演變下雙贏的結果。




### 參考資料

[^1]: [Mobile01 - 現在SSD硬碟可以拿來跑資料庫嗎?][mobile01-ssdb]
[^2]: 維基百科 - 軟體版本號通常訂定規則為：major.minor(.build)，major 是最大的版本編號，minor 為其次，某些軟體可能再細分作 build，為更小的版本編號。
[^3]: Main、Restricted、Universe、Multiverse 分類為四個種類作為區別支援的級別。

[mobile01-ssdb]: http://www.mobile01.com/topicdetail.php?f=506&t=2982822&p=1
[software-release-version]: https://zh.wikipedia.org/wiki/軟件版本號
[ubuntu]: https://zh.wikipedia.org/wiki/Ubuntu