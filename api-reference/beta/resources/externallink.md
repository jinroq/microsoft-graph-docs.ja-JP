---
title: externalLink リソースの種類
description: OneNote のページまたはノートブックを開く URL です。
ms.openlocfilehash: 8f0af6b3bfd327dff0d228ea181443d742332d0f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069896"
---
# <a name="externallink-resource-type"></a><span data-ttu-id="3d2bc-103">externalLink リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3d2bc-103">externalLink resource type</span></span>

> <span data-ttu-id="3d2bc-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3d2bc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3d2bc-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3d2bc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3d2bc-106">OneNote のページまたはノートブックを開く URL です。</span><span class="sxs-lookup"><span data-stu-id="3d2bc-106">A url that opens a OneNote page or notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3d2bc-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3d2bc-107">JSON representation</span></span>

<span data-ttu-id="3d2bc-108">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="3d2bc-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="3d2bc-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3d2bc-109">Properties</span></span>
| <span data-ttu-id="3d2bc-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3d2bc-110">Property</span></span>     | <span data-ttu-id="3d2bc-111">型</span><span class="sxs-lookup"><span data-stu-id="3d2bc-111">Type</span></span>   |<span data-ttu-id="3d2bc-112">説明</span><span class="sxs-lookup"><span data-stu-id="3d2bc-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3d2bc-113">href</span><span class="sxs-lookup"><span data-stu-id="3d2bc-113">href</span></span>|<span data-ttu-id="3d2bc-114">String</span><span class="sxs-lookup"><span data-stu-id="3d2bc-114">String</span></span>|<span data-ttu-id="3d2bc-115">そのリンクの URL です。</span><span class="sxs-lookup"><span data-stu-id="3d2bc-115">The url of the link.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "externalLink resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->