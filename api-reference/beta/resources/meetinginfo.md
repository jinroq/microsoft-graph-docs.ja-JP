---
title: meetingInfo リソースの種類
description: 会議の情報を作成または、ミーティングに参加するために指定します。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b3590227e55ee217c63110c8f90e1a1741eac81d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947919"
---
# <a name="meetinginfo-resource-type"></a><span data-ttu-id="4f53a-103">meetingInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4f53a-103">meetingInfo resource type</span></span>

> <span data-ttu-id="4f53a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4f53a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4f53a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4f53a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4f53a-106">会議の情報を作成または、ミーティングに参加するために指定します。</span><span class="sxs-lookup"><span data-stu-id="4f53a-106">Meeting information specified to create or join a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="4f53a-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4f53a-107">Properties</span></span>

| <span data-ttu-id="4f53a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4f53a-108">Property</span></span>       | <span data-ttu-id="4f53a-109">種類</span><span class="sxs-lookup"><span data-stu-id="4f53a-109">Type</span></span>    | <span data-ttu-id="4f53a-110">説明</span><span class="sxs-lookup"><span data-stu-id="4f53a-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4f53a-111">allowConversationWithoutHost</span><span class="sxs-lookup"><span data-stu-id="4f53a-111">allowConversationWithoutHost</span></span> | <span data-ttu-id="4f53a-112">ブール型</span><span class="sxs-lookup"><span data-stu-id="4f53a-112">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="4f53a-113">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4f53a-113">JSON representation</span></span>

<span data-ttu-id="4f53a-114">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4f53a-114">The following is a JSON representation of the resource.</span></span>

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
