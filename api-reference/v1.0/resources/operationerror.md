---
title: operationError リソースの種類
description: TeamsAsyncOperation のエラーについて説明します。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 8a46943fad974c2e7a12041e9def6a8a6ad6c9a3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035715"
---
# <a name="operationerror-resource-type"></a><span data-ttu-id="47b13-103">operationError リソースの種類</span><span class="sxs-lookup"><span data-stu-id="47b13-103">operationError resource type</span></span>



<span data-ttu-id="47b13-104">[TeamsAsyncOperation](teamsasyncoperation.md)のエラーについて説明します。</span><span class="sxs-lookup"><span data-stu-id="47b13-104">Describes errors in [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="operationerror-properties"></a><span data-ttu-id="47b13-105">operationError プロパティ</span><span class="sxs-lookup"><span data-stu-id="47b13-105">operationError Properties</span></span>
| <span data-ttu-id="47b13-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="47b13-106">Property</span></span>     | <span data-ttu-id="47b13-107">型</span><span class="sxs-lookup"><span data-stu-id="47b13-107">Type</span></span>   |<span data-ttu-id="47b13-108">説明</span><span class="sxs-lookup"><span data-stu-id="47b13-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="47b13-109">code</span><span class="sxs-lookup"><span data-stu-id="47b13-109">code</span></span>|<span data-ttu-id="47b13-110">string (読み取り専用)</span><span class="sxs-lookup"><span data-stu-id="47b13-110">string (readonly)</span></span>|<span data-ttu-id="47b13-111">操作エラーコード。</span><span class="sxs-lookup"><span data-stu-id="47b13-111">Operation error code.</span></span>|
|<span data-ttu-id="47b13-112">message</span><span class="sxs-lookup"><span data-stu-id="47b13-112">message</span></span>|<span data-ttu-id="47b13-113">string (読み取り専用)</span><span class="sxs-lookup"><span data-stu-id="47b13-113">string (readonly)</span></span>|<span data-ttu-id="47b13-114">操作エラーメッセージ。</span><span class="sxs-lookup"><span data-stu-id="47b13-114">Operation error message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="47b13-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="47b13-115">JSON representation</span></span>

<span data-ttu-id="47b13-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="47b13-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.operationError"
}-->

```json
{
    "code": "TeamUnavailable",
    "message": "The team was not found."
}
```

<!-- uuid: 069fadaa-52db-4ced-85d5-74f7caa2c66f
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "operation error resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
