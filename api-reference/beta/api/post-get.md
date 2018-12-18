---
title: 投稿を取得する
description: '指定したスレッド内の投稿のプロパティと関係を取得します。 両方の親を指定することができます。 '
author: dkershaw10
ms.openlocfilehash: 98bed589c1982411f3c0b989e28e04d2e6166466
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361237"
---
# <a name="get-post"></a><span data-ttu-id="24b74-104">投稿を取得する</span><span class="sxs-lookup"><span data-stu-id="24b74-104">Get post</span></span>

> <span data-ttu-id="24b74-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="24b74-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="24b74-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="24b74-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="24b74-p103">指定したスレッド内の投稿のプロパティと関係を取得します。親の会話とスレッドの両方を指定したり、親の会話を参照せずにスレッドを指定したりすることができます。</span><span class="sxs-lookup"><span data-stu-id="24b74-p103">Get the properties and relationships of a post in a specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

<span data-ttu-id="24b74-109">**投稿**リソースは[拡張機能](/graph/extensibility-overview)をサポートしているため、`GET` 操作を使用して、**投稿**インスタンスでカスタム プロパティと拡張機能データを取得することもできます。</span><span class="sxs-lookup"><span data-stu-id="24b74-109">Since the **post** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **post** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="24b74-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="24b74-110">Permissions</span></span>
<span data-ttu-id="24b74-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="24b74-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24b74-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="24b74-113">Permission type</span></span>      | <span data-ttu-id="24b74-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="24b74-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="24b74-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="24b74-115">Delegated (work or school account)</span></span> | <span data-ttu-id="24b74-116">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24b74-116">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="24b74-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="24b74-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24b74-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="24b74-118">Not supported.</span></span>    |
|<span data-ttu-id="24b74-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="24b74-119">Application</span></span> | <span data-ttu-id="24b74-120">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24b74-120">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="24b74-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="24b74-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="24b74-122">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="24b74-122">Optional query parameters</span></span>
<span data-ttu-id="24b74-123">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="24b74-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="24b74-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="24b74-124">Request headers</span></span>
| <span data-ttu-id="24b74-125">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="24b74-125">Header</span></span>       | <span data-ttu-id="24b74-126">値</span><span class="sxs-lookup"><span data-stu-id="24b74-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="24b74-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="24b74-127">Authorization</span></span>  | <span data-ttu-id="24b74-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="24b74-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="24b74-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="24b74-130">Request body</span></span>
<span data-ttu-id="24b74-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="24b74-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24b74-132">応答</span><span class="sxs-lookup"><span data-stu-id="24b74-132">Response</span></span>

<span data-ttu-id="24b74-133">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[投稿](../resources/post.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="24b74-133">If successful, this method returns a `200 OK` response code and [post](../resources/post.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="24b74-134">例</span><span class="sxs-lookup"><span data-stu-id="24b74-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="24b74-135">要求</span><span class="sxs-lookup"><span data-stu-id="24b74-135">Request</span></span>
<span data-ttu-id="24b74-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="24b74-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_post"
}-->
```http
GET https://graph.microsoft.com/beta/groups/0d75b8dc-c42d-44dd-890a-751a99c0589f/threads/AAQkAD8EJUmcWwTJi06Cew==/posts/AQMkADgAAAIJbQAAAA==
```
##### <a name="response"></a><span data-ttu-id="24b74-137">応答</span><span class="sxs-lookup"><span data-stu-id="24b74-137">Response</span></span>
<span data-ttu-id="24b74-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="24b74-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.post"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups('0d75b8dc-c42d-44dd-890a-751a99c0589f')/threads('AAQkAD8EJUmcWwTJi06Cew%3D%3D')/posts/$entity",
    "@odata.etag":"W/\"CQAAABYAAAC/3QURwysWS6IJYYw5exv4AAAAAAlK\"",
    "id":"AQMkADgAAAIJbQAAAA==",
    "createdDateTime":"2018-01-11T17:36:17Z",
    "lastModifiedDateTime":"2018-01-11T17:36:17Z",
    "importance": "normal",
    "changeKey":"CQAAABYAAAC/3QURwysWS6IJYYw5exv4AAAAAAlK",
    "categories":[

    ],
    "receivedDateTime":"2018-01-11T17:36:17Z",
    "hasAttachments":false,
    "body":{
        "contentType":"html",
        "content":"<html><body></body></html>"
    },
    "from":{
        "emailAddress":{
            "name":"Marketing",
            "address":"Marketing@M365B489948.onmicrosoft.com"
        }
    },
    "sender":{
        "emailAddress":{
            "name":"Marketing",
            "address":"Marketing@M365B489948.onmicrosoft.com"
        }
    }
}
```

## <a name="see-also"></a><span data-ttu-id="24b74-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="24b74-141">See also</span></span>

- [<span data-ttu-id="24b74-142">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="24b74-142">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="24b74-143">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="24b74-143">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="24b74-144">スキーマ拡張機能を使用したグループへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="24b74-144">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get post",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
