---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: BaseItem
ms.openlocfilehash: d70a75be0be4d7ecbd010288cb313b8394736932
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074414"
---
# <a name="baseitem-resource-type"></a>BaseItem リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

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
| ID                   | 文字列            | ドライブの一意識別子。読み取り専用です。                                         |
| createdBy            | [identitySet][]   | アイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。        |
| createdDateTime      | dateTimeOffset    | アイテム作成の日時。読み取り専用です。                                             |
| eTag                 | 文字列            | アイテムの ETag。読み取り専用です。                                                          |
| lastModifiedBy       | [identitySet][]   | アイテムを最終更新したユーザーの ID、デバイス、アプリケーション。読み取り専用です。 |
| lastModifiedDateTime | dateTimeOffset    | アイテムが最後に変更された日時。読み取り専用です。                                   |
| name                 | 文字列            | アイテムの名前。読み取り/書き込み。                                                      |
| parentReference      | [itemReference][] | 親の情報 (アイテムに親がある場合)。読み取り/書き込み。                              |
| webUrl               | string (URL)      | ブラウザーでリソースを表示するための URL。読み取り専用です。                              |

[identitySet]: identityset.md
[itemReference]: itemreference.md

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
