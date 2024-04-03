---
product: adobe experience manager
solution: Experience Manager
description: 諮詢Experience Manager檔案
type: Documentation
git-repo: https://github.com/AdobeDocs/adobe-consulting-services.zh-Hant
index: y
source-git-commit: e2dac4b36fb94d72b72ef6f73a77e3f566539444
workflow-type: tm+mt
source-wordcount: '81'
ht-degree: 54%

---


# 內部使用的中繼資料

GitHub編寫系統中的中繼資料為階層式，而且會定義以下相對於前一項的遞增層級。

1. metadata.md
1. ToC
1. 文章

metadata.md 檔案中所定義的中繼資料會套用到整個存放庫，但可以在 ToC 和文章層級被覆寫。 中繼資料的任何覆寫都應該盡量在最低層級進行。

metadata.md

* `product`
* `git-repo`
* `index: y`

ToCs

* `sub-product`
* `user-guide-title`

文章

* `title`
* `description`

有關中繼資料的其他資訊，請參閱 [內部撰寫指南](https://experienceleague.adobe.com/docs/authoring-guide-exl/using/authoring/metadata.html).
