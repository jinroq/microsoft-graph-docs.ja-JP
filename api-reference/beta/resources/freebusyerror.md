---
title: freeBusyError リソースの種類
description: ユーザー、配布リスト、またはリソースの空き時間情報を取得しようとしたときに発生したエラー情報を表します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 82350bc8cfeece76e0cd5c6873810988194cfb01
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971964"
---
# <a name="freebusyerror-resource-type"></a>freeBusyError リソースの種類

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
ユーザー、配布リスト、またはリソースの空き時間情報を取得しようとしたときに発生したエラー情報を表します。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|メッセージ​​ |String |エラーについて説明します。 |
|responseCode |String |ユーザー、配布リスト、またはリソースの可用性を照会するための応答コード。 |


## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.freeBusyError"
}-->

```json
{
  "message": "String",
  "responseCode": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "freeBusyError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
