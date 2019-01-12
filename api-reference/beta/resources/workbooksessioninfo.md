---
title: workbookSessionInfo リソース型
description: ブック セッションについての情報を提供します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: a2975fdf58d0f1d3a72f1f76853125d0a98bb485
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962451"
---
# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="4cb4b-103">workbookSessionInfo リソース型</span><span class="sxs-lookup"><span data-stu-id="4cb4b-103">workbookSessionInfo resource type</span></span>

<span data-ttu-id="4cb4b-104">ブック セッションについての情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="4cb4b-104">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="4cb4b-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4cb4b-105">JSON representation</span></span>

<span data-ttu-id="4cb4b-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="4cb4b-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="4cb4b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4cb4b-107">Properties</span></span>

| <span data-ttu-id="4cb4b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4cb4b-108">Property</span></span> | <span data-ttu-id="4cb4b-109">種類</span><span class="sxs-lookup"><span data-stu-id="4cb4b-109">Type</span></span>  | <span data-ttu-id="4cb4b-110">説明</span><span class="sxs-lookup"><span data-stu-id="4cb4b-110">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="4cb4b-111">ID</span><span class="sxs-lookup"><span data-stu-id="4cb4b-111">id</span></span>  | <span data-ttu-id="4cb4b-112">文字列</span><span class="sxs-lookup"><span data-stu-id="4cb4b-112">string</span></span> | <span data-ttu-id="4cb4b-113">ブック セッションの ID。</span><span class="sxs-lookup"><span data-stu-id="4cb4b-113">Id of the workbook session.</span></span> |
| <span data-ttu-id="4cb4b-114">persistChanges</span><span class="sxs-lookup"><span data-stu-id="4cb4b-114">persistChanges</span></span> | <span data-ttu-id="4cb4b-115">文字列</span><span class="sxs-lookup"><span data-stu-id="4cb4b-115">string</span></span> |  <span data-ttu-id="4cb4b-116">`true`: 永続セッションの場合。</span><span class="sxs-lookup"><span data-stu-id="4cb4b-116">`true` for persistent session.</span></span> <span data-ttu-id="4cb4b-117">`false`: 非永続セッション (表示モード) の場合。</span><span class="sxs-lookup"><span data-stu-id="4cb4b-117">`false` for non-persistent session (view mode)</span></span> |

