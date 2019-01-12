---
title: onenoteEntityBaseModel リソース
description: これは、OneNote のエンティティの基本型です。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 53ed86ae22f3ac9fccdef98e56382cd9440e71e2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923132"
---
# <a name="onenoteentitybasemodel-resource"></a><span data-ttu-id="0941d-103">onenoteEntityBaseModel リソース</span><span class="sxs-lookup"><span data-stu-id="0941d-103">onenoteEntityBaseModel resource</span></span>

<span data-ttu-id="0941d-104">これは、OneNote のエンティティの基本型です。</span><span class="sxs-lookup"><span data-stu-id="0941d-104">This is the base type for OneNote entities.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0941d-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0941d-105">JSON representation</span></span>

<span data-ttu-id="0941d-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0941d-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="0941d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0941d-107">Properties</span></span>
| <span data-ttu-id="0941d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0941d-108">Property</span></span>     | <span data-ttu-id="0941d-109">種類</span><span class="sxs-lookup"><span data-stu-id="0941d-109">Type</span></span>   |<span data-ttu-id="0941d-110">説明</span><span class="sxs-lookup"><span data-stu-id="0941d-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0941d-111">self</span><span class="sxs-lookup"><span data-stu-id="0941d-111">self</span></span>|<span data-ttu-id="0941d-112">String</span><span class="sxs-lookup"><span data-stu-id="0941d-112">String</span></span>|<span data-ttu-id="0941d-p101">ページに関する詳細情報を入手できるエンドポイント。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0941d-p101">The endpoint where you can get details about the page. Read-only.</span></span>|

<!-- uuid: bfb567de-2a2a-4b81-bf47-a55626a0c166
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
