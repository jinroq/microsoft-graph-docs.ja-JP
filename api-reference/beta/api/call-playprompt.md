---
title: '呼び出し: playPrompt'
description: 呼び出しでプロンプトを再生します。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 571c8b412e6e8099aaee020ef45e2ad55b1e5707
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33635863"
---
# <a name="call-playprompt"></a><span data-ttu-id="8d276-103">呼び出し: playPrompt</span><span class="sxs-lookup"><span data-stu-id="8d276-103">call: playPrompt</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d276-104">呼び出しでプロンプトを再生します。</span><span class="sxs-lookup"><span data-stu-id="8d276-104">Play a prompt in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="8d276-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8d276-105">Permissions</span></span>
<span data-ttu-id="8d276-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8d276-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8d276-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8d276-108">Permission type</span></span>                        | <span data-ttu-id="8d276-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8d276-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8d276-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8d276-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8d276-111">サポートされません。</span><span class="sxs-lookup"><span data-stu-id="8d276-111">Not Supported.</span></span>                               |
| <span data-ttu-id="8d276-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8d276-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d276-113">サポートされません。</span><span class="sxs-lookup"><span data-stu-id="8d276-113">Not Supported.</span></span>                               |
| <span data-ttu-id="8d276-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8d276-114">Application</span></span>                            | <span data-ttu-id="8d276-115">なし。</span><span class="sxs-lookup"><span data-stu-id="8d276-115">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="8d276-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8d276-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/playPrompt
POST /applications/{id}/calls/{id}/playPrompt
```

## <a name="request-headers"></a><span data-ttu-id="8d276-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8d276-117">Request headers</span></span>
| <span data-ttu-id="8d276-118">名前</span><span class="sxs-lookup"><span data-stu-id="8d276-118">Name</span></span>          | <span data-ttu-id="8d276-119">説明</span><span class="sxs-lookup"><span data-stu-id="8d276-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="8d276-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d276-120">Authorization</span></span> | <span data-ttu-id="8d276-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8d276-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8d276-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="8d276-123">Request body</span></span>
<span data-ttu-id="8d276-124">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="8d276-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8d276-125">パラメーター</span><span class="sxs-lookup"><span data-stu-id="8d276-125">Parameter</span></span>      | <span data-ttu-id="8d276-126">型</span><span class="sxs-lookup"><span data-stu-id="8d276-126">Type</span></span>    |<span data-ttu-id="8d276-127">説明</span><span class="sxs-lookup"><span data-stu-id="8d276-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8d276-128">促し</span><span class="sxs-lookup"><span data-stu-id="8d276-128">prompts</span></span>|<span data-ttu-id="8d276-129">[prompt](../resources/prompt.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="8d276-129">[prompt](../resources/prompt.md) collection</span></span>||
|<span data-ttu-id="8d276-130">clientContext</span><span class="sxs-lookup"><span data-stu-id="8d276-130">clientContext</span></span>|<span data-ttu-id="8d276-131">String</span><span class="sxs-lookup"><span data-stu-id="8d276-131">String</span></span>|<span data-ttu-id="8d276-132">クライアントコンテキスト。</span><span class="sxs-lookup"><span data-stu-id="8d276-132">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="8d276-133">応答</span><span class="sxs-lookup"><span data-stu-id="8d276-133">Response</span></span>
<span data-ttu-id="8d276-134">成功した場合、この`200 OK`メソッドは応答コードと、応答本文で[playPromptOperation](../resources/playPromptOperation.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8d276-134">If successful, this method returns `200 OK` response code and [playPromptOperation](../resources/playPromptOperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d276-135">例</span><span class="sxs-lookup"><span data-stu-id="8d276-135">Example</span></span>
<span data-ttu-id="8d276-136">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="8d276-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="8d276-137">要求</span><span class="sxs-lookup"><span data-stu-id="8d276-137">Request</span></span>
<span data-ttu-id="8d276-138">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="8d276-138">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="8d276-139">応答</span><span class="sxs-lookup"><span data-stu-id="8d276-139">Response</span></span>

> <span data-ttu-id="8d276-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="8d276-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.playPromptOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="8d276-142">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="8d276-142">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8d276-143">Java</span><span class="sxs-lookup"><span data-stu-id="8d276-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/call-playPrompt-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="notification---operation-completed"></a><span data-ttu-id="8d276-144">通知-操作が完了しました</span><span class="sxs-lookup"><span data-stu-id="8d276-144">Notification - operation completed</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "call: playPrompt",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/call-playprompt.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
