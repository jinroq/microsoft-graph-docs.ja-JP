---
author: psampath
ms.author: psampath
ms.date: 06/20/2018
title: StoragePlanInformation
localization_priority: Normal
ms.openlocfilehash: 3911d3af5f2149d1043ed246e7c11d287c840842
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342953"
---
# <a name="storageplaninformation-resource-type"></a>storageplan 情報リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**storageplan information**リソースは、ドライブの記憶域クォータプランに関する情報を提供します。

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

| プロパティ名     | 種類      | 説明                                                             |
|:------------------|:----------|:----------------------------------------------------------------------- |
| upgradeavailable  | Boolean   | 利用可能なストレージクォータプランが高であるかどうかを示します。 値の取得のみ可能です。 |


<!--
{
  "type": "#page.annotation",
  "description": "storagePlanInformation resource contains information about storage quota plans that make up the drive's storage space quota.",
  "keywords": "quota,plans,upgradeAvailable",
  "section": "documentation",
  "tocPath": "Resources/StoragePlanInformation",
  "suppressions": []
}
-->

