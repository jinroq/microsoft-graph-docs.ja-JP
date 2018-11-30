---
title: onenoteEntityBaseModel リソース
description: これは、OneNote のエンティティの基本型です。
ms.openlocfilehash: 68a864437cec59d9b5f0d3e69161b49bca80231c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021744"
---
# <a name="onenoteentitybasemodel-resource"></a><span data-ttu-id="e20ae-103">onenoteEntityBaseModel リソース</span><span class="sxs-lookup"><span data-stu-id="e20ae-103">onenoteEntityBaseModel resource</span></span>

<span data-ttu-id="e20ae-104">これは、OneNote のエンティティの基本型です。</span><span class="sxs-lookup"><span data-stu-id="e20ae-104">This is the base type for OneNote entities.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e20ae-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e20ae-105">JSON representation</span></span>

<span data-ttu-id="e20ae-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e20ae-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [
    "self"
  ],
  "@odata.type": "microsoft.graph.onenoteEntityBaseModel"
}-->

```json
{
  "self": "string"
}

```
## <a name="properties"></a><span data-ttu-id="e20ae-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e20ae-107">Properties</span></span>
| <span data-ttu-id="e20ae-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e20ae-108">Property</span></span>     | <span data-ttu-id="e20ae-109">型</span><span class="sxs-lookup"><span data-stu-id="e20ae-109">Type</span></span>   |<span data-ttu-id="e20ae-110">説明</span><span class="sxs-lookup"><span data-stu-id="e20ae-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e20ae-111">self</span><span class="sxs-lookup"><span data-stu-id="e20ae-111">self</span></span>|<span data-ttu-id="e20ae-112">String</span><span class="sxs-lookup"><span data-stu-id="e20ae-112">String</span></span>|<span data-ttu-id="e20ae-p101">ページに関する詳細情報を入手できるエンドポイント。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="e20ae-p101">The endpoint where you can get details about the page. Read-only.</span></span>|

<!-- uuid: bfb567de-2a2a-4b81-bf47-a55626a0c166
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->