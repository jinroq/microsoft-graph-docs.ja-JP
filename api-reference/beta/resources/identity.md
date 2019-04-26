---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/14/2017
title: ID
localization_priority: Normal
ms.openlocfilehash: a2ba76d5bac372be0a40001028dfb54e690a14fa
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333672"
---
# <a name="identity-resource-type"></a>id リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**ID** リソースは、_アクター_ の ID を表します。たとえば、アクターは、ユーザー、デバイス、アプリケーションです。

## <a name="json-representation"></a>JSON 表記

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.identity", "optionalProperties": ["displayName", "tenantId", "thumbnails"], "openType": true } -->

```json
{
  "displayName": "string",
  "id": "string",
  "tenantId": "string",
  "thumbnails": { "@odata.type": "microsoft.graph.thumbnailSet" }
}
```

## <a name="properties"></a>プロパティ

| プロパティ            | 型   | 説明                                                                                                                                                                                                                                                                                                           |
|:--------------------|:-------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| displayName         | 文字列 | ID の表示名。使用可能でない場合や、最新の状態ではない場合があることにご注意ください。たとえば、ユーザーが表示名を変更する場合、API は、将来の応答に新しい値を表示することがあります。しかし、ユーザーに関連付けられたアイテムについては、[delta](../api/driveitem-delta.md) の使用時に変更されたことは表示されません。  |
| id                  | String | ID の一意識別子。                                                                                                                                                                                                                                                                                   |
| tenantId            | String | テナントの一意の id (オプション)。                                                                                                                                                                                                                                                                             |

## <a name="remarks"></a>注釈

状況によっては、アクターの一意識別子は利用できないことがあります。その場合、ID の **displayName** プロパティが返されますが、**id** プロパティはリソースから失われます。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Identity contains information about an app, user, or group.",
  "keywords": "identity,owner,modifier,app,user,group",
  "section": "documentation",
  "tocPath": "Resources/Identity",
  "suppressions": []
}
-->
