---
title: '呼び出す: レコード'
description: 呼び出しを記録します。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 1f119cfece969c01e68773e5985eab4010dc9874
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574860"
---
# <a name="call-record"></a><span data-ttu-id="7550f-103">呼び出す: レコード</span><span class="sxs-lookup"><span data-stu-id="7550f-103">call: record</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7550f-104">呼び出しを記録します。</span><span class="sxs-lookup"><span data-stu-id="7550f-104">Record the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="7550f-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7550f-105">Permissions</span></span>
<span data-ttu-id="7550f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7550f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7550f-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7550f-108">Permission type</span></span> | <span data-ttu-id="7550f-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7550f-109">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="7550f-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7550f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="7550f-111">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="7550f-111">Not Supported</span></span>        |
| <span data-ttu-id="7550f-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7550f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7550f-113">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="7550f-113">Not Supported</span></span>        |
| <span data-ttu-id="7550f-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7550f-114">Application</span></span>     | <span data-ttu-id="7550f-115">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="7550f-115">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="7550f-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7550f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/record
POST /applications/{id}/calls/{id}/record
```

## <a name="request-headers"></a><span data-ttu-id="7550f-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7550f-117">Request headers</span></span>
| <span data-ttu-id="7550f-118">名前</span><span class="sxs-lookup"><span data-stu-id="7550f-118">Name</span></span>          | <span data-ttu-id="7550f-119">説明</span><span class="sxs-lookup"><span data-stu-id="7550f-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="7550f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7550f-120">Authorization</span></span> | <span data-ttu-id="7550f-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7550f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7550f-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="7550f-123">Request body</span></span>
<span data-ttu-id="7550f-124">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="7550f-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7550f-125">パラメーター</span><span class="sxs-lookup"><span data-stu-id="7550f-125">Parameter</span></span>      | <span data-ttu-id="7550f-126">型</span><span class="sxs-lookup"><span data-stu-id="7550f-126">Type</span></span>    |<span data-ttu-id="7550f-127">説明</span><span class="sxs-lookup"><span data-stu-id="7550f-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7550f-128">メッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="7550f-128">prompts</span></span>|<span data-ttu-id="7550f-129">[mediaPrompt](../resources/mediaprompt.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7550f-129">[mediaPrompt](../resources/mediaprompt.md) collection</span></span> | <span data-ttu-id="7550f-130">レコーディングの前に (もしあれば) を再生するメッセージのコレクションを開始します。</span><span class="sxs-lookup"><span data-stu-id="7550f-130">Collection of prompts to play (if any) before recording starts.</span></span> <span data-ttu-id="7550f-131">ユーザー"playPrompt"のアクションを個別に指定、またはほとんどすべてのレコードは、前のプロンプトに「記録」の一部として指定することができます。</span><span class="sxs-lookup"><span data-stu-id="7550f-131">Customers can choose to specify "playPrompt" action separately or specify as part of "record" - mostly all records are preceeded by a prompt</span></span> |
|<span data-ttu-id="7550f-132">bargeInAllowed</span><span class="sxs-lookup"><span data-stu-id="7550f-132">bargeInAllowed</span></span>|<span data-ttu-id="7550f-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="7550f-133">Boolean</span></span>| <span data-ttu-id="7550f-134">プロンプトが終了する前に、選択肢を入力できるようにします。</span><span class="sxs-lookup"><span data-stu-id="7550f-134">Allow users to enter choice before prompt finishes.</span></span>                                                                 |
|<span data-ttu-id="7550f-135">initialSilenceTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="7550f-135">initialSilenceTimeoutInSeconds</span></span> | <span data-ttu-id="7550f-136">Int32</span><span class="sxs-lookup"><span data-stu-id="7550f-136">Int32</span></span>| <span data-ttu-id="7550f-137">最大初期無音タイムアウトし、操作が失敗、私たちの前にレコードの操作を始める時から使用します。</span><span class="sxs-lookup"><span data-stu-id="7550f-137">Maximum initial silence allowed from the time we start the record operation before we timeout and fail the operation.</span></span> <span data-ttu-id="7550f-138">プロンプトを再生していることは、プロンプトが終了するとこのタイマーが開始されます。</span><span class="sxs-lookup"><span data-stu-id="7550f-138">If we are playing a prompt, then this timer starts after prompt finishes.</span></span> |
|<span data-ttu-id="7550f-139">maxSilenceTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="7550f-139">maxSilenceTimeoutInSeconds</span></span>|<span data-ttu-id="7550f-140">Int32</span><span class="sxs-lookup"><span data-stu-id="7550f-140">Int32</span></span>| <span data-ttu-id="7550f-141">無音部分の最大のタイムアウト (秒) です。</span><span class="sxs-lookup"><span data-stu-id="7550f-141">The maximum silence timeout in seconds.</span></span>|
|<span data-ttu-id="7550f-142">maxRecordDurationInSeconds</span><span class="sxs-lookup"><span data-stu-id="7550f-142">maxRecordDurationInSeconds</span></span>|<span data-ttu-id="7550f-143">Int32</span><span class="sxs-lookup"><span data-stu-id="7550f-143">Int32</span></span>| <span data-ttu-id="7550f-144">秒単位で最大のレコードの期間です。</span><span class="sxs-lookup"><span data-stu-id="7550f-144">The maximum record duration in seconds.</span></span>|
|<span data-ttu-id="7550f-145">playBeep</span><span class="sxs-lookup"><span data-stu-id="7550f-145">playBeep</span></span>|<span data-ttu-id="7550f-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="7550f-146">Boolean</span></span>| <span data-ttu-id="7550f-147">プロンプトを再生した後、ビープ音を再生します。</span><span class="sxs-lookup"><span data-stu-id="7550f-147">Plays a beep after playing the prompt.</span></span>|
|<span data-ttu-id="7550f-148">streamWhileRecording</span><span class="sxs-lookup"><span data-stu-id="7550f-148">streamWhileRecording</span></span>|<span data-ttu-id="7550f-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="7550f-149">Boolean</span></span>|<span data-ttu-id="7550f-150">True の場合、リソースの場所に設定する場合、録画の開始と同時に提供されます。</span><span class="sxs-lookup"><span data-stu-id="7550f-150">If set to true, a resource location will be provided as soon as the recording starts.</span></span> |
|<span data-ttu-id="7550f-151">stopTones</span><span class="sxs-lookup"><span data-stu-id="7550f-151">stopTones</span></span>|<span data-ttu-id="7550f-152">String コレクション</span><span class="sxs-lookup"><span data-stu-id="7550f-152">String collection</span></span>|<span data-ttu-id="7550f-153">音の録音を終了するために指定を停止します。</span><span class="sxs-lookup"><span data-stu-id="7550f-153">Stop tones specified to end recording.</span></span>|
|<span data-ttu-id="7550f-154">clientContext</span><span class="sxs-lookup"><span data-stu-id="7550f-154">clientContext</span></span>|<span data-ttu-id="7550f-155">String</span><span class="sxs-lookup"><span data-stu-id="7550f-155">String</span></span>|<span data-ttu-id="7550f-156">クライアントのコンテキスト。</span><span class="sxs-lookup"><span data-stu-id="7550f-156">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="7550f-157">応答</span><span class="sxs-lookup"><span data-stu-id="7550f-157">Response</span></span>
<span data-ttu-id="7550f-158">返します。`202 Accepted`応答コードと、Location ヘッダーをこの要求用に作成された[commsOperation](../resources/commsoperation.md)の uri を持つ。</span><span class="sxs-lookup"><span data-stu-id="7550f-158">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="7550f-159">例</span><span class="sxs-lookup"><span data-stu-id="7550f-159">Example</span></span>
<span data-ttu-id="7550f-160">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="7550f-160">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="7550f-161">要求</span><span class="sxs-lookup"><span data-stu-id="7550f-161">Request</span></span>
<span data-ttu-id="7550f-162">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="7550f-162">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call-record"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/record
Content-Type: application/json
Content-Length: 394

{
  "bargeInAllowed": true,
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
  "prompts": [
    {
      "@odata.type": "#microsoft.graph.mediaPrompt",
      "mediaInfo": {
        "uri": "https://cdn.contoso.com/beep.wav",
        "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
      },
      "loop": 5
    }
  ],
  "maxRecordDurationInSeconds": 1800,
  "initialSilenceTimeoutInSeconds": 10,
  "maxSilenceTimeoutInSeconds": 2,
  "recordingFormat": "wav",
  "playBeep": true,
  "streamWhileRecording": true,
  "stopTones": [ "#", "11", "*" ]
}
```

##### <a name="response"></a><span data-ttu-id="7550f-163">応答</span><span class="sxs-lookup"><span data-stu-id="7550f-163">Response</span></span>

> <span data-ttu-id="7550f-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="7550f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.recordOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="7550f-166">通知の操作が完了しました</span><span class="sxs-lookup"><span data-stu-id="7550f-166">Notification - operation completed</span></span>

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "deleted",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.recordOperation",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"54451\"",
        "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
        "status": "completed",
        "recordResourceLocation": "https://file.location/17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
        "recordResourceAccessToken": "<access-token>",
        "completionReason": "stopToneDetected"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call: record",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/call-record.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
