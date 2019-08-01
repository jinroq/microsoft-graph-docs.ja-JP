---
title: teamsTabConfiguration リソースの種類 (オープンタイプ)
description: タブの内容を決定する設定。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2a3c16c69acefb8f746d11807a898e74de7620be
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033685"
---
# <a name="teamstabconfiguration-resource-type-open-type"></a>teamsTabConfiguration リソースの種類 (オープンタイプ)



[タブ](teamstab.md)の内容を決定する設定。タブが対話的に構成されている場合、この情報はタブプロバイダーアプリケーションによって設定されます。
次のプロパティに加えて、一部のタブプロバイダーアプリケーションは、追加のカスタムプロパティを指定します。

## <a name="properties"></a>プロパティ

|プロパティ|型|説明|
|-|-|-|
|  entityId   |   string |  タブプロバイダによってホストされているエンティティの識別子。     |
|  contentUrl |   string |  Teams でのタブのコンテンツのレンダリングに使用される Url。 必須です。    |
|  removeUrl  |   string |  Teams クライアントを使用してタブを削除したときに Teams クライアントによって呼び出される Url。     |
|  websiteUrl |   string |  Teams の外部にタブのコンテンツを表示するための Url。     |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsTabConfiguration"
}-->

```json
{
   "entityId": "string",
   "contentUrl": "string (HTTPS Url)",
   "websiteUrl": "string (HTTPS Url)",
   "removeUrl": "string (HTTPS Url)"  
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsTabConfiguration complex type (Open Type)",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
