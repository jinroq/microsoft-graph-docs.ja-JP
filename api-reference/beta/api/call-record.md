---
title: '通話: レコード'
description: 通話を録音します。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 473816bb52d441b4111632a69d767319ff59a17e
ms.sourcegitcommit: bbed891d16995b4a8ce866169dddb96abdc28776
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/02/2019
ms.locfileid: "36062013"
---
# <a name="call-record"></a><span data-ttu-id="8787e-103">通話: レコード</span><span class="sxs-lookup"><span data-stu-id="8787e-103">call: record</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8787e-104">通話から短いオーディオクリップを録音します。</span><span class="sxs-lookup"><span data-stu-id="8787e-104">Record a short audio clip from the call.</span></span> <span data-ttu-id="8787e-105">これは、ボットがプロンプトに従って発信者からの音声応答を取得したい場合に便利です。</span><span class="sxs-lookup"><span data-stu-id="8787e-105">This is useful if the bot wants to capture a voice response from the caller following a prompt.</span></span>

> [!Note]
> <span data-ttu-id="8787e-106">Record アクションは、 [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md)を使用して開始された[通話](../resources/call.md)に対してのみサポートされます。</span><span class="sxs-lookup"><span data-stu-id="8787e-106">The record action is supported only for [calls](../resources/call.md) that are initiated with [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span></span> <span data-ttu-id="8787e-107">この操作では、呼び出し全体が記録されることはありません。</span><span class="sxs-lookup"><span data-stu-id="8787e-107">This action does not record the entire call.</span></span> <span data-ttu-id="8787e-108">録音の最大長は5分です。</span><span class="sxs-lookup"><span data-stu-id="8787e-108">The maximum length of the recording is 5 minutes.</span></span> <span data-ttu-id="8787e-109">レコーディングは、クラウドコミュニケーションプラットフォームによって permamently には保存されず、通話が終了した直後に破棄されます。</span><span class="sxs-lookup"><span data-stu-id="8787e-109">The recording is not saved permamently by the Cloud Communications Platform and is discarded shortly after the call ends.</span></span> <span data-ttu-id="8787e-110">Bot は、録音操作が終了した後で、(完了した通知で指定された**recordingLocation**値を使用して) すぐにレコーディングをダウンロードする必要があります。</span><span class="sxs-lookup"><span data-stu-id="8787e-110">The bot must download the recording promptly (using the **recordingLocation** value given in the completed notification) after the recording operation finishes.</span></span>


## <a name="permissions"></a><span data-ttu-id="8787e-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8787e-111">Permissions</span></span>
<span data-ttu-id="8787e-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8787e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8787e-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8787e-114">Permission type</span></span> | <span data-ttu-id="8787e-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8787e-115">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="8787e-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8787e-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="8787e-117">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="8787e-117">Not Supported</span></span>        |
| <span data-ttu-id="8787e-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8787e-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8787e-119">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="8787e-119">Not Supported</span></span>        |
| <span data-ttu-id="8787e-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8787e-120">Application</span></span>     | <span data-ttu-id="8787e-121">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="8787e-121">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="8787e-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8787e-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/record
POST /applications/{id}/calls/{id}/record
```

## <a name="request-headers"></a><span data-ttu-id="8787e-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8787e-123">Request headers</span></span>
| <span data-ttu-id="8787e-124">名前</span><span class="sxs-lookup"><span data-stu-id="8787e-124">Name</span></span>          | <span data-ttu-id="8787e-125">説明</span><span class="sxs-lookup"><span data-stu-id="8787e-125">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="8787e-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="8787e-126">Authorization</span></span> | <span data-ttu-id="8787e-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8787e-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8787e-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="8787e-129">Request body</span></span>
<span data-ttu-id="8787e-130">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="8787e-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8787e-131">パラメーター</span><span class="sxs-lookup"><span data-stu-id="8787e-131">Parameter</span></span>      | <span data-ttu-id="8787e-132">型</span><span class="sxs-lookup"><span data-stu-id="8787e-132">Type</span></span>    |<span data-ttu-id="8787e-133">説明</span><span class="sxs-lookup"><span data-stu-id="8787e-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8787e-134">促し</span><span class="sxs-lookup"><span data-stu-id="8787e-134">prompts</span></span>|<span data-ttu-id="8787e-135">[Mediaprompt](../resources/mediaprompt.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="8787e-135">[mediaPrompt](../resources/mediaprompt.md) collection</span></span> | <span data-ttu-id="8787e-136">レコーディングの開始前に再生するプロンプトのコレクション (ある場合)。</span><span class="sxs-lookup"><span data-stu-id="8787e-136">Collection of prompts to play (if any) before recording starts.</span></span> <span data-ttu-id="8787e-137">ユーザーは、"playPrompt" アクションを個別に指定するか、"record" の一部として指定することができます。ほとんどすべてのレコードはプロンプトで preceeded れます。</span><span class="sxs-lookup"><span data-stu-id="8787e-137">Customers can choose to specify "playPrompt" action separately or specify as part of "record" - mostly all records are preceeded by a prompt.</span></span> <span data-ttu-id="8787e-138">Current support は、コレクションの一部として1つのプロンプトのみを対象としています。</span><span class="sxs-lookup"><span data-stu-id="8787e-138">Current support is only for a single prompt as part of the collection.</span></span> |
|<span data-ttu-id="8787e-139">bargeInAllowed</span><span class="sxs-lookup"><span data-stu-id="8787e-139">bargeInAllowed</span></span>|<span data-ttu-id="8787e-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="8787e-140">Boolean</span></span>| <span data-ttu-id="8787e-141">True の場合、このレコードの要求は、キューに登録されている他の既存のレコード/再生プロンプト要求になります。</span><span class="sxs-lookup"><span data-stu-id="8787e-141">If true, this record request will barge into other existing queued-up/currently-processing record/playprompt requests.</span></span> <span data-ttu-id="8787e-142">既定値は false です。</span><span class="sxs-lookup"><span data-stu-id="8787e-142">Default = false.</span></span> |
|<span data-ttu-id="8787e-143">initialSilenceTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="8787e-143">initialSilenceTimeoutInSeconds</span></span> | <span data-ttu-id="8787e-144">Int32</span><span class="sxs-lookup"><span data-stu-id="8787e-144">Int32</span></span>| <span data-ttu-id="8787e-145">操作を開始する前にレコード操作を開始するときに許容される最大初期無音時間 (ユーザー無音)。</span><span class="sxs-lookup"><span data-stu-id="8787e-145">Maximum initial silence (user silence) allowed from the time we start the record operation before we timeout and fail the operation.</span></span> <span data-ttu-id="8787e-146">プロンプトを再生している場合は、プロンプトが終了した後、このタイマーが開始されます。</span><span class="sxs-lookup"><span data-stu-id="8787e-146">If we are playing a prompt, then this timer starts after prompt finishes.</span></span> <span data-ttu-id="8787e-147">既定値 = 5 秒、最小値 = 1 秒、最大 = 300 秒</span><span class="sxs-lookup"><span data-stu-id="8787e-147">Default = 5 seconds, Min = 1 second, Max = 300 seconds</span></span> |
|<span data-ttu-id="8787e-148">maxSilenceTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="8787e-148">maxSilenceTimeoutInSeconds</span></span>|<span data-ttu-id="8787e-149">Int32</span><span class="sxs-lookup"><span data-stu-id="8787e-149">Int32</span></span>| <span data-ttu-id="8787e-150">ユーザーが話し始めた後に許可される最大無音時間 (一時停止時間)。</span><span class="sxs-lookup"><span data-stu-id="8787e-150">Maximum silence (pause) time allowed after a user has started speaking.</span></span> <span data-ttu-id="8787e-151">既定値は5秒、最小値は1秒、最大値は300秒です。</span><span class="sxs-lookup"><span data-stu-id="8787e-151">Default = 5 seconds, Min = 1 second, Max = 300 seconds.</span></span>|
|<span data-ttu-id="8787e-152">maxRecordDurationInSeconds</span><span class="sxs-lookup"><span data-stu-id="8787e-152">maxRecordDurationInSeconds</span></span>|<span data-ttu-id="8787e-153">Int32</span><span class="sxs-lookup"><span data-stu-id="8787e-153">Int32</span></span>| <span data-ttu-id="8787e-154">レコーディングを停止する前のレコード操作の最大期間。</span><span class="sxs-lookup"><span data-stu-id="8787e-154">Max duration for a record operation before stopping recording.</span></span> <span data-ttu-id="8787e-155">既定値は5秒、最小値は1秒、最大値は300秒です。</span><span class="sxs-lookup"><span data-stu-id="8787e-155">Default = 5 seconds, Min = 1 second, Max = 300 seconds.</span></span>|
|<span data-ttu-id="8787e-156">再生のビープ音</span><span class="sxs-lookup"><span data-stu-id="8787e-156">playBeep</span></span>|<span data-ttu-id="8787e-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="8787e-157">Boolean</span></span>| <span data-ttu-id="8787e-158">True の場合は、ユーザーにメッセージの録音を開始できることを示す警告音を鳴らします。</span><span class="sxs-lookup"><span data-stu-id="8787e-158">If true, plays a beep to indicate to the user that they can start recording their message.</span></span> <span data-ttu-id="8787e-159">既定値は true です。</span><span class="sxs-lookup"><span data-stu-id="8787e-159">Default = true.</span></span>|
|<span data-ttu-id="8787e-160">stopTones</span><span class="sxs-lookup"><span data-stu-id="8787e-160">stopTones</span></span>|<span data-ttu-id="8787e-161">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="8787e-161">String collection</span></span>|<span data-ttu-id="8787e-162">録音を終了するために指定されたトーンを停止します。</span><span class="sxs-lookup"><span data-stu-id="8787e-162">Stop tones specified to end recording.</span></span>|
|<span data-ttu-id="8787e-163">clientContext</span><span class="sxs-lookup"><span data-stu-id="8787e-163">clientContext</span></span>|<span data-ttu-id="8787e-164">String</span><span class="sxs-lookup"><span data-stu-id="8787e-164">String</span></span>|<span data-ttu-id="8787e-165">一意のクライアントコンテキスト文字列。</span><span class="sxs-lookup"><span data-stu-id="8787e-165">Unique Client Context string.</span></span> <span data-ttu-id="8787e-166">最大256文字を使用できます。</span><span class="sxs-lookup"><span data-stu-id="8787e-166">Can have a maximum of 256 characters.</span></span>|

## <a name="response"></a><span data-ttu-id="8787e-167">応答</span><span class="sxs-lookup"><span data-stu-id="8787e-167">Response</span></span>
<span data-ttu-id="8787e-168">このメソッドは、 `200 OK`応答コードと、この要求に対して作成された[RECORDOPERATION](../resources/recordoperation.md)への URI を持つ Location ヘッダーを返します。</span><span class="sxs-lookup"><span data-stu-id="8787e-168">This method returns a `200 OK` response code and a Location header with a URI to the [recordOperation](../resources/recordoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="8787e-169">例</span><span class="sxs-lookup"><span data-stu-id="8787e-169">Example</span></span>
<span data-ttu-id="8787e-170">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="8787e-170">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="8787e-171">要求</span><span class="sxs-lookup"><span data-stu-id="8787e-171">Request</span></span>
<span data-ttu-id="8787e-172">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="8787e-172">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8787e-173">プロトコル</span><span class="sxs-lookup"><span data-stu-id="8787e-173">HTTP</span></span>](#tab/http)
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
      }
    }
  ],
  "maxRecordDurationInSeconds": 10,
  "initialSilenceTimeoutInSeconds": 5,
  "maxSilenceTimeoutInSeconds": 2,
  "playBeep": true,
  "stopTones": [ "#", "1", "*" ]
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8787e-174">Javascript</span><span class="sxs-lookup"><span data-stu-id="8787e-174">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-record-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8787e-175">応答</span><span class="sxs-lookup"><span data-stu-id="8787e-175">Response</span></span>
<span data-ttu-id="8787e-176">次の例は応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="8787e-176">The following example shows the response.</span></span>

> <span data-ttu-id="8787e-p112">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="8787e-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.recordOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5

{
  "@odata.type": "#microsoft.graph.recordOperation",
  "status": "running",
  "createdDateTime": "2018-09-06T15:58:41Z",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "completionReason": null,
  "resultInfo": null,
  "recordingLocation": null,
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}

```

##### <a name="notification---operation-completed"></a><span data-ttu-id="8787e-179">通知-操作が完了しました</span><span class="sxs-lookup"><span data-stu-id="8787e-179">Notification - operation completed</span></span>

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
        "recordingLocation": "https://file.location/17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
        "recordingAccessToken": "<access-token>",
        "completionReason": "stopToneDetected"
      }
    }
  ]
}
```

##### <a name="get-recording-file---request"></a><span data-ttu-id="8787e-180">レコーディングファイルの取得-要求</span><span class="sxs-lookup"><span data-stu-id="8787e-180">Get recording file - Request</span></span>
<span data-ttu-id="8787e-181">次の例は、レコーディングの内容を取得する要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="8787e-181">The following example shows the request to get the content of the recording.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "download_recorded_file",
}-->
```http
GET https://file.location/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
Authorization: Bearer <recordingAccessToken>
```

##### <a name="get-recording-file---response"></a><span data-ttu-id="8787e-182">レコーディングファイル応答の取得</span><span class="sxs-lookup"><span data-stu-id="8787e-182">Get recording file - Response</span></span>
<span data-ttu-id="8787e-183">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="8787e-183">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "ignored",
  "name": "download_recorded_file",
  "truncated": true
}-->
```http
GET https://file.location/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
Transfer-Encoding: chunked
Date: Thu, 17 Jan 2019 01:46:37 GMT
Content-Type: application/octet-stream

(application/octet-stream of size 160696 bytes)
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
  ]
}
-->
