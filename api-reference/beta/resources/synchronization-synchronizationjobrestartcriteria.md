---
title: synchronizationJobRestartCriteria リソースの種類
description: 同期ジョブの範囲を定義し[ます。再起動](../api/synchronization_synchronizationjob_restart.md)アクション。
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8fb363b74f1daff678d0751aca4a9033b01d9832
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964656"
---
# <a name="synchronizationjobrestartcriteria-resource-type"></a>synchronizationJobRestartCriteria リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

同期ジョブの範囲を定義し[ます。再起動](../api/synchronization-synchronizationjob-restart.md)アクション。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|resetScope|String| `Full`、 `Watermark` `Escrows`、、、、 `ConnectorDataStore`の各値のコンマ区切りの組み合わせ。 `QuarantineState` すべて`Full`のオプションを使用する場合に使用します。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationJobRestartCriteria"
}-->

```json
{
  "resetScope": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationJobRestartCriteria resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
