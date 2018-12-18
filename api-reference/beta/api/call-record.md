---
title: '呼び出す: レコード'
description: 呼び出しを記録します。
author: VinodRavichandran
ms.openlocfilehash: 5de56ca417f5a6d06e8116802eeba2dd3d39e399
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303550"
---
# <a name="call-record"></a><span data-ttu-id="baab1-103">呼び出す: レコード</span><span class="sxs-lookup"><span data-stu-id="baab1-103">call: record</span></span>

> <span data-ttu-id="baab1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="baab1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="baab1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="baab1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="baab1-106">呼び出しを記録します。</span><span class="sxs-lookup"><span data-stu-id="baab1-106">Record the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="baab1-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="baab1-107">Permissions</span></span>
<span data-ttu-id="baab1-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="baab1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="baab1-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="baab1-110">Permission type</span></span> | <span data-ttu-id="baab1-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="baab1-111">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="baab1-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="baab1-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="baab1-113">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="baab1-113">Not Supported</span></span>        |
| <span data-ttu-id="baab1-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="baab1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="baab1-115">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="baab1-115">Not Supported</span></span>        |
| <span data-ttu-id="baab1-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="baab1-116">Application</span></span>     | <span data-ttu-id="baab1-117">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="baab1-117">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="baab1-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="baab1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/record
POST /applications/{id}/calls/{id}/record
```

## <a name="request-headers"></a><span data-ttu-id="baab1-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="baab1-119">Request headers</span></span>
| <span data-ttu-id="baab1-120">名前</span><span class="sxs-lookup"><span data-stu-id="baab1-120">Name</span></span>          | <span data-ttu-id="baab1-121">説明</span><span class="sxs-lookup"><span data-stu-id="baab1-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="baab1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="baab1-122">Authorization</span></span> | <span data-ttu-id="baab1-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="baab1-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="baab1-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="baab1-125">Request body</span></span>
<span data-ttu-id="baab1-126">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="baab1-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="baab1-127">パラメーター</span><span class="sxs-lookup"><span data-stu-id="baab1-127">Parameter</span></span>      | <span data-ttu-id="baab1-128">種類</span><span class="sxs-lookup"><span data-stu-id="baab1-128">Type</span></span>    |<span data-ttu-id="baab1-129">説明</span><span class="sxs-lookup"><span data-stu-id="baab1-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="baab1-130">メッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="baab1-130">prompts</span></span>|<span data-ttu-id="baab1-131">[mediaprompt](../resources/mediaprompt.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="baab1-131">[mediaprompt](../resources/mediaprompt.md) collection</span></span> | <span data-ttu-id="baab1-132">レコーディングの前に (もしあれば) を再生するメッセージのコレクションを開始します。</span><span class="sxs-lookup"><span data-stu-id="baab1-132">Collection of prompts to play (if any) before recording starts.</span></span> <span data-ttu-id="baab1-133">ユーザー"playPrompt"のアクションを個別に指定、またはほとんどすべてのレコードは、前のプロンプトに「記録」の一部として指定することができます。</span><span class="sxs-lookup"><span data-stu-id="baab1-133">Customers can choose to specify "playPrompt" action separately or specify as part of "record" - mostly all records are preceeded by a prompt</span></span> |
|<span data-ttu-id="baab1-134">bargeInAllowed</span><span class="sxs-lookup"><span data-stu-id="baab1-134">bargeInAllowed</span></span>|<span data-ttu-id="baab1-135">ブール型</span><span class="sxs-lookup"><span data-stu-id="baab1-135">Boolean</span></span>| <span data-ttu-id="baab1-136">プロンプトが終了する前に、選択肢を入力できるようにします。</span><span class="sxs-lookup"><span data-stu-id="baab1-136">Allow users to enter choice before prompt finishes.</span></span>                                                                 |
|<span data-ttu-id="baab1-137">initialSilenceTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="baab1-137">initialSilenceTimeoutInSeconds</span></span> | <span data-ttu-id="baab1-138">Int32</span><span class="sxs-lookup"><span data-stu-id="baab1-138">Int32</span></span>| <span data-ttu-id="baab1-139">最大初期無音タイムアウトし、操作が失敗、私たちの前にレコードの操作を始める時から使用します。</span><span class="sxs-lookup"><span data-stu-id="baab1-139">Maximum initial silence allowed from the time we start the record operation before we timeout and fail the operation.</span></span> <span data-ttu-id="baab1-140">プロンプトを再生していることは、プロンプトが終了するとこのタイマーが開始されます。</span><span class="sxs-lookup"><span data-stu-id="baab1-140">If we are playing a prompt, then this timer starts after prompt finishes.</span></span> |
|<span data-ttu-id="baab1-141">maxSilenceTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="baab1-141">maxSilenceTimeoutInSeconds</span></span>|<span data-ttu-id="baab1-142">Int32</span><span class="sxs-lookup"><span data-stu-id="baab1-142">Int32</span></span>| <span data-ttu-id="baab1-143">無音部分の最大のタイムアウト (秒) です。</span><span class="sxs-lookup"><span data-stu-id="baab1-143">The maximum silence timeout in seconds.</span></span>|
|<span data-ttu-id="baab1-144">maxRecordDurationInSeconds</span><span class="sxs-lookup"><span data-stu-id="baab1-144">maxRecordDurationInSeconds</span></span>|<span data-ttu-id="baab1-145">Int32</span><span class="sxs-lookup"><span data-stu-id="baab1-145">Int32</span></span>| <span data-ttu-id="baab1-146">秒単位で最大のレコードの期間です。</span><span class="sxs-lookup"><span data-stu-id="baab1-146">The maximum record duration in seconds.</span></span>|
|<span data-ttu-id="baab1-147">playBeep</span><span class="sxs-lookup"><span data-stu-id="baab1-147">playBeep</span></span>|<span data-ttu-id="baab1-148">ブール型</span><span class="sxs-lookup"><span data-stu-id="baab1-148">Boolean</span></span>| <span data-ttu-id="baab1-149">プロンプトを再生した後、ビープ音を再生します。</span><span class="sxs-lookup"><span data-stu-id="baab1-149">Plays a beep after playing the prompt.</span></span>|
|<span data-ttu-id="baab1-150">streamWhileRecording</span><span class="sxs-lookup"><span data-stu-id="baab1-150">streamWhileRecording</span></span>|<span data-ttu-id="baab1-151">ブール型</span><span class="sxs-lookup"><span data-stu-id="baab1-151">Boolean</span></span>|<span data-ttu-id="baab1-152">True の場合、リソースの場所に設定する場合、録画の開始と同時に提供されます。</span><span class="sxs-lookup"><span data-stu-id="baab1-152">If set to true, a resource location will be provided as soon as the recording starts.</span></span> |
|<span data-ttu-id="baab1-153">stopTones</span><span class="sxs-lookup"><span data-stu-id="baab1-153">stopTones</span></span>|<span data-ttu-id="baab1-154">String コレクション</span><span class="sxs-lookup"><span data-stu-id="baab1-154">String collection</span></span>|<span data-ttu-id="baab1-155">音の録音を終了するために指定を停止します。</span><span class="sxs-lookup"><span data-stu-id="baab1-155">Stop tones specified to end recording.</span></span>|
|<span data-ttu-id="baab1-156">clientContext</span><span class="sxs-lookup"><span data-stu-id="baab1-156">clientContext</span></span>|<span data-ttu-id="baab1-157">String</span><span class="sxs-lookup"><span data-stu-id="baab1-157">String</span></span>|<span data-ttu-id="baab1-158">クライアントのコンテキスト。</span><span class="sxs-lookup"><span data-stu-id="baab1-158">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="baab1-159">応答</span><span class="sxs-lookup"><span data-stu-id="baab1-159">Response</span></span>
<span data-ttu-id="baab1-160">返します。`202 Accepted`応答コードと、Location ヘッダーをこの要求用に作成された[commsOperation](../resources/commsoperation.md)の uri を持つ。</span><span class="sxs-lookup"><span data-stu-id="baab1-160">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="baab1-161">例</span><span class="sxs-lookup"><span data-stu-id="baab1-161">Example</span></span>
<span data-ttu-id="baab1-162">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="baab1-162">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="baab1-163">要求</span><span class="sxs-lookup"><span data-stu-id="baab1-163">Request</span></span>
<span data-ttu-id="baab1-164">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="baab1-164">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call_record"
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

##### <a name="response"></a><span data-ttu-id="baab1-165">応答</span><span class="sxs-lookup"><span data-stu-id="baab1-165">Response</span></span>

> <span data-ttu-id="baab1-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="baab1-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.recordOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="baab1-168">通知の操作が完了しました</span><span class="sxs-lookup"><span data-stu-id="baab1-168">Notification - operation completed</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "call: record",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
