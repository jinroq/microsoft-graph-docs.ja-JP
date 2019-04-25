---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: ID
localization_priority: Normal
ms.openlocfilehash: 103657764b2f7073d553a01cd3794c0abecdf4f4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567817"
---
# <a name="identity-resource-type"></a>ID リソースの種類

**ID** リソースは、_アクター_ の ID を表します。たとえば、アクターは、ユーザー、デバイス、アプリケーションです。

## <a name="json-representation"></a>JSON 表記

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.identity",
  "openType": true,
 "optionalProperties": ["displayName", "thumbnails"] } -->
```json
{
  "displayName": "string",
  "id": "string",
  "thumbnails": { "@odata.type": "microsoft.graph.thumbnailSet" }
}
```

## <a name="properties"></a>プロパティ

| プロパティ    | 型   | 説明                                                                                                                                                                                                                                                                                                           |
|:------------|:-------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| displayName | String | ID の表示名。使用可能でない場合や、最新の状態ではない場合があることにご注意ください。たとえば、ユーザーが表示名を変更する場合、API は、将来の応答に新しい値を表示することがあります。しかし、ユーザーに関連付けられたアイテムについては、[delta](../api/driveitem-delta.md) の使用時に変更されたことは表示されません。     |
| id          | String | ID の一意識別子。                                                                                                                                                                                                                                                                                   |

## <a name="remarks"></a>注釈

状況によっては、アクターの一意識別子は利用できないことがあります。その場合、ID の **displayName** プロパティが返されますが、**id** プロパティはリソースから失われます。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity contains information about an app, user, or group.",
  "keywords": "identity,owner,modifier,app,user,group",
  "section": "documentation",
  "tocPath": "Resources/Identity"

} -->
