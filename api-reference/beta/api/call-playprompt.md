---
title: '電話: playPrompt'
description: 呼び出しではプロンプトを再生します。
author: VinodRavichandran
ms.openlocfilehash: e432375fdfc9d31822698997f4fda27180e08ac9
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380346"
---
# <a name="call-playprompt"></a><span data-ttu-id="eb192-103">電話: playPrompt</span><span class="sxs-lookup"><span data-stu-id="eb192-103">call: playPrompt</span></span>

> <span data-ttu-id="eb192-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="eb192-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eb192-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eb192-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="eb192-106">呼び出しではプロンプトを再生します。</span><span class="sxs-lookup"><span data-stu-id="eb192-106">Play a prompt in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="eb192-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="eb192-107">Permissions</span></span>
<span data-ttu-id="eb192-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eb192-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="eb192-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="eb192-110">Permission type</span></span>                        | <span data-ttu-id="eb192-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="eb192-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="eb192-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="eb192-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="eb192-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eb192-113">Not Supported.</span></span>                               |
| <span data-ttu-id="eb192-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="eb192-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb192-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eb192-115">Not Supported.</span></span>                               |
| <span data-ttu-id="eb192-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="eb192-116">Application</span></span>                            | <span data-ttu-id="eb192-117">なし。</span><span class="sxs-lookup"><span data-stu-id="eb192-117">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="eb192-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="eb192-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/playPrompt
POST /applications/{id}/calls/{id}/playPrompt
```

## <a name="request-headers"></a><span data-ttu-id="eb192-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="eb192-119">Request headers</span></span>
| <span data-ttu-id="eb192-120">名前</span><span class="sxs-lookup"><span data-stu-id="eb192-120">Name</span></span>          | <span data-ttu-id="eb192-121">説明</span><span class="sxs-lookup"><span data-stu-id="eb192-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="eb192-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb192-122">Authorization</span></span> | <span data-ttu-id="eb192-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="eb192-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eb192-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="eb192-125">Request body</span></span>
<span data-ttu-id="eb192-126">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="eb192-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="eb192-127">パラメーター</span><span class="sxs-lookup"><span data-stu-id="eb192-127">Parameter</span></span>      | <span data-ttu-id="eb192-128">型</span><span class="sxs-lookup"><span data-stu-id="eb192-128">Type</span></span>    |<span data-ttu-id="eb192-129">説明</span><span class="sxs-lookup"><span data-stu-id="eb192-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eb192-130">メッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="eb192-130">prompts</span></span>|<span data-ttu-id="eb192-131">[プロンプト](../resources/prompt.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="eb192-131">[prompt](../resources/prompt.md) collection</span></span>||
|<span data-ttu-id="eb192-132">clientContext</span><span class="sxs-lookup"><span data-stu-id="eb192-132">clientContext</span></span>|<span data-ttu-id="eb192-133">String</span><span class="sxs-lookup"><span data-stu-id="eb192-133">String</span></span>|<span data-ttu-id="eb192-134">クライアントのコンテキスト。</span><span class="sxs-lookup"><span data-stu-id="eb192-134">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="eb192-135">応答</span><span class="sxs-lookup"><span data-stu-id="eb192-135">Response</span></span>
<span data-ttu-id="eb192-136">かどうかは成功すると、このメソッドを返します`200 OK`、応答の本体で応答コードと[playPromptOperation](../resources/playPromptOperation.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="eb192-136">If successful, this method returns `200 OK` response code and [playPromptOperation](../resources/playPromptOperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb192-137">例</span><span class="sxs-lookup"><span data-stu-id="eb192-137">Example</span></span>
<span data-ttu-id="eb192-138">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="eb192-138">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="eb192-139">要求</span><span class="sxs-lookup"><span data-stu-id="eb192-139">Request</span></span>
<span data-ttu-id="eb192-140">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="eb192-140">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call-playPrompt"
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

##### <a name="response"></a><span data-ttu-id="eb192-141">応答</span><span class="sxs-lookup"><span data-stu-id="eb192-141">Response</span></span>

> <span data-ttu-id="eb192-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="eb192-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.playPromptOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="eb192-144">通知の操作が完了しました</span><span class="sxs-lookup"><span data-stu-id="eb192-144">Notification - operation completed</span></span>

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
        "@odata.type": "#microsoft.graph.playPromptOperation",
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