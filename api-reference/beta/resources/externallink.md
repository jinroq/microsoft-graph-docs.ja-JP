---
title: externalLink リソースの種類
description: OneNote のページまたはノートブックを開く URL です。
localization_priority: Normal
ms.openlocfilehash: ce832d5bd661408a55fdcde24f03b3955880a1ba
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828246"
---
# <a name="externallink-resource-type"></a><span data-ttu-id="3140f-103">externalLink リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3140f-103">externalLink resource type</span></span>

> <span data-ttu-id="3140f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3140f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3140f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3140f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3140f-106">OneNote のページまたはノートブックを開く URL です。</span><span class="sxs-lookup"><span data-stu-id="3140f-106">A url that opens a OneNote page or notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3140f-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3140f-107">JSON representation</span></span>

<span data-ttu-id="3140f-108">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="3140f-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="3140f-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3140f-109">Properties</span></span>
| <span data-ttu-id="3140f-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3140f-110">Property</span></span>     | <span data-ttu-id="3140f-111">種類</span><span class="sxs-lookup"><span data-stu-id="3140f-111">Type</span></span>   |<span data-ttu-id="3140f-112">説明</span><span class="sxs-lookup"><span data-stu-id="3140f-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3140f-113">href</span><span class="sxs-lookup"><span data-stu-id="3140f-113">href</span></span>|<span data-ttu-id="3140f-114">String</span><span class="sxs-lookup"><span data-stu-id="3140f-114">String</span></span>|<span data-ttu-id="3140f-115">そのリンクの URL です。</span><span class="sxs-lookup"><span data-stu-id="3140f-115">The url of the link.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "externalLink resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
