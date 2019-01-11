---
title: oneNoteIdentitySet リソースの種類
description: '**準備中のサポート**'
localization_priority: Normal
ms.openlocfilehash: d2969d073503a9fd586641abeb3d82f719db8545
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874089"
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
| プロパティ     | 種類   |説明|
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
