---
title: meetingInfo リソースの種類
description: 会議の情報を作成または、ミーティングに参加するために指定します。
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 24ac0247fd39569276f2cb288646eca578447e07
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817753"
---
# <a name="meetinginfo-resource-type"></a><span data-ttu-id="135e9-103">meetingInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="135e9-103">meetingInfo resource type</span></span>

> <span data-ttu-id="135e9-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="135e9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="135e9-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="135e9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="135e9-106">会議の情報を作成または、ミーティングに参加するために指定します。</span><span class="sxs-lookup"><span data-stu-id="135e9-106">Meeting information specified to create or join a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="135e9-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="135e9-107">Properties</span></span>

| <span data-ttu-id="135e9-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="135e9-108">Property</span></span>       | <span data-ttu-id="135e9-109">種類</span><span class="sxs-lookup"><span data-stu-id="135e9-109">Type</span></span>    | <span data-ttu-id="135e9-110">説明</span><span class="sxs-lookup"><span data-stu-id="135e9-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="135e9-111">allowConversationWithoutHost</span><span class="sxs-lookup"><span data-stu-id="135e9-111">allowConversationWithoutHost</span></span> | <span data-ttu-id="135e9-112">ブール型</span><span class="sxs-lookup"><span data-stu-id="135e9-112">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="135e9-113">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="135e9-113">JSON representation</span></span>

<span data-ttu-id="135e9-114">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="135e9-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
