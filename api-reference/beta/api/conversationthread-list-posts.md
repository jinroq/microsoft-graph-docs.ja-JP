---
title: 投稿を一覧表示する
description: '指定したスレッドの投稿を取得します。 親スレッドと、スレッドの両方を指定することができますか、 '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 9275540b933a87f266d040e25c37ab22e0371736
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970886"
---
# <a name="list-posts"></a><span data-ttu-id="178e4-104">投稿を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="178e4-104">List posts</span></span>

> <span data-ttu-id="178e4-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="178e4-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="178e4-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="178e4-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="178e4-p103">指定したスレッドの投稿を取得します。親の会話とスレッドの両方を指定したり、親の会話を参照せずにスレッドを指定したりすることができます。</span><span class="sxs-lookup"><span data-stu-id="178e4-p103">Get the posts of the specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="178e4-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="178e4-109">Permissions</span></span>
<span data-ttu-id="178e4-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="178e4-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="178e4-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="178e4-112">Permission type</span></span>      | <span data-ttu-id="178e4-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="178e4-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="178e4-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="178e4-114">Delegated (work or school account)</span></span> | <span data-ttu-id="178e4-115">Group.ReadWrite.All、Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="178e4-115">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="178e4-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="178e4-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="178e4-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="178e4-117">Not supported.</span></span>    |
|<span data-ttu-id="178e4-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="178e4-118">Application</span></span> | <span data-ttu-id="178e4-119">Group.ReadWrite.All、Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="178e4-119">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="178e4-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="178e4-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts
GET /groups/{id}/conversations/{id}/threads/{id}/posts

```
## <a name="optional-query-parameters"></a><span data-ttu-id="178e4-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="178e4-121">Optional query parameters</span></span>
<span data-ttu-id="178e4-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="178e4-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="178e4-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="178e4-123">Request headers</span></span>
| <span data-ttu-id="178e4-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="178e4-124">Header</span></span>       | <span data-ttu-id="178e4-125">値</span><span class="sxs-lookup"><span data-stu-id="178e4-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="178e4-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="178e4-126">Authorization</span></span>  | <span data-ttu-id="178e4-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="178e4-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="178e4-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="178e4-129">Request body</span></span>
<span data-ttu-id="178e4-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="178e4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="178e4-131">応答</span><span class="sxs-lookup"><span data-stu-id="178e4-131">Response</span></span>

<span data-ttu-id="178e4-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Post](../resources/post.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="178e4-132">If successful, this method returns a `200 OK` response code and collection of [Post](../resources/post.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="178e4-133">例</span><span class="sxs-lookup"><span data-stu-id="178e4-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="178e4-134">要求</span><span class="sxs-lookup"><span data-stu-id="178e4-134">Request</span></span>
<span data-ttu-id="178e4-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="178e4-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_posts"
}-->
```http
GET https://graph.microsoft.com/beta/groups/0d75b8dc-c42d-44dd-890a-751a99c0589f/threads/AAQkAD8EJUmcWwTJi06Cew==/posts
```
##### <a name="response"></a><span data-ttu-id="178e4-136">応答</span><span class="sxs-lookup"><span data-stu-id="178e4-136">Response</span></span>
<span data-ttu-id="178e4-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="178e4-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.post",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups('0d75b8dc-c42d-44dd-890a-751a99c0589f')/threads('AAQkAD8EJUmcWwTJi06Cew%3D%3D')/posts",
    "value":[
        {
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
    ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List posts",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
