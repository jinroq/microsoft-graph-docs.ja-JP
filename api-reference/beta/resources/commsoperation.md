---
title: commsOperation リソースの種類
description: 特定の実行時間の長い操作のステータス。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 79fc6801e95854b2530f8a28c13f7180ed02203f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957726"
---
# <a name="commsoperation-resource-type"></a><span data-ttu-id="79c56-103">commsOperation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="79c56-103">commsOperation resource type</span></span>

> <span data-ttu-id="79c56-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="79c56-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="79c56-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79c56-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="79c56-106">特定の実行時間の長い操作のステータス。</span><span class="sxs-lookup"><span data-stu-id="79c56-106">The status of certain long-running operations.</span></span>

## <a name="methods"></a><span data-ttu-id="79c56-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="79c56-107">Methods</span></span>
<span data-ttu-id="79c56-108">なし</span><span class="sxs-lookup"><span data-stu-id="79c56-108">None</span></span>

## <a name="properties"></a><span data-ttu-id="79c56-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="79c56-109">Properties</span></span>

| <span data-ttu-id="79c56-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="79c56-110">Property</span></span>           | <span data-ttu-id="79c56-111">種類</span><span class="sxs-lookup"><span data-stu-id="79c56-111">Type</span></span>                        | <span data-ttu-id="79c56-112">説明</span><span class="sxs-lookup"><span data-stu-id="79c56-112">Description</span></span>                                                                     |
| :----------------- | :-------------------------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="79c56-113">clientContext</span><span class="sxs-lookup"><span data-stu-id="79c56-113">clientContext</span></span>      | <span data-ttu-id="79c56-114">String</span><span class="sxs-lookup"><span data-stu-id="79c56-114">String</span></span>                      | <span data-ttu-id="79c56-115">クライアントのコンテキスト。</span><span class="sxs-lookup"><span data-stu-id="79c56-115">The client context.</span></span>                                                             |
| <span data-ttu-id="79c56-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="79c56-116">createdDateTime</span></span>    | <span data-ttu-id="79c56-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79c56-117">DateTimeOffset</span></span>              | <span data-ttu-id="79c56-118">操作の開始時刻です。</span><span class="sxs-lookup"><span data-stu-id="79c56-118">The start time of the operation.</span></span>                                                |
| <span data-ttu-id="79c56-119">id</span><span class="sxs-lookup"><span data-stu-id="79c56-119">id</span></span>                 | <span data-ttu-id="79c56-120">String</span><span class="sxs-lookup"><span data-stu-id="79c56-120">String</span></span>                      | <span data-ttu-id="79c56-121">操作 ID です。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="79c56-121">The operation id. Read-only.</span></span> <span data-ttu-id="79c56-122">サーバーを生成します。</span><span class="sxs-lookup"><span data-stu-id="79c56-122">Server generated.</span></span>                                  |
| <span data-ttu-id="79c56-123">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="79c56-123">lastActionDateTime</span></span> | <span data-ttu-id="79c56-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79c56-124">DateTimeOffset</span></span>              | <span data-ttu-id="79c56-125">操作の最後の操作の時間です。</span><span class="sxs-lookup"><span data-stu-id="79c56-125">The time of the last action of the operation.</span></span>                                   |
| <span data-ttu-id="79c56-126">resultInfo</span><span class="sxs-lookup"><span data-stu-id="79c56-126">resultInfo</span></span>         | [<span data-ttu-id="79c56-127">resultInfo</span><span class="sxs-lookup"><span data-stu-id="79c56-127">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="79c56-128">結果の情報です。</span><span class="sxs-lookup"><span data-stu-id="79c56-128">The result information.</span></span> <span data-ttu-id="79c56-129">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="79c56-129">Read-only.</span></span> <span data-ttu-id="79c56-130">サーバーを生成します。</span><span class="sxs-lookup"><span data-stu-id="79c56-130">Server generated.</span></span>                            |
| <span data-ttu-id="79c56-131">status</span><span class="sxs-lookup"><span data-stu-id="79c56-131">status</span></span>             | <span data-ttu-id="79c56-132">String</span><span class="sxs-lookup"><span data-stu-id="79c56-132">String</span></span>                      | <span data-ttu-id="79c56-133">使用可能な値: `notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="79c56-133">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="79c56-134">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="79c56-134">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="79c56-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="79c56-135">Relationships</span></span>
<span data-ttu-id="79c56-136">なし</span><span class="sxs-lookup"><span data-stu-id="79c56-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="79c56-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="79c56-137">JSON representation</span></span>

<span data-ttu-id="79c56-138">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="79c56-138">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="79c56-139">例</span><span class="sxs-lookup"><span data-stu-id="79c56-139">Example</span></span>

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
