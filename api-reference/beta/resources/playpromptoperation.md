---
title: playPromptOperation リソースの種類
description: Playprompt アクションの結果を取得する playPrompt 操作。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 663675bb895d452c9ad50c89f22f1a51efca20a9
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536996"
---
# <a name="playpromptoperation-resource-type"></a><span data-ttu-id="f75aa-103">playPromptOperation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f75aa-103">playPromptOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f75aa-104">Playprompt アクションの結果を取得する playPrompt 操作。</span><span class="sxs-lookup"><span data-stu-id="f75aa-104">The playPrompt operation to obtain the result of the playPrompt action.</span></span>

## <a name="properties"></a><span data-ttu-id="f75aa-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f75aa-105">Properties</span></span>

| <span data-ttu-id="f75aa-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f75aa-106">Property</span></span>            | <span data-ttu-id="f75aa-107">型</span><span class="sxs-lookup"><span data-stu-id="f75aa-107">Type</span></span>                        | <span data-ttu-id="f75aa-108">説明</span><span class="sxs-lookup"><span data-stu-id="f75aa-108">Description</span></span>|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| <span data-ttu-id="f75aa-109">clientContext</span><span class="sxs-lookup"><span data-stu-id="f75aa-109">clientContext</span></span>       | <span data-ttu-id="f75aa-110">String</span><span class="sxs-lookup"><span data-stu-id="f75aa-110">String</span></span>                      | <span data-ttu-id="f75aa-111">クライアントコンテキスト。</span><span class="sxs-lookup"><span data-stu-id="f75aa-111">The client context.</span></span>                                                                |
| <span data-ttu-id="f75aa-112">「補完の理由」</span><span class="sxs-lookup"><span data-stu-id="f75aa-112">completionReason</span></span>    | <span data-ttu-id="f75aa-113">String</span><span class="sxs-lookup"><span data-stu-id="f75aa-113">String</span></span>                      | <span data-ttu-id="f75aa-114">可能な値は、`unknown`、`completedSuccessfully`、`mediaOperationCanceled` です。</span><span class="sxs-lookup"><span data-stu-id="f75aa-114">Possible values are: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`.</span></span> |
| <span data-ttu-id="f75aa-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f75aa-115">createdDateTime</span></span>     | <span data-ttu-id="f75aa-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f75aa-116">DateTimeOffset</span></span>              | <span data-ttu-id="f75aa-117">操作の開始時刻。</span><span class="sxs-lookup"><span data-stu-id="f75aa-117">The start time of the operation.</span></span>                                                   |
| <span data-ttu-id="f75aa-118">id</span><span class="sxs-lookup"><span data-stu-id="f75aa-118">id</span></span>                  | <span data-ttu-id="f75aa-119">文字列</span><span class="sxs-lookup"><span data-stu-id="f75aa-119">String</span></span>                      | <span data-ttu-id="f75aa-120">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f75aa-120">Read-only.</span></span>                                                                         |
| <span data-ttu-id="f75aa-121">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="f75aa-121">lastActionDateTime</span></span>  | <span data-ttu-id="f75aa-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f75aa-122">DateTimeOffset</span></span>              | <span data-ttu-id="f75aa-123">操作の最後の操作の時刻。</span><span class="sxs-lookup"><span data-stu-id="f75aa-123">The time of the last action of the operation.</span></span>                                      |
| <span data-ttu-id="f75aa-124">resultInfo</span><span class="sxs-lookup"><span data-stu-id="f75aa-124">resultInfo</span></span>          | [<span data-ttu-id="f75aa-125">resultInfo</span><span class="sxs-lookup"><span data-stu-id="f75aa-125">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="f75aa-126">結果の情報。</span><span class="sxs-lookup"><span data-stu-id="f75aa-126">The result information.</span></span> <span data-ttu-id="f75aa-127">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f75aa-127">Read-only.</span></span> <span data-ttu-id="f75aa-128">サーバーによって生成されます。</span><span class="sxs-lookup"><span data-stu-id="f75aa-128">Server generated.</span></span>                               |
| <span data-ttu-id="f75aa-129">status</span><span class="sxs-lookup"><span data-stu-id="f75aa-129">status</span></span>              | <span data-ttu-id="f75aa-130">String</span><span class="sxs-lookup"><span data-stu-id="f75aa-130">String</span></span>                      | <span data-ttu-id="f75aa-131">使用可能な値: `notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="f75aa-131">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span>               |

## <a name="relationships"></a><span data-ttu-id="f75aa-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f75aa-132">Relationships</span></span>
<span data-ttu-id="f75aa-133">なし</span><span class="sxs-lookup"><span data-stu-id="f75aa-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f75aa-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f75aa-134">JSON representation</span></span>

<span data-ttu-id="f75aa-135">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f75aa-135">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "playPromptOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
