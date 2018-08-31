---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: BaseItem
ms.openlocfilehash: eaf73cf54671393b61cc37b5a5d1922060640882
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/21/2018
ms.locfileid: "23268915"
---
# <a name="baseitem-resource-type"></a>BaseItem リソース型

**baseItem** リソースは、他のいくつかのリソースの種類間で共有されるプロパティの共通セットを含む抽象リソースです。**baseItem** から派生するリソースには以下が含まれます。

* [drive](drive.md)
* [driveItem](driveitem.md)
* [site](site.md)
* [sharedDriveItem](shareddriveitem.md)

## <a name="json-representation"></a>JSON 表記

以下は、**baseItem** リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "createdBy", "lastModifiedBy", "description", "parentReference", "webUrl" ],
  "keyProperty": "id",
  "abstract": true,
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.baseItem"
}-->

```json
{
  "id": "string (identifier)",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "datetime",
  "description": "string",
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "datetime",
  "name": "string",
  "parentReference": { "@odata.type": "microsoft.graph.itemReference" },
  "webUrl": "url"
}
```

## <a name="properties"></a>プロパティ

| プロパティ             | タイプ              | 説明                                                                            |
| :------------------- | :---------------- | :------------------------------------------------------------------------------------- |
| ID                   | 文字列            | ドライブの一意識別子。読み取り専用です。                                         |
| createdBy            | [identitySet][]   | アイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。        |
| createdDateTime      | dateTimeOffset    | アイテム作成の日時。読み取り専用です。                                             |
| 説明          | 文字列            | ユーザーに表示されるアイテムの説明を提供します。 省略可能。                             |
| eTag                 | 文字列            | アイテムの ETag。読み取り専用です。                                                          |
| lastModifiedBy       | [identitySet][]   | アイテムを最終更新したユーザーの ID、デバイス、アプリケーション。読み取り専用です。 |
| lastModifiedDateTime | dateTimeOffset    | アイテムが最後に変更された日時。読み取り専用です。                                   |
| name                 | 文字列            | アイテムの名前。読み取り/書き込み。                                                      |
| parentReference      | [itemReference][] | 親の情報 (アイテムに親がある場合)。読み取り/書き込み。                              |
| webUrl               | string (URL)      | ブラウザーでリソースを表示するための URL。読み取り専用です。                              |

## <a name="relationships"></a>リレーションシップ

| リレーションシップ       | 型     | 説明
|:-------------------|:---------|:---------------------------------------------
| createdByUser      | [ユーザー][] | アイテムを作成したユーザーの ID です。 読み取り専用です。
| lastModifiedByUser | [ユーザー][] | アイテムを最後に変更したユーザーの ID です。 読み取り専用です。

[identitySet]: identityset.md
[itemReference]: itemreference.md
[ユーザー]: user.md

## <a name="remarks"></a>備考

の種類は直接使用できません。`baseItem`

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/BaseItem"
} -->
