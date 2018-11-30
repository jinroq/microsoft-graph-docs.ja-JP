---
title: オペレーション リソースの種類
description: 実行時間の長い操作のステータス。
ms.openlocfilehash: 622a17233a25709047ea852b7df5020aee3ae343
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020705"
---
# <a name="operation-resource-type"></a><span data-ttu-id="9dc44-103">オペレーション リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9dc44-103">operation resource type</span></span>

<span data-ttu-id="9dc44-104">実行時間の長い操作のステータス。</span><span class="sxs-lookup"><span data-stu-id="9dc44-104">The status of a long-running operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9dc44-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9dc44-105">JSON representation</span></span>

<span data-ttu-id="9dc44-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9dc44-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="9dc44-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9dc44-107">Properties</span></span>
| <span data-ttu-id="9dc44-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9dc44-108">Property</span></span>     | <span data-ttu-id="9dc44-109">型</span><span class="sxs-lookup"><span data-stu-id="9dc44-109">Type</span></span>   |<span data-ttu-id="9dc44-110">説明</span><span class="sxs-lookup"><span data-stu-id="9dc44-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9dc44-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9dc44-111">createdDateTime</span></span>| <span data-ttu-id="9dc44-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9dc44-112">DateTimeOffset</span></span> |<span data-ttu-id="9dc44-113">操作の開始時刻です。</span><span class="sxs-lookup"><span data-stu-id="9dc44-113">The start time of the operation.</span></span>|
|<span data-ttu-id="9dc44-114">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="9dc44-114">lastActionDateTime</span></span>| <span data-ttu-id="9dc44-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9dc44-115">DateTimeOffset</span></span> |<span data-ttu-id="9dc44-116">操作の最後の操作の時間です。</span><span class="sxs-lookup"><span data-stu-id="9dc44-116">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="9dc44-117">status</span><span class="sxs-lookup"><span data-stu-id="9dc44-117">status</span></span>|<span data-ttu-id="9dc44-118">operationStatus</span><span class="sxs-lookup"><span data-stu-id="9dc44-118">operationStatus</span></span>|<span data-ttu-id="9dc44-119">操作の現在の状態: `notStarted`、`running`、`completed`、`failed`</span><span class="sxs-lookup"><span data-stu-id="9dc44-119">The current status of the operation: `notStarted`, `running`, `completed`, `failed`</span></span> |

<!-- uuid: 13fa92b1-3b41-498b-aab1-f943464a124f
2018-03-30 10:29:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
