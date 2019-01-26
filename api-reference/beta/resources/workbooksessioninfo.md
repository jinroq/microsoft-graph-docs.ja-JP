---
title: workbookSessionInfo リソース型
description: ブック セッションについての情報を提供します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 502781c4049c9451f5ed67ff97222abf4df462d7
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575619"
---
# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="1e5f3-103">workbookSessionInfo リソース型</span><span class="sxs-lookup"><span data-stu-id="1e5f3-103">workbookSessionInfo resource type</span></span>

<span data-ttu-id="1e5f3-104">ブック セッションについての情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="1e5f3-104">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="1e5f3-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1e5f3-105">JSON representation</span></span>

<span data-ttu-id="1e5f3-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="1e5f3-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="1e5f3-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1e5f3-107">Properties</span></span>

| <span data-ttu-id="1e5f3-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1e5f3-108">Property</span></span> | <span data-ttu-id="1e5f3-109">型</span><span class="sxs-lookup"><span data-stu-id="1e5f3-109">Type</span></span>  | <span data-ttu-id="1e5f3-110">説明</span><span class="sxs-lookup"><span data-stu-id="1e5f3-110">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="1e5f3-111">id</span><span class="sxs-lookup"><span data-stu-id="1e5f3-111">id</span></span>  | <span data-ttu-id="1e5f3-112">文字列</span><span class="sxs-lookup"><span data-stu-id="1e5f3-112">string</span></span> | <span data-ttu-id="1e5f3-113">ブック セッションの ID。</span><span class="sxs-lookup"><span data-stu-id="1e5f3-113">Id of the workbook session.</span></span> |
| <span data-ttu-id="1e5f3-114">persistChanges</span><span class="sxs-lookup"><span data-stu-id="1e5f3-114">persistChanges</span></span> | <span data-ttu-id="1e5f3-115">boolean</span><span class="sxs-lookup"><span data-stu-id="1e5f3-115">boolean</span></span> |  <span data-ttu-id="1e5f3-116">`true`: 永続セッションの場合。</span><span class="sxs-lookup"><span data-stu-id="1e5f3-116">`true` for persistent session.</span></span> <span data-ttu-id="1e5f3-117">`false`: 非永続セッション (表示モード) の場合。</span><span class="sxs-lookup"><span data-stu-id="1e5f3-117">`false` for non-persistent session (view mode)</span></span> |

