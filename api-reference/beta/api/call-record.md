---
title: '通話: レコード'
description: 通話を録音します。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4dc409a502b18da9c0e897054a7c1d6386fa096f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461298"
---
# <a name="call-record"></a><span data-ttu-id="5b739-103">通話: レコード</span><span class="sxs-lookup"><span data-stu-id="5b739-103">call: record</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b739-104">通話を録音します。</span><span class="sxs-lookup"><span data-stu-id="5b739-104">Record the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="5b739-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5b739-105">Permissions</span></span>
<span data-ttu-id="5b739-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5b739-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5b739-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5b739-108">Permission type</span></span> | <span data-ttu-id="5b739-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5b739-109">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="5b739-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5b739-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="5b739-111">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="5b739-111">Not Supported</span></span>        |
| <span data-ttu-id="5b739-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5b739-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b739-113">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="5b739-113">Not Supported</span></span>        |
| <span data-ttu-id="5b739-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5b739-114">Application</span></span>     | <span data-ttu-id="5b739-115">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="5b739-115">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="5b739-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5b739-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/record
POST /applications/{id}/calls/{id}/record
```

## <a name="request-headers"></a><span data-ttu-id="5b739-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5b739-117">Request headers</span></span>
| <span data-ttu-id="5b739-118">名前</span><span class="sxs-lookup"><span data-stu-id="5b739-118">Name</span></span>          | <span data-ttu-id="5b739-119">説明</span><span class="sxs-lookup"><span data-stu-id="5b739-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="5b739-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b739-120">Authorization</span></span> | <span data-ttu-id="5b739-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5b739-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5b739-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="5b739-123">Request body</span></span>
<span data-ttu-id="5b739-124">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="5b739-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5b739-125">パラメーター</span><span class="sxs-lookup"><span data-stu-id="5b739-125">Parameter</span></span>      | <span data-ttu-id="5b739-126">型</span><span class="sxs-lookup"><span data-stu-id="5b739-126">Type</span></span>    |<span data-ttu-id="5b739-127">説明</span><span class="sxs-lookup"><span data-stu-id="5b739-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5b739-128">促し</span><span class="sxs-lookup"><span data-stu-id="5b739-128">prompts</span></span>|<span data-ttu-id="5b739-129">[mediaprompt](../resources/mediaprompt.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="5b739-129">[mediaprompt](../resources/mediaprompt.md) collection</span></span> | <span data-ttu-id="5b739-130">レコーディングの開始前に再生するプロンプトのコレクション (ある場合)。</span><span class="sxs-lookup"><span data-stu-id="5b739-130">Collection of prompts to play (if any) before recording starts.</span></span> <span data-ttu-id="5b739-131">ユーザーは、"playprompt" アクションを個別に指定するか、"record" の一部として指定することができます。ほとんどすべてのレコードはプロンプトで preceeded されます。</span><span class="sxs-lookup"><span data-stu-id="5b739-131">Customers can choose to specify "playPrompt" action separately or specify as part of "record" - mostly all records are preceeded by a prompt</span></span> |
|<span data-ttu-id="5b739-132">bargeinallowed</span><span class="sxs-lookup"><span data-stu-id="5b739-132">bargeInAllowed</span></span>|<span data-ttu-id="5b739-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b739-133">Boolean</span></span>| <span data-ttu-id="5b739-134">ユーザーが選択肢を入力できるようにしてから、プロンプトを終了します。</span><span class="sxs-lookup"><span data-stu-id="5b739-134">Allow users to enter choice before prompt finishes.</span></span>                                                                 |
|<span data-ttu-id="5b739-135">initialSilenceTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="5b739-135">initialSilenceTimeoutInSeconds</span></span> | <span data-ttu-id="5b739-136">Int32</span><span class="sxs-lookup"><span data-stu-id="5b739-136">Int32</span></span>| <span data-ttu-id="5b739-137">操作を開始する前にレコード操作を開始するときに許容される最大初期無音</span><span class="sxs-lookup"><span data-stu-id="5b739-137">Maximum initial silence allowed from the time we start the record operation before we timeout and fail the operation.</span></span> <span data-ttu-id="5b739-138">プロンプトを再生している場合は、プロンプトが終了した後、このタイマーが開始されます。</span><span class="sxs-lookup"><span data-stu-id="5b739-138">If we are playing a prompt, then this timer starts after prompt finishes.</span></span> |
|<span data-ttu-id="5b739-139">maxSilenceTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="5b739-139">maxSilenceTimeoutInSeconds</span></span>|<span data-ttu-id="5b739-140">Int32</span><span class="sxs-lookup"><span data-stu-id="5b739-140">Int32</span></span>| <span data-ttu-id="5b739-141">最大無音タイムアウト (秒単位)。</span><span class="sxs-lookup"><span data-stu-id="5b739-141">The maximum silence timeout in seconds.</span></span>|
|<span data-ttu-id="5b739-142">maxRecordDurationInSeconds</span><span class="sxs-lookup"><span data-stu-id="5b739-142">maxRecordDurationInSeconds</span></span>|<span data-ttu-id="5b739-143">Int32</span><span class="sxs-lookup"><span data-stu-id="5b739-143">Int32</span></span>| <span data-ttu-id="5b739-144">最大レコード期間 (秒単位)。</span><span class="sxs-lookup"><span data-stu-id="5b739-144">The maximum record duration in seconds.</span></span>|
|<span data-ttu-id="5b739-145">再生のビープ音</span><span class="sxs-lookup"><span data-stu-id="5b739-145">playBeep</span></span>|<span data-ttu-id="5b739-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b739-146">Boolean</span></span>| <span data-ttu-id="5b739-147">プロンプトを再生した後、ビープ音を鳴らします。</span><span class="sxs-lookup"><span data-stu-id="5b739-147">Plays a beep after playing the prompt.</span></span>|
|<span data-ttu-id="5b739-148">streamWhileRecording</span><span class="sxs-lookup"><span data-stu-id="5b739-148">streamWhileRecording</span></span>|<span data-ttu-id="5b739-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b739-149">Boolean</span></span>|<span data-ttu-id="5b739-150">true に設定すると、レコーディングが開始されるとすぐにリソースの場所が提供されます。</span><span class="sxs-lookup"><span data-stu-id="5b739-150">If set to true, a resource location will be provided as soon as the recording starts.</span></span> |
|<span data-ttu-id="5b739-151">stoptones</span><span class="sxs-lookup"><span data-stu-id="5b739-151">stopTones</span></span>|<span data-ttu-id="5b739-152">String collection</span><span class="sxs-lookup"><span data-stu-id="5b739-152">String collection</span></span>|<span data-ttu-id="5b739-153">録音を終了するために指定されたトーンを停止します。</span><span class="sxs-lookup"><span data-stu-id="5b739-153">Stop tones specified to end recording.</span></span>|
|<span data-ttu-id="5b739-154">clientContext</span><span class="sxs-lookup"><span data-stu-id="5b739-154">clientContext</span></span>|<span data-ttu-id="5b739-155">String</span><span class="sxs-lookup"><span data-stu-id="5b739-155">String</span></span>|<span data-ttu-id="5b739-156">クライアントコンテキスト。</span><span class="sxs-lookup"><span data-stu-id="5b739-156">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="5b739-157">応答</span><span class="sxs-lookup"><span data-stu-id="5b739-157">Response</span></span>
<span data-ttu-id="5b739-158">この`202 Accepted`要求に対して作成された[commsOperation](../resources/commsoperation.md)への uri を持つ応答コードと位置ヘッダーを返します。</span><span class="sxs-lookup"><span data-stu-id="5b739-158">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="5b739-159">例</span><span class="sxs-lookup"><span data-stu-id="5b739-159">Example</span></span>
<span data-ttu-id="5b739-160">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="5b739-160">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="5b739-161">要求</span><span class="sxs-lookup"><span data-stu-id="5b739-161">Request</span></span>
<span data-ttu-id="5b739-162">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="5b739-162">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="5b739-163">応答</span><span class="sxs-lookup"><span data-stu-id="5b739-163">Response</span></span>

> <span data-ttu-id="5b739-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="5b739-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.recordOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="5b739-166">通知-操作が完了しました</span><span class="sxs-lookup"><span data-stu-id="5b739-166">Notification - operation completed</span></span>

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
