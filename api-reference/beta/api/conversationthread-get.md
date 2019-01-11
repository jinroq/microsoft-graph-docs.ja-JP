---
title: Get conversationThread
description: 'グループに属している特定のスレッドを取得します。 親スレッドと、スレッドの両方を指定することができますか、 '
localization_priority: Normal
ms.openlocfilehash: 8c9dce87a1e3a4a9fd07c97c1b472d2e4e57ffcc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854510"
---
# <a name="get-conversationthread"></a><span data-ttu-id="b55cd-104">Get conversationThread</span><span class="sxs-lookup"><span data-stu-id="b55cd-104">Get conversationThread</span></span>

> <span data-ttu-id="b55cd-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b55cd-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b55cd-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b55cd-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b55cd-p103">グループに属している特定のスレッドを取得します。親の会話とスレッドの両方を指定したり、親の会話を参照せずにスレッドを指定したりすることができます。</span><span class="sxs-lookup"><span data-stu-id="b55cd-p103">Get a specific thread that belongs to a group. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span> 
## <a name="permissions"></a><span data-ttu-id="b55cd-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b55cd-109">Permissions</span></span>
<span data-ttu-id="b55cd-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b55cd-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b55cd-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b55cd-112">Permission type</span></span>      | <span data-ttu-id="b55cd-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b55cd-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b55cd-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b55cd-114">Delegated (work or school account)</span></span> | <span data-ttu-id="b55cd-115">Group.ReadWrite.All、Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="b55cd-115">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="b55cd-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b55cd-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b55cd-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b55cd-117">Not supported.</span></span>    |
|<span data-ttu-id="b55cd-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b55cd-118">Application</span></span> | <span data-ttu-id="b55cd-119">Group.ReadWrite.All、Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="b55cd-119">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b55cd-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b55cd-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}
GET /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="optional-query-parameters"></a><span data-ttu-id="b55cd-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="b55cd-121">Optional query parameters</span></span>
<span data-ttu-id="b55cd-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="b55cd-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b55cd-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b55cd-123">Request headers</span></span>
| <span data-ttu-id="b55cd-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b55cd-124">Header</span></span>       | <span data-ttu-id="b55cd-125">値</span><span class="sxs-lookup"><span data-stu-id="b55cd-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b55cd-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="b55cd-126">Authorization</span></span>  | <span data-ttu-id="b55cd-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b55cd-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b55cd-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="b55cd-129">Request body</span></span>
<span data-ttu-id="b55cd-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b55cd-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b55cd-131">応答</span><span class="sxs-lookup"><span data-stu-id="b55cd-131">Response</span></span>

<span data-ttu-id="b55cd-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [conversationThread](../resources/conversationthread.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b55cd-132">If successful, this method returns a `200 OK` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b55cd-133">例</span><span class="sxs-lookup"><span data-stu-id="b55cd-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b55cd-134">要求</span><span class="sxs-lookup"><span data-stu-id="b55cd-134">Request</span></span>
<span data-ttu-id="b55cd-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b55cd-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversationthread"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/threads/{id}
```
##### <a name="response"></a><span data-ttu-id="b55cd-136">応答</span><span class="sxs-lookup"><span data-stu-id="b55cd-136">Response</span></span>
<span data-ttu-id="b55cd-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b55cd-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 419

{
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ],
  "topic": "topic-value",
  "hasAttachments": true,
  "lastDeliveredDateTime": "2016-10-19T10:37:00Z",
  "uniqueSenders": [
    "uniqueSenders-value"
  ],
  "ccRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get conversationThread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
