---
title: playPromptOperation リソースの種類
description: PlayPrompt アクションの結果を取得する playPrompt の操作です。
author: VinodRavichandran
ms.openlocfilehash: d63b8f6cfa96706104cd7baaa08475974b12ca13
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380953"
---
# <a name="playpromptoperation-resource-type"></a><span data-ttu-id="d141b-103">playPromptOperation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d141b-103">playPromptOperation resource type</span></span>

> <span data-ttu-id="d141b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d141b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d141b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d141b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d141b-106">PlayPrompt アクションの結果を取得する playPrompt の操作です。</span><span class="sxs-lookup"><span data-stu-id="d141b-106">The playPrompt operation to obtain the result of the playPrompt action.</span></span>

## <a name="properties"></a><span data-ttu-id="d141b-107">Properties</span><span class="sxs-lookup"><span data-stu-id="d141b-107">Properties</span></span>

| <span data-ttu-id="d141b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d141b-108">Property</span></span>            | <span data-ttu-id="d141b-109">型</span><span class="sxs-lookup"><span data-stu-id="d141b-109">Type</span></span>                        | <span data-ttu-id="d141b-110">説明</span><span class="sxs-lookup"><span data-stu-id="d141b-110">Description</span></span>|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| <span data-ttu-id="d141b-111">clientContext</span><span class="sxs-lookup"><span data-stu-id="d141b-111">clientContext</span></span>       | <span data-ttu-id="d141b-112">String</span><span class="sxs-lookup"><span data-stu-id="d141b-112">String</span></span>                      | <span data-ttu-id="d141b-113">クライアントのコンテキスト。</span><span class="sxs-lookup"><span data-stu-id="d141b-113">The client context.</span></span>                                                                |
| <span data-ttu-id="d141b-114">completionReason</span><span class="sxs-lookup"><span data-stu-id="d141b-114">completionReason</span></span>    | <span data-ttu-id="d141b-115">String</span><span class="sxs-lookup"><span data-stu-id="d141b-115">String</span></span>                      | <span data-ttu-id="d141b-116">可能な値は、`unknown`、`completedSuccessfully`、`mediaOperationCanceled` です。</span><span class="sxs-lookup"><span data-stu-id="d141b-116">Possible values are: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`.</span></span> |
| <span data-ttu-id="d141b-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d141b-117">createdDateTime</span></span>     | <span data-ttu-id="d141b-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d141b-118">DateTimeOffset</span></span>              | <span data-ttu-id="d141b-119">操作の開始時刻です。</span><span class="sxs-lookup"><span data-stu-id="d141b-119">The start time of the operation.</span></span>                                                   |
| <span data-ttu-id="d141b-120">id</span><span class="sxs-lookup"><span data-stu-id="d141b-120">id</span></span>                  | <span data-ttu-id="d141b-121">String</span><span class="sxs-lookup"><span data-stu-id="d141b-121">String</span></span>                      | <span data-ttu-id="d141b-122">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d141b-122">Read-only.</span></span>                                                                         |
| <span data-ttu-id="d141b-123">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="d141b-123">lastActionDateTime</span></span>  | <span data-ttu-id="d141b-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d141b-124">DateTimeOffset</span></span>              | <span data-ttu-id="d141b-125">操作の最後の操作の時間です。</span><span class="sxs-lookup"><span data-stu-id="d141b-125">The time of the last action of the operation.</span></span>                                      |
| <span data-ttu-id="d141b-126">resultInfo</span><span class="sxs-lookup"><span data-stu-id="d141b-126">resultInfo</span></span>          | [<span data-ttu-id="d141b-127">resultInfo</span><span class="sxs-lookup"><span data-stu-id="d141b-127">resultInfo</span></span>](resultInfo.md) | <span data-ttu-id="d141b-128">結果の情報です。</span><span class="sxs-lookup"><span data-stu-id="d141b-128">The result information.</span></span> <span data-ttu-id="d141b-129">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d141b-129">Read-only.</span></span> <span data-ttu-id="d141b-130">サーバーを生成します。</span><span class="sxs-lookup"><span data-stu-id="d141b-130">Server generated.</span></span>                               |
| <span data-ttu-id="d141b-131">status</span><span class="sxs-lookup"><span data-stu-id="d141b-131">status</span></span>              | <span data-ttu-id="d141b-132">String</span><span class="sxs-lookup"><span data-stu-id="d141b-132">String</span></span>                      | <span data-ttu-id="d141b-133">可能な値は、`notStarted`、`running`、`completed`、`failed` です。</span><span class="sxs-lookup"><span data-stu-id="d141b-133">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span>               |

## <a name="relationships"></a><span data-ttu-id="d141b-134">関係</span><span class="sxs-lookup"><span data-stu-id="d141b-134">Relationships</span></span>
<span data-ttu-id="d141b-135">なし</span><span class="sxs-lookup"><span data-stu-id="d141b-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d141b-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d141b-136">JSON representation</span></span>

<span data-ttu-id="d141b-137">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d141b-137">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.playPromptOperation"
}-->
```json
{
  "clientContext": "String",
  "completionReason": "unknown | completedSuccessfully | mediaOperationCanceled",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "playPromptOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
