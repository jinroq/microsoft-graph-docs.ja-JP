---
title: 会議情報リソースの種類
description: 会議を作成または参加するために指定された会議情報。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c1126a3408b8353e927b5653fe60dd4a89125051
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457138"
---
# <a name="meetinginfo-resource-type"></a><span data-ttu-id="a1083-103">会議情報リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a1083-103">meetingInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a1083-104">会議を作成または参加するために指定された会議情報。</span><span class="sxs-lookup"><span data-stu-id="a1083-104">Meeting information specified to create or join a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="a1083-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a1083-105">Properties</span></span>

| <span data-ttu-id="a1083-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a1083-106">Property</span></span>       | <span data-ttu-id="a1083-107">型</span><span class="sxs-lookup"><span data-stu-id="a1083-107">Type</span></span>    | <span data-ttu-id="a1083-108">説明</span><span class="sxs-lookup"><span data-stu-id="a1083-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a1083-109">allowConversationWithoutHost</span><span class="sxs-lookup"><span data-stu-id="a1083-109">allowConversationWithoutHost</span></span> | <span data-ttu-id="a1083-110">ブール型</span><span class="sxs-lookup"><span data-stu-id="a1083-110">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="a1083-111">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a1083-111">JSON representation</span></span>

<span data-ttu-id="a1083-112">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a1083-112">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/meetinginfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
