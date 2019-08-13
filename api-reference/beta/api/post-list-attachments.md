---
title: 添付ファイルを一覧表示する
description: 投稿に添付された Attachment オブジェクトのリストを取得します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 0cf2e384d56622f6f97f1a49529b8a5178a9e4d9
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36361300"
---
# <a name="list-attachments"></a><span data-ttu-id="83b01-103">添付ファイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="83b01-103">List attachments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83b01-104">投稿に添付された [Attachment](../resources/attachment.md) オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="83b01-104">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a post.</span></span>
## <a name="permissions"></a><span data-ttu-id="83b01-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="83b01-105">Permissions</span></span>
<span data-ttu-id="83b01-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="83b01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83b01-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="83b01-108">Permission type</span></span>      | <span data-ttu-id="83b01-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="83b01-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="83b01-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="83b01-110">Delegated (work or school account)</span></span> | <span data-ttu-id="83b01-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83b01-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="83b01-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="83b01-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83b01-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="83b01-113">Not supported.</span></span>    |
|<span data-ttu-id="83b01-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="83b01-114">Application</span></span> | <span data-ttu-id="83b01-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83b01-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="83b01-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="83b01-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="83b01-117">グループの[会話](../resources/conversation.md)に属する[スレッド](../resources/conversationthread.md)内の[投稿](../resources/post.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="83b01-117">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="83b01-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="83b01-118">Optional query parameters</span></span>
<span data-ttu-id="83b01-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="83b01-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="83b01-120">特に、$expand クエリパラメーターを使用して、post のすべての添付ファイルを残りの post プロパティにインラインで含めることができます。</span><span class="sxs-lookup"><span data-stu-id="83b01-120">In particular, you can use the $expand query parameter to include all of the post attachments inline with the rest of the post properties.</span></span> <span data-ttu-id="83b01-121">次に例を示します。</span><span class="sxs-lookup"><span data-stu-id="83b01-121">For example:</span></span>

```
GET https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}?$expand=attachments
```
## <a name="request-headers"></a><span data-ttu-id="83b01-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="83b01-122">Request headers</span></span>
| <span data-ttu-id="83b01-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="83b01-123">Header</span></span>       | <span data-ttu-id="83b01-124">値</span><span class="sxs-lookup"><span data-stu-id="83b01-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="83b01-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="83b01-125">Authorization</span></span>  | <span data-ttu-id="83b01-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="83b01-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="83b01-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="83b01-128">Request body</span></span>
<span data-ttu-id="83b01-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="83b01-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="83b01-130">応答</span><span class="sxs-lookup"><span data-stu-id="83b01-130">Response</span></span>

<span data-ttu-id="83b01-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Attachment](../resources/attachment.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="83b01-131">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="83b01-132">例</span><span class="sxs-lookup"><span data-stu-id="83b01-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="83b01-133">要求</span><span class="sxs-lookup"><span data-stu-id="83b01-133">Request</span></span>
<span data-ttu-id="83b01-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="83b01-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="83b01-135">プロトコル</span><span class="sxs-lookup"><span data-stu-id="83b01-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_get_attachments"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}/attachments
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="83b01-136">C#</span><span class="sxs-lookup"><span data-stu-id="83b01-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-get-attachments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="83b01-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="83b01-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-get-attachments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="83b01-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="83b01-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-get-attachments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="83b01-139">Java</span><span class="sxs-lookup"><span data-stu-id="83b01-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-get-attachments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="83b01-140">応答</span><span class="sxs-lookup"><span data-stu-id="83b01-140">Response</span></span>
<span data-ttu-id="83b01-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="83b01-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "value": [
    {
      "@odata.type": "#Microsoft.OutlookServices.FileAttachment",
      "id": "id-value",
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "2016-10-19T10:37:00Z",
      "isInline": false,
      "name": "name-value",
      "size": 99
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
