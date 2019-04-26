---
title: operationerror リソースの種類
description: teamsAsyncOperation のエラーについて説明します。
localization_priority: Normal
ms.openlocfilehash: 957f1ed2960c33f2e7bc07f79e7f749a3b9f15a5
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341764"
---
# <a name="operationerror-resource-type"></a><span data-ttu-id="2b0ce-103">operationerror リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2b0ce-103">operationError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b0ce-104">[teamsAsyncOperation](teamsasyncoperation.md)のエラーについて説明します。</span><span class="sxs-lookup"><span data-stu-id="2b0ce-104">Describes errors in [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="operationerror-properties"></a><span data-ttu-id="2b0ce-105">operationerror プロパティ</span><span class="sxs-lookup"><span data-stu-id="2b0ce-105">operationError Properties</span></span>
| <span data-ttu-id="2b0ce-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2b0ce-106">Property</span></span>     | <span data-ttu-id="2b0ce-107">型</span><span class="sxs-lookup"><span data-stu-id="2b0ce-107">Type</span></span>   |<span data-ttu-id="2b0ce-108">説明</span><span class="sxs-lookup"><span data-stu-id="2b0ce-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2b0ce-109">code</span><span class="sxs-lookup"><span data-stu-id="2b0ce-109">code</span></span>|<span data-ttu-id="2b0ce-110">string (読み取り専用)</span><span class="sxs-lookup"><span data-stu-id="2b0ce-110">string (readonly)</span></span>|<span data-ttu-id="2b0ce-111">操作エラーコード。</span><span class="sxs-lookup"><span data-stu-id="2b0ce-111">Operation error code.</span></span>|
|<span data-ttu-id="2b0ce-112">メッセージ​​</span><span class="sxs-lookup"><span data-stu-id="2b0ce-112">message</span></span>|<span data-ttu-id="2b0ce-113">string (読み取り専用)</span><span class="sxs-lookup"><span data-stu-id="2b0ce-113">string (readonly)</span></span>|<span data-ttu-id="2b0ce-114">操作エラーメッセージ。</span><span class="sxs-lookup"><span data-stu-id="2b0ce-114">Operation error message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2b0ce-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2b0ce-115">JSON representation</span></span>

<span data-ttu-id="2b0ce-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2b0ce-116">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "operation error resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
