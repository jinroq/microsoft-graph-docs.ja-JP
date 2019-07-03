---
title: スレッドを一覧表示する
description: グループの会話のすべてのスレッドを取得します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 4462313ce8fbcf2043e4710b58aed83500edb226
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35437488"
---
# <a name="list-threads"></a><span data-ttu-id="3f326-103">スレッドを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="3f326-103">List threads</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f326-104">グループの会話のすべてのスレッドを取得します。</span><span class="sxs-lookup"><span data-stu-id="3f326-104">Get all the threads in a group conversation.</span></span>
<span data-ttu-id="3f326-105">注:[グループのすべてのスレッドを取得する](group-list-threads.md)ことも可能です。</span><span class="sxs-lookup"><span data-stu-id="3f326-105">Note: You can also [get all the threads of a group](group-list-threads.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="3f326-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3f326-106">Permissions</span></span>
<span data-ttu-id="3f326-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3f326-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f326-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3f326-109">Permission type</span></span>      | <span data-ttu-id="3f326-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3f326-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3f326-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3f326-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3f326-112">グループ読み取り。すべてを取得します。</span><span class="sxs-lookup"><span data-stu-id="3f326-112">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="3f326-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3f326-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3f326-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3f326-114">Not supported.</span></span>    |
|<span data-ttu-id="3f326-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3f326-115">Application</span></span> | <span data-ttu-id="3f326-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3f326-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3f326-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3f326-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}/threads
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3f326-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="3f326-118">Optional query parameters</span></span>
<span data-ttu-id="3f326-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="3f326-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3f326-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3f326-120">Request headers</span></span>
| <span data-ttu-id="3f326-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3f326-121">Header</span></span>       | <span data-ttu-id="3f326-122">値</span><span class="sxs-lookup"><span data-stu-id="3f326-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3f326-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3f326-123">Authorization</span></span>  | <span data-ttu-id="3f326-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3f326-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3f326-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="3f326-126">Request body</span></span>
<span data-ttu-id="3f326-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="3f326-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3f326-128">応答</span><span class="sxs-lookup"><span data-stu-id="3f326-128">Response</span></span>

<span data-ttu-id="3f326-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [conversationThread](../resources/conversationthread.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="3f326-129">If successful, this method returns a `200 OK` response code and collection of [conversationThread](../resources/conversationthread.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3f326-130">例</span><span class="sxs-lookup"><span data-stu-id="3f326-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3f326-131">要求</span><span class="sxs-lookup"><span data-stu-id="3f326-131">Request</span></span>
<span data-ttu-id="3f326-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3f326-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3f326-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="3f326-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_threads"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/conversations/{id}/threads
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3f326-134">C#</span><span class="sxs-lookup"><span data-stu-id="3f326-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-threads-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3f326-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="3f326-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-threads-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3f326-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="3f326-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-threads-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3f326-137">応答</span><span class="sxs-lookup"><span data-stu-id="3f326-137">Response</span></span>
<span data-ttu-id="3f326-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3f326-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 536

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List threads",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
