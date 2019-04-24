---
title: workbookSessionInfo リソース型
description: ブック セッションについての情報を提供します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: a2975fdf58d0f1d3a72f1f76853125d0a98bb485
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32453284"
---
# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="22661-103">workbookSessionInfo リソース型</span><span class="sxs-lookup"><span data-stu-id="22661-103">workbookSessionInfo resource type</span></span>

<span data-ttu-id="22661-104">ブック セッションについての情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="22661-104">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="22661-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="22661-105">JSON representation</span></span>

<span data-ttu-id="22661-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="22661-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="22661-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="22661-107">Properties</span></span>

| <span data-ttu-id="22661-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="22661-108">Property</span></span> | <span data-ttu-id="22661-109">型</span><span class="sxs-lookup"><span data-stu-id="22661-109">Type</span></span>  | <span data-ttu-id="22661-110">説明</span><span class="sxs-lookup"><span data-stu-id="22661-110">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="22661-111">id</span><span class="sxs-lookup"><span data-stu-id="22661-111">id</span></span>  | <span data-ttu-id="22661-112">string</span><span class="sxs-lookup"><span data-stu-id="22661-112">string</span></span> | <span data-ttu-id="22661-113">ブック セッションの ID。</span><span class="sxs-lookup"><span data-stu-id="22661-113">Id of the workbook session.</span></span> |
| <span data-ttu-id="22661-114">persistChanges</span><span class="sxs-lookup"><span data-stu-id="22661-114">persistChanges</span></span> | <span data-ttu-id="22661-115">string</span><span class="sxs-lookup"><span data-stu-id="22661-115">string</span></span> |  <span data-ttu-id="22661-116">`true`: 永続セッションの場合。</span><span class="sxs-lookup"><span data-stu-id="22661-116">`true` for persistent session.</span></span> <span data-ttu-id="22661-117">`false`: 非永続セッション (表示モード) の場合。</span><span class="sxs-lookup"><span data-stu-id="22661-117">`false` for non-persistent session (view mode)</span></span> |

