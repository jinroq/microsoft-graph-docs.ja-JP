---
title: '電話: subscribeToTone'
description: (デュアル トーン多重周波数信号) DTMF を購読します。 これにより、ユーザーは、'プッシュホン' 電話のキーを押したときに通知することができます。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 929fac43017df2bdee106dd9687c221c65a20fbd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916881"
---
# <a name="call-subscribetotone"></a><span data-ttu-id="cf89e-104">電話: subscribeToTone</span><span class="sxs-lookup"><span data-stu-id="cf89e-104">call: subscribeToTone</span></span>

> <span data-ttu-id="cf89e-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cf89e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cf89e-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cf89e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cf89e-107">(デュアル トーン多重周波数信号) DTMF を購読します。</span><span class="sxs-lookup"><span data-stu-id="cf89e-107">Subscribe to DTMF (dual-tone multi-frequency signaling).</span></span> <span data-ttu-id="cf89e-108">これにより、ユーザーは、「プッシュホン」電話キーを押したときに通知することができます。</span><span class="sxs-lookup"><span data-stu-id="cf89e-108">This allows you to be notified when the user presses keys on a "touchtone" phone.</span></span>

## <a name="permissions"></a><span data-ttu-id="cf89e-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cf89e-109">Permissions</span></span>
<span data-ttu-id="cf89e-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cf89e-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cf89e-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cf89e-112">Permission type</span></span> | <span data-ttu-id="cf89e-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cf89e-113">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="cf89e-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cf89e-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="cf89e-115">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="cf89e-115">Not Supported</span></span>        |
| <span data-ttu-id="cf89e-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cf89e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf89e-117">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="cf89e-117">Not Supported</span></span>        |
| <span data-ttu-id="cf89e-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cf89e-118">Application</span></span>     | <span data-ttu-id="cf89e-119">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="cf89e-119">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="cf89e-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cf89e-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/subscribeToTone
POST /applications/{id}/calls/{id}/subscribeToTone
```

## <a name="request-headers"></a><span data-ttu-id="cf89e-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cf89e-121">Request headers</span></span>
| <span data-ttu-id="cf89e-122">名前</span><span class="sxs-lookup"><span data-stu-id="cf89e-122">Name</span></span>          | <span data-ttu-id="cf89e-123">説明</span><span class="sxs-lookup"><span data-stu-id="cf89e-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="cf89e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf89e-124">Authorization</span></span> | <span data-ttu-id="cf89e-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="cf89e-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cf89e-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="cf89e-127">Request body</span></span>
<span data-ttu-id="cf89e-128">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="cf89e-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cf89e-129">パラメーター</span><span class="sxs-lookup"><span data-stu-id="cf89e-129">Parameter</span></span>      | <span data-ttu-id="cf89e-130">Type</span><span class="sxs-lookup"><span data-stu-id="cf89e-130">Type</span></span>    | <span data-ttu-id="cf89e-131">説明</span><span class="sxs-lookup"><span data-stu-id="cf89e-131">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="cf89e-132">clientContext</span><span class="sxs-lookup"><span data-stu-id="cf89e-132">clientContext</span></span>  | <span data-ttu-id="cf89e-133">String</span><span class="sxs-lookup"><span data-stu-id="cf89e-133">String</span></span>  | <span data-ttu-id="cf89e-134">クライアントのコンテキスト。</span><span class="sxs-lookup"><span data-stu-id="cf89e-134">The client context.</span></span> |

## <a name="response"></a><span data-ttu-id="cf89e-135">応答</span><span class="sxs-lookup"><span data-stu-id="cf89e-135">Response</span></span>
<span data-ttu-id="cf89e-136">返します。`202 Accepted`応答コードと、Location ヘッダーをこの要求用に作成された[commsOperation](../resources/commsoperation.md)の uri を持つ。</span><span class="sxs-lookup"><span data-stu-id="cf89e-136">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="cf89e-137">例</span><span class="sxs-lookup"><span data-stu-id="cf89e-137">Example</span></span>
<span data-ttu-id="cf89e-138">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="cf89e-138">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="cf89e-139">要求</span><span class="sxs-lookup"><span data-stu-id="cf89e-139">Request</span></span>
<span data-ttu-id="cf89e-140">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="cf89e-140">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call-subscribeToTone"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/subscribeToTone
Content-Type: application/json
Content-Length: 46

{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

##### <a name="response"></a><span data-ttu-id="cf89e-141">応答</span><span class="sxs-lookup"><span data-stu-id="cf89e-141">Response</span></span>

> <span data-ttu-id="cf89e-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="cf89e-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="cf89e-144">通知の操作が完了しました</span><span class="sxs-lookup"><span data-stu-id="cf89e-144">Notification - operation completed</span></span>

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
