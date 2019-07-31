---
title: profilePhoto リソースの種類
description: Exchange Online または Azure Active Directory (AAD) からアクセスされるユーザー、グループ、または Outlook 連絡先のプロファイル写真。 base 64 でエンコードされていないバイナリ データです。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: eee47378343aef1b0a471ac186099d4598124862
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965678"
---
# <a name="profilephoto-resource-type"></a>profilePhoto リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Exchange Online または Azure Active Directory (AAD) からアクセスされるユーザー、グループ、または Outlook 連絡先のプロファイル写真。 base 64 でエンコードされていないバイナリ データです。

Exchange Online 上でサポートされている HD Photo のサイズは次のとおりです。'48x48'、'64x64'、'96x96'、'120x120'、'240x240'、'360x360'、'432x432'、'504x504'、'648x648'。 AAD では、写真は任意の次元にすることができます。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[ProfilePhoto を取得する](../api/profilephoto-get.md) | [profilePhoto](profilephoto.md) |指定した **profilePhoto** またはそのメタデータ (**profilePhoto** プロパティ) を取得します。 |
|[Update](../api/profilephoto-update.md) | [profilePhoto](profilephoto.md)  |指定されたユーザー、グループ、または連絡先に写真を割り当てます。写真はバイナリ形式にする必要があります。既存の写真が置き換えられます (存在する場合)。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id|string|読み取り専用です。|
|height|int32|写真の高さ。読み取り専用です。|
|width|int32|写真の幅。読み取り専用です。|

## <a name="relationships"></a>リレーションシップ
なし


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.profilePhoto"
}-->

```json
{
  "id": "240X240",
  "height": 240,
  "width": 240
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "profilePhoto resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
