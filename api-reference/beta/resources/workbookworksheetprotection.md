---
title: workbookWorksheetProtection リソースの種類
description: シート オブジェクトの保護を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: ed6f52074836368eade8851ea32f1e8ef64e493e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007040"
---
# <a name="workbookworksheetprotection-resource-type"></a>workbookWorksheetProtection リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

シート オブジェクトの保護を表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[WorkbookWorksheetProtection を取得する](../api/worksheetprotection-get.md) | [workbookWorksheetProtection](workbookworksheetprotection.md) |WorkbookWorksheetProtection オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Protect](../api/worksheetprotection-protect.md)|None|ワークシートを保護します。ワークシートが保護されている場合はスローします。|
|[Unprotect](../api/worksheetprotection-unprotect.md)|なし|ワークシートの保護を解除します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|オプション|[workbookWorksheetProtectionOptions](workbookworksheetprotectionoptions.md)|シートの保護のオプション。 読み取り専用です。|
|protected|ブール値|ワークシートが保護されているかどうかを示します。読み取り専用です。|

## <a name="relationships"></a>リレーションシップ
なし。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "options"
  ],
  "@odata.type": "microsoft.graph.workbookWorksheetProtection"
}-->

```json
{
  "protected": "boolean"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "workbookWorksheetProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
