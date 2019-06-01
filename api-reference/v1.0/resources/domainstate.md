---
title: domainState リソースの種類
description: ドメインでスケジュールされた非同期操作の状態を表します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 19da0630abf4b27899af9e5c6be12254d91e9499
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657694"
---
# <a name="domainstate-resource-type"></a><span data-ttu-id="f34bf-103">domainState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f34bf-103">domainState resource type</span></span>

<span data-ttu-id="f34bf-104">ドメインでスケジュールされた非同期操作の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="f34bf-104">Represents the status of asynchronous operations scheduled on a domain.</span></span>

## <a name="properties"></a><span data-ttu-id="f34bf-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f34bf-105">Properties</span></span>

| <span data-ttu-id="f34bf-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f34bf-106">Property</span></span>   | <span data-ttu-id="f34bf-107">型</span><span class="sxs-lookup"><span data-stu-id="f34bf-107">Type</span></span> | <span data-ttu-id="f34bf-108">説明</span><span class="sxs-lookup"><span data-stu-id="f34bf-108">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="f34bf-109">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="f34bf-109">lastActionDateTime</span></span> | <span data-ttu-id="f34bf-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f34bf-110">DateTimeOffset</span></span> | <span data-ttu-id="f34bf-111">最後のアクティビティが発生したときのタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="f34bf-111">Timestamp for when the last activity occurred.</span></span> <span data-ttu-id="f34bf-112">この値は、操作がスケジュールされたとき、非同期タスクが開始されたとき、および操作が完了したときに更新されます。</span><span class="sxs-lookup"><span data-stu-id="f34bf-112">The value is updated when an operation is scheduled, the asynchronous task starts, and when the operation completes.</span></span> |
| <span data-ttu-id="f34bf-113">operation</span><span class="sxs-lookup"><span data-stu-id="f34bf-113">operation</span></span> | <span data-ttu-id="f34bf-114">String</span><span class="sxs-lookup"><span data-stu-id="f34bf-114">String</span></span> | <span data-ttu-id="f34bf-115">非同期操作の種類。</span><span class="sxs-lookup"><span data-stu-id="f34bf-115">Type of asynchronous operation.</span></span> <span data-ttu-id="f34bf-116">指定できる値は、 *Forcedelete*または*ベリファイ*です</span><span class="sxs-lookup"><span data-stu-id="f34bf-116">The values can be *ForceDelete* or *Verification*</span></span> |
| <span data-ttu-id="f34bf-117">status</span><span class="sxs-lookup"><span data-stu-id="f34bf-117">status</span></span> | <span data-ttu-id="f34bf-118">String</span><span class="sxs-lookup"><span data-stu-id="f34bf-118">String</span></span> | <span data-ttu-id="f34bf-119">操作の現在の状態。</span><span class="sxs-lookup"><span data-stu-id="f34bf-119">Current status of the operation.</span></span> <br> <span data-ttu-id="f34bf-120">*スケジュール*済み-操作はスケジュールされていますが、開始されていません。</span><span class="sxs-lookup"><span data-stu-id="f34bf-120">*Scheduled* - Operation has been scheduled but has not started.</span></span> <br> <span data-ttu-id="f34bf-121">*InProgress* -タスクが開始され、進行中です。</span><span class="sxs-lookup"><span data-stu-id="f34bf-121">*InProgress* - Task has started and is in progress.</span></span> <br> <span data-ttu-id="f34bf-122">*失敗*-操作が失敗しました。</span><span class="sxs-lookup"><span data-stu-id="f34bf-122">*Failed* - Operation has failed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f34bf-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f34bf-123">JSON representation</span></span>
<span data-ttu-id="f34bf-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f34bf-124">Here is a JSON representation of the resource.</span></span>

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
