---
title: operationError リソースの種類
description: TeamsAsyncOperation で発生したエラーをについて説明します。
localization_priority: Normal
ms.openlocfilehash: 22590d7d955cf01385292d2796ad960b1c0ced41
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824585"
---
# <a name="operationerror-resource-type"></a><span data-ttu-id="8d0a7-103">operationError リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8d0a7-103">operationError resource type</span></span>



<span data-ttu-id="8d0a7-104">[TeamsAsyncOperation](teamsasyncoperation.md)で発生したエラーをについて説明します。</span><span class="sxs-lookup"><span data-stu-id="8d0a7-104">Describes errors in [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="operationerror-properties"></a><span data-ttu-id="8d0a7-105">operationError プロパティ</span><span class="sxs-lookup"><span data-stu-id="8d0a7-105">operationError Properties</span></span>
| <span data-ttu-id="8d0a7-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8d0a7-106">Property</span></span>     | <span data-ttu-id="8d0a7-107">種類</span><span class="sxs-lookup"><span data-stu-id="8d0a7-107">Type</span></span>   |<span data-ttu-id="8d0a7-108">説明</span><span class="sxs-lookup"><span data-stu-id="8d0a7-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8d0a7-109">code</span><span class="sxs-lookup"><span data-stu-id="8d0a7-109">code</span></span>|<span data-ttu-id="8d0a7-110">文字列 (読み取り専用)</span><span class="sxs-lookup"><span data-stu-id="8d0a7-110">string (readonly)</span></span>|<span data-ttu-id="8d0a7-111">操作のエラー コードです。</span><span class="sxs-lookup"><span data-stu-id="8d0a7-111">Operation error code.</span></span>|
|<span data-ttu-id="8d0a7-112">message</span><span class="sxs-lookup"><span data-stu-id="8d0a7-112">message</span></span>|<span data-ttu-id="8d0a7-113">文字列 (読み取り専用)</span><span class="sxs-lookup"><span data-stu-id="8d0a7-113">string (readonly)</span></span>|<span data-ttu-id="8d0a7-114">エラー メッセージを操作します。</span><span class="sxs-lookup"><span data-stu-id="8d0a7-114">Operation error message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8d0a7-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8d0a7-115">JSON representation</span></span>

<span data-ttu-id="8d0a7-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8d0a7-116">The following is a JSON representation of the resource.</span></span>

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
