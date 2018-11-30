---
title: commsOperation リソースの種類
description: 特定の実行時間の長い操作のステータス。
ms.openlocfilehash: d9adf240bff566dc0af5e369da24c7f8658a6c1c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071187"
---
# <a name="commsoperation-resource-type"></a><span data-ttu-id="13757-103">commsOperation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="13757-103">commsOperation resource type</span></span>

> <span data-ttu-id="13757-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="13757-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="13757-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="13757-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="13757-106">特定の実行時間の長い操作のステータス。</span><span class="sxs-lookup"><span data-stu-id="13757-106">The status of certain long-running operations.</span></span>

## <a name="methods"></a><span data-ttu-id="13757-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="13757-107">Methods</span></span>
<span data-ttu-id="13757-108">なし</span><span class="sxs-lookup"><span data-stu-id="13757-108">None</span></span>

## <a name="properties"></a><span data-ttu-id="13757-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="13757-109">Properties</span></span>

| <span data-ttu-id="13757-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="13757-110">Property</span></span>           | <span data-ttu-id="13757-111">型</span><span class="sxs-lookup"><span data-stu-id="13757-111">Type</span></span>                        | <span data-ttu-id="13757-112">説明</span><span class="sxs-lookup"><span data-stu-id="13757-112">Description</span></span>                                                                     |
| :----------------- | :-------------------------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="13757-113">clientContext</span><span class="sxs-lookup"><span data-stu-id="13757-113">clientContext</span></span>      | <span data-ttu-id="13757-114">String</span><span class="sxs-lookup"><span data-stu-id="13757-114">String</span></span>                      | <span data-ttu-id="13757-115">クライアントのコンテキスト。</span><span class="sxs-lookup"><span data-stu-id="13757-115">The client context.</span></span>                                                             |
| <span data-ttu-id="13757-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="13757-116">createdDateTime</span></span>    | <span data-ttu-id="13757-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13757-117">DateTimeOffset</span></span>              | <span data-ttu-id="13757-118">操作の開始時刻です。</span><span class="sxs-lookup"><span data-stu-id="13757-118">The start time of the operation.</span></span>                                                |
| <span data-ttu-id="13757-119">id</span><span class="sxs-lookup"><span data-stu-id="13757-119">id</span></span>                 | <span data-ttu-id="13757-120">String</span><span class="sxs-lookup"><span data-stu-id="13757-120">String</span></span>                      | <span data-ttu-id="13757-121">操作 ID です。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="13757-121">The operation id. Read-only.</span></span> <span data-ttu-id="13757-122">サーバーを生成します。</span><span class="sxs-lookup"><span data-stu-id="13757-122">Server generated.</span></span>                                  |
| <span data-ttu-id="13757-123">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="13757-123">lastActionDateTime</span></span> | <span data-ttu-id="13757-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13757-124">DateTimeOffset</span></span>              | <span data-ttu-id="13757-125">操作の最後の操作の時間です。</span><span class="sxs-lookup"><span data-stu-id="13757-125">The time of the last action of the operation.</span></span>                                   |
| <span data-ttu-id="13757-126">resultInfo</span><span class="sxs-lookup"><span data-stu-id="13757-126">resultInfo</span></span>         | [<span data-ttu-id="13757-127">resultInfo</span><span class="sxs-lookup"><span data-stu-id="13757-127">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="13757-128">結果の情報です。</span><span class="sxs-lookup"><span data-stu-id="13757-128">The result information.</span></span> <span data-ttu-id="13757-129">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="13757-129">Read-only.</span></span> <span data-ttu-id="13757-130">サーバーを生成します。</span><span class="sxs-lookup"><span data-stu-id="13757-130">Server generated.</span></span>                            |
| <span data-ttu-id="13757-131">status</span><span class="sxs-lookup"><span data-stu-id="13757-131">status</span></span>             | <span data-ttu-id="13757-132">String</span><span class="sxs-lookup"><span data-stu-id="13757-132">String</span></span>                      | <span data-ttu-id="13757-133">使用可能な値: `notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="13757-133">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="13757-134">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="13757-134">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="13757-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="13757-135">Relationships</span></span>
<span data-ttu-id="13757-136">なし</span><span class="sxs-lookup"><span data-stu-id="13757-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="13757-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="13757-137">JSON representation</span></span>

<span data-ttu-id="13757-138">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="13757-138">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="13757-139">使用例</span><span class="sxs-lookup"><span data-stu-id="13757-139">Example</span></span>

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
