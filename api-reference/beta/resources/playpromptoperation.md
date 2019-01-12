---
title: playPromptOperation リソースの種類
description: PlayPrompt アクションの結果を取得する playPrompt の操作です。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d451418482d1adf1a4b7e16dc8a6eb8ca7febdb7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937818"
---
# <a name="playpromptoperation-resource-type"></a><span data-ttu-id="13a5a-103">playPromptOperation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="13a5a-103">playPromptOperation resource type</span></span>

> <span data-ttu-id="13a5a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="13a5a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="13a5a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="13a5a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="13a5a-106">PlayPrompt アクションの結果を取得する playPrompt の操作です。</span><span class="sxs-lookup"><span data-stu-id="13a5a-106">The playPrompt operation to obtain the result of the playPrompt action.</span></span>

## <a name="properties"></a><span data-ttu-id="13a5a-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="13a5a-107">Properties</span></span>

| <span data-ttu-id="13a5a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="13a5a-108">Property</span></span>            | <span data-ttu-id="13a5a-109">種類</span><span class="sxs-lookup"><span data-stu-id="13a5a-109">Type</span></span>                        | <span data-ttu-id="13a5a-110">説明</span><span class="sxs-lookup"><span data-stu-id="13a5a-110">Description</span></span>|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| <span data-ttu-id="13a5a-111">clientContext</span><span class="sxs-lookup"><span data-stu-id="13a5a-111">clientContext</span></span>       | <span data-ttu-id="13a5a-112">String</span><span class="sxs-lookup"><span data-stu-id="13a5a-112">String</span></span>                      | <span data-ttu-id="13a5a-113">クライアントのコンテキスト。</span><span class="sxs-lookup"><span data-stu-id="13a5a-113">The client context.</span></span>                                                                |
| <span data-ttu-id="13a5a-114">completionReason</span><span class="sxs-lookup"><span data-stu-id="13a5a-114">completionReason</span></span>    | <span data-ttu-id="13a5a-115">String</span><span class="sxs-lookup"><span data-stu-id="13a5a-115">String</span></span>                      | <span data-ttu-id="13a5a-116">可能な値は、`unknown`、`completedSuccessfully`、`mediaOperationCanceled` です。</span><span class="sxs-lookup"><span data-stu-id="13a5a-116">Possible values are: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`.</span></span> |
| <span data-ttu-id="13a5a-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="13a5a-117">createdDateTime</span></span>     | <span data-ttu-id="13a5a-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13a5a-118">DateTimeOffset</span></span>              | <span data-ttu-id="13a5a-119">操作の開始時刻です。</span><span class="sxs-lookup"><span data-stu-id="13a5a-119">The start time of the operation.</span></span>                                                   |
| <span data-ttu-id="13a5a-120">id</span><span class="sxs-lookup"><span data-stu-id="13a5a-120">id</span></span>                  | <span data-ttu-id="13a5a-121">String</span><span class="sxs-lookup"><span data-stu-id="13a5a-121">String</span></span>                      | <span data-ttu-id="13a5a-122">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="13a5a-122">Read-only.</span></span>                                                                         |
| <span data-ttu-id="13a5a-123">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="13a5a-123">lastActionDateTime</span></span>  | <span data-ttu-id="13a5a-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13a5a-124">DateTimeOffset</span></span>              | <span data-ttu-id="13a5a-125">操作の最後の操作の時間です。</span><span class="sxs-lookup"><span data-stu-id="13a5a-125">The time of the last action of the operation.</span></span>                                      |
| <span data-ttu-id="13a5a-126">resultInfo</span><span class="sxs-lookup"><span data-stu-id="13a5a-126">resultInfo</span></span>          | [<span data-ttu-id="13a5a-127">resultInfo</span><span class="sxs-lookup"><span data-stu-id="13a5a-127">resultInfo</span></span>](resultInfo.md) | <span data-ttu-id="13a5a-128">結果の情報です。</span><span class="sxs-lookup"><span data-stu-id="13a5a-128">The result information.</span></span> <span data-ttu-id="13a5a-129">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="13a5a-129">Read-only.</span></span> <span data-ttu-id="13a5a-130">サーバーを生成します。</span><span class="sxs-lookup"><span data-stu-id="13a5a-130">Server generated.</span></span>                               |
| <span data-ttu-id="13a5a-131">status</span><span class="sxs-lookup"><span data-stu-id="13a5a-131">status</span></span>              | <span data-ttu-id="13a5a-132">String</span><span class="sxs-lookup"><span data-stu-id="13a5a-132">String</span></span>                      | <span data-ttu-id="13a5a-133">可能な値は、`notStarted`、`running`、`completed`、`failed` です。</span><span class="sxs-lookup"><span data-stu-id="13a5a-133">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span>               |

## <a name="relationships"></a><span data-ttu-id="13a5a-134">関係</span><span class="sxs-lookup"><span data-stu-id="13a5a-134">Relationships</span></span>
<span data-ttu-id="13a5a-135">なし</span><span class="sxs-lookup"><span data-stu-id="13a5a-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="13a5a-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="13a5a-136">JSON representation</span></span>

<span data-ttu-id="13a5a-137">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="13a5a-137">The following is a JSON representation of the resource.</span></span>

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
