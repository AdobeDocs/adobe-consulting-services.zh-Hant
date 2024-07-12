---
title: Veeva Vault整合常見問題集
description: Veeva Vault整合常見問題集
exl-id: c308ebb3-7881-4094-9f35-c67a96fb5ab1
source-git-commit: e4a5e55ac9b79a8de7dfa8ddd3d0ad99560917b8
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 0%

---

# 常見問題

**哪些中繼資料應該同步至Veeva？**

請務必根據Veeva入口網站中的內容型別（例如促銷活動）瞭解中繼資料。 檢閱Veeva入口網站後，在AEM中建構內容中繼資料結構，以保留每個資產/頁面的所有相關中繼資料，並設定整合以在兩個系統之間對應中繼資料。

**整合是否支援Veeva連結檔案？ 如果沒有，支援哪些關聯性型別？**

不適用。 請參閱[Veeva檔案](https://vaulthelp2.vod309.com/wordpress/admin-user-help/documents-admin-user-help/about-document-relationships/)。 「已連結」檔案（參考關係型別）是無法透過API建立或刪除的標準關係型別之一，因為它們具有特殊的儲存庫行為。 元件、支援檔案和任何不在此清單中的其他專案，應該能夠透過AEM Veeva雲端設定進行設定。

**整合是否支援AEM模組化內容？**

是，此整合支援AEM內容片段和體驗片段。

**整合是否支援Veeva模組化內容？**

否，目前不可以。

**整合是否將Veeva視覺註解同步至AEM？**

否，目前不可以。 視覺註解只能透過API作為PDF存取。

**我們如何設定整合所同步之VVPM檔案的許可權？**

整合使用服務使用者透過API上傳檔案。  檔案預設和覆寫規則（檔案的預設角色）僅在VVPM使用者介面中受支援，在使用API時不會套用。 建議使用DAC （動態存取控制）進行角色指派。 DAC會透過所有接觸點強制執行，包括API。 [請在這裡參閱檔案。](http://vaulthelp2.vod309.com/wordpress/admin-user-help/ah-user-permissions-access-control/about-dynamic-access-control-for-documents/)

**整合是否支援多個VPM執行個體？**

整合使用雲端設定方法，可允許從一個AEM例項設定多個Veeva端點。

**整合是否支援AEM發佈？**

否，此整合僅適用於AEM作者。 這是為了在內容發佈之前促進MLR稽核週期。
