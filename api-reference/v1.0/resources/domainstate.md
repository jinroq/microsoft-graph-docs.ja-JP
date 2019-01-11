---
title: domainState リソースの種類
description: ドメイン上でスケジュールされている非同期操作の状態を表します。
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: f24a5a9c493dc1cea16cb9038b85dc0a793bdfee
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880648"
---
# <a name="domainstate-resource-type"></a><span data-ttu-id="987ae-103">domainState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="987ae-103">domainState resource type</span></span>

<span data-ttu-id="987ae-104">ドメイン上でスケジュールされている非同期操作の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="987ae-104">Represents the status of asynchronous operations scheduled on a domain.</span></span>

## <a name="properties"></a><span data-ttu-id="987ae-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="987ae-105">Properties</span></span>

| <span data-ttu-id="987ae-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="987ae-106">Property</span></span>   | <span data-ttu-id="987ae-107">種類</span><span class="sxs-lookup"><span data-stu-id="987ae-107">Type</span></span> | <span data-ttu-id="987ae-108">説明</span><span class="sxs-lookup"><span data-stu-id="987ae-108">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="987ae-109">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="987ae-109">lastActionDateTime</span></span> | <span data-ttu-id="987ae-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="987ae-110">DateTimeOffset</span></span> | <span data-ttu-id="987ae-p101">最後のアクティビティが発生したときのタイムスタンプ。値は、操作のスケジュール時、非同期タスクの開始時、操作の完了時に更新されます。</span><span class="sxs-lookup"><span data-stu-id="987ae-p101">Timestamp for when the last activity occurred. The value is updated when an operation is scheduled, the asynchronous task starts, and when the operation completes.</span></span> |
| <span data-ttu-id="987ae-113">操作​​</span><span class="sxs-lookup"><span data-stu-id="987ae-113">operation</span></span> | <span data-ttu-id="987ae-114">String</span><span class="sxs-lookup"><span data-stu-id="987ae-114">String</span></span> | <span data-ttu-id="987ae-p102">非同期操作の種類。値は、*ForceDelete* または *Verification* のいずれかです。</span><span class="sxs-lookup"><span data-stu-id="987ae-p102">Type of asynchronous operation. The values can be *ForceDelete* or *Verification*</span></span> |
| <span data-ttu-id="987ae-117">status</span><span class="sxs-lookup"><span data-stu-id="987ae-117">status</span></span> | <span data-ttu-id="987ae-118">String</span><span class="sxs-lookup"><span data-stu-id="987ae-118">String</span></span> | <span data-ttu-id="987ae-119">操作の現在の状態。</span><span class="sxs-lookup"><span data-stu-id="987ae-119">Current status of the operation.</span></span> <br> <span data-ttu-id="987ae-120">*Scheduled* - 操作はスケジュールされていますが、開始されていません。</span><span class="sxs-lookup"><span data-stu-id="987ae-120">*Scheduled* - Operation has been scheduled but has not started.</span></span> <br> <span data-ttu-id="987ae-121">*InProgress* - タスクが開始され、実行中です。</span><span class="sxs-lookup"><span data-stu-id="987ae-121">*InProgress* - Task has started and is in progress.</span></span> <br> <span data-ttu-id="987ae-122">*Failed* - 操作が失敗しました。</span><span class="sxs-lookup"><span data-stu-id="987ae-122">*Failed* - Operation has failed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="987ae-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="987ae-123">JSON representation</span></span>
<span data-ttu-id="987ae-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="987ae-124">Here is a JSON representation of the resource.</span></span>

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
