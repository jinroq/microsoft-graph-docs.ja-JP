---
title: profilePhoto リソースの種類
description: Exchange Online からアクセスされるユーザー、グループ、または Outlook の連絡先のプロフィール写真。base 64 でエンコードされていないバイナリ データです。
localization_priority: Priority
ms.openlocfilehash: b1901928a97356b2a9808a446d34981fd74bf456
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876567"
---
# <a name="profilephoto-resource-type"></a>profilePhoto リソースの種類
Exchange Online からアクセスされるユーザー、グループ、または Outlook の連絡先のプロフィール写真。base 64 でエンコードされていないバイナリ データです。

Exchange Online 上でサポートされている HD Photo のサイズは次のとおりです。'48x48'、'64x64'、'96x96'、'120x120'、'240x240'、'360x360'、'432x432'、'504x504'、'648x648'。 

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[ProfilePhoto を取得する](../api/profilephoto-get.md) | [profilePhoto](profilephoto.md) |指定した **profilePhoto** またはそのメタデータ (profilePhoto プロパティ) を取得します。|
|[Update](../api/profilephoto-update.md) | [profilePhoto](profilephoto.md)  |指定されたユーザー、グループ、または連絡先に写真を割り当てます。写真はバイナリ形式にする必要があります。既存の写真が置き換えられます (存在する場合)。|

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|ID|文字列|読み取り専用です。|
|height|int32|写真の高さ。読み取り専用です。|
|width|int32|写真の幅。読み取り専用です。|

## <a name="relationships"></a>リレーションシップ
なし


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "isMediaEntity": true,
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
<!-- {
  "type": "#page.annotation",
  "description": "profilePhoto resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
