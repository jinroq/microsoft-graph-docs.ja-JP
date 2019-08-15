---
title: '通話: subscribeToTone'
description: DTMF (デュアルトーンマルチ周波数信号) をサブスクライブします。 これにより、ユーザーが ' Dialpad ' のキーを押したときに通知を受けることができます。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 83e6c1b9795ea1caf27a166fd523c70b51909df0
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36418867"
---
# <a name="call-subscribetotone"></a><span data-ttu-id="acd03-104">通話: subscribeToTone</span><span class="sxs-lookup"><span data-stu-id="acd03-104">call: subscribeToTone</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="acd03-105">DTMF (デュアルトーンマルチ周波数信号) をサブスクライブします。</span><span class="sxs-lookup"><span data-stu-id="acd03-105">Subscribe to DTMF (dual-tone multi-frequency signaling).</span></span> <span data-ttu-id="acd03-106">これにより、ユーザーが "Dialpad" のキーを押したときに通知を受けることができます。</span><span class="sxs-lookup"><span data-stu-id="acd03-106">This allows you to be notified when the user presses keys on a "Dialpad".</span></span>

> [!Note]
> <span data-ttu-id="acd03-107">**SubscribeToTone**アクションは、 [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md)で開始された[通話](../resources/call.md)に対してのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="acd03-107">The **subscribeToTone** action is supported only for [calls](../resources/call.md) that are initiated with [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="acd03-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="acd03-108">Permissions</span></span>
<span data-ttu-id="acd03-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="acd03-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="acd03-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="acd03-111">Permission type</span></span> | <span data-ttu-id="acd03-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="acd03-112">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="acd03-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="acd03-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="acd03-114">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="acd03-114">Not Supported</span></span>        |
| <span data-ttu-id="acd03-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="acd03-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="acd03-116">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="acd03-116">Not Supported</span></span>        |
| <span data-ttu-id="acd03-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="acd03-117">Application</span></span>     | <span data-ttu-id="acd03-118">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="acd03-118">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="acd03-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="acd03-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/subscribeToTone
POST /applications/{id}/calls/{id}/subscribeToTone
```

## <a name="request-headers"></a><span data-ttu-id="acd03-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="acd03-120">Request headers</span></span>
| <span data-ttu-id="acd03-121">名前</span><span class="sxs-lookup"><span data-stu-id="acd03-121">Name</span></span>          | <span data-ttu-id="acd03-122">説明</span><span class="sxs-lookup"><span data-stu-id="acd03-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="acd03-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="acd03-123">Authorization</span></span> | <span data-ttu-id="acd03-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="acd03-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="acd03-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="acd03-126">Request body</span></span>
<span data-ttu-id="acd03-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="acd03-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="acd03-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="acd03-128">Parameter</span></span>      | <span data-ttu-id="acd03-129">型</span><span class="sxs-lookup"><span data-stu-id="acd03-129">Type</span></span>    | <span data-ttu-id="acd03-130">説明</span><span class="sxs-lookup"><span data-stu-id="acd03-130">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="acd03-131">clientContext</span><span class="sxs-lookup"><span data-stu-id="acd03-131">clientContext</span></span>  | <span data-ttu-id="acd03-132">String</span><span class="sxs-lookup"><span data-stu-id="acd03-132">String</span></span>  | <span data-ttu-id="acd03-133">一意のクライアントコンテキスト文字列。</span><span class="sxs-lookup"><span data-stu-id="acd03-133">Unique client context string.</span></span> <span data-ttu-id="acd03-134">最大256文字を使用できます。</span><span class="sxs-lookup"><span data-stu-id="acd03-134">Can have a maximum of 256 characters.</span></span> |

## <a name="response"></a><span data-ttu-id="acd03-135">応答</span><span class="sxs-lookup"><span data-stu-id="acd03-135">Response</span></span>
<span data-ttu-id="acd03-136">成功した場合、このメソッドは `200 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="acd03-136">If successful, this method returns `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="acd03-137">例</span><span class="sxs-lookup"><span data-stu-id="acd03-137">Example</span></span>
<span data-ttu-id="acd03-138">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="acd03-138">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="acd03-139">要求</span><span class="sxs-lookup"><span data-stu-id="acd03-139">Request</span></span>
<span data-ttu-id="acd03-140">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="acd03-140">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="acd03-141">プロトコル</span><span class="sxs-lookup"><span data-stu-id="acd03-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-subscribeToTone"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/subscribeToTone
Content-Type: application/json
Content-Length: 46

{
  "clientContext": "fd1c7836-4d84-4e24-b6aa-23188688cc54"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="acd03-142">C#</span><span class="sxs-lookup"><span data-stu-id="acd03-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-subscribetotone-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="acd03-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="acd03-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-subscribetotone-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="acd03-144">目的-C</span><span class="sxs-lookup"><span data-stu-id="acd03-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-subscribetotone-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="acd03-145">応答</span><span class="sxs-lookup"><span data-stu-id="acd03-145">Response</span></span>

> <span data-ttu-id="acd03-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="acd03-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 200 OK

{
  "id": "ea91863c-d0a6-4de0-b73a-4c8d63da5d87",
  "status": "completed",
  "createdDateTime": "2019-07-18T19:52:30Z",
  "lastActionDateTime": "2019-07-18T19:52:31Z",
  "clientContext": "fd1c7836-4d84-4e24-b6aa-23188688cc54",
}
```


##### <a name="notification---tone-notification"></a><span data-ttu-id="acd03-148">通知-トーン通知</span><span class="sxs-lookup"><span data-stu-id="acd03-148">Notification - Tone notification</span></span>

<span data-ttu-id="acd03-149">通知には、 [toneinfo](../resources/toneinfo.md)リソースで押されたトーンの情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="acd03-149">The notification contain information of the tone pressed in the [toneinfo](../resources/toneinfo.md) resource.</span></span>

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
      "resource": "/app/calls/421f1100-411f-4a29-8514-dbbb9caff45",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "established",
        "toneInfo": {
          "@odata.type": "#microsoft.graph.toneInfo",
          "sequenceId": 1,
          "tone": "tone1"
        }
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
  "description": "call: subscribeToTone",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
