---
title: domainState リソースの種類
description: ドメイン上でスケジュールされている非同期操作の状態を表します。
author: lleonard-msft
ms.openlocfilehash: 08484f29202ab348e2eca443a95f63ffbe645220
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351675"
---
# <a name="domainstate-resource-type"></a><span data-ttu-id="c8696-103">domainState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c8696-103">domainState resource type</span></span>

<span data-ttu-id="c8696-104">ドメイン上でスケジュールされている非同期操作の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="c8696-104">Represents the status of asynchronous operations scheduled on a domain.</span></span>

## <a name="properties"></a><span data-ttu-id="c8696-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c8696-105">Properties</span></span>

| <span data-ttu-id="c8696-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c8696-106">Property</span></span>   | <span data-ttu-id="c8696-107">種類</span><span class="sxs-lookup"><span data-stu-id="c8696-107">Type</span></span> | <span data-ttu-id="c8696-108">説明</span><span class="sxs-lookup"><span data-stu-id="c8696-108">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="c8696-109">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="c8696-109">lastActionDateTime</span></span> | <span data-ttu-id="c8696-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8696-110">DateTimeOffset</span></span> | <span data-ttu-id="c8696-p101">最後のアクティビティが発生したときのタイムスタンプ。値は、操作のスケジュール時、非同期タスクの開始時、操作の完了時に更新されます。</span><span class="sxs-lookup"><span data-stu-id="c8696-p101">Timestamp for when the last activity occurred. The value is updated when an operation is scheduled, the asynchronous task starts, and when the operation completes.</span></span> |
| <span data-ttu-id="c8696-113">操作​​</span><span class="sxs-lookup"><span data-stu-id="c8696-113">operation</span></span> | <span data-ttu-id="c8696-114">String</span><span class="sxs-lookup"><span data-stu-id="c8696-114">String</span></span> | <span data-ttu-id="c8696-p102">非同期操作の種類。値は、*ForceDelete* または *Verification* のいずれかです。</span><span class="sxs-lookup"><span data-stu-id="c8696-p102">Type of asynchronous operation. The values can be *ForceDelete* or *Verification*</span></span> |
| <span data-ttu-id="c8696-117">status</span><span class="sxs-lookup"><span data-stu-id="c8696-117">status</span></span> | <span data-ttu-id="c8696-118">String</span><span class="sxs-lookup"><span data-stu-id="c8696-118">String</span></span> | <span data-ttu-id="c8696-119">操作の現在の状態。</span><span class="sxs-lookup"><span data-stu-id="c8696-119">Current status of the operation.</span></span> <br> <span data-ttu-id="c8696-120">*Scheduled* - 操作はスケジュールされていますが、開始されていません。</span><span class="sxs-lookup"><span data-stu-id="c8696-120">*Scheduled* - Operation has been scheduled but has not started.</span></span> <br> <span data-ttu-id="c8696-121">*InProgress* - タスクが開始され、実行中です。</span><span class="sxs-lookup"><span data-stu-id="c8696-121">*InProgress* - Task has started and is in progress.</span></span> <br> <span data-ttu-id="c8696-122">*Failed* - 操作が失敗しました。</span><span class="sxs-lookup"><span data-stu-id="c8696-122">*Failed* - Operation has failed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c8696-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c8696-123">JSON representation</span></span>
<span data-ttu-id="c8696-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c8696-124">Here is a JSON representation of the resource.</span></span>

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