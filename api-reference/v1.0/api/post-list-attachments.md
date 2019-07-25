---
title: 添付ファイルを一覧表示する
description: 投稿に添付された Attachment オブジェクトのリストを取得します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: c700252556c61e147f1b7ff60c0667f8bc4fe406
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888737"
---
# <a name="list-attachments"></a><span data-ttu-id="a32f4-103">添付ファイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="a32f4-103">List attachments</span></span>

<span data-ttu-id="a32f4-104">投稿に添付された [Attachment](../resources/attachment.md) オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="a32f4-104">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a post.</span></span>
## <a name="permissions"></a><span data-ttu-id="a32f4-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a32f4-105">Permissions</span></span>
<span data-ttu-id="a32f4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a32f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a32f4-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a32f4-108">Permission type</span></span>      | <span data-ttu-id="a32f4-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a32f4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a32f4-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a32f4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a32f4-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a32f4-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a32f4-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a32f4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a32f4-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a32f4-113">Not supported.</span></span>    |
|<span data-ttu-id="a32f4-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a32f4-114">Application</span></span> | <span data-ttu-id="a32f4-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a32f4-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a32f4-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a32f4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="a32f4-117">グループの[会話](../resources/conversation.md)に属する[スレッド](../resources/conversationthread.md)内の[投稿](../resources/post.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="a32f4-117">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a32f4-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="a32f4-118">Optional query parameters</span></span>
<span data-ttu-id="a32f4-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="a32f4-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a32f4-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a32f4-120">Request headers</span></span>
| <span data-ttu-id="a32f4-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a32f4-121">Header</span></span>       | <span data-ttu-id="a32f4-122">値</span><span class="sxs-lookup"><span data-stu-id="a32f4-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a32f4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a32f4-123">Authorization</span></span>  | <span data-ttu-id="a32f4-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a32f4-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a32f4-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="a32f4-126">Request body</span></span>
<span data-ttu-id="a32f4-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a32f4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a32f4-128">応答</span><span class="sxs-lookup"><span data-stu-id="a32f4-128">Response</span></span>

<span data-ttu-id="a32f4-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Attachment](../resources/attachment.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="a32f4-129">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a32f4-130">例</span><span class="sxs-lookup"><span data-stu-id="a32f4-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a32f4-131">要求</span><span class="sxs-lookup"><span data-stu-id="a32f4-131">Request</span></span>
<span data-ttu-id="a32f4-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a32f4-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a32f4-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="a32f4-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_get_attachments"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/attachments
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a32f4-134">C#</span><span class="sxs-lookup"><span data-stu-id="a32f4-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-get-attachments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a32f4-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="a32f4-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-get-attachments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a32f4-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="a32f4-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-get-attachments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a32f4-137">Java</span><span class="sxs-lookup"><span data-stu-id="a32f4-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-get-attachments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a32f4-138">応答</span><span class="sxs-lookup"><span data-stu-id="a32f4-138">Response</span></span>
<span data-ttu-id="a32f4-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a32f4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.attachment)",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "value": [
    {
      "@odata.type": "microsoft.graph.fileAttachment",
      "id": "id-value",
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "base64-contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "datetime-value",
      "isInline": false,
      "name": "name-value",
      "size": 99
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
