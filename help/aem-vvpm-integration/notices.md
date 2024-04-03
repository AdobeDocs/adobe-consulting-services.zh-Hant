---
title: Veeva Vault整合注意事項
description: Veeva Vault整合注意事項
exl-id: 1a188671-d123-4475-a607-65743ba0dadd
source-git-commit: 07eab1e439626bd3bb3416c9e7d0c1666927a7aa
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 1%

---

# 最佳實務、護欄和通知

## 版本

此整合需要下列最低軟體版本：

* Adobe Experience Manager， 6.5.5+
* Veeva Vault PromoMats，20R3.2+

## 資料隱私

此整合旨在於Adobe Experience Manager與Veeva Vault PromoMats之間傳輸內容。 身為資料控管單位，貴公司有責任遵守適用於您收集和使用資料的任何隱私權法規。

## 內容同步頻率

觸發整合工作流程時，AEM內容和中繼資料會從AEM同步至VVPN。 這可以自動或手動完成。 VPM中繼資料會從VPM同步至AEM。 這可透過排程器自動完成，或透過按一下按鈕手動完成。

## 整合限制與最佳作法和護欄

使用此整合時，請考量下列限制：

* 同步中繼資料時，僅支援下列資料型別：「文字」和「多行文字」。
* 雖然整合支援AEM模組化內容（內容片段和體驗片段），但並不支援VVPM模組化內容。
* 不支援VVPM連結檔案。
* 不支援將VPM視覺註解從VPM同步至AEM。
* 整合不會將內容從VVPM匯入至AEM。
* 不支援中繼資料驗證。
* 檔案數量會根據Veeva授權而有所限制。 另請參閱 [授許可權制](#veeva-license-limitations).
* API呼叫的數量會根據Veeva授權而有所限制。 如需詳細資訊，請參閱 [API限制](https://developer.veevavault.com/docs/#what-are-rate-limits). 另請參閱 [授許可權制](#veeva-license-limitations).

## Veeva授許可權制

您可以瀏覽至VVPM一般設定，監控執行個體限制。

![Veeva限制](assets/veeva-limits.png)
