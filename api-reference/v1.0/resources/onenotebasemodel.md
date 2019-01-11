---
title: onenoteEntityBaseModel リソース
description: これは、OneNote のエンティティの基本型です。
author: Jewan-microsoft
localization_priority: Normal
ms.openlocfilehash: 0c6a3d4916bf54eeec5856f51af87fa79e1f6e6c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821232"
---
# <a name="onenoteentitybasemodel-resource"></a><span data-ttu-id="05976-103">onenoteEntityBaseModel リソース</span><span class="sxs-lookup"><span data-stu-id="05976-103">onenoteEntityBaseModel resource</span></span>

<span data-ttu-id="05976-104">これは、OneNote のエンティティの基本型です。</span><span class="sxs-lookup"><span data-stu-id="05976-104">This is the base type for OneNote entities.</span></span>

## <a name="json-representation"></a><span data-ttu-id="05976-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="05976-105">JSON representation</span></span>

<span data-ttu-id="05976-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="05976-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="05976-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="05976-107">Properties</span></span>
| <span data-ttu-id="05976-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="05976-108">Property</span></span>     | <span data-ttu-id="05976-109">種類</span><span class="sxs-lookup"><span data-stu-id="05976-109">Type</span></span>   |<span data-ttu-id="05976-110">説明</span><span class="sxs-lookup"><span data-stu-id="05976-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="05976-111">self</span><span class="sxs-lookup"><span data-stu-id="05976-111">self</span></span>|<span data-ttu-id="05976-112">String</span><span class="sxs-lookup"><span data-stu-id="05976-112">String</span></span>|<span data-ttu-id="05976-p101">ページに関する詳細情報を入手できるエンドポイント。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="05976-p101">The endpoint where you can get details about the page. Read-only.</span></span>|

<!-- uuid: bfb567de-2a2a-4b81-bf47-a55626a0c166
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
