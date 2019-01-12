---
title: '電話: cancelMediaProcessing'
description: キャンセル メディアのすべての処理中、PlayPrompt、またはレコードの操作。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: db5a918f630fc54cc6eb574896e9e42af179c05a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921998"
---
# <a name="call-cancelmediaprocessing"></a><span data-ttu-id="bd464-103">電話: cancelMediaProcessing</span><span class="sxs-lookup"><span data-stu-id="bd464-103">call: cancelMediaProcessing</span></span>

> <span data-ttu-id="bd464-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bd464-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bd464-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bd464-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bd464-106">キャンセル メディアのすべての処理中、PlayPrompt、またはレコードの操作。</span><span class="sxs-lookup"><span data-stu-id="bd464-106">Cancels media processing for all in-progress any PlayPrompt or Record operations.</span></span>

## <a name="permissions"></a><span data-ttu-id="bd464-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bd464-107">Permissions</span></span>
<span data-ttu-id="bd464-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bd464-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bd464-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bd464-110">Permission type</span></span>                        | <span data-ttu-id="bd464-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bd464-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bd464-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bd464-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="bd464-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bd464-113">Not Supported.</span></span>                              |
| <span data-ttu-id="bd464-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bd464-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd464-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bd464-115">Not Supported.</span></span>                              |
| <span data-ttu-id="bd464-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bd464-116">Application</span></span>                            | <span data-ttu-id="bd464-117">なし。</span><span class="sxs-lookup"><span data-stu-id="bd464-117">None.</span></span>                                       |

## <a name="http-request"></a><span data-ttu-id="bd464-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bd464-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/cancelMediaProcessing
POST /applications/{id}/calls/{id}/cancelMediaProcessing
```

## <a name="request-headers"></a><span data-ttu-id="bd464-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bd464-119">Request headers</span></span>
| <span data-ttu-id="bd464-120">名前</span><span class="sxs-lookup"><span data-stu-id="bd464-120">Name</span></span>          | <span data-ttu-id="bd464-121">説明</span><span class="sxs-lookup"><span data-stu-id="bd464-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="bd464-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd464-122">Authorization</span></span> | <span data-ttu-id="bd464-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="bd464-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bd464-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="bd464-125">Request body</span></span>
<span data-ttu-id="bd464-126">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="bd464-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="bd464-127">パラメーター</span><span class="sxs-lookup"><span data-stu-id="bd464-127">Parameter</span></span>      | <span data-ttu-id="bd464-128">Type</span><span class="sxs-lookup"><span data-stu-id="bd464-128">Type</span></span>    | <span data-ttu-id="bd464-129">説明</span><span class="sxs-lookup"><span data-stu-id="bd464-129">Description</span></span>                                                    |
|:---------------|:--------|:---------------------------------------------------------------|
| <span data-ttu-id="bd464-130">all</span><span class="sxs-lookup"><span data-stu-id="bd464-130">all</span></span>            | <span data-ttu-id="bd464-131">ブール型</span><span class="sxs-lookup"><span data-stu-id="bd464-131">Boolean</span></span> | <span data-ttu-id="bd464-132">操作または現在のすべてを停止するかどうかを示すフラグです。</span><span class="sxs-lookup"><span data-stu-id="bd464-132">The flag indicating whether to stop all operations or current.</span></span> |
| <span data-ttu-id="bd464-133">clientContext</span><span class="sxs-lookup"><span data-stu-id="bd464-133">clientContext</span></span>  | <span data-ttu-id="bd464-134">String</span><span class="sxs-lookup"><span data-stu-id="bd464-134">String</span></span>  | <span data-ttu-id="bd464-135">クライアントのコンテキスト。</span><span class="sxs-lookup"><span data-stu-id="bd464-135">The client context.</span></span>                                            |

## <a name="response"></a><span data-ttu-id="bd464-136">応答</span><span class="sxs-lookup"><span data-stu-id="bd464-136">Response</span></span>
<span data-ttu-id="bd464-137">返します。`202 Accepted`応答コードと、Location ヘッダーをこの要求用に作成された[commsOperation](../resources/commsoperation.md)の uri を持つ。</span><span class="sxs-lookup"><span data-stu-id="bd464-137">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="bd464-138">例</span><span class="sxs-lookup"><span data-stu-id="bd464-138">Example</span></span>
<span data-ttu-id="bd464-139">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="bd464-139">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="bd464-140">要求</span><span class="sxs-lookup"><span data-stu-id="bd464-140">Request</span></span>
<span data-ttu-id="bd464-141">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="bd464-141">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call-cancelMediaProcessing"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/cancelMediaProcessing
Content-Type: application/json
Content-Length: 62

{
  "all": true,
  "clientContext": "clientContext-value"
}
```

##### <a name="response"></a><span data-ttu-id="bd464-142">応答</span><span class="sxs-lookup"><span data-stu-id="bd464-142">Response</span></span>

> <span data-ttu-id="bd464-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="bd464-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="bd464-145">通知の操作が完了しました</span><span class="sxs-lookup"><span data-stu-id="bd464-145">Notification - operation completed</span></span>

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
  "description": "call: cancelMediaProcessing",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
