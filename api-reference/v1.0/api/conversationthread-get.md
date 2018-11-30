---
title: Get conversationThread
description: 'グループに属している特定のスレッドを取得します。 親スレッドと、スレッドの両方を指定することができますか、 '
ms.openlocfilehash: 1c4e0da5a85464c07844c976140425a70fd48b76
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021885"
---
# <a name="get-conversationthread"></a><span data-ttu-id="e3d3a-104">Get conversationThread</span><span class="sxs-lookup"><span data-stu-id="e3d3a-104">Get conversationThread</span></span>

<span data-ttu-id="e3d3a-p102">グループに属している特定のスレッドを取得します。親の会話とスレッドの両方を指定したり、親の会話を参照せずにスレッドを指定したりすることができます。</span><span class="sxs-lookup"><span data-stu-id="e3d3a-p102">Get a specific thread that belongs to a group. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span> 
## <a name="permissions"></a><span data-ttu-id="e3d3a-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e3d3a-107">Permissions</span></span>
<span data-ttu-id="e3d3a-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e3d3a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3d3a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e3d3a-110">Permission type</span></span>      | <span data-ttu-id="e3d3a-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e3d3a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3d3a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e3d3a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e3d3a-113">Group.ReadWrite.All、Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3d3a-113">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="e3d3a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e3d3a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3d3a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e3d3a-115">Not supported.</span></span>    |
|<span data-ttu-id="e3d3a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e3d3a-116">Application</span></span> | <span data-ttu-id="e3d3a-117">Group.ReadWrite.All、Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3d3a-117">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e3d3a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e3d3a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}
GET /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="optional-query-parameters"></a><span data-ttu-id="e3d3a-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e3d3a-119">Optional query parameters</span></span>
<span data-ttu-id="e3d3a-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e3d3a-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e3d3a-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e3d3a-121">Request headers</span></span>
| <span data-ttu-id="e3d3a-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e3d3a-122">Header</span></span>       | <span data-ttu-id="e3d3a-123">値</span><span class="sxs-lookup"><span data-stu-id="e3d3a-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e3d3a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3d3a-124">Authorization</span></span>  | <span data-ttu-id="e3d3a-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e3d3a-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e3d3a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="e3d3a-127">Request body</span></span>
<span data-ttu-id="e3d3a-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e3d3a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3d3a-129">応答</span><span class="sxs-lookup"><span data-stu-id="e3d3a-129">Response</span></span>

<span data-ttu-id="e3d3a-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [conversationThread](../resources/conversationthread.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e3d3a-130">If successful, this method returns a `200 OK` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e3d3a-131">例</span><span class="sxs-lookup"><span data-stu-id="e3d3a-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e3d3a-132">要求</span><span class="sxs-lookup"><span data-stu-id="e3d3a-132">Request</span></span>
<span data-ttu-id="e3d3a-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e3d3a-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversationthread"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}
```
##### <a name="response"></a><span data-ttu-id="e3d3a-134">応答</span><span class="sxs-lookup"><span data-stu-id="e3d3a-134">Response</span></span>
<span data-ttu-id="e3d3a-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e3d3a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "lastDeliveredDateTime": "datetime-value",
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
