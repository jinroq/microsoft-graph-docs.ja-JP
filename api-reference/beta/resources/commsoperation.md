---
title: commsOperation リソースの種類
description: 長時間実行されている特定の操作の状態。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a10b652179a8a3d369c07d34cb2681c4986b3abf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012899"
---
# <a name="commsoperation-resource-type"></a><span data-ttu-id="f4fe2-103">commsOperation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f4fe2-103">commsOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4fe2-104">長時間実行されている特定の操作の状態。</span><span class="sxs-lookup"><span data-stu-id="f4fe2-104">The status of certain long-running operations.</span></span>

## <a name="methods"></a><span data-ttu-id="f4fe2-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="f4fe2-105">Methods</span></span>
<span data-ttu-id="f4fe2-106">None</span><span class="sxs-lookup"><span data-stu-id="f4fe2-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="f4fe2-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f4fe2-107">Properties</span></span>

| <span data-ttu-id="f4fe2-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f4fe2-108">Property</span></span>           | <span data-ttu-id="f4fe2-109">型</span><span class="sxs-lookup"><span data-stu-id="f4fe2-109">Type</span></span>                        | <span data-ttu-id="f4fe2-110">説明</span><span class="sxs-lookup"><span data-stu-id="f4fe2-110">Description</span></span>                                                                     |
| :----------------- | :-------------------------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="f4fe2-111">clientContext</span><span class="sxs-lookup"><span data-stu-id="f4fe2-111">clientContext</span></span>      | <span data-ttu-id="f4fe2-112">String</span><span class="sxs-lookup"><span data-stu-id="f4fe2-112">String</span></span>                      | <span data-ttu-id="f4fe2-113">クライアントコンテキスト。</span><span class="sxs-lookup"><span data-stu-id="f4fe2-113">The client context.</span></span>                                                             |
| <span data-ttu-id="f4fe2-114">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f4fe2-114">createdDateTime</span></span>    | <span data-ttu-id="f4fe2-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4fe2-115">DateTimeOffset</span></span>              | <span data-ttu-id="f4fe2-116">操作の開始時刻。</span><span class="sxs-lookup"><span data-stu-id="f4fe2-116">The start time of the operation.</span></span>                                                |
| <span data-ttu-id="f4fe2-117">id</span><span class="sxs-lookup"><span data-stu-id="f4fe2-117">id</span></span>                 | <span data-ttu-id="f4fe2-118">文字列</span><span class="sxs-lookup"><span data-stu-id="f4fe2-118">String</span></span>                      | <span data-ttu-id="f4fe2-119">操作 id。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f4fe2-119">The operation id. Read-only.</span></span> <span data-ttu-id="f4fe2-120">サーバーによって生成されます。</span><span class="sxs-lookup"><span data-stu-id="f4fe2-120">Server generated.</span></span>                                  |
| <span data-ttu-id="f4fe2-121">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="f4fe2-121">lastActionDateTime</span></span> | <span data-ttu-id="f4fe2-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4fe2-122">DateTimeOffset</span></span>              | <span data-ttu-id="f4fe2-123">操作の最後の操作の時刻。</span><span class="sxs-lookup"><span data-stu-id="f4fe2-123">The time of the last action of the operation.</span></span>                                   |
| <span data-ttu-id="f4fe2-124">resultInfo</span><span class="sxs-lookup"><span data-stu-id="f4fe2-124">resultInfo</span></span>         | [<span data-ttu-id="f4fe2-125">resultInfo</span><span class="sxs-lookup"><span data-stu-id="f4fe2-125">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="f4fe2-126">結果の情報。</span><span class="sxs-lookup"><span data-stu-id="f4fe2-126">The result information.</span></span> <span data-ttu-id="f4fe2-127">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f4fe2-127">Read-only.</span></span> <span data-ttu-id="f4fe2-128">サーバーによって生成されます。</span><span class="sxs-lookup"><span data-stu-id="f4fe2-128">Server generated.</span></span>                            |
| <span data-ttu-id="f4fe2-129">status</span><span class="sxs-lookup"><span data-stu-id="f4fe2-129">status</span></span>             | <span data-ttu-id="f4fe2-130">String</span><span class="sxs-lookup"><span data-stu-id="f4fe2-130">String</span></span>                      | <span data-ttu-id="f4fe2-131">使用可能な値: `notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="f4fe2-131">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="f4fe2-132">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="f4fe2-132">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="f4fe2-133">関係</span><span class="sxs-lookup"><span data-stu-id="f4fe2-133">Relationships</span></span>
<span data-ttu-id="f4fe2-134">なし</span><span class="sxs-lookup"><span data-stu-id="f4fe2-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f4fe2-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f4fe2-135">JSON representation</span></span>

<span data-ttu-id="f4fe2-136">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f4fe2-136">The following is a JSON representation of the resource.</span></span>

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
  "resultInfo": { "@odata.type": "microsoft.graph.resultInfo" },
  "status": "notStarted | running | completed | failed"
}
```

## <a name="example"></a><span data-ttu-id="f4fe2-137">例</span><span class="sxs-lookup"><span data-stu-id="f4fe2-137">Example</span></span>

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
    "@odata.type": "microsoft.graph.resultInfo",
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
  "suppressions": []
}
-->
