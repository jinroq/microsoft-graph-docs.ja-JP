---
title: playPromptOperation リソースの種類
description: Playprompt アクションの結果を取得する playPrompt 操作。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b79fa774c112433b09d75eb04f16823f2dad9b6c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008979"
---
# <a name="playpromptoperation-resource-type"></a><span data-ttu-id="37432-103">playPromptOperation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="37432-103">playPromptOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37432-104">Playprompt アクションの結果を取得する playPrompt 操作。</span><span class="sxs-lookup"><span data-stu-id="37432-104">The playPrompt operation to obtain the result of the playPrompt action.</span></span>

## <a name="properties"></a><span data-ttu-id="37432-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="37432-105">Properties</span></span>

| <span data-ttu-id="37432-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="37432-106">Property</span></span>            | <span data-ttu-id="37432-107">型</span><span class="sxs-lookup"><span data-stu-id="37432-107">Type</span></span>                        | <span data-ttu-id="37432-108">説明</span><span class="sxs-lookup"><span data-stu-id="37432-108">Description</span></span>|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| <span data-ttu-id="37432-109">clientContext</span><span class="sxs-lookup"><span data-stu-id="37432-109">clientContext</span></span>       | <span data-ttu-id="37432-110">String</span><span class="sxs-lookup"><span data-stu-id="37432-110">String</span></span>                      | <span data-ttu-id="37432-111">クライアントコンテキスト。</span><span class="sxs-lookup"><span data-stu-id="37432-111">The client context.</span></span>                                                                |
| <span data-ttu-id="37432-112">「補完の理由」</span><span class="sxs-lookup"><span data-stu-id="37432-112">completionReason</span></span>    | <span data-ttu-id="37432-113">String</span><span class="sxs-lookup"><span data-stu-id="37432-113">String</span></span>                      | <span data-ttu-id="37432-114">可能な値は、`unknown`、`completedSuccessfully`、`mediaOperationCanceled` です。</span><span class="sxs-lookup"><span data-stu-id="37432-114">Possible values are: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`.</span></span> |
| <span data-ttu-id="37432-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="37432-115">createdDateTime</span></span>     | <span data-ttu-id="37432-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37432-116">DateTimeOffset</span></span>              | <span data-ttu-id="37432-117">操作の開始時刻。</span><span class="sxs-lookup"><span data-stu-id="37432-117">The start time of the operation.</span></span>                                                   |
| <span data-ttu-id="37432-118">id</span><span class="sxs-lookup"><span data-stu-id="37432-118">id</span></span>                  | <span data-ttu-id="37432-119">文字列</span><span class="sxs-lookup"><span data-stu-id="37432-119">String</span></span>                      | <span data-ttu-id="37432-120">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="37432-120">Read-only.</span></span>                                                                         |
| <span data-ttu-id="37432-121">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="37432-121">lastActionDateTime</span></span>  | <span data-ttu-id="37432-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37432-122">DateTimeOffset</span></span>              | <span data-ttu-id="37432-123">操作の最後の操作の時刻。</span><span class="sxs-lookup"><span data-stu-id="37432-123">The time of the last action of the operation.</span></span>                                      |
| <span data-ttu-id="37432-124">resultInfo</span><span class="sxs-lookup"><span data-stu-id="37432-124">resultInfo</span></span>          | [<span data-ttu-id="37432-125">resultInfo</span><span class="sxs-lookup"><span data-stu-id="37432-125">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="37432-126">結果の情報。</span><span class="sxs-lookup"><span data-stu-id="37432-126">The result information.</span></span> <span data-ttu-id="37432-127">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="37432-127">Read-only.</span></span> <span data-ttu-id="37432-128">サーバーによって生成されます。</span><span class="sxs-lookup"><span data-stu-id="37432-128">Server generated.</span></span>                               |
| <span data-ttu-id="37432-129">status</span><span class="sxs-lookup"><span data-stu-id="37432-129">status</span></span>              | <span data-ttu-id="37432-130">String</span><span class="sxs-lookup"><span data-stu-id="37432-130">String</span></span>                      | <span data-ttu-id="37432-131">使用可能な値: `notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="37432-131">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span>               |

## <a name="relationships"></a><span data-ttu-id="37432-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="37432-132">Relationships</span></span>
<span data-ttu-id="37432-133">なし</span><span class="sxs-lookup"><span data-stu-id="37432-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="37432-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="37432-134">JSON representation</span></span>

<span data-ttu-id="37432-135">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="37432-135">The following is a JSON representation of the resource.</span></span>

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
