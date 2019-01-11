---
title: workbookSessionInfo リソース型
description: ブック セッションについての情報を提供します。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 25812d48626c7dc5e468915f7308941a4f74b38e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860964"
---
# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="e534d-103">workbookSessionInfo リソース型</span><span class="sxs-lookup"><span data-stu-id="e534d-103">workbookSessionInfo resource type</span></span>

<span data-ttu-id="e534d-104">ブック セッションについての情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="e534d-104">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="e534d-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e534d-105">JSON representation</span></span>

<span data-ttu-id="e534d-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="e534d-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="e534d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e534d-107">Properties</span></span>

| <span data-ttu-id="e534d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e534d-108">Property</span></span> | <span data-ttu-id="e534d-109">種類</span><span class="sxs-lookup"><span data-stu-id="e534d-109">Type</span></span>  | <span data-ttu-id="e534d-110">説明</span><span class="sxs-lookup"><span data-stu-id="e534d-110">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="e534d-111">ID</span><span class="sxs-lookup"><span data-stu-id="e534d-111">id</span></span>  | <span data-ttu-id="e534d-112">文字列</span><span class="sxs-lookup"><span data-stu-id="e534d-112">string</span></span> | <span data-ttu-id="e534d-113">ブック セッションの ID。</span><span class="sxs-lookup"><span data-stu-id="e534d-113">Id of the workbook session.</span></span> |
| <span data-ttu-id="e534d-114">persistChanges</span><span class="sxs-lookup"><span data-stu-id="e534d-114">persistChanges</span></span> | <span data-ttu-id="e534d-115">文字列</span><span class="sxs-lookup"><span data-stu-id="e534d-115">string</span></span> |  <span data-ttu-id="e534d-116">`true`: 永続セッションの場合。</span><span class="sxs-lookup"><span data-stu-id="e534d-116">`true` for persistent session.</span></span> <span data-ttu-id="e534d-117">`false`: 非永続セッション (表示モード) の場合。</span><span class="sxs-lookup"><span data-stu-id="e534d-117">`false` for non-persistent session (view mode)</span></span> |

