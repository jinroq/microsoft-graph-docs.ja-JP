---
title: oneNoteIdentitySet リソースの種類
description: '**まもなくサポートが提供される**'
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 9ffbc20a73aaed885d118094a7d1946459eb7efc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009364"
---
# <a name="onenoteidentityset-resource-type"></a>oneNoteIdentitySet リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**まもなくサポートが提供される**

OneNoteIdentitySet 型は、 [OneNoteIdentity](onenoteidentity.md)オブジェクトのキー付きコレクションです。
_作成者_または_最終更新者_など、_ノートブック_、_セクション_、または_ページ_のさまざまなイベントに関連付けられている id のセットを表すために使用されます。 
 
現在、1つのキーの_**ユーザー**_ が含まれています。  その後、アイテムを変更するためのデバイスやアプリケーションなどのキーが追加されることがあります。

後で、この型は、identity [set](identityset.md)と統合されます。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteIdentityset"
}-->

```json
{
  "user": {"@odata.type": "microsoft.graph.onenoteIdentity"}
}

```
## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|user|[oneNoteIdentity](onenoteidentity.md)|ユーザーを表す OneNoteIdentity リソース。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oneNoteIdentitySet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
