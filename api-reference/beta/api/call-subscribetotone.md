---
title: '電話: subscribeToTone'
description: " 電話です。"
ms.openlocfilehash: c3793931c2f06e54cdac278f0f0539b42d7e622c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071021"
---
# <a name="call-subscribetotone"></a><span data-ttu-id="a6934-103">電話: subscribeToTone</span><span class="sxs-lookup"><span data-stu-id="a6934-103">call: subscribeToTone</span></span>

> <span data-ttu-id="a6934-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a6934-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a6934-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a6934-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a6934-106">(デュアル トーン多重周波数信号) DTMF を購読します。</span><span class="sxs-lookup"><span data-stu-id="a6934-106">Subscribe to DTMF (dual-tone multi-frequency signaling).</span></span> <span data-ttu-id="a6934-107">これにより、ユーザーは、「プッシュホン」電話キーを押したときに通知することができます。</span><span class="sxs-lookup"><span data-stu-id="a6934-107">This allows you to be notified when the user presses keys on a "touchtone" phone.</span></span>

## <a name="permissions"></a><span data-ttu-id="a6934-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a6934-108">Permissions</span></span>
<span data-ttu-id="a6934-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a6934-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a6934-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a6934-111">Permission type</span></span> | <span data-ttu-id="a6934-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a6934-112">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="a6934-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a6934-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="a6934-114">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="a6934-114">Not Supported</span></span>        |
| <span data-ttu-id="a6934-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a6934-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6934-116">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="a6934-116">Not Supported</span></span>        |
| <span data-ttu-id="a6934-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a6934-117">Application</span></span>     | <span data-ttu-id="a6934-118">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="a6934-118">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="a6934-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a6934-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/subscribeToTone
POST /applications/{id}/calls/{id}/subscribeToTone
```

## <a name="request-headers"></a><span data-ttu-id="a6934-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a6934-120">Request headers</span></span>
| <span data-ttu-id="a6934-121">名前</span><span class="sxs-lookup"><span data-stu-id="a6934-121">Name</span></span>          | <span data-ttu-id="a6934-122">説明</span><span class="sxs-lookup"><span data-stu-id="a6934-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="a6934-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6934-123">Authorization</span></span> | <span data-ttu-id="a6934-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a6934-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a6934-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="a6934-126">Request body</span></span>
<span data-ttu-id="a6934-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="a6934-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a6934-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="a6934-128">Parameter</span></span>      | <span data-ttu-id="a6934-129">型</span><span class="sxs-lookup"><span data-stu-id="a6934-129">Type</span></span>    | <span data-ttu-id="a6934-130">説明</span><span class="sxs-lookup"><span data-stu-id="a6934-130">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="a6934-131">clientContext</span><span class="sxs-lookup"><span data-stu-id="a6934-131">clientContext</span></span>  | <span data-ttu-id="a6934-132">String</span><span class="sxs-lookup"><span data-stu-id="a6934-132">String</span></span>  | <span data-ttu-id="a6934-133">クライアントのコンテキスト。</span><span class="sxs-lookup"><span data-stu-id="a6934-133">The client context.</span></span> |

## <a name="response"></a><span data-ttu-id="a6934-134">応答</span><span class="sxs-lookup"><span data-stu-id="a6934-134">Response</span></span>
<span data-ttu-id="a6934-135">返します。`202 Accepted`応答コードと、Location ヘッダーをこの要求用に作成された[commsOperation](../resources/commsoperation.md)の uri を持つ。</span><span class="sxs-lookup"><span data-stu-id="a6934-135">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="a6934-136">例</span><span class="sxs-lookup"><span data-stu-id="a6934-136">Example</span></span>
<span data-ttu-id="a6934-137">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="a6934-137">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="a6934-138">要求</span><span class="sxs-lookup"><span data-stu-id="a6934-138">Request</span></span>
<span data-ttu-id="a6934-139">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="a6934-139">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call_subscribeToTone"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/subscribeToTone
Content-Type: application/json
Content-Length: 46

{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

##### <a name="response"></a><span data-ttu-id="a6934-140">応答</span><span class="sxs-lookup"><span data-stu-id="a6934-140">Response</span></span>

> <span data-ttu-id="a6934-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="a6934-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="a6934-143">通知の操作が完了しました</span><span class="sxs-lookup"><span data-stu-id="a6934-143">Notification - operation completed</span></span>

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
  "description": "call: subscribeToTone",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
