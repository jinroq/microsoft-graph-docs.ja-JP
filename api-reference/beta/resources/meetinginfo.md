---
title: 会議情報リソースの種類
description: 会議を作成または参加するために指定された会議情報。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: da3e89e0aa28868debd4b6ea98291fa88b42bb0b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966872"
---
# <a name="meetinginfo-resource-type"></a><span data-ttu-id="d63e1-103">会議情報リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d63e1-103">meetingInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d63e1-104">会議を作成または参加するために指定された会議情報。</span><span class="sxs-lookup"><span data-stu-id="d63e1-104">Meeting information specified to create or join a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="d63e1-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d63e1-105">Properties</span></span>

| <span data-ttu-id="d63e1-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d63e1-106">Property</span></span>       | <span data-ttu-id="d63e1-107">型</span><span class="sxs-lookup"><span data-stu-id="d63e1-107">Type</span></span>    | <span data-ttu-id="d63e1-108">説明</span><span class="sxs-lookup"><span data-stu-id="d63e1-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d63e1-109">allowConversationWithoutHost</span><span class="sxs-lookup"><span data-stu-id="d63e1-109">allowConversationWithoutHost</span></span> | <span data-ttu-id="d63e1-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="d63e1-110">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="d63e1-111">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d63e1-111">JSON representation</span></span>

<span data-ttu-id="d63e1-112">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d63e1-112">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "meetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
