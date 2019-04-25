---
title: domainState リソースの種類
description: ドメインでスケジュールされた非同期操作の状態を表します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6a7741448b9c91be32f67f89cbafa5a579320083
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562780"
---
# <a name="domainstate-resource-type"></a><span data-ttu-id="30f66-103">domainState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="30f66-103">domainState resource type</span></span>

<span data-ttu-id="30f66-104">ドメインでスケジュールされた非同期操作の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="30f66-104">Represents the status of asynchronous operations scheduled on a domain.</span></span>

## <a name="properties"></a><span data-ttu-id="30f66-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="30f66-105">Properties</span></span>

| <span data-ttu-id="30f66-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="30f66-106">Property</span></span>   | <span data-ttu-id="30f66-107">型</span><span class="sxs-lookup"><span data-stu-id="30f66-107">Type</span></span> | <span data-ttu-id="30f66-108">説明</span><span class="sxs-lookup"><span data-stu-id="30f66-108">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="30f66-109">lastactiondatetime</span><span class="sxs-lookup"><span data-stu-id="30f66-109">lastActionDateTime</span></span> | <span data-ttu-id="30f66-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30f66-110">DateTimeOffset</span></span> | <span data-ttu-id="30f66-111">最後のアクティビティが発生したときのタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="30f66-111">Timestamp for when the last activity occurred.</span></span> <span data-ttu-id="30f66-112">この値は、操作がスケジュールされたとき、非同期タスクが開始されたとき、および操作が完了したときに更新されます。</span><span class="sxs-lookup"><span data-stu-id="30f66-112">The value is updated when an operation is scheduled, the asynchronous task starts, and when the operation completes.</span></span> |
| <span data-ttu-id="30f66-113">operation</span><span class="sxs-lookup"><span data-stu-id="30f66-113">operation</span></span> | <span data-ttu-id="30f66-114">String</span><span class="sxs-lookup"><span data-stu-id="30f66-114">String</span></span> | <span data-ttu-id="30f66-115">非同期操作の種類。</span><span class="sxs-lookup"><span data-stu-id="30f66-115">Type of asynchronous operation.</span></span> <span data-ttu-id="30f66-116">指定できる値は、 *forcedelete*または*ベリファイ*です</span><span class="sxs-lookup"><span data-stu-id="30f66-116">The values can be *ForceDelete* or *Verification*</span></span> |
| <span data-ttu-id="30f66-117">status</span><span class="sxs-lookup"><span data-stu-id="30f66-117">status</span></span> | <span data-ttu-id="30f66-118">String</span><span class="sxs-lookup"><span data-stu-id="30f66-118">String</span></span> | <span data-ttu-id="30f66-119">操作の現在の状態。</span><span class="sxs-lookup"><span data-stu-id="30f66-119">Current status of the operation.</span></span> <br> <span data-ttu-id="30f66-120">*スケジュール*済み-操作はスケジュールされていますが、開始されていません。</span><span class="sxs-lookup"><span data-stu-id="30f66-120">*Scheduled* - Operation has been scheduled but has not started.</span></span> <br> <span data-ttu-id="30f66-121">*InProgress* -タスクが開始され、進行中です。</span><span class="sxs-lookup"><span data-stu-id="30f66-121">*InProgress* - Task has started and is in progress.</span></span> <br> <span data-ttu-id="30f66-122">*失敗*-操作が失敗しました。</span><span class="sxs-lookup"><span data-stu-id="30f66-122">*Failed* - Operation has failed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="30f66-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="30f66-123">JSON representation</span></span>
<span data-ttu-id="30f66-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="30f66-124">Here is a JSON representation of the resource.</span></span>

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
