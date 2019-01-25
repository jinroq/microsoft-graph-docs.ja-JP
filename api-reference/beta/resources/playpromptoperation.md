---
title: playPromptOperation リソースの種類
description: PlayPrompt アクションの結果を取得する playPrompt の操作です。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a6ecdb06c910923d35f9d36590ad09fd7835fccb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515203"
---
# <a name="playpromptoperation-resource-type"></a><span data-ttu-id="c266a-103">playPromptOperation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c266a-103">playPromptOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c266a-104">PlayPrompt アクションの結果を取得する playPrompt の操作です。</span><span class="sxs-lookup"><span data-stu-id="c266a-104">The playPrompt operation to obtain the result of the playPrompt action.</span></span>

## <a name="properties"></a><span data-ttu-id="c266a-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c266a-105">Properties</span></span>

| <span data-ttu-id="c266a-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c266a-106">Property</span></span>            | <span data-ttu-id="c266a-107">型</span><span class="sxs-lookup"><span data-stu-id="c266a-107">Type</span></span>                        | <span data-ttu-id="c266a-108">説明</span><span class="sxs-lookup"><span data-stu-id="c266a-108">Description</span></span>|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| <span data-ttu-id="c266a-109">ClientContext</span><span class="sxs-lookup"><span data-stu-id="c266a-109">clientContext</span></span>       | <span data-ttu-id="c266a-110">String</span><span class="sxs-lookup"><span data-stu-id="c266a-110">String</span></span>                      | <span data-ttu-id="c266a-111">クライアントのコンテキスト。</span><span class="sxs-lookup"><span data-stu-id="c266a-111">The client context.</span></span>                                                                |
| <span data-ttu-id="c266a-112">completionReason</span><span class="sxs-lookup"><span data-stu-id="c266a-112">completionReason</span></span>    | <span data-ttu-id="c266a-113">String</span><span class="sxs-lookup"><span data-stu-id="c266a-113">String</span></span>                      | <span data-ttu-id="c266a-114">可能な値は、`unknown`、`completedSuccessfully`、`mediaOperationCanceled` です。</span><span class="sxs-lookup"><span data-stu-id="c266a-114">Possible values are: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`.</span></span> |
| <span data-ttu-id="c266a-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c266a-115">createdDateTime</span></span>     | <span data-ttu-id="c266a-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c266a-116">DateTimeOffset</span></span>              | <span data-ttu-id="c266a-117">操作の開始時刻です。</span><span class="sxs-lookup"><span data-stu-id="c266a-117">The start time of the operation.</span></span>                                                   |
| <span data-ttu-id="c266a-118">id</span><span class="sxs-lookup"><span data-stu-id="c266a-118">id</span></span>                  | <span data-ttu-id="c266a-119">文字列</span><span class="sxs-lookup"><span data-stu-id="c266a-119">String</span></span>                      | <span data-ttu-id="c266a-120">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c266a-120">Read-only.</span></span>                                                                         |
| <span data-ttu-id="c266a-121">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="c266a-121">lastActionDateTime</span></span>  | <span data-ttu-id="c266a-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c266a-122">DateTimeOffset</span></span>              | <span data-ttu-id="c266a-123">操作の最後の操作の時間です。</span><span class="sxs-lookup"><span data-stu-id="c266a-123">The time of the last action of the operation.</span></span>                                      |
| <span data-ttu-id="c266a-124">resultInfo</span><span class="sxs-lookup"><span data-stu-id="c266a-124">resultInfo</span></span>          | [<span data-ttu-id="c266a-125">resultInfo</span><span class="sxs-lookup"><span data-stu-id="c266a-125">resultInfo</span></span>](resultInfo.md) | <span data-ttu-id="c266a-126">結果の情報です。</span><span class="sxs-lookup"><span data-stu-id="c266a-126">The result information.</span></span> <span data-ttu-id="c266a-127">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c266a-127">Read-only.</span></span> <span data-ttu-id="c266a-128">サーバーを生成します。</span><span class="sxs-lookup"><span data-stu-id="c266a-128">Server generated.</span></span>                               |
| <span data-ttu-id="c266a-129">status</span><span class="sxs-lookup"><span data-stu-id="c266a-129">status</span></span>              | <span data-ttu-id="c266a-130">String</span><span class="sxs-lookup"><span data-stu-id="c266a-130">String</span></span>                      | <span data-ttu-id="c266a-131">可能な値は、`notStarted`、`running`、`completed`、`failed` です。</span><span class="sxs-lookup"><span data-stu-id="c266a-131">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span>               |

## <a name="relationships"></a><span data-ttu-id="c266a-132">関係</span><span class="sxs-lookup"><span data-stu-id="c266a-132">Relationships</span></span>
<span data-ttu-id="c266a-133">なし</span><span class="sxs-lookup"><span data-stu-id="c266a-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c266a-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c266a-134">JSON representation</span></span>

<span data-ttu-id="c266a-135">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c266a-135">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/playpromptoperation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
