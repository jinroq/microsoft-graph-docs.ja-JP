---
title: operation リソースの種類
description: 長時間実行されている操作の状態。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 8088d704d5a075131d5ee1b2c3b9edf75785708b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035729"
---
# <a name="operation-resource-type"></a><span data-ttu-id="a1bb7-103">operation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a1bb7-103">operation resource type</span></span>

<span data-ttu-id="a1bb7-104">長時間実行されている操作の状態。</span><span class="sxs-lookup"><span data-stu-id="a1bb7-104">The status of a long-running operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a1bb7-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a1bb7-105">JSON representation</span></span>

<span data-ttu-id="a1bb7-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a1bb7-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="a1bb7-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a1bb7-107">Properties</span></span>
| <span data-ttu-id="a1bb7-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a1bb7-108">Property</span></span>     | <span data-ttu-id="a1bb7-109">型</span><span class="sxs-lookup"><span data-stu-id="a1bb7-109">Type</span></span>   |<span data-ttu-id="a1bb7-110">説明</span><span class="sxs-lookup"><span data-stu-id="a1bb7-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a1bb7-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a1bb7-111">createdDateTime</span></span>| <span data-ttu-id="a1bb7-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1bb7-112">DateTimeOffset</span></span> |<span data-ttu-id="a1bb7-113">操作の開始時刻。</span><span class="sxs-lookup"><span data-stu-id="a1bb7-113">The start time of the operation.</span></span>|
|<span data-ttu-id="a1bb7-114">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="a1bb7-114">lastActionDateTime</span></span>| <span data-ttu-id="a1bb7-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1bb7-115">DateTimeOffset</span></span> |<span data-ttu-id="a1bb7-116">操作の最後の操作の時刻。</span><span class="sxs-lookup"><span data-stu-id="a1bb7-116">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="a1bb7-117">status</span><span class="sxs-lookup"><span data-stu-id="a1bb7-117">status</span></span>|<span data-ttu-id="a1bb7-118">operationStatus</span><span class="sxs-lookup"><span data-stu-id="a1bb7-118">operationStatus</span></span>|<span data-ttu-id="a1bb7-119">操作の現在の状態: `notStarted`、 `running` `completed`、、`failed`</span><span class="sxs-lookup"><span data-stu-id="a1bb7-119">The current status of the operation: `notStarted`, `running`, `completed`, `failed`</span></span> |

<!-- uuid: 13fa92b1-3b41-498b-aab1-f943464a124f
2018-03-30 10:29:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
