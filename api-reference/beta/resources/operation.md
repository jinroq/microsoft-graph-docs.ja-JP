---
title: operation リソースの種類
description: 長時間実行されている操作の状態。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 237e16373db30db9f4a9ed61c6182f6dd826d956
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966364"
---
# <a name="operation-resource-type"></a><span data-ttu-id="b931c-103">operation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b931c-103">operation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b931c-104">長時間実行されている操作の状態。</span><span class="sxs-lookup"><span data-stu-id="b931c-104">The status of a long-running operation.</span></span>

## <a name="methods"></a><span data-ttu-id="b931c-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="b931c-105">Methods</span></span>

<span data-ttu-id="b931c-106">None</span><span class="sxs-lookup"><span data-stu-id="b931c-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="b931c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b931c-107">Properties</span></span>

| <span data-ttu-id="b931c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b931c-108">Property</span></span>           | <span data-ttu-id="b931c-109">型</span><span class="sxs-lookup"><span data-stu-id="b931c-109">Type</span></span>            | <span data-ttu-id="b931c-110">説明</span><span class="sxs-lookup"><span data-stu-id="b931c-110">Description</span></span>                                                                     |
| :----------------- | :-------------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="b931c-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b931c-111">createdDateTime</span></span>    | <span data-ttu-id="b931c-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b931c-112">DateTimeOffset</span></span>  | <span data-ttu-id="b931c-113">操作の開始時刻。</span><span class="sxs-lookup"><span data-stu-id="b931c-113">The start time of the operation.</span></span>                                                |
| <span data-ttu-id="b931c-114">id</span><span class="sxs-lookup"><span data-stu-id="b931c-114">id</span></span>                 | <span data-ttu-id="b931c-115">文字列</span><span class="sxs-lookup"><span data-stu-id="b931c-115">String</span></span>          | <span data-ttu-id="b931c-116">操作 id。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b931c-116">The operation id. Read-only.</span></span> <span data-ttu-id="b931c-117">サーバーによって生成されます。</span><span class="sxs-lookup"><span data-stu-id="b931c-117">Server generated.</span></span>                                  |
| <span data-ttu-id="b931c-118">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="b931c-118">lastActionDateTime</span></span> | <span data-ttu-id="b931c-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b931c-119">DateTimeOffset</span></span>  | <span data-ttu-id="b931c-120">操作の最後の操作の時刻。</span><span class="sxs-lookup"><span data-stu-id="b931c-120">The time of the last action of the operation.</span></span>                                   |
| <span data-ttu-id="b931c-121">status</span><span class="sxs-lookup"><span data-stu-id="b931c-121">status</span></span>             | <span data-ttu-id="b931c-122">String</span><span class="sxs-lookup"><span data-stu-id="b931c-122">String</span></span>          | <span data-ttu-id="b931c-123">使用可能な値: `notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="b931c-123">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="b931c-124">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b931c-124">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="b931c-125">関係</span><span class="sxs-lookup"><span data-stu-id="b931c-125">Relationships</span></span>

<span data-ttu-id="b931c-126">なし</span><span class="sxs-lookup"><span data-stu-id="b931c-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b931c-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b931c-127">JSON representation</span></span>

<span data-ttu-id="b931c-128">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b931c-128">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="b931c-129">例</span><span class="sxs-lookup"><span data-stu-id="b931c-129">Example</span></span>

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
  "suppressions": []
}
-->
