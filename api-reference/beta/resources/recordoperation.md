---
title: recordOperation リソースの種類
description: RecordOperation 型
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 6b9deb566e5b527a9f20db69441fa96908212a38
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512508"
---
# <a name="recordoperation-resource-type"></a><span data-ttu-id="4f26c-103">recordOperation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4f26c-103">recordOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f26c-104">RecordOperation 型</span><span class="sxs-lookup"><span data-stu-id="4f26c-104">The recordOperation type</span></span>

## <a name="properties"></a><span data-ttu-id="4f26c-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4f26c-105">Properties</span></span>

| <span data-ttu-id="4f26c-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4f26c-106">Property</span></span>                       | <span data-ttu-id="4f26c-107">型</span><span class="sxs-lookup"><span data-stu-id="4f26c-107">Type</span></span>                        | <span data-ttu-id="4f26c-108">説明</span><span class="sxs-lookup"><span data-stu-id="4f26c-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="4f26c-109">ClientContext</span><span class="sxs-lookup"><span data-stu-id="4f26c-109">clientContext</span></span>                  | <span data-ttu-id="4f26c-110">String</span><span class="sxs-lookup"><span data-stu-id="4f26c-110">String</span></span>                      | <span data-ttu-id="4f26c-111">クライアントのコンテキスト。</span><span class="sxs-lookup"><span data-stu-id="4f26c-111">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="4f26c-112">completionReason</span><span class="sxs-lookup"><span data-stu-id="4f26c-112">completionReason</span></span>               | <span data-ttu-id="4f26c-113">String</span><span class="sxs-lookup"><span data-stu-id="4f26c-113">String</span></span>                      | <span data-ttu-id="4f26c-114">可能な値は、`operationCanceled`、`stopToneDetected`、`maxRecordDurationReached`、`initialSilenceTimeout`、`maxSilenceTimeout`、`playPromptFailed`、`playBeepFailed`、`mediaReceiveTimeout`、`unspecifiedError`、`none` です。</span><span class="sxs-lookup"><span data-stu-id="4f26c-114">Possible values are: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`.</span></span> |
| <span data-ttu-id="4f26c-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4f26c-115">createdDateTime</span></span>                | <span data-ttu-id="4f26c-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f26c-116">DateTimeOffset</span></span>              | <span data-ttu-id="4f26c-117">レコーディングが作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="4f26c-117">The time when the recording was created.</span></span>                                                                                                          |
| <span data-ttu-id="4f26c-118">id</span><span class="sxs-lookup"><span data-stu-id="4f26c-118">id</span></span>                             | <span data-ttu-id="4f26c-119">String</span><span class="sxs-lookup"><span data-stu-id="4f26c-119">String</span></span>                      | <span data-ttu-id="4f26c-120">サーバー操作の id です。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4f26c-120">The server operation id. Read-only.</span></span> <span data-ttu-id="4f26c-121">サーバーを生成します。</span><span class="sxs-lookup"><span data-stu-id="4f26c-121">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="4f26c-122">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="4f26c-122">lastActionDateTime</span></span>             | <span data-ttu-id="4f26c-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f26c-123">DateTimeOffset</span></span>              | <span data-ttu-id="4f26c-124">操作の最後の操作の時間です。</span><span class="sxs-lookup"><span data-stu-id="4f26c-124">The time of the last action of the operation.</span></span>                                                                                                     |
| <span data-ttu-id="4f26c-125">recordResourceAccessToken</span><span class="sxs-lookup"><span data-stu-id="4f26c-125">recordResourceAccessToken</span></span>      | <span data-ttu-id="4f26c-126">String</span><span class="sxs-lookup"><span data-stu-id="4f26c-126">String</span></span>                      | <span data-ttu-id="4f26c-127">記録を取得するために必要なアクセス トークンです。</span><span class="sxs-lookup"><span data-stu-id="4f26c-127">The access token required to retrieve the recording.</span></span>                                                                                              |
| <span data-ttu-id="4f26c-128">recordResourceLocation</span><span class="sxs-lookup"><span data-stu-id="4f26c-128">recordResourceLocation</span></span>         | <span data-ttu-id="4f26c-129">String</span><span class="sxs-lookup"><span data-stu-id="4f26c-129">String</span></span>                      | <span data-ttu-id="4f26c-130">記録が保存されている場所です。</span><span class="sxs-lookup"><span data-stu-id="4f26c-130">The location where the recording is located.</span></span>                                                                                                      |
| <span data-ttu-id="4f26c-131">resultInfo</span><span class="sxs-lookup"><span data-stu-id="4f26c-131">resultInfo</span></span>                     | [<span data-ttu-id="4f26c-132">resultInfo</span><span class="sxs-lookup"><span data-stu-id="4f26c-132">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="4f26c-133">結果の情報です。</span><span class="sxs-lookup"><span data-stu-id="4f26c-133">The result information.</span></span>  <span data-ttu-id="4f26c-134">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4f26c-134">Read-only.</span></span> <span data-ttu-id="4f26c-135">サーバーを生成します。</span><span class="sxs-lookup"><span data-stu-id="4f26c-135">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="4f26c-136">status</span><span class="sxs-lookup"><span data-stu-id="4f26c-136">status</span></span>                         | <span data-ttu-id="4f26c-137">String</span><span class="sxs-lookup"><span data-stu-id="4f26c-137">String</span></span>                      | <span data-ttu-id="4f26c-138">使用可能な値: `notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="4f26c-138">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="4f26c-139">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4f26c-139">Read-only.</span></span> <span data-ttu-id="4f26c-140">サーバーを生成します。</span><span class="sxs-lookup"><span data-stu-id="4f26c-140">Server generated.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="4f26c-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4f26c-141">Relationships</span></span>
<span data-ttu-id="4f26c-142">なし</span><span class="sxs-lookup"><span data-stu-id="4f26c-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4f26c-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4f26c-143">JSON representation</span></span>

<span data-ttu-id="4f26c-144">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4f26c-144">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="4f26c-145">例</span><span class="sxs-lookup"><span data-stu-id="4f26c-145">Example</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/recordoperation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
