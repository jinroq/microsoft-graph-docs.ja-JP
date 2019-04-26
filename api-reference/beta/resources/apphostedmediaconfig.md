---
title: appHostedMediaConfig リソースの種類
description: アプリケーションによってホストされているメディアスタック。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 0cb34d0673404c90607a8f1ac442ca1b7c504ce9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339182"
---
# <a name="apphostedmediaconfig-resource-type"></a>appHostedMediaConfig リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

アプリケーションによってホストされているメディアスタック。

## <a name="properties"></a>プロパティ

| プロパティ                          | 型    | 説明                                                     |
| :-------------------------------- | :------ | :---------------------------------------------------------------|
| blob                              | String  | スマートメディアエージェントによって生成されたメディア構成 blob。    |
| removefromdefaultaudiogroup       | Boolean | 既定のオーディオグループからの音声の削除                       |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.mediaConfig",
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
<!--
{
  "type": "#page.annotation",
  "description": "appHostedMediaConfig resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
