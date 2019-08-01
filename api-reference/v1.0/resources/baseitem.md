---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: BaseItem
localization_priority: Normal
description: BaseItem リソースは、他のいくつかのリソースの種類で共有される共通のプロパティセットが含まれる抽象リソースです。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 2bde386a736805d52758f6d80e629c585f82d87e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029982"
---
# <a name="baseitem-resource-type"></a>BaseItem リソースの種類

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

| プロパティ             | 型              | 説明                                                                            |
| :------------------- | :---------------- | :------------------------------------------------------------------------------------- |
| id                   | 文字列            | ドライブの一意識別子。読み取り専用。                                         |
| createdBy            | [identitySet][]   | アイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。        |
| createdDateTime      | dateTimeOffset    | アイテム作成の日時。読み取り専用です。                                             |
| 説明          | String            | ユーザーに表示されるアイテムの説明を提供します。 省略可能。                             |
| eTag                 | string            | アイテムの ETag。読み取り専用です。                                                          |
| lastModifiedBy       | [identitySet][]   | アイテムを最終更新したユーザーの ID、デバイス、アプリケーション。読み取り専用です。 |
| lastModifiedDateTime | dateTimeOffset    | アイテムが最後に変更された日時。読み取り専用です。                                   |
| name                 | string            | アイテムの名前。読み取り/書き込み。                                                      |
| parentReference      | [itemReference][] | 親の情報 (アイテムに親がある場合)。読み取り/書き込み。                              |
| webUrl               | string (URL)      | ブラウザーでリソースを表示するための URL。読み取り専用です。                              |

## <a name="relationships"></a>リレーションシップ

| リレーションシップ       | 型     | 説明
|:-------------------|:---------|:---------------------------------------------
| createdByUser      | [user][] | アイテムを作成したユーザーの ID です。 読み取り専用です。
| lastModifiedByUser | [user][] | アイテムを最後に変更したユーザーの ID です。 読み取り専用です。

[identitySet]: identityset.md
[itemReference]: itemreference.md
[ユーザー]: user.md

## <a name="remarks"></a>備考

`baseItem` の種類は直接使用できません。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/BaseItem"
} -->
