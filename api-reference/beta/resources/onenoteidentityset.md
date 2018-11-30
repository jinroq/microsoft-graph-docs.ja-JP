---
title: oneNoteIdentitySet リソースの種類
description: '**準備中のサポート**'
ms.openlocfilehash: bbfd49c1ea4c0af7812ec67f40490ed8627a65a7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067666"
---
# <a name="onenoteidentityset-resource-type"></a>oneNoteIdentitySet リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

**準備中のサポート**

OneNoteIdentitySet 型は、 [OneNoteIdentity](onenoteidentity.md)オブジェクトのキー付きコレクションです。
関連付けられているさまざまなイベントの_ノートブック_、_セクション_または_ページ_の_作成者_または_最終更新者_などの id のセットを表すために使用されます。 
 
現在 1 つのキー、_**ユーザー**_ が含まれています。  将来的には、デバイス、またはアイテムを変更するのにはアプリケーション キーが追加されます。

[IdentitySet](identityset.md)でこの型をマージする将来的には、

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteidentityset"
}-->

```json
{
  "user": {"@odata.type": "microsoft.graph.oneNoteIdentity"}
}

```
## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|user|[oneNoteIdentity](onenoteidentity.md)|OneNoteIdentity のリソースで、ユーザーを表します。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "oneNoteIdentitySet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
