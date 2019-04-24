---
title: operation リソースの種類
description: 長時間実行されている操作の状態。
localization_priority: Normal
ms.openlocfilehash: 4f2e2c9a6fb9eb6d26a3511c637e79822919e2f5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462677"
---
# <a name="operation-resource-type"></a><span data-ttu-id="3bcb5-103">operation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3bcb5-103">operation resource type</span></span>

<span data-ttu-id="3bcb5-104">長時間実行されている操作の状態。</span><span class="sxs-lookup"><span data-stu-id="3bcb5-104">The status of a long-running operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3bcb5-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3bcb5-105">JSON representation</span></span>

<span data-ttu-id="3bcb5-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3bcb5-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="3bcb5-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3bcb5-107">Properties</span></span>
| <span data-ttu-id="3bcb5-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3bcb5-108">Property</span></span>     | <span data-ttu-id="3bcb5-109">型</span><span class="sxs-lookup"><span data-stu-id="3bcb5-109">Type</span></span>   |<span data-ttu-id="3bcb5-110">説明</span><span class="sxs-lookup"><span data-stu-id="3bcb5-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3bcb5-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3bcb5-111">createdDateTime</span></span>| <span data-ttu-id="3bcb5-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3bcb5-112">DateTimeOffset</span></span> |<span data-ttu-id="3bcb5-113">操作の開始時刻。</span><span class="sxs-lookup"><span data-stu-id="3bcb5-113">The start time of the operation.</span></span>|
|<span data-ttu-id="3bcb5-114">lastactiondatetime</span><span class="sxs-lookup"><span data-stu-id="3bcb5-114">lastActionDateTime</span></span>| <span data-ttu-id="3bcb5-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3bcb5-115">DateTimeOffset</span></span> |<span data-ttu-id="3bcb5-116">操作の最後の操作の時刻。</span><span class="sxs-lookup"><span data-stu-id="3bcb5-116">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="3bcb5-117">status</span><span class="sxs-lookup"><span data-stu-id="3bcb5-117">status</span></span>|<span data-ttu-id="3bcb5-118">operationstatus</span><span class="sxs-lookup"><span data-stu-id="3bcb5-118">operationStatus</span></span>|<span data-ttu-id="3bcb5-119">操作の現在の状態: `notStarted`、 `running` `completed`、、`failed`</span><span class="sxs-lookup"><span data-stu-id="3bcb5-119">The current status of the operation: `notStarted`, `running`, `completed`, `failed`</span></span> |

<!-- uuid: 13fa92b1-3b41-498b-aab1-f943464a124f
2018-03-30 10:29:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
