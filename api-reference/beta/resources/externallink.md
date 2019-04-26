---
title: externallink リソースの種類
description: OneNote のページまたはノートブックを開く url。
localization_priority: Normal
ms.openlocfilehash: d5658382585f5c7f7c5a9fe457e17976979091c6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333939"
---
# <a name="externallink-resource-type"></a><span data-ttu-id="e46f3-103">externallink リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e46f3-103">externalLink resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e46f3-104">OneNote のページまたはノートブックを開く url。</span><span class="sxs-lookup"><span data-stu-id="e46f3-104">A url that opens a OneNote page or notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e46f3-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e46f3-105">JSON representation</span></span>

<span data-ttu-id="e46f3-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="e46f3-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalLink"
}-->

```json
{
  "href": "string"
}

```
## <a name="properties"></a><span data-ttu-id="e46f3-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e46f3-107">Properties</span></span>
| <span data-ttu-id="e46f3-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e46f3-108">Property</span></span>     | <span data-ttu-id="e46f3-109">型</span><span class="sxs-lookup"><span data-stu-id="e46f3-109">Type</span></span>   |<span data-ttu-id="e46f3-110">説明</span><span class="sxs-lookup"><span data-stu-id="e46f3-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e46f3-111">href</span><span class="sxs-lookup"><span data-stu-id="e46f3-111">href</span></span>|<span data-ttu-id="e46f3-112">String</span><span class="sxs-lookup"><span data-stu-id="e46f3-112">String</span></span>|<span data-ttu-id="e46f3-113">リンクの url。</span><span class="sxs-lookup"><span data-stu-id="e46f3-113">The url of the link.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "externalLink resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
