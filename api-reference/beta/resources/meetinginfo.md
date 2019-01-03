---
title: meetingInfo リソースの種類
description: 会議の情報を作成または、ミーティングに参加するために指定します。
author: VinodRavichandran
ms.openlocfilehash: f8039f05a2f25e254f7aefd740055babc1598dc1
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380311"
---
# <a name="meetinginfo-resource-type"></a><span data-ttu-id="51b0f-103">meetingInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="51b0f-103">meetingInfo resource type</span></span>

> <span data-ttu-id="51b0f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="51b0f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="51b0f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="51b0f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="51b0f-106">会議の情報を作成または、ミーティングに参加するために指定します。</span><span class="sxs-lookup"><span data-stu-id="51b0f-106">Meeting information specified to create or join a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="51b0f-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="51b0f-107">Properties</span></span>

| <span data-ttu-id="51b0f-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="51b0f-108">Property</span></span>       | <span data-ttu-id="51b0f-109">型</span><span class="sxs-lookup"><span data-stu-id="51b0f-109">Type</span></span>    | <span data-ttu-id="51b0f-110">説明</span><span class="sxs-lookup"><span data-stu-id="51b0f-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="51b0f-111">allowConversationWithoutHost</span><span class="sxs-lookup"><span data-stu-id="51b0f-111">allowConversationWithoutHost</span></span> | <span data-ttu-id="51b0f-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="51b0f-112">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="51b0f-113">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="51b0f-113">JSON representation</span></span>

<span data-ttu-id="51b0f-114">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="51b0f-114">The following is a JSON representation of the resource.</span></span>

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