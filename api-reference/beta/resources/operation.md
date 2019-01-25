---
title: オペレーション リソースの種類
description: 実行時間の長い操作のステータス。
localization_priority: Normal
ms.openlocfilehash: 3ad9848387dab2de928f7ace2fa4b905720be615
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520187"
---
# <a name="operation-resource-type"></a><span data-ttu-id="e6c84-103">オペレーション リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e6c84-103">operation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6c84-104">実行時間の長い操作のステータス。</span><span class="sxs-lookup"><span data-stu-id="e6c84-104">The status of a long-running operation.</span></span>

## <a name="methods"></a><span data-ttu-id="e6c84-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="e6c84-105">Methods</span></span>

<span data-ttu-id="e6c84-106">なし</span><span class="sxs-lookup"><span data-stu-id="e6c84-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="e6c84-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e6c84-107">Properties</span></span>

| <span data-ttu-id="e6c84-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e6c84-108">Property</span></span>           | <span data-ttu-id="e6c84-109">型</span><span class="sxs-lookup"><span data-stu-id="e6c84-109">Type</span></span>            | <span data-ttu-id="e6c84-110">説明</span><span class="sxs-lookup"><span data-stu-id="e6c84-110">Description</span></span>                                                                     |
| :----------------- | :-------------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="e6c84-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e6c84-111">createdDateTime</span></span>    | <span data-ttu-id="e6c84-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6c84-112">DateTimeOffset</span></span>  | <span data-ttu-id="e6c84-113">操作の開始時刻です。</span><span class="sxs-lookup"><span data-stu-id="e6c84-113">The start time of the operation.</span></span>                                                |
| <span data-ttu-id="e6c84-114">id</span><span class="sxs-lookup"><span data-stu-id="e6c84-114">id</span></span>                 | <span data-ttu-id="e6c84-115">String</span><span class="sxs-lookup"><span data-stu-id="e6c84-115">String</span></span>          | <span data-ttu-id="e6c84-116">操作 ID です。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="e6c84-116">The operation id. Read-only.</span></span> <span data-ttu-id="e6c84-117">サーバーを生成します。</span><span class="sxs-lookup"><span data-stu-id="e6c84-117">Server generated.</span></span>                                  |
| <span data-ttu-id="e6c84-118">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="e6c84-118">lastActionDateTime</span></span> | <span data-ttu-id="e6c84-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6c84-119">DateTimeOffset</span></span>  | <span data-ttu-id="e6c84-120">操作の最後の操作の時間です。</span><span class="sxs-lookup"><span data-stu-id="e6c84-120">The time of the last action of the operation.</span></span>                                   |
| <span data-ttu-id="e6c84-121">status</span><span class="sxs-lookup"><span data-stu-id="e6c84-121">status</span></span>             | <span data-ttu-id="e6c84-122">String</span><span class="sxs-lookup"><span data-stu-id="e6c84-122">String</span></span>          | <span data-ttu-id="e6c84-123">使用可能な値: `notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="e6c84-123">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="e6c84-124">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="e6c84-124">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="e6c84-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e6c84-125">Relationships</span></span>

<span data-ttu-id="e6c84-126">None</span><span class="sxs-lookup"><span data-stu-id="e6c84-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e6c84-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e6c84-127">JSON representation</span></span>

<span data-ttu-id="e6c84-128">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e6c84-128">The following is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.operation"
}-->
```json
{
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "status": "notStarted | running | completed | failed"
}
```

## <a name="example"></a><span data-ttu-id="e6c84-129">例</span><span class="sxs-lookup"><span data-stu-id="e6c84-129">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.operation"
}-->
```json
{
  "createdDateTime": "2018-09-06T15:58:41Z",
  "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "status": "completed"
}
```

<!-- uuid: 13fa92b1-3b41-498b-aab1-f943464a124f
2018-03-30 10:29:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/operation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
