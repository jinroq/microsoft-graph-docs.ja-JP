---
author: JeremyKelley
description: Identity Set リソースは、id リソースのキー付きコレクションです。
ms.date: 09/10/2017
title: IdentitySet
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: c43981c1f7e79567afe901217030a0b5abed6f53
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006291"
---
# <a name="identityset-resource-type"></a>id セットリソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Identity **set**リソースは、 [id](identity.md)リソースのキー付きコレクションです。

_作成者_または_最終更新者_など、アイテムのさまざまなイベントに関連付けられている id のセットを表すために使用されます。

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.identitySet",
  "optionalProperties": [
    "application",
    "applicationInstance",
    "conversation",
    "conversationIdentityType",
    "device",
    "encrypted",
    "guest",
    "phone",
    "user"
  ],
  "openType": true
} -->
```json
{
  "application": {"@odata.type": "microsoft.graph.identity"},
  "applicationInstance": {"@odata.type": "microsoft.graph.identity"},
  "conversation": {"@odata.type": "microsoft.graph.identity"},
  "conversationIdentityType": {"@odata.type": "microsoft.graph.identity"},
  "device": {"@odata.type": "microsoft.graph.identity"},
  "encrypted": {"@odata.type": "microsoft.graph.identity"},
  "guest": {"@odata.type": "microsoft.graph.identity"},
  "phone": {"@odata.type": "microsoft.graph.identity"},
  "user": {"@odata.type": "microsoft.graph.identity"}
}
```

## <a name="properties"></a>プロパティ

| プロパティ    | 型                    | 説明                                             |
|:------------|:------------------------|:--------------------------------------------------------|
| application | [ID](identity.md) | 省略可能。このアクションに関連付けられているアプリケーション。  |
| conversation| [Identity](identity.md) | 省略可能。 このアクションに関連付けられているチームまたはチャネル。       |
| conversationIdentityType| [Identity](identity.md) | 省略可能。 **会話**プロパティがチームまたはチャネルを識別するかどうかを示します。|
| デバイス      | [ID](identity.md) | 省略可能。このアクションに関連付けられているデバイス。       |
| phone       | [identity](identity.md) | 省略可能。 このアクションに関連付けられている電話番号。 |
| user        | [Identity](identity.md) | 省略可能。このアクションに関連付けられているユーザー。         |

## <a name="remarks"></a>注釈 

「[呼び出し](call.md)を使用したリソースの**設定**」を参照してください。


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->
