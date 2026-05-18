---
product: adobe experience manager
solution: Experience Manager
product_v2: id: fd1f54a9-f50c-467d-8956-cebbaf4f3eb8
description: 諮詢Experience Manager檔案
type: Documentation
git-repo: https://github.com/AdobeDocs/adobe-consulting-services.en
index: true
source-git-commit: 78d98fcb8f43f48cab7de480af1eac087526cec5
workflow-type: tm+mt
source-wordcount: 94
ht-degree: 2%

---


# 內部使用的中繼資料

GitHub編寫系統中的中繼資料為階層式，而且會定義以下相對於前一項的遞增層級。

1. metadata.md
1. ToC
1. 文章

metadata.md檔案中定義的中繼資料會套用至整個存放庫，但可以在ToC和文章層級覆寫。 中繼資料的任何覆寫都應該儘可能在最低層級進行。

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

在[內部撰寫指南](https://experienceleague.adobe.com/docs/authoring-guide-exl/using/authoring/metadata.html)中找到有關中繼資料的其他資訊。
