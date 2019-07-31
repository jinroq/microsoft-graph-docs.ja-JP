---
title: appHostedMediaConfig リソースの種類
description: アプリケーションによってホストされているメディアスタック。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: abc9cd8aa916c4e0b9141f79151fbd7e9f2d3b8b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013368"
---
# <a name="apphostedmediaconfig-resource-type"></a>appHostedMediaConfig リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

アプリケーションによってホストされているメディアスタック。

## <a name="properties"></a>プロパティ

| プロパティ                          | 型    | 説明                                                     |
| :-------------------------------- | :------ | :---------------------------------------------------------------|
| blob                              | String  | スマートメディアエージェントによって生成されたメディア構成 blob。    |
| removeFromDefaultAudioGroup       | Boolean | 既定のオーディオグループからの音声の削除                       |

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
