---
title: workbookSessionInfo リソース型
description: ブック セッションについての情報を提供します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: a2975fdf58d0f1d3a72f1f76853125d0a98bb485
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642220"
---
# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="db54f-103">workbookSessionInfo リソース型</span><span class="sxs-lookup"><span data-stu-id="db54f-103">workbookSessionInfo resource type</span></span>

<span data-ttu-id="db54f-104">ブック セッションについての情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="db54f-104">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="db54f-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="db54f-105">JSON representation</span></span>

<span data-ttu-id="db54f-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="db54f-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.workbookSessionInfo"
}-->

```json
{
  "id": "string",
  "persistChanges": true
}
```

## <a name="properties"></a><span data-ttu-id="db54f-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="db54f-107">Properties</span></span>

| <span data-ttu-id="db54f-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="db54f-108">Property</span></span> | <span data-ttu-id="db54f-109">型</span><span class="sxs-lookup"><span data-stu-id="db54f-109">Type</span></span>  | <span data-ttu-id="db54f-110">説明</span><span class="sxs-lookup"><span data-stu-id="db54f-110">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="db54f-111">id</span><span class="sxs-lookup"><span data-stu-id="db54f-111">id</span></span>  | <span data-ttu-id="db54f-112">string</span><span class="sxs-lookup"><span data-stu-id="db54f-112">string</span></span> | <span data-ttu-id="db54f-113">ブック セッションの ID。</span><span class="sxs-lookup"><span data-stu-id="db54f-113">Id of the workbook session.</span></span> |
| <span data-ttu-id="db54f-114">persistChanges</span><span class="sxs-lookup"><span data-stu-id="db54f-114">persistChanges</span></span> | <span data-ttu-id="db54f-115">string</span><span class="sxs-lookup"><span data-stu-id="db54f-115">string</span></span> |  <span data-ttu-id="db54f-116">`true`: 永続セッションの場合。</span><span class="sxs-lookup"><span data-stu-id="db54f-116">`true` for persistent session.</span></span> <span data-ttu-id="db54f-117">`false`: 非永続セッション (表示モード) の場合。</span><span class="sxs-lookup"><span data-stu-id="db54f-117">`false` for non-persistent session (view mode)</span></span> |

