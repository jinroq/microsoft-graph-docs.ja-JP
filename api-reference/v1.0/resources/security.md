---
title: セキュリティリソースの種類
description: セキュリティリソースは、セキュリティオブジェクトモデルのエントリポイントです。 単一のセキュリティリソースを返します。 使用可能なプロパティは含まれていません。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: c7bf3f279e50efb451188426d030e356d55ad6be
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579213"
---
# <a name="security-resource-type"></a>セキュリティリソースの種類

セキュリティリソースは、セキュリティオブジェクトモデルのエントリポイントです。 単一のセキュリティリソースを返します。 使用可能なプロパティは含まれていません。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型 | 説明 |
|:-------------|:------------|:------------|
| [警告の一覧表示](../api/alert-list.md) | [alert](alert.md)コレクション | 通知オブジェクトのコレクションを取得します。 |
| [通知を取得する](../api/alert-get.md) | [alert](alert.md)コレクション | 通知オブジェクトを取得します。 |
| [アラートを更新する](../api/alert-update.md) | [alert](alert.md)コレクション | 通知オブジェクトを取得します。 |

## <a name="properties"></a>プロパティ
なし

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型        | 説明 |
|:-------------|:------------|:------------|
|アラート|[alert](alert.md)コレクション| 読み取り専用。Null 許容型です。|


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

**セキュリティ**リソースは、グラフのルートで使用できます。

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
