---
title: commsOperation リソースの種類
description: 特定の実行時間の長い操作のステータス。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b7914bd9692b4d9a94294f9a09659467e10550a6
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642206"
---
# <a name="commsoperation-resource-type"></a><span data-ttu-id="08659-103">commsOperation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="08659-103">commsOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08659-104">特定の実行時間の長い操作のステータス。</span><span class="sxs-lookup"><span data-stu-id="08659-104">The status of certain long-running operations.</span></span>

## <a name="methods"></a><span data-ttu-id="08659-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="08659-105">Methods</span></span>
<span data-ttu-id="08659-106">なし</span><span class="sxs-lookup"><span data-stu-id="08659-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="08659-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="08659-107">Properties</span></span>

| <span data-ttu-id="08659-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="08659-108">Property</span></span>           | <span data-ttu-id="08659-109">型</span><span class="sxs-lookup"><span data-stu-id="08659-109">Type</span></span>                        | <span data-ttu-id="08659-110">説明</span><span class="sxs-lookup"><span data-stu-id="08659-110">Description</span></span>                                                                     |
| :----------------- | :-------------------------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="08659-111">clientContext</span><span class="sxs-lookup"><span data-stu-id="08659-111">clientContext</span></span>      | <span data-ttu-id="08659-112">String</span><span class="sxs-lookup"><span data-stu-id="08659-112">String</span></span>                      | <span data-ttu-id="08659-113">クライアントのコンテキスト。</span><span class="sxs-lookup"><span data-stu-id="08659-113">The client context.</span></span>                                                             |
| <span data-ttu-id="08659-114">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="08659-114">createdDateTime</span></span>    | <span data-ttu-id="08659-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08659-115">DateTimeOffset</span></span>              | <span data-ttu-id="08659-116">操作の開始時刻です。</span><span class="sxs-lookup"><span data-stu-id="08659-116">The start time of the operation.</span></span>                                                |
| <span data-ttu-id="08659-117">id</span><span class="sxs-lookup"><span data-stu-id="08659-117">id</span></span>                 | <span data-ttu-id="08659-118">String</span><span class="sxs-lookup"><span data-stu-id="08659-118">String</span></span>                      | <span data-ttu-id="08659-119">操作 ID です。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="08659-119">The operation id. Read-only.</span></span> <span data-ttu-id="08659-120">サーバーによって生成されます。</span><span class="sxs-lookup"><span data-stu-id="08659-120">Server generated.</span></span>                                  |
| <span data-ttu-id="08659-121">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="08659-121">lastActionDateTime</span></span> | <span data-ttu-id="08659-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08659-122">DateTimeOffset</span></span>              | <span data-ttu-id="08659-123">操作の最後の操作の時間です。</span><span class="sxs-lookup"><span data-stu-id="08659-123">The time of the last action of the operation.</span></span>                                   |
| <span data-ttu-id="08659-124">resultInfo</span><span class="sxs-lookup"><span data-stu-id="08659-124">resultInfo</span></span>         | [<span data-ttu-id="08659-125">resultInfo</span><span class="sxs-lookup"><span data-stu-id="08659-125">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="08659-126">結果の情報。</span><span class="sxs-lookup"><span data-stu-id="08659-126">The result information.</span></span> <span data-ttu-id="08659-127">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="08659-127">Read-only.</span></span> <span data-ttu-id="08659-128">サーバーによって生成されます。</span><span class="sxs-lookup"><span data-stu-id="08659-128">Server generated.</span></span>                            |
| <span data-ttu-id="08659-129">status</span><span class="sxs-lookup"><span data-stu-id="08659-129">status</span></span>             | <span data-ttu-id="08659-130">String</span><span class="sxs-lookup"><span data-stu-id="08659-130">String</span></span>                      | <span data-ttu-id="08659-131">使用可能な値: `notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="08659-131">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="08659-132">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="08659-132">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="08659-133">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="08659-133">Relationships</span></span>
<span data-ttu-id="08659-134">なし</span><span class="sxs-lookup"><span data-stu-id="08659-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="08659-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="08659-135">JSON representation</span></span>

<span data-ttu-id="08659-136">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="08659-136">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.commsOperation"
}-->
```json
{
  "clientContext": "String",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "resultInfo": { "@odata.type": "#microsoft.graph.resultInfo" },
  "status": "notStarted | running | completed | failed"
}
```

## <a name="example"></a><span data-ttu-id="08659-137">例</span><span class="sxs-lookup"><span data-stu-id="08659-137">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsOperation"
}-->
```json
{
  "clientContext": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "createdDateTime": "2018-09-06T15:58:41Z",
  "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "resultInfo": {
    "@odata.type": "#microsoft.graph.resultInfo",
    "code": "200"
  },
  "status": "completed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "commsOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/commsoperation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
