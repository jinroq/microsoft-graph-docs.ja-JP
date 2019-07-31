---
title: '呼び出し: playPrompt'
description: 呼び出しでプロンプトを再生します。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8ca1a83628ebbb5da2bfec41307b53e01c381883
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35944461"
---
# <a name="call-playprompt"></a><span data-ttu-id="0831b-103">呼び出し: playPrompt</span><span class="sxs-lookup"><span data-stu-id="0831b-103">call: playPrompt</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0831b-104">呼び出しでプロンプトを再生します。</span><span class="sxs-lookup"><span data-stu-id="0831b-104">Play a prompt in the call.</span></span>

<span data-ttu-id="0831b-105">操作を処理する方法の詳細については、「 [commsOperation](../resources/commsoperation.md) 」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0831b-105">For more information about how to handle operations, see [commsOperation](../resources/commsoperation.md)</span></span>

## <a name="permissions"></a><span data-ttu-id="0831b-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0831b-106">Permissions</span></span>
<span data-ttu-id="0831b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0831b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0831b-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0831b-109">Permission type</span></span>                        | <span data-ttu-id="0831b-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0831b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0831b-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0831b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0831b-112">サポートされません。</span><span class="sxs-lookup"><span data-stu-id="0831b-112">Not Supported.</span></span>                               |
| <span data-ttu-id="0831b-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0831b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0831b-114">サポートされません。</span><span class="sxs-lookup"><span data-stu-id="0831b-114">Not Supported.</span></span>                               |
| <span data-ttu-id="0831b-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0831b-115">Application</span></span>                            | <span data-ttu-id="0831b-116">なし。</span><span class="sxs-lookup"><span data-stu-id="0831b-116">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="0831b-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0831b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/playPrompt
POST /applications/{id}/calls/{id}/playPrompt
```

## <a name="request-headers"></a><span data-ttu-id="0831b-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0831b-118">Request headers</span></span>
| <span data-ttu-id="0831b-119">名前</span><span class="sxs-lookup"><span data-stu-id="0831b-119">Name</span></span>          | <span data-ttu-id="0831b-120">説明</span><span class="sxs-lookup"><span data-stu-id="0831b-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="0831b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0831b-121">Authorization</span></span> | <span data-ttu-id="0831b-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0831b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0831b-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="0831b-124">Request body</span></span>
<span data-ttu-id="0831b-125">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="0831b-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0831b-126">パラメーター</span><span class="sxs-lookup"><span data-stu-id="0831b-126">Parameter</span></span>      | <span data-ttu-id="0831b-127">型</span><span class="sxs-lookup"><span data-stu-id="0831b-127">Type</span></span>    |<span data-ttu-id="0831b-128">説明</span><span class="sxs-lookup"><span data-stu-id="0831b-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0831b-129">促し</span><span class="sxs-lookup"><span data-stu-id="0831b-129">prompts</span></span>|<span data-ttu-id="0831b-130">[prompt](../resources/prompt.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0831b-130">[prompt](../resources/prompt.md) collection</span></span>| <span data-ttu-id="0831b-131">現時点では、1つのプロンプトと種類[mediaprompt](../resources/mediaprompt.md)のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="0831b-131">Currently only a single prompt and of type [MediaPrompt](../resources/mediaprompt.md) is supported.</span></span>|
|<span data-ttu-id="0831b-132">for</span><span class="sxs-lookup"><span data-stu-id="0831b-132">loop</span></span>|<span data-ttu-id="0831b-133">bool</span><span class="sxs-lookup"><span data-stu-id="0831b-133">bool</span></span>| <span data-ttu-id="0831b-134">ループ値を指定します。</span><span class="sxs-lookup"><span data-stu-id="0831b-134">The loop value.</span></span> <span data-ttu-id="0831b-135">true は、無限にループすることを示します。</span><span class="sxs-lookup"><span data-stu-id="0831b-135">true indicates to loop infinitely.</span></span> <span data-ttu-id="0831b-136">既定値は false です。</span><span class="sxs-lookup"><span data-stu-id="0831b-136">The default value is false.</span></span> |
|<span data-ttu-id="0831b-137">clientContext</span><span class="sxs-lookup"><span data-stu-id="0831b-137">clientContext</span></span>|<span data-ttu-id="0831b-138">String</span><span class="sxs-lookup"><span data-stu-id="0831b-138">String</span></span>|<span data-ttu-id="0831b-139">クライアントコンテキスト。</span><span class="sxs-lookup"><span data-stu-id="0831b-139">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="0831b-140">応答</span><span class="sxs-lookup"><span data-stu-id="0831b-140">Response</span></span>
<span data-ttu-id="0831b-141">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[playPromptOperation](../resources/playpromptoperation.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0831b-141">If successful, this method returns a `200 OK` response code and a [playPromptOperation](../resources/playpromptoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0831b-142">例</span><span class="sxs-lookup"><span data-stu-id="0831b-142">Example</span></span>
<span data-ttu-id="0831b-143">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="0831b-143">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="0831b-144">要求</span><span class="sxs-lookup"><span data-stu-id="0831b-144">Request</span></span>
<span data-ttu-id="0831b-145">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="0831b-145">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0831b-146">プロトコル</span><span class="sxs-lookup"><span data-stu-id="0831b-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-playPrompt"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/playPrompt
Content-Type: application/json
Content-Length: 166

{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
  "prompts": [
    {
      "@odata.type": "#microsoft.graph.mediaPrompt",
      "mediaInfo": {
        "@odata.type": "#microsoft.graph.mediaInfo",
        "uri": "https://cdn.contoso.com/beep.wav",
        "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
      },
    },
  ],
  "loop": false
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0831b-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="0831b-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-playprompt-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0831b-148">応答</span><span class="sxs-lookup"><span data-stu-id="0831b-148">Response</span></span>

> <span data-ttu-id="0831b-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="0831b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.playPromptOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5

{
  "@odata.type": "#microsoft.graph.playPromptOperation",
  "id": "0fe0623f-d628-42ed-b4bd-8ac290072cc5",
  "status": "running",
  "createdDateTime": "2018-09-06T15:58:41Z",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}

```

##### <a name="notification---operation-completed"></a><span data-ttu-id="0831b-151">通知-操作が完了しました</span><span class="sxs-lookup"><span data-stu-id="0831b-151">Notification - operation completed</span></span>

 ><span data-ttu-id="0831b-152">**注:** 無限ループが発生した場合、この通知は送信されません。</span><span class="sxs-lookup"><span data-stu-id="0831b-152">**Note:** If infinite looping occurs, this notification is not sent.</span></span>
 
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
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
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
<!--
{
  "type": "#page.annotation",
  "description": "call: playPrompt",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
