---
title: セキュリティ リソースの種類
description: セキュリティ リソースは、セキュリティ オブジェクト モデルのエントリ ポイントです。 シングルトンのセキュリティ リソースを返します。 使用可能なプロパティが含まれていません。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: c7bf3f279e50efb451188426d030e356d55ad6be
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983255"
---
# <a name="security-resource-type"></a>セキュリティ リソースの種類

セキュリティ リソースは、セキュリティ オブジェクト モデルのエントリ ポイントです。 シングルトンのセキュリティ リソースを返します。 使用可能なプロパティが含まれていません。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型 | 説明 |
|:-------------|:------------|:------------|
| [警告の一覧表示](../api/alert-list.md) | [アラート](alert.md)のコレクション | Alert オブジェクトのコレクションを取得します。 |
| [アラートを取得します。](../api/alert-get.md) | [アラート](alert.md)のコレクション | Alert オブジェクトを取得します。 |
| [アラートを更新します。](../api/alert-update.md) | [アラート](alert.md)のコレクション | Alert オブジェクトを取得します。 |

## <a name="properties"></a>プロパティ
なし

## <a name="relationships"></a>関係
| リレーションシップ | 型        | 説明 |
|:-------------|:------------|:------------|
|alerts|[アラート](alert.md)のコレクション| 読み取り専用です。Null 許容型。|


## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.security"
}-->

```json
{
}
```

## <a name="example"></a>例

**セキュリティ**リソースは、グラフのルートに使用できます。

<!--{
  "blockType": "request"
}-->
```http
GET https://graph.microsoft.com/v1.0/security
```

<!--{
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security"
}-->
```json
HTTP/1.1 200 OK
Content-type: application/json

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "security resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
