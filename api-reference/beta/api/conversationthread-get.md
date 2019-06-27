---
title: Get conversationThread
description: 'グループに属している特定のスレッドを取得します。 親の会話とスレッドの両方を指定できます。または、 '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: b5b8d69a2d213db6ff357d01939c4b84e68a0dfc
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35261083"
---
# <a name="get-conversationthread"></a><span data-ttu-id="51dda-104">conversationThread を取得する</span><span class="sxs-lookup"><span data-stu-id="51dda-104">Get conversationThread</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51dda-p102">グループに属している特定のスレッドを取得します。親の会話とスレッドの両方を指定したり、親の会話を参照せずにスレッドを指定したりすることができます。</span><span class="sxs-lookup"><span data-stu-id="51dda-p102">Get a specific thread that belongs to a group. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span> 
## <a name="permissions"></a><span data-ttu-id="51dda-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="51dda-107">Permissions</span></span>
<span data-ttu-id="51dda-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="51dda-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51dda-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="51dda-110">Permission type</span></span>      | <span data-ttu-id="51dda-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="51dda-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="51dda-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="51dda-112">Delegated (work or school account)</span></span> | <span data-ttu-id="51dda-113">グループ読み取り。すべてを取得します。</span><span class="sxs-lookup"><span data-stu-id="51dda-113">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="51dda-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="51dda-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51dda-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="51dda-115">Not supported.</span></span>    |
|<span data-ttu-id="51dda-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="51dda-116">Application</span></span> | <span data-ttu-id="51dda-117">グループ読み取り。すべてを取得します。</span><span class="sxs-lookup"><span data-stu-id="51dda-117">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="51dda-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="51dda-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}
GET /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="optional-query-parameters"></a><span data-ttu-id="51dda-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="51dda-119">Optional query parameters</span></span>
<span data-ttu-id="51dda-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="51dda-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="51dda-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="51dda-121">Request headers</span></span>
| <span data-ttu-id="51dda-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="51dda-122">Header</span></span>       | <span data-ttu-id="51dda-123">値</span><span class="sxs-lookup"><span data-stu-id="51dda-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="51dda-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="51dda-124">Authorization</span></span>  | <span data-ttu-id="51dda-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="51dda-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="51dda-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="51dda-127">Request body</span></span>
<span data-ttu-id="51dda-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="51dda-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51dda-129">応答</span><span class="sxs-lookup"><span data-stu-id="51dda-129">Response</span></span>

<span data-ttu-id="51dda-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [conversationThread](../resources/conversationthread.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="51dda-130">If successful, this method returns a `200 OK` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="51dda-131">例</span><span class="sxs-lookup"><span data-stu-id="51dda-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="51dda-132">要求</span><span class="sxs-lookup"><span data-stu-id="51dda-132">Request</span></span>
<span data-ttu-id="51dda-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="51dda-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversationthread"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/threads/{id}
```
##### <a name="response"></a><span data-ttu-id="51dda-134">応答</span><span class="sxs-lookup"><span data-stu-id="51dda-134">Response</span></span>
<span data-ttu-id="51dda-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="51dda-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="51dda-138">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="51dda-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="51dda-139">C#</span><span class="sxs-lookup"><span data-stu-id="51dda-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_conversationthread-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="51dda-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="51dda-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_conversationthread-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="51dda-141">目的-C</span><span class="sxs-lookup"><span data-stu-id="51dda-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_conversationthread-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get conversationThread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/conversationthread-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/conversationthread-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/conversationthread-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
