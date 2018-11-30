---
title: workbookSessionInfo リソース型
description: ブック セッションについての情報を提供します。
ms.openlocfilehash: 84d0306a7a25aaa29e4f1eb9b87708cc97d6b50f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022096"
---
# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="12a72-103">workbookSessionInfo リソース型</span><span class="sxs-lookup"><span data-stu-id="12a72-103">workbookSessionInfo resource type</span></span>

<span data-ttu-id="12a72-104">ブック セッションについての情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="12a72-104">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="12a72-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="12a72-105">JSON representation</span></span>

<span data-ttu-id="12a72-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="12a72-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="12a72-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="12a72-107">Properties</span></span>

| <span data-ttu-id="12a72-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="12a72-108">Property</span></span> | <span data-ttu-id="12a72-109">型</span><span class="sxs-lookup"><span data-stu-id="12a72-109">Type</span></span>  | <span data-ttu-id="12a72-110">説明</span><span class="sxs-lookup"><span data-stu-id="12a72-110">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="12a72-111">ID</span><span class="sxs-lookup"><span data-stu-id="12a72-111">id</span></span>  | <span data-ttu-id="12a72-112">文字列</span><span class="sxs-lookup"><span data-stu-id="12a72-112">string</span></span> | <span data-ttu-id="12a72-113">ブック セッションの ID。</span><span class="sxs-lookup"><span data-stu-id="12a72-113">Id of the workbook session.</span></span> |
| <span data-ttu-id="12a72-114">persistChanges</span><span class="sxs-lookup"><span data-stu-id="12a72-114">persistChanges</span></span> | <span data-ttu-id="12a72-115">ブール</span><span class="sxs-lookup"><span data-stu-id="12a72-115">boolean</span></span> |  <span data-ttu-id="12a72-116">`true`: 永続セッションの場合。</span><span class="sxs-lookup"><span data-stu-id="12a72-116">`true` for persistent session.</span></span> <span data-ttu-id="12a72-117">`false`: 非永続セッション (表示モード) の場合。</span><span class="sxs-lookup"><span data-stu-id="12a72-117">`false` for non-persistent session (view mode)</span></span> |

