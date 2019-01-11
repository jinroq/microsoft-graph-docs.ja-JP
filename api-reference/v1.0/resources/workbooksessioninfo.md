---
title: workbookSessionInfo リソース型
description: ブック セッションについての情報を提供します。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 900ebdcefbdfa83e7b72b1c926a441f1c497626a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826930"
---
# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="cf5af-103">workbookSessionInfo リソース型</span><span class="sxs-lookup"><span data-stu-id="cf5af-103">workbookSessionInfo resource type</span></span>

<span data-ttu-id="cf5af-104">ブック セッションについての情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="cf5af-104">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="cf5af-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cf5af-105">JSON representation</span></span>

<span data-ttu-id="cf5af-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="cf5af-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="cf5af-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cf5af-107">Properties</span></span>

| <span data-ttu-id="cf5af-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cf5af-108">Property</span></span> | <span data-ttu-id="cf5af-109">種類</span><span class="sxs-lookup"><span data-stu-id="cf5af-109">Type</span></span>  | <span data-ttu-id="cf5af-110">説明</span><span class="sxs-lookup"><span data-stu-id="cf5af-110">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="cf5af-111">ID</span><span class="sxs-lookup"><span data-stu-id="cf5af-111">id</span></span>  | <span data-ttu-id="cf5af-112">文字列</span><span class="sxs-lookup"><span data-stu-id="cf5af-112">string</span></span> | <span data-ttu-id="cf5af-113">ブック セッションの ID。</span><span class="sxs-lookup"><span data-stu-id="cf5af-113">Id of the workbook session.</span></span> |
| <span data-ttu-id="cf5af-114">persistChanges</span><span class="sxs-lookup"><span data-stu-id="cf5af-114">persistChanges</span></span> | <span data-ttu-id="cf5af-115">ブール</span><span class="sxs-lookup"><span data-stu-id="cf5af-115">boolean</span></span> |  <span data-ttu-id="cf5af-116">`true`: 永続セッションの場合。</span><span class="sxs-lookup"><span data-stu-id="cf5af-116">`true` for persistent session.</span></span> <span data-ttu-id="cf5af-117">`false`: 非永続セッション (表示モード) の場合。</span><span class="sxs-lookup"><span data-stu-id="cf5af-117">`false` for non-persistent session (view mode)</span></span> |

