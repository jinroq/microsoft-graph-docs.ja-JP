---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharedDriveItem
localization_priority: Normal
description: sharedDriveItem リソースは、Shares API を使用して共有 driveItem にアクセスする場合に返されます。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 1f6684e9c266a800f5a76a7085a8af22ea9518e8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034336"
---
# <a name="shareddriveitem-resource-type"></a>SharedDriveItem リソースの種類

**sharedDriveItem** リソースは、[Shares](../api/shares-get.md) API を使用して共有 [driveItem](driveitem.md) にアクセスする場合に返されます。

## <a name="json-representation"></a>JSON 表記

以下は、**sharedDriveItem** リソースの JSON 表記です。

**sharedDriveItem** リソースは [**baseItem**](baseitem.md) から派生し、そのリソースからプロパティを継承します。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.baseItem",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.sharedDriveItem"
}-->

```json
{
  "id": "string",
  "name": "string",
  "owner": { "@odata.type": "microsoft.graph.identitySet" },

  "driveItem": { "@odata.type": "microsoft.graph.driveItem" },
  "items": [ { "@odata.type": "microsoft.graph.driveItem" }],
  "list": { "@odata.type": "microsoft.graph.list" },
  "listItem": { "@odata.type": "microsoft.graph.listItem" },
  "root": { "@odata.type": "microsoft.graph.driveItem" },
  "site": { "@odata.type": "microsoft.graph.site" }
}
```

## <a name="properties"></a>プロパティ

| プロパティ | 型                          | 説明                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| id       | 文字列                        | アクセスされている共有の一意識別子。              |
| name     | String                        | 共有項目の表示名。                             |
| owner    | [IdentitySet](identityset.md) | 参照されている共有アイテムの所有者に関する情報。 |

## <a name="relationships"></a>リレーションシップ

| リレーションシップ名 | 種類                | 説明
| ------------------|:--------------------|:-----------------------------------
| **driveItem**     | [**driveItem**][driveItem]   | 基になる **driveItem** にアクセスするために使用
| **list**          | [**一覧**][list]        | 基になる **list** にアクセスするために使用
| **listItem**      | [**listItem**][listItem]    | 基になる **listItem** にアクセスするために使用
| **site**          | [**サイト**][site]        | 基になる **site** にアクセスするために使用

または、個人用の OneDrive アカウントから共有される **driveItem** には、次のリレーションシップも使用できます。

| リレーションシップ名 | 種類                         | 説明
| ------------------|:-----------------------------|:-----------------------------------
| **items**         | [**Drive item**][driveItem]コレクション | 共有ルートに含まれているすべての driveItem。 このコレクションを列挙することはできません。
| **root**          | [**driveItem**][driveItem]   | 基になる**ドライブ項目**へのアクセスに使用されます。 非推奨-- `driveItem`代わりに使用します。

[driveItem]: driveitem.md
[list]: list.md
[listItem]: listitem.md
[site]: site.md

## <a name="methods"></a>メソッド

| Method                                  | REST パス                |
| :-------------------------------------- | :----------------------- |
| [共有アイテムを取得する](../api/shares-get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a>備考

DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。

<!-- {
  "type": "#page.annotation",
  "description": "Share resource returns information about a shared item or collection of items.",
  "keywords": "share,shared,sharing root,shared files, shared items",
  "section": "documentation",
  "tocPath": "Resources/Share"
} -->
