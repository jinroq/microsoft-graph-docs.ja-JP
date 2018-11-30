---
title: '電話: playPrompt'
description: 呼び出しではプロンプトを再生します。
ms.openlocfilehash: a5fb5d34264298726add6cf2742d1319bfcb6c95
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071104"
---
# <a name="call-playprompt"></a><span data-ttu-id="6c10f-103">電話: playPrompt</span><span class="sxs-lookup"><span data-stu-id="6c10f-103">call: playPrompt</span></span>

> <span data-ttu-id="6c10f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6c10f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6c10f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6c10f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6c10f-106">呼び出しではプロンプトを再生します。</span><span class="sxs-lookup"><span data-stu-id="6c10f-106">Play a prompt in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="6c10f-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6c10f-107">Permissions</span></span>
<span data-ttu-id="6c10f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6c10f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6c10f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6c10f-110">Permission type</span></span>                        | <span data-ttu-id="6c10f-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6c10f-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6c10f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6c10f-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="6c10f-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6c10f-113">Not Supported.</span></span>                               |
| <span data-ttu-id="6c10f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6c10f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c10f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6c10f-115">Not Supported.</span></span>                               |
| <span data-ttu-id="6c10f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6c10f-116">Application</span></span>                            | <span data-ttu-id="6c10f-117">なし。</span><span class="sxs-lookup"><span data-stu-id="6c10f-117">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="6c10f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6c10f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/playPrompt
POST /applications/{id}/calls/{id}/playPrompt
```

## <a name="request-headers"></a><span data-ttu-id="6c10f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6c10f-119">Request headers</span></span>
| <span data-ttu-id="6c10f-120">名前</span><span class="sxs-lookup"><span data-stu-id="6c10f-120">Name</span></span>          | <span data-ttu-id="6c10f-121">説明</span><span class="sxs-lookup"><span data-stu-id="6c10f-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="6c10f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c10f-122">Authorization</span></span> | <span data-ttu-id="6c10f-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6c10f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6c10f-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="6c10f-125">Request body</span></span>
<span data-ttu-id="6c10f-126">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="6c10f-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6c10f-127">パラメーター</span><span class="sxs-lookup"><span data-stu-id="6c10f-127">Parameter</span></span>      | <span data-ttu-id="6c10f-128">型</span><span class="sxs-lookup"><span data-stu-id="6c10f-128">Type</span></span>    |<span data-ttu-id="6c10f-129">説明</span><span class="sxs-lookup"><span data-stu-id="6c10f-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6c10f-130">メッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="6c10f-130">prompts</span></span>|<span data-ttu-id="6c10f-131">[プロンプト](../resources/prompt.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="6c10f-131">[prompt](../resources/prompt.md) collection</span></span>||
|<span data-ttu-id="6c10f-132">clientContext</span><span class="sxs-lookup"><span data-stu-id="6c10f-132">clientContext</span></span>|<span data-ttu-id="6c10f-133">String</span><span class="sxs-lookup"><span data-stu-id="6c10f-133">String</span></span>|<span data-ttu-id="6c10f-134">クライアントのコンテキスト。</span><span class="sxs-lookup"><span data-stu-id="6c10f-134">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="6c10f-135">応答</span><span class="sxs-lookup"><span data-stu-id="6c10f-135">Response</span></span>
<span data-ttu-id="6c10f-136">返します。`202 Accepted`応答コードと、Location ヘッダーをこの要求用に作成された[commsOperation](../resources/commsoperation.md)の uri を持つ。</span><span class="sxs-lookup"><span data-stu-id="6c10f-136">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="6c10f-137">例</span><span class="sxs-lookup"><span data-stu-id="6c10f-137">Example</span></span>
<span data-ttu-id="6c10f-138">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="6c10f-138">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="6c10f-139">要求</span><span class="sxs-lookup"><span data-stu-id="6c10f-139">Request</span></span>
<span data-ttu-id="6c10f-140">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="6c10f-140">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call_playPrompt"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/playPrompt
Content-Type: application/json
Content-Length: 166

{
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
  ]
}
```

##### <a name="response"></a><span data-ttu-id="6c10f-141">応答</span><span class="sxs-lookup"><span data-stu-id="6c10f-141">Response</span></span>

> <span data-ttu-id="6c10f-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="6c10f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="6c10f-144">通知の操作が完了しました</span><span class="sxs-lookup"><span data-stu-id="6c10f-144">Notification - operation completed</span></span>

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
        "@odata.type": "#microsoft.graph.commsOperation",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"54451\"",
        "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
        "status": "completed"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "call: playPrompt",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
