---
title: commsOperation リソースの種類
description: 特定の実行時間の長い操作のステータス。
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: d70ad6535d5ae829de4b9bac3c5b9fea9b53188b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821449"
---
# <a name="commsoperation-resource-type"></a><span data-ttu-id="b0bb8-103">commsOperation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b0bb8-103">commsOperation resource type</span></span>

> <span data-ttu-id="b0bb8-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b0bb8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b0bb8-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b0bb8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b0bb8-106">特定の実行時間の長い操作のステータス。</span><span class="sxs-lookup"><span data-stu-id="b0bb8-106">The status of certain long-running operations.</span></span>

## <a name="methods"></a><span data-ttu-id="b0bb8-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="b0bb8-107">Methods</span></span>
<span data-ttu-id="b0bb8-108">なし</span><span class="sxs-lookup"><span data-stu-id="b0bb8-108">None</span></span>

## <a name="properties"></a><span data-ttu-id="b0bb8-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b0bb8-109">Properties</span></span>

| <span data-ttu-id="b0bb8-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b0bb8-110">Property</span></span>           | <span data-ttu-id="b0bb8-111">種類</span><span class="sxs-lookup"><span data-stu-id="b0bb8-111">Type</span></span>                        | <span data-ttu-id="b0bb8-112">説明</span><span class="sxs-lookup"><span data-stu-id="b0bb8-112">Description</span></span>                                                                     |
| :----------------- | :-------------------------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="b0bb8-113">clientContext</span><span class="sxs-lookup"><span data-stu-id="b0bb8-113">clientContext</span></span>      | <span data-ttu-id="b0bb8-114">String</span><span class="sxs-lookup"><span data-stu-id="b0bb8-114">String</span></span>                      | <span data-ttu-id="b0bb8-115">クライアントのコンテキスト。</span><span class="sxs-lookup"><span data-stu-id="b0bb8-115">The client context.</span></span>                                                             |
| <span data-ttu-id="b0bb8-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b0bb8-116">createdDateTime</span></span>    | <span data-ttu-id="b0bb8-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0bb8-117">DateTimeOffset</span></span>              | <span data-ttu-id="b0bb8-118">操作の開始時刻です。</span><span class="sxs-lookup"><span data-stu-id="b0bb8-118">The start time of the operation.</span></span>                                                |
| <span data-ttu-id="b0bb8-119">id</span><span class="sxs-lookup"><span data-stu-id="b0bb8-119">id</span></span>                 | <span data-ttu-id="b0bb8-120">String</span><span class="sxs-lookup"><span data-stu-id="b0bb8-120">String</span></span>                      | <span data-ttu-id="b0bb8-121">操作 ID です。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b0bb8-121">The operation id. Read-only.</span></span> <span data-ttu-id="b0bb8-122">サーバーを生成します。</span><span class="sxs-lookup"><span data-stu-id="b0bb8-122">Server generated.</span></span>                                  |
| <span data-ttu-id="b0bb8-123">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="b0bb8-123">lastActionDateTime</span></span> | <span data-ttu-id="b0bb8-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0bb8-124">DateTimeOffset</span></span>              | <span data-ttu-id="b0bb8-125">操作の最後の操作の時間です。</span><span class="sxs-lookup"><span data-stu-id="b0bb8-125">The time of the last action of the operation.</span></span>                                   |
| <span data-ttu-id="b0bb8-126">resultInfo</span><span class="sxs-lookup"><span data-stu-id="b0bb8-126">resultInfo</span></span>         | [<span data-ttu-id="b0bb8-127">resultInfo</span><span class="sxs-lookup"><span data-stu-id="b0bb8-127">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="b0bb8-128">結果の情報です。</span><span class="sxs-lookup"><span data-stu-id="b0bb8-128">The result information.</span></span> <span data-ttu-id="b0bb8-129">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b0bb8-129">Read-only.</span></span> <span data-ttu-id="b0bb8-130">サーバーを生成します。</span><span class="sxs-lookup"><span data-stu-id="b0bb8-130">Server generated.</span></span>                            |
| <span data-ttu-id="b0bb8-131">status</span><span class="sxs-lookup"><span data-stu-id="b0bb8-131">status</span></span>             | <span data-ttu-id="b0bb8-132">String</span><span class="sxs-lookup"><span data-stu-id="b0bb8-132">String</span></span>                      | <span data-ttu-id="b0bb8-133">使用可能な値: `notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="b0bb8-133">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="b0bb8-134">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b0bb8-134">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="b0bb8-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b0bb8-135">Relationships</span></span>
<span data-ttu-id="b0bb8-136">なし</span><span class="sxs-lookup"><span data-stu-id="b0bb8-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0bb8-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b0bb8-137">JSON representation</span></span>

<span data-ttu-id="b0bb8-138">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b0bb8-138">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="b0bb8-139">例</span><span class="sxs-lookup"><span data-stu-id="b0bb8-139">Example</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "commsOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
