---
title: workbookSessionInfo リソース型
description: ブック セッションについての情報を提供します。
ms.openlocfilehash: c04afe17c10edd8b136465d6d7ae3dbedb6307ed
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069828"
---
# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="03916-103">workbookSessionInfo リソース型</span><span class="sxs-lookup"><span data-stu-id="03916-103">workbookSessionInfo resource type</span></span>

<span data-ttu-id="03916-104">ブック セッションについての情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="03916-104">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="03916-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="03916-105">JSON representation</span></span>

<span data-ttu-id="03916-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="03916-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="03916-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="03916-107">Properties</span></span>

| <span data-ttu-id="03916-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="03916-108">Property</span></span> | <span data-ttu-id="03916-109">型</span><span class="sxs-lookup"><span data-stu-id="03916-109">Type</span></span>  | <span data-ttu-id="03916-110">説明</span><span class="sxs-lookup"><span data-stu-id="03916-110">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="03916-111">ID</span><span class="sxs-lookup"><span data-stu-id="03916-111">id</span></span>  | <span data-ttu-id="03916-112">文字列</span><span class="sxs-lookup"><span data-stu-id="03916-112">string</span></span> | <span data-ttu-id="03916-113">ブック セッションの ID。</span><span class="sxs-lookup"><span data-stu-id="03916-113">Id of the workbook session.</span></span> |
| <span data-ttu-id="03916-114">persistChanges</span><span class="sxs-lookup"><span data-stu-id="03916-114">persistChanges</span></span> | <span data-ttu-id="03916-115">文字列</span><span class="sxs-lookup"><span data-stu-id="03916-115">string</span></span> |  <span data-ttu-id="03916-116">`true`: 永続セッションの場合。</span><span class="sxs-lookup"><span data-stu-id="03916-116">`true` for persistent session.</span></span> <span data-ttu-id="03916-117">`false`: 非永続セッション (表示モード) の場合。</span><span class="sxs-lookup"><span data-stu-id="03916-117">`false` for non-persistent session (view mode)</span></span> |

