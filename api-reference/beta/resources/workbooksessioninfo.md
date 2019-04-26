---
title: workbookSessionInfo リソース型
description: ブック セッションについての情報を提供します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 3035574b92dfa703b926a81163efbb7f6eff764b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345782"
---
# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="35b80-103">workbookSessionInfo リソース型</span><span class="sxs-lookup"><span data-stu-id="35b80-103">workbookSessionInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35b80-104">ブック セッションについての情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="35b80-104">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="35b80-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="35b80-105">JSON representation</span></span>

<span data-ttu-id="35b80-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="35b80-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="35b80-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="35b80-107">Properties</span></span>

| <span data-ttu-id="35b80-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="35b80-108">Property</span></span> | <span data-ttu-id="35b80-109">型</span><span class="sxs-lookup"><span data-stu-id="35b80-109">Type</span></span>  | <span data-ttu-id="35b80-110">説明</span><span class="sxs-lookup"><span data-stu-id="35b80-110">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="35b80-111">id</span><span class="sxs-lookup"><span data-stu-id="35b80-111">id</span></span>  | <span data-ttu-id="35b80-112">string</span><span class="sxs-lookup"><span data-stu-id="35b80-112">string</span></span> | <span data-ttu-id="35b80-113">ブック セッションの ID。</span><span class="sxs-lookup"><span data-stu-id="35b80-113">Id of the workbook session.</span></span> |
| <span data-ttu-id="35b80-114">persistChanges</span><span class="sxs-lookup"><span data-stu-id="35b80-114">persistChanges</span></span> | <span data-ttu-id="35b80-115">string</span><span class="sxs-lookup"><span data-stu-id="35b80-115">string</span></span> |  <span data-ttu-id="35b80-116">`true`: 永続セッションの場合。</span><span class="sxs-lookup"><span data-stu-id="35b80-116">`true` for persistent session.</span></span> <span data-ttu-id="35b80-117">`false`: 非永続セッション (表示モード) の場合。</span><span class="sxs-lookup"><span data-stu-id="35b80-117">`false` for non-persistent session (view mode)</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "workbookSessionInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
