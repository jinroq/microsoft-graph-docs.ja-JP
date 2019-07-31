---
title: externalLink リソースの種類
description: OneNote のページまたはノートブックを開く url。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 3f1eaa45ce335dace0d4f0ff715481fca0518bf3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973573"
---
# <a name="externallink-resource-type"></a><span data-ttu-id="9a50b-103">externalLink リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9a50b-103">externalLink resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a50b-104">OneNote のページまたはノートブックを開く url。</span><span class="sxs-lookup"><span data-stu-id="9a50b-104">A url that opens a OneNote page or notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9a50b-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9a50b-105">JSON representation</span></span>

<span data-ttu-id="9a50b-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="9a50b-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="9a50b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9a50b-107">Properties</span></span>
| <span data-ttu-id="9a50b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9a50b-108">Property</span></span>     | <span data-ttu-id="9a50b-109">型</span><span class="sxs-lookup"><span data-stu-id="9a50b-109">Type</span></span>   |<span data-ttu-id="9a50b-110">説明</span><span class="sxs-lookup"><span data-stu-id="9a50b-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9a50b-111">href</span><span class="sxs-lookup"><span data-stu-id="9a50b-111">href</span></span>|<span data-ttu-id="9a50b-112">String</span><span class="sxs-lookup"><span data-stu-id="9a50b-112">String</span></span>|<span data-ttu-id="9a50b-113">リンクの url。</span><span class="sxs-lookup"><span data-stu-id="9a50b-113">The url of the link.</span></span>|

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
