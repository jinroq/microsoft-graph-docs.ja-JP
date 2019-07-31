---
title: recordOperation リソースの種類
description: RecordOperation の種類
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 00b05cd86eeb9cf8be26cdc09fb8a9b254b510db
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008804"
---
# <a name="recordoperation-resource-type"></a><span data-ttu-id="b9fc3-103">recordOperation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b9fc3-103">recordOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9fc3-104">RecordOperation の種類</span><span class="sxs-lookup"><span data-stu-id="b9fc3-104">The recordOperation type</span></span>

## <a name="properties"></a><span data-ttu-id="b9fc3-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b9fc3-105">Properties</span></span>

| <span data-ttu-id="b9fc3-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b9fc3-106">Property</span></span>                       | <span data-ttu-id="b9fc3-107">型</span><span class="sxs-lookup"><span data-stu-id="b9fc3-107">Type</span></span>                        | <span data-ttu-id="b9fc3-108">説明</span><span class="sxs-lookup"><span data-stu-id="b9fc3-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="b9fc3-109">clientContext</span><span class="sxs-lookup"><span data-stu-id="b9fc3-109">clientContext</span></span>                  | <span data-ttu-id="b9fc3-110">String</span><span class="sxs-lookup"><span data-stu-id="b9fc3-110">String</span></span>                      | <span data-ttu-id="b9fc3-111">クライアントコンテキスト。</span><span class="sxs-lookup"><span data-stu-id="b9fc3-111">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="b9fc3-112">「補完の理由」</span><span class="sxs-lookup"><span data-stu-id="b9fc3-112">completionReason</span></span>               | <span data-ttu-id="b9fc3-113">String</span><span class="sxs-lookup"><span data-stu-id="b9fc3-113">String</span></span>                      | <span data-ttu-id="b9fc3-114">可能な値は、`operationCanceled`、`stopToneDetected`、`maxRecordDurationReached`、`initialSilenceTimeout`、`maxSilenceTimeout`、`playPromptFailed`、`playBeepFailed`、`mediaReceiveTimeout`、`unspecifiedError`、`none` です。</span><span class="sxs-lookup"><span data-stu-id="b9fc3-114">Possible values are: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`.</span></span> |
| <span data-ttu-id="b9fc3-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b9fc3-115">createdDateTime</span></span>                | <span data-ttu-id="b9fc3-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9fc3-116">DateTimeOffset</span></span>              | <span data-ttu-id="b9fc3-117">レコーディングが作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="b9fc3-117">The time when the recording was created.</span></span>                                                                                                          |
| <span data-ttu-id="b9fc3-118">id</span><span class="sxs-lookup"><span data-stu-id="b9fc3-118">id</span></span>                             | <span data-ttu-id="b9fc3-119">文字列</span><span class="sxs-lookup"><span data-stu-id="b9fc3-119">String</span></span>                      | <span data-ttu-id="b9fc3-120">サーバー操作 id。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b9fc3-120">The server operation id. Read-only.</span></span> <span data-ttu-id="b9fc3-121">サーバーによって生成されます。</span><span class="sxs-lookup"><span data-stu-id="b9fc3-121">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="b9fc3-122">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="b9fc3-122">lastActionDateTime</span></span>             | <span data-ttu-id="b9fc3-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9fc3-123">DateTimeOffset</span></span>              | <span data-ttu-id="b9fc3-124">操作の最後の操作の時刻。</span><span class="sxs-lookup"><span data-stu-id="b9fc3-124">The time of the last action of the operation.</span></span>                                                                                                     |
| <span data-ttu-id="b9fc3-125">recordResourceAccessToken</span><span class="sxs-lookup"><span data-stu-id="b9fc3-125">recordResourceAccessToken</span></span>      | <span data-ttu-id="b9fc3-126">String</span><span class="sxs-lookup"><span data-stu-id="b9fc3-126">String</span></span>                      | <span data-ttu-id="b9fc3-127">レコーディングを取得するために必要なアクセストークン。</span><span class="sxs-lookup"><span data-stu-id="b9fc3-127">The access token required to retrieve the recording.</span></span>                                                                                              |
| <span data-ttu-id="b9fc3-128">recordResourceLocation</span><span class="sxs-lookup"><span data-stu-id="b9fc3-128">recordResourceLocation</span></span>         | <span data-ttu-id="b9fc3-129">String</span><span class="sxs-lookup"><span data-stu-id="b9fc3-129">String</span></span>                      | <span data-ttu-id="b9fc3-130">レコーディングが配置されている場所。</span><span class="sxs-lookup"><span data-stu-id="b9fc3-130">The location where the recording is located.</span></span>                                                                                                      |
| <span data-ttu-id="b9fc3-131">resultInfo</span><span class="sxs-lookup"><span data-stu-id="b9fc3-131">resultInfo</span></span>                     | [<span data-ttu-id="b9fc3-132">resultInfo</span><span class="sxs-lookup"><span data-stu-id="b9fc3-132">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="b9fc3-133">結果の情報。</span><span class="sxs-lookup"><span data-stu-id="b9fc3-133">The result information.</span></span>  <span data-ttu-id="b9fc3-134">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b9fc3-134">Read-only.</span></span> <span data-ttu-id="b9fc3-135">サーバーによって生成されます。</span><span class="sxs-lookup"><span data-stu-id="b9fc3-135">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="b9fc3-136">status</span><span class="sxs-lookup"><span data-stu-id="b9fc3-136">status</span></span>                         | <span data-ttu-id="b9fc3-137">String</span><span class="sxs-lookup"><span data-stu-id="b9fc3-137">String</span></span>                      | <span data-ttu-id="b9fc3-138">使用可能な値: `notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="b9fc3-138">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="b9fc3-139">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b9fc3-139">Read-only.</span></span> <span data-ttu-id="b9fc3-140">サーバーによって生成されます。</span><span class="sxs-lookup"><span data-stu-id="b9fc3-140">Server generated.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="b9fc3-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b9fc3-141">Relationships</span></span>
<span data-ttu-id="b9fc3-142">なし</span><span class="sxs-lookup"><span data-stu-id="b9fc3-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b9fc3-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b9fc3-143">JSON representation</span></span>

<span data-ttu-id="b9fc3-144">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b9fc3-144">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recordOperation"
}-->
```json
{
  "clientContext": "String",
  "completionReason": "operationCanceled | stopToneDetected | maxRecordDurationReached | initialSilenceTimeout | maxSilenceTimeout | playPromptFailed | playBeepFailed | mediaReceiveTimeout | unspecifiedError | none",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "recordResourceAccessToken": "String",
  "recordResourceLocation": "String",
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

## <a name="example"></a><span data-ttu-id="b9fc3-145">例</span><span class="sxs-lookup"><span data-stu-id="b9fc3-145">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.recordOperation",
  "truncated": true
}-->
```json
{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
  "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "recordResourceAccessToken": "<access-token>",
  "recordResourceLocation": "https://resource.location/ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "status": "completed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "recordOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
