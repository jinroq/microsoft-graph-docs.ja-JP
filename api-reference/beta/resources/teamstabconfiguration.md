---
title: teamsTabConfiguration リソースの種類 (オープン型)
description: タブの内容を決定する設定です。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 515e5896591b58054f161ff740f68b0ca4913663
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913486"
---
# <a name="teamstabconfiguration-resource-type-open-type"></a>teamsTabConfiguration リソースの種類 (オープン型)

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

[タブ](teamstab.md)の内容を決定する設定です。タブが対話形式で構成されている場合、この情報は、タブ プロバイダー アプリケーションによって設定されます。
に加えて、以下のプロパティは、タブ プロバイダー アプリケーションをいくつかは、追加のカスタム プロパティを指定します。

## <a name="properties"></a>プロパティ

|プロパティ|種類|説明|
|-|-|-|
|  entityId   |   文字列 |  タブ プロバイダーによってホストされているエンティティの識別子です。     |
|  contentUrl |   文字列 |  チームでのタブの内容を表示するために使用される Url です。 必須。    |
|  removeUrl  |   文字列 |  チームのクライアントを使用してタブが削除されたときに、チーム クライアントによって呼び出される Url。     |
|  websiteUrl |   文字列 |  チーム以外のタブの内容を表示するための Url です。     |

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
