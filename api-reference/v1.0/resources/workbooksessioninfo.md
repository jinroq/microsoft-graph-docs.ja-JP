---
title: workbookSessionInfo リソース型
description: ブック セッションについての情報を提供します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: f2e6b925e7cc1790b1c6d4f08bab02fa92f19936
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033335"
---
# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="2b882-103">workbookSessionInfo リソース型</span><span class="sxs-lookup"><span data-stu-id="2b882-103">workbookSessionInfo resource type</span></span>

<span data-ttu-id="2b882-104">ブック セッションについての情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="2b882-104">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="2b882-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2b882-105">JSON representation</span></span>

<span data-ttu-id="2b882-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="2b882-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="2b882-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2b882-107">Properties</span></span>

| <span data-ttu-id="2b882-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2b882-108">Property</span></span> | <span data-ttu-id="2b882-109">型</span><span class="sxs-lookup"><span data-stu-id="2b882-109">Type</span></span>  | <span data-ttu-id="2b882-110">説明</span><span class="sxs-lookup"><span data-stu-id="2b882-110">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="2b882-111">id</span><span class="sxs-lookup"><span data-stu-id="2b882-111">id</span></span>  | <span data-ttu-id="2b882-112">string</span><span class="sxs-lookup"><span data-stu-id="2b882-112">string</span></span> | <span data-ttu-id="2b882-113">ブック セッションの ID。</span><span class="sxs-lookup"><span data-stu-id="2b882-113">Id of the workbook session.</span></span> |
| <span data-ttu-id="2b882-114">persistChanges</span><span class="sxs-lookup"><span data-stu-id="2b882-114">persistChanges</span></span> | <span data-ttu-id="2b882-115">ブール値</span><span class="sxs-lookup"><span data-stu-id="2b882-115">boolean</span></span> |  <span data-ttu-id="2b882-116">`true`: 永続セッションの場合。</span><span class="sxs-lookup"><span data-stu-id="2b882-116">`true` for persistent session.</span></span> <span data-ttu-id="2b882-117">`false`: 非永続セッション (表示モード) の場合。</span><span class="sxs-lookup"><span data-stu-id="2b882-117">`false` for non-persistent session (view mode)</span></span> |

