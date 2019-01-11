---
title: オペレーション リソースの種類
description: 実行時間の長い操作のステータス。
localization_priority: Normal
ms.openlocfilehash: 4f2e2c9a6fb9eb6d26a3511c637e79822919e2f5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884967"
---
# <a name="operation-resource-type"></a><span data-ttu-id="00e5a-103">オペレーション リソースの種類</span><span class="sxs-lookup"><span data-stu-id="00e5a-103">operation resource type</span></span>

<span data-ttu-id="00e5a-104">実行時間の長い操作のステータス。</span><span class="sxs-lookup"><span data-stu-id="00e5a-104">The status of a long-running operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="00e5a-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="00e5a-105">JSON representation</span></span>

<span data-ttu-id="00e5a-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="00e5a-106">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.operation"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "lastActionDateTime": "String (timestamp)",
  "status": "notStarted | running | completed | failed"
}

```
## <a name="properties"></a><span data-ttu-id="00e5a-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="00e5a-107">Properties</span></span>
| <span data-ttu-id="00e5a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="00e5a-108">Property</span></span>     | <span data-ttu-id="00e5a-109">種類</span><span class="sxs-lookup"><span data-stu-id="00e5a-109">Type</span></span>   |<span data-ttu-id="00e5a-110">説明</span><span class="sxs-lookup"><span data-stu-id="00e5a-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="00e5a-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="00e5a-111">createdDateTime</span></span>| <span data-ttu-id="00e5a-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00e5a-112">DateTimeOffset</span></span> |<span data-ttu-id="00e5a-113">操作の開始時刻です。</span><span class="sxs-lookup"><span data-stu-id="00e5a-113">The start time of the operation.</span></span>|
|<span data-ttu-id="00e5a-114">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="00e5a-114">lastActionDateTime</span></span>| <span data-ttu-id="00e5a-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00e5a-115">DateTimeOffset</span></span> |<span data-ttu-id="00e5a-116">操作の最後の操作の時間です。</span><span class="sxs-lookup"><span data-stu-id="00e5a-116">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="00e5a-117">status</span><span class="sxs-lookup"><span data-stu-id="00e5a-117">status</span></span>|<span data-ttu-id="00e5a-118">operationStatus</span><span class="sxs-lookup"><span data-stu-id="00e5a-118">operationStatus</span></span>|<span data-ttu-id="00e5a-119">操作の現在の状態: `notStarted`、`running`、`completed`、`failed`</span><span class="sxs-lookup"><span data-stu-id="00e5a-119">The current status of the operation: `notStarted`, `running`, `completed`, `failed`</span></span> |

<!-- uuid: 13fa92b1-3b41-498b-aab1-f943464a124f
2018-03-30 10:29:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
