---
title: appHostedMediaConfig リソースの種類
description: メディア スタックは、アプリケーションによってホストされています。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 36f869be347e2d55ec90079c62c5b6ebef85f144
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928585"
---
# <a name="apphostedmediaconfig-resource-type"></a>appHostedMediaConfig リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

メディア スタックは、アプリケーションによってホストされています。

## <a name="properties"></a>プロパティ

| プロパティ                          | 種類    | 説明                                                     |
| :-------------------------------- | :------ | :---------------------------------------------------------------|
| blob                              | String  | スマート メディア エージェントによって生成されたメディア構成の blob です。    |
| removeFromDefaultAudioGroup       | ブール型 | オーディオの既定のグループからのオーディオを削除します。                       |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.appHostedMediaConfig"
}-->
```json
{
  "blob": "String",
  "removeFromDefaultAudioGroup": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "appHostedMediaConfig resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
