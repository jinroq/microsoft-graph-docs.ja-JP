---
title: freeBusyError リソースの種類
description: ユーザー、配布リスト、またはリソースの空き時間情報を取得しようとしたときに発生したエラー情報を表します。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ca306ba5a40ffc08147c8e8449ab03bf51afd745
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030283"
---
# <a name="freebusyerror-resource-type"></a>freeBusyError リソースの種類

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
  "tocPath": ""
}
-->
