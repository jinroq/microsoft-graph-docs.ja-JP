---
title: オペレーション リソースの種類
description: 実行時間の長い操作のステータス。
ms.openlocfilehash: 71e6a1c47e1f3b18f1481700320779714d716bec
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069168"
---
# <a name="operation-resource-type"></a><span data-ttu-id="83f05-103">オペレーション リソースの種類</span><span class="sxs-lookup"><span data-stu-id="83f05-103">operation resource type</span></span>

> <span data-ttu-id="83f05-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="83f05-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="83f05-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="83f05-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="83f05-106">実行時間の長い操作のステータス。</span><span class="sxs-lookup"><span data-stu-id="83f05-106">The status of a long-running operation.</span></span>

## <a name="methods"></a><span data-ttu-id="83f05-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="83f05-107">Methods</span></span>

<span data-ttu-id="83f05-108">なし</span><span class="sxs-lookup"><span data-stu-id="83f05-108">None</span></span>

## <a name="properties"></a><span data-ttu-id="83f05-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="83f05-109">Properties</span></span>

| <span data-ttu-id="83f05-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="83f05-110">Property</span></span>           | <span data-ttu-id="83f05-111">型</span><span class="sxs-lookup"><span data-stu-id="83f05-111">Type</span></span>            | <span data-ttu-id="83f05-112">説明</span><span class="sxs-lookup"><span data-stu-id="83f05-112">Description</span></span>                                                                     |
| :----------------- | :-------------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="83f05-113">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="83f05-113">createdDateTime</span></span>    | <span data-ttu-id="83f05-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83f05-114">DateTimeOffset</span></span>  | <span data-ttu-id="83f05-115">操作の開始時刻です。</span><span class="sxs-lookup"><span data-stu-id="83f05-115">The start time of the operation.</span></span>                                                |
| <span data-ttu-id="83f05-116">id</span><span class="sxs-lookup"><span data-stu-id="83f05-116">id</span></span>                 | <span data-ttu-id="83f05-117">String</span><span class="sxs-lookup"><span data-stu-id="83f05-117">String</span></span>          | <span data-ttu-id="83f05-118">操作 ID です。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="83f05-118">The operation id. Read-only.</span></span> <span data-ttu-id="83f05-119">サーバーを生成します。</span><span class="sxs-lookup"><span data-stu-id="83f05-119">Server generated.</span></span>                                  |
| <span data-ttu-id="83f05-120">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="83f05-120">lastActionDateTime</span></span> | <span data-ttu-id="83f05-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83f05-121">DateTimeOffset</span></span>  | <span data-ttu-id="83f05-122">操作の最後の操作の時間です。</span><span class="sxs-lookup"><span data-stu-id="83f05-122">The time of the last action of the operation.</span></span>                                   |
| <span data-ttu-id="83f05-123">status</span><span class="sxs-lookup"><span data-stu-id="83f05-123">status</span></span>             | <span data-ttu-id="83f05-124">String</span><span class="sxs-lookup"><span data-stu-id="83f05-124">String</span></span>          | <span data-ttu-id="83f05-125">使用可能な値: `notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="83f05-125">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="83f05-126">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="83f05-126">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="83f05-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="83f05-127">Relationships</span></span>

<span data-ttu-id="83f05-128">なし</span><span class="sxs-lookup"><span data-stu-id="83f05-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="83f05-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="83f05-129">JSON representation</span></span>

<span data-ttu-id="83f05-130">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="83f05-130">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="83f05-131">使用例</span><span class="sxs-lookup"><span data-stu-id="83f05-131">Example</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->