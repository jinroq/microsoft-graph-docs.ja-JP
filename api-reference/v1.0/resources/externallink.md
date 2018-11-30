---
title: externalLink リソースの種類
description: OneNote のページまたはノートブックを開く URL です。
ms.openlocfilehash: ae25c6220545ff55259a18b6180225cc602e129b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021064"
---
# <a name="externallink-resource-type"></a><span data-ttu-id="ad39e-103">externalLink リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ad39e-103">externalLink resource type</span></span>

<span data-ttu-id="ad39e-104">OneNote のページまたはノートブックを開く URL です。</span><span class="sxs-lookup"><span data-stu-id="ad39e-104">A url that opens a OneNote page or notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ad39e-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ad39e-105">JSON representation</span></span>

<span data-ttu-id="ad39e-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="ad39e-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="ad39e-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ad39e-107">Properties</span></span>
| <span data-ttu-id="ad39e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ad39e-108">Property</span></span>     | <span data-ttu-id="ad39e-109">型</span><span class="sxs-lookup"><span data-stu-id="ad39e-109">Type</span></span>   |<span data-ttu-id="ad39e-110">説明</span><span class="sxs-lookup"><span data-stu-id="ad39e-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ad39e-111">href</span><span class="sxs-lookup"><span data-stu-id="ad39e-111">href</span></span>|<span data-ttu-id="ad39e-112">String</span><span class="sxs-lookup"><span data-stu-id="ad39e-112">String</span></span>|<span data-ttu-id="ad39e-113">そのリンクの URL です。</span><span class="sxs-lookup"><span data-stu-id="ad39e-113">The url of the link.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "externalLink resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->