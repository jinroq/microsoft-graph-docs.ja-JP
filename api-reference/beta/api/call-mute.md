---
title: '呼び出す: ミュート'
description: 自体を消すには、アプリケーションを使用できます。
author: VinodRavichandran
ms.openlocfilehash: 54de4aa598500d1effa1c66c74e5809ad3570959
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27341588"
---
# <a name="call-mute"></a><span data-ttu-id="29a2a-103">呼び出す: ミュート</span><span class="sxs-lookup"><span data-stu-id="29a2a-103">call: mute</span></span>

> <span data-ttu-id="29a2a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="29a2a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="29a2a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="29a2a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="29a2a-106">自体を消すには、アプリケーションを使用できます。</span><span class="sxs-lookup"><span data-stu-id="29a2a-106">Allows the application to mute itself.</span></span>

## <a name="permissions"></a><span data-ttu-id="29a2a-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="29a2a-107">Permissions</span></span>
<span data-ttu-id="29a2a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="29a2a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="29a2a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="29a2a-110">Permission type</span></span>                        | <span data-ttu-id="29a2a-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="29a2a-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="29a2a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="29a2a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="29a2a-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="29a2a-113">Not Supported.</span></span>                               |
| <span data-ttu-id="29a2a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="29a2a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29a2a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="29a2a-115">Not Supported.</span></span>                               |
| <span data-ttu-id="29a2a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="29a2a-116">Application</span></span>                            | <span data-ttu-id="29a2a-117">なし。</span><span class="sxs-lookup"><span data-stu-id="29a2a-117">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="29a2a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="29a2a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/mute
POST /applications/{id}/calls/{id}/mute
```

## <a name="request-headers"></a><span data-ttu-id="29a2a-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="29a2a-119">Request headers</span></span>
| <span data-ttu-id="29a2a-120">名前</span><span class="sxs-lookup"><span data-stu-id="29a2a-120">Name</span></span>          | <span data-ttu-id="29a2a-121">説明</span><span class="sxs-lookup"><span data-stu-id="29a2a-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="29a2a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="29a2a-122">Authorization</span></span> | <span data-ttu-id="29a2a-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="29a2a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="29a2a-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="29a2a-125">Request body</span></span>
<span data-ttu-id="29a2a-126">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="29a2a-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="29a2a-127">パラメーター</span><span class="sxs-lookup"><span data-stu-id="29a2a-127">Parameter</span></span>      | <span data-ttu-id="29a2a-128">種類</span><span class="sxs-lookup"><span data-stu-id="29a2a-128">Type</span></span>    |<span data-ttu-id="29a2a-129">説明</span><span class="sxs-lookup"><span data-stu-id="29a2a-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="29a2a-130">clientContext</span><span class="sxs-lookup"><span data-stu-id="29a2a-130">clientContext</span></span>|<span data-ttu-id="29a2a-131">String</span><span class="sxs-lookup"><span data-stu-id="29a2a-131">String</span></span>|<span data-ttu-id="29a2a-132">クライアントのコンテキスト。</span><span class="sxs-lookup"><span data-stu-id="29a2a-132">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="29a2a-133">応答</span><span class="sxs-lookup"><span data-stu-id="29a2a-133">Response</span></span>
<span data-ttu-id="29a2a-134">かどうかは成功すると、このメソッドを返します`200 OK`応答コードおよび応答の本文に[commsOperation](../resources/commsoperation.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="29a2a-134">If successful, this method returns `200 OK` response code and a [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29a2a-135">例</span><span class="sxs-lookup"><span data-stu-id="29a2a-135">Example</span></span>
<span data-ttu-id="29a2a-136">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="29a2a-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="29a2a-137">要求</span><span class="sxs-lookup"><span data-stu-id="29a2a-137">Request</span></span>
<span data-ttu-id="29a2a-138">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="29a2a-138">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call_mute"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/mute
Content-Type: application/json
Content-Length: 46

{
  "clientContext": "clientContext-value"
}
```

##### <a name="response"></a><span data-ttu-id="29a2a-139">応答</span><span class="sxs-lookup"><span data-stu-id="29a2a-139">Response</span></span>

> <span data-ttu-id="29a2a-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="29a2a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "call: mute",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
