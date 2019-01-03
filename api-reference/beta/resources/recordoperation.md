---
title: recordOperation リソースの種類
description: RecordOperation 型
author: VinodRavichandran
ms.openlocfilehash: 54b39f30df1dd53a95260b549ae9fab2eedddfd8
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380423"
---
# <a name="recordoperation-resource-type"></a><span data-ttu-id="35d96-103">recordOperation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="35d96-103">recordOperation resource type</span></span>

> <span data-ttu-id="35d96-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="35d96-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="35d96-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="35d96-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="35d96-106">RecordOperation 型</span><span class="sxs-lookup"><span data-stu-id="35d96-106">The recordOperation type</span></span>

## <a name="properties"></a><span data-ttu-id="35d96-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="35d96-107">Properties</span></span>

| <span data-ttu-id="35d96-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="35d96-108">Property</span></span>                       | <span data-ttu-id="35d96-109">型</span><span class="sxs-lookup"><span data-stu-id="35d96-109">Type</span></span>                        | <span data-ttu-id="35d96-110">説明</span><span class="sxs-lookup"><span data-stu-id="35d96-110">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="35d96-111">clientContext</span><span class="sxs-lookup"><span data-stu-id="35d96-111">clientContext</span></span>                  | <span data-ttu-id="35d96-112">String</span><span class="sxs-lookup"><span data-stu-id="35d96-112">String</span></span>                      | <span data-ttu-id="35d96-113">クライアントのコンテキスト。</span><span class="sxs-lookup"><span data-stu-id="35d96-113">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="35d96-114">completionReason</span><span class="sxs-lookup"><span data-stu-id="35d96-114">completionReason</span></span>               | <span data-ttu-id="35d96-115">String</span><span class="sxs-lookup"><span data-stu-id="35d96-115">String</span></span>                      | <span data-ttu-id="35d96-116">可能な値は、`operationCanceled`、`stopToneDetected`、`maxRecordDurationReached`、`initialSilenceTimeout`、`maxSilenceTimeout`、`playPromptFailed`、`playBeepFailed`、`mediaReceiveTimeout`、`unspecifiedError`、`none` です。</span><span class="sxs-lookup"><span data-stu-id="35d96-116">Possible values are: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`.</span></span> |
| <span data-ttu-id="35d96-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="35d96-117">createdDateTime</span></span>                | <span data-ttu-id="35d96-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35d96-118">DateTimeOffset</span></span>              | <span data-ttu-id="35d96-119">レコーディングが作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="35d96-119">The time when the recording was created.</span></span>                                                                                                          |
| <span data-ttu-id="35d96-120">id</span><span class="sxs-lookup"><span data-stu-id="35d96-120">id</span></span>                             | <span data-ttu-id="35d96-121">String</span><span class="sxs-lookup"><span data-stu-id="35d96-121">String</span></span>                      | <span data-ttu-id="35d96-122">サーバー操作の id です。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="35d96-122">The server operation id. Read-only.</span></span> <span data-ttu-id="35d96-123">サーバーを生成します。</span><span class="sxs-lookup"><span data-stu-id="35d96-123">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="35d96-124">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="35d96-124">lastActionDateTime</span></span>             | <span data-ttu-id="35d96-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35d96-125">DateTimeOffset</span></span>              | <span data-ttu-id="35d96-126">操作の最後の操作の時間です。</span><span class="sxs-lookup"><span data-stu-id="35d96-126">The time of the last action of the operation.</span></span>                                                                                                     |
| <span data-ttu-id="35d96-127">recordResourceAccessToken</span><span class="sxs-lookup"><span data-stu-id="35d96-127">recordResourceAccessToken</span></span>      | <span data-ttu-id="35d96-128">String</span><span class="sxs-lookup"><span data-stu-id="35d96-128">String</span></span>                      | <span data-ttu-id="35d96-129">記録を取得するために必要なアクセス トークンです。</span><span class="sxs-lookup"><span data-stu-id="35d96-129">The access token required to retrieve the recording.</span></span>                                                                                              |
| <span data-ttu-id="35d96-130">recordResourceLocation</span><span class="sxs-lookup"><span data-stu-id="35d96-130">recordResourceLocation</span></span>         | <span data-ttu-id="35d96-131">String</span><span class="sxs-lookup"><span data-stu-id="35d96-131">String</span></span>                      | <span data-ttu-id="35d96-132">記録が保存されている場所です。</span><span class="sxs-lookup"><span data-stu-id="35d96-132">The location where the recording is located.</span></span>                                                                                                      |
| <span data-ttu-id="35d96-133">resultInfo</span><span class="sxs-lookup"><span data-stu-id="35d96-133">resultInfo</span></span>                     | [<span data-ttu-id="35d96-134">resultInfo</span><span class="sxs-lookup"><span data-stu-id="35d96-134">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="35d96-135">結果の情報です。</span><span class="sxs-lookup"><span data-stu-id="35d96-135">The result information.</span></span>  <span data-ttu-id="35d96-136">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="35d96-136">Read-only.</span></span> <span data-ttu-id="35d96-137">サーバーを生成します。</span><span class="sxs-lookup"><span data-stu-id="35d96-137">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="35d96-138">status</span><span class="sxs-lookup"><span data-stu-id="35d96-138">status</span></span>                         | <span data-ttu-id="35d96-139">String</span><span class="sxs-lookup"><span data-stu-id="35d96-139">String</span></span>                      | <span data-ttu-id="35d96-140">使用可能な値: `notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="35d96-140">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="35d96-141">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="35d96-141">Read-only.</span></span> <span data-ttu-id="35d96-142">サーバーを生成します。</span><span class="sxs-lookup"><span data-stu-id="35d96-142">Server generated.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="35d96-143">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="35d96-143">Relationships</span></span>
<span data-ttu-id="35d96-144">なし</span><span class="sxs-lookup"><span data-stu-id="35d96-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="35d96-145">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="35d96-145">JSON representation</span></span>

<span data-ttu-id="35d96-146">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="35d96-146">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="35d96-147">例</span><span class="sxs-lookup"><span data-stu-id="35d96-147">Example</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "recordOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->