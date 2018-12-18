---
title: workbookSessionInfo リソース型
description: ブック セッションについての情報を提供します。
author: lumine2008
ms.openlocfilehash: 5a86fd4dfd653f16445eeccad8478db56db0ac5f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316843"
---
# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="bfda9-103">workbookSessionInfo リソース型</span><span class="sxs-lookup"><span data-stu-id="bfda9-103">workbookSessionInfo resource type</span></span>

<span data-ttu-id="bfda9-104">ブック セッションについての情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="bfda9-104">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="bfda9-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bfda9-105">JSON representation</span></span>

<span data-ttu-id="bfda9-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="bfda9-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="bfda9-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bfda9-107">Properties</span></span>

| <span data-ttu-id="bfda9-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bfda9-108">Property</span></span> | <span data-ttu-id="bfda9-109">種類</span><span class="sxs-lookup"><span data-stu-id="bfda9-109">Type</span></span>  | <span data-ttu-id="bfda9-110">説明</span><span class="sxs-lookup"><span data-stu-id="bfda9-110">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="bfda9-111">ID</span><span class="sxs-lookup"><span data-stu-id="bfda9-111">id</span></span>  | <span data-ttu-id="bfda9-112">string</span><span class="sxs-lookup"><span data-stu-id="bfda9-112">string</span></span> | <span data-ttu-id="bfda9-113">ブック セッションの ID。</span><span class="sxs-lookup"><span data-stu-id="bfda9-113">Id of the workbook session.</span></span> |
| <span data-ttu-id="bfda9-114">persistChanges</span><span class="sxs-lookup"><span data-stu-id="bfda9-114">persistChanges</span></span> | <span data-ttu-id="bfda9-115">string</span><span class="sxs-lookup"><span data-stu-id="bfda9-115">string</span></span> |  <span data-ttu-id="bfda9-116">`true`: 永続セッションの場合。</span><span class="sxs-lookup"><span data-stu-id="bfda9-116">`true` for persistent session.</span></span> <span data-ttu-id="bfda9-117">`false`: 非永続セッション (表示モード) の場合。</span><span class="sxs-lookup"><span data-stu-id="bfda9-117">`false` for non-persistent session (view mode)</span></span> |

