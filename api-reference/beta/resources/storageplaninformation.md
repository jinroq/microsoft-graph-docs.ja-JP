---
author: psampath
ms.author: psampath
ms.date: 06/20/2018
title: StoragePlanInformation
localization_priority: Normal
ms.openlocfilehash: bbe4faaffbf53c24d4d0f5b8ea1f5ee1e1966a2c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860124"
---
# <a name="storageplaninformation-resource-type"></a>storagePlanInformation リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

**StoragePlanInformation**リソースでは、ドライブの記憶域のクォータの計画に関する情報を提供します。

### <a name="json-representation"></a>JSON 表記

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
   "@odata.type": "microsoft.graph.storagePlanInformation",
} -->

```json
{
  "upgradeAvailable": true
}

```
## <a name="properties"></a>プロパティ

| プロパティ名     | Type      | 説明                                                             |
|:------------------|:----------|:----------------------------------------------------------------------- |
| upgradeAvailable  | ブール型   | 高いストレージ クォータのプランが利用できることを示します。 読み取り専用です。 |


<!-- {
  "type": "#page.annotation",
  "description": "storagePlanInformation resource contains information about storage quota plans that make up the drive's storage space quota.",
  "keywords": "quota,plans,upgradeAvailable",
  "section": "documentation",
  "tocPath": "Resources/StoragePlanInformation"
} -->

