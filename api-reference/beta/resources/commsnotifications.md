---
title: commsNotifications リソースの種類
description: 通信サーバーによって 1 つのバッチで複数の通知を送信するための通知の一覧です。
author: VinodRavichandran
ms.openlocfilehash: 052520a99081e5c09cd6e3ec3b74f74e9527d38d
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380451"
---
# <a name="commsnotifications-resource-type"></a><span data-ttu-id="6e86b-103">commsNotifications リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6e86b-103">commsNotifications resource type</span></span>

> <span data-ttu-id="6e86b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6e86b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6e86b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6e86b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6e86b-106">通信サーバーによって 1 つのバッチで複数の通知を送信するための通知の一覧です。</span><span class="sxs-lookup"><span data-stu-id="6e86b-106">List of notifications used by the Communications servers for sending multiple notifications in a single batch.</span></span>

## <a name="properties"></a><span data-ttu-id="6e86b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6e86b-107">Properties</span></span>

| <span data-ttu-id="6e86b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6e86b-108">Property</span></span>       | <span data-ttu-id="6e86b-109">型</span><span class="sxs-lookup"><span data-stu-id="6e86b-109">Type</span></span>                                                 | <span data-ttu-id="6e86b-110">説明</span><span class="sxs-lookup"><span data-stu-id="6e86b-110">Description</span></span>                                   |
|:---------------|:-----------------------------------------------------|:----------------------------------------------|
| <span data-ttu-id="6e86b-111">value</span><span class="sxs-lookup"><span data-stu-id="6e86b-111">value</span></span>          | <span data-ttu-id="6e86b-112">[commsNotification](commsnotification.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="6e86b-112">[commsNotification](commsnotification.md) collection</span></span> | <span data-ttu-id="6e86b-113">リソースに変更を通知します。</span><span class="sxs-lookup"><span data-stu-id="6e86b-113">The notification of a change in the resource.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6e86b-114">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6e86b-114">JSON representation</span></span>

<span data-ttu-id="6e86b-115">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6e86b-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [ { "@odata.type": "#microsoft.graph.commsNotification" } ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "commsNotifications resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->