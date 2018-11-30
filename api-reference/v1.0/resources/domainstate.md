---
title: domainState リソースの種類
description: ドメイン上でスケジュールされている非同期操作の状態を表します。
ms.openlocfilehash: 73a83eddb46b9305a6d74e283bae1c009361195d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022724"
---
# <a name="domainstate-resource-type"></a><span data-ttu-id="c352a-103">domainState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c352a-103">domainState resource type</span></span>

<span data-ttu-id="c352a-104">ドメイン上でスケジュールされている非同期操作の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="c352a-104">Represents the status of asynchronous operations scheduled on a domain.</span></span>

## <a name="properties"></a><span data-ttu-id="c352a-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c352a-105">Properties</span></span>

| <span data-ttu-id="c352a-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c352a-106">Property</span></span>   | <span data-ttu-id="c352a-107">型</span><span class="sxs-lookup"><span data-stu-id="c352a-107">Type</span></span> | <span data-ttu-id="c352a-108">説明</span><span class="sxs-lookup"><span data-stu-id="c352a-108">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="c352a-109">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="c352a-109">lastActionDateTime</span></span> | <span data-ttu-id="c352a-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c352a-110">DateTimeOffset</span></span> | <span data-ttu-id="c352a-p101">最後のアクティビティが発生したときのタイムスタンプ。値は、操作のスケジュール時、非同期タスクの開始時、操作の完了時に更新されます。</span><span class="sxs-lookup"><span data-stu-id="c352a-p101">Timestamp for when the last activity occurred. The value is updated when an operation is scheduled, the asynchronous task starts, and when the operation completes.</span></span> |
| <span data-ttu-id="c352a-113">操作​​</span><span class="sxs-lookup"><span data-stu-id="c352a-113">operation</span></span> | <span data-ttu-id="c352a-114">String</span><span class="sxs-lookup"><span data-stu-id="c352a-114">String</span></span> | <span data-ttu-id="c352a-p102">非同期操作の種類。値は、*ForceDelete* または *Verification* のいずれかです。</span><span class="sxs-lookup"><span data-stu-id="c352a-p102">Type of asynchronous operation. The values can be *ForceDelete* or *Verification*</span></span> |
| <span data-ttu-id="c352a-117">status</span><span class="sxs-lookup"><span data-stu-id="c352a-117">status</span></span> | <span data-ttu-id="c352a-118">String</span><span class="sxs-lookup"><span data-stu-id="c352a-118">String</span></span> | <span data-ttu-id="c352a-119">操作の現在の状態。</span><span class="sxs-lookup"><span data-stu-id="c352a-119">Current status of the operation.</span></span> <br> <span data-ttu-id="c352a-120">*Scheduled* - 操作はスケジュールされていますが、開始されていません。</span><span class="sxs-lookup"><span data-stu-id="c352a-120">*Scheduled* - Operation has been scheduled but has not started.</span></span> <br> <span data-ttu-id="c352a-121">*InProgress* - タスクが開始され、実行中です。</span><span class="sxs-lookup"><span data-stu-id="c352a-121">*InProgress* - Task has started and is in progress.</span></span> <br> <span data-ttu-id="c352a-122">*Failed* - 操作が失敗しました。</span><span class="sxs-lookup"><span data-stu-id="c352a-122">*Failed* - Operation has failed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c352a-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c352a-123">JSON representation</span></span>
<span data-ttu-id="c352a-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c352a-124">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainState"
}-->

```json
{
  "lastActionDateTime": "String (timestamp)",
  "operation": "String",
  "status": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->