---
title: mentionsPreview リソースの種類
description: リソースインスタンス内のメンションオブジェクトに関する情報を表します。
localization_priority: Normal
author: simonhult
ms.prod: insights
ms.openlocfilehash: 55eb69d9ef9f6c3686026f6d46a9c78cc4df167b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523486"
---
# <a name="mentionspreview-resource-type"></a><span data-ttu-id="4bd13-103">mentionsPreview リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4bd13-103">mentionsPreview resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4bd13-104">リソースインスタンス内の[メンション](../resources/mention.md)オブジェクトに関する情報を表します。</span><span class="sxs-lookup"><span data-stu-id="4bd13-104">Represents information about [mention](../resources/mention.md) objects in a resource instance.</span></span>

## <a name="properties"></a><span data-ttu-id="4bd13-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4bd13-105">Properties</span></span>
| <span data-ttu-id="4bd13-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4bd13-106">Property</span></span>     | <span data-ttu-id="4bd13-107">型</span><span class="sxs-lookup"><span data-stu-id="4bd13-107">Type</span></span>   |<span data-ttu-id="4bd13-108">説明</span><span class="sxs-lookup"><span data-stu-id="4bd13-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4bd13-109">説明</span><span class="sxs-lookup"><span data-stu-id="4bd13-109">isMentioned</span></span> | <span data-ttu-id="4bd13-110">ブール型</span><span class="sxs-lookup"><span data-stu-id="4bd13-110">Boolean</span></span> | <span data-ttu-id="4bd13-111">True の場合は、サインインしているユーザーが親リソースインスタンスで言及されます。</span><span class="sxs-lookup"><span data-stu-id="4bd13-111">True if the signed-in user is mentioned in the parent resource instance.</span></span> <span data-ttu-id="4bd13-112">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4bd13-112">Read-only.</span></span> <span data-ttu-id="4bd13-113">フィルターをサポートします。</span><span class="sxs-lookup"><span data-stu-id="4bd13-113">Supports filter.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4bd13-114">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4bd13-114">JSON representation</span></span>

<span data-ttu-id="4bd13-115">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4bd13-115">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mentionsPreview"
}-->

```json
{
  "isMentioned": "Boolean"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mentionsPreview resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/mentionspreview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
