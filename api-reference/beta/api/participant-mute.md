---
title: '参加者: ミュート'
description: 呼び出しで特定の参加者をミュートします。
ms.openlocfilehash: 939fd0fd94304318786b0ecb7ae72da28b55e4b9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069263"
---
# <a name="participant-mute"></a><span data-ttu-id="615cf-103">参加者: ミュート</span><span class="sxs-lookup"><span data-stu-id="615cf-103">participant: mute</span></span>

> <span data-ttu-id="615cf-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="615cf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="615cf-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="615cf-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="615cf-106">呼び出しで特定の参加者をミュートします。</span><span class="sxs-lookup"><span data-stu-id="615cf-106">Mute a specific participant in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="615cf-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="615cf-107">Permissions</span></span>
<span data-ttu-id="615cf-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="615cf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="615cf-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="615cf-110">Permission type</span></span> | <span data-ttu-id="615cf-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="615cf-111">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="615cf-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="615cf-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="615cf-113">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="615cf-113">Not Supported</span></span>        |
| <span data-ttu-id="615cf-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="615cf-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="615cf-115">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="615cf-115">Not Supported</span></span>        |
| <span data-ttu-id="615cf-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="615cf-116">Application</span></span>     | <span data-ttu-id="615cf-117">なし</span><span class="sxs-lookup"><span data-stu-id="615cf-117">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="615cf-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="615cf-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/{id}/mute
POST /applications/{id}/calls/{id}/participants/{id}/mute
```

## <a name="request-headers"></a><span data-ttu-id="615cf-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="615cf-119">Request headers</span></span>
| <span data-ttu-id="615cf-120">名前</span><span class="sxs-lookup"><span data-stu-id="615cf-120">Name</span></span>          | <span data-ttu-id="615cf-121">説明</span><span class="sxs-lookup"><span data-stu-id="615cf-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="615cf-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="615cf-122">Authorization</span></span> | <span data-ttu-id="615cf-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="615cf-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="615cf-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="615cf-125">Request body</span></span>
<span data-ttu-id="615cf-126">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="615cf-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="615cf-127">パラメーター</span><span class="sxs-lookup"><span data-stu-id="615cf-127">Parameter</span></span>      | <span data-ttu-id="615cf-128">型</span><span class="sxs-lookup"><span data-stu-id="615cf-128">Type</span></span>    |<span data-ttu-id="615cf-129">説明</span><span class="sxs-lookup"><span data-stu-id="615cf-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="615cf-130">clientContext</span><span class="sxs-lookup"><span data-stu-id="615cf-130">clientContext</span></span>|<span data-ttu-id="615cf-131">String</span><span class="sxs-lookup"><span data-stu-id="615cf-131">String</span></span>|<span data-ttu-id="615cf-132">クライアントのコンテキスト。</span><span class="sxs-lookup"><span data-stu-id="615cf-132">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="615cf-133">応答</span><span class="sxs-lookup"><span data-stu-id="615cf-133">Response</span></span>
<span data-ttu-id="615cf-134">かどうかは成功すると、このメソッドを返します`200 OK`、応答の本体で応答コードと[commsOperation](../resources/commsoperation.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="615cf-134">If successful, this method returns `200 OK` response code and [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="615cf-135">例</span><span class="sxs-lookup"><span data-stu-id="615cf-135">Example</span></span>
<span data-ttu-id="615cf-136">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="615cf-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="615cf-137">要求</span><span class="sxs-lookup"><span data-stu-id="615cf-137">Request</span></span>
<span data-ttu-id="615cf-138">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="615cf-138">The following example shows the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "participant_mute"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/participants/{id}/mute
Content-Type: application/json
Content-Length: 46

{
  "clientContext": "clientContext-value"
}
```

##### <a name="response"></a><span data-ttu-id="615cf-139">応答</span><span class="sxs-lookup"><span data-stu-id="615cf-139">Response</span></span>

> <span data-ttu-id="615cf-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="615cf-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.commsOperation",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 259

{
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "completed",
  "createdDateTime": "2018-09-06T15:58:41Z",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

## <a name="example---mute-specific-participant"></a><span data-ttu-id="615cf-142">例: 特定の参加者をミュート</span><span class="sxs-lookup"><span data-stu-id="615cf-142">Example - Mute specific participant</span></span>

##### <a name="request"></a><span data-ttu-id="615cf-143">要求</span><span class="sxs-lookup"><span data-stu-id="615cf-143">Request</span></span>

```http
POST /app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants/0698446E77E24E4D85F80597083CB830/mute
Authorization: Bearer <TOKEN>
Content-Type: application/json

{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

##### <a name="response"></a><span data-ttu-id="615cf-144">応答</span><span class="sxs-lookup"><span data-stu-id="615cf-144">Response</span></span>

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 259
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsOperation",
  "truncated": true
}-->
```json
{
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "completed",
  "createdDateTime": "2018-09-06T15:58:41Z",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

##### <a name="notification---roster-updated-with-participant-muted"></a><span data-ttu-id="615cf-145">名簿の参加者がミュートされている更新の通知-</span><span class="sxs-lookup"><span data-stu-id="615cf-145">Notification - roster updated with participant muted</span></span>

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
      "changeType": "updated",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants",
      "resourceData": [
        {
          "@odata.type": "#microsoft.graph.participant",
          "id": "0698446E77E24E4D85F80597083CB830",
          "info": {
            "identity": {
              "user": {
                "displayName": "Test User",
                "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
              }
            },
            "region": "westus",
            "languageId": "en-US"
          },
          "mediaStreams": [
            {
              "mediaType": "audio",
              "label": "main-audio",
              "sourceId": "1",
              "direction": "sendReceive",
              "serverMuted": false
            }
          ],
          "isMuted": true,
          "isInLobby": false
        },
        {
          "@odata.type": "#microsoft.graph.participant",
          "id": "123456W77E24E4D85F80597083CB830",
          "info": {
            "identity": {
              "application": {
                "displayName": "Test Bot",
                "id": "1234A46B-3D17-4ADC-8DCE-DC4E7D556789"
              }
            },
            "region": "westus",
            "languageId": "en-US"
          },
          "mediaStreams": [
            {
              "mediaType": "audio",
              "label": "main-audio",
              "sourceId": "2",
              "direction": "sendReceive",
              "serverMuted": false
            }
          ],
          "isInLobby": false
        }
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "participant: mute",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
