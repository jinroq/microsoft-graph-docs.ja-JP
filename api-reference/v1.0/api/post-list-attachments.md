---
title: 添付ファイルを一覧表示する
description: 投稿に添付された Attachment オブジェクトのリストを取得します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: e6182c864a421330f6168582611bc9adb6d1e7b3
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33608575"
---
# <a name="list-attachments"></a><span data-ttu-id="69f86-103">添付ファイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="69f86-103">List attachments</span></span>

<span data-ttu-id="69f86-104">投稿に添付された [Attachment](../resources/attachment.md) オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="69f86-104">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a post.</span></span>
## <a name="permissions"></a><span data-ttu-id="69f86-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="69f86-105">Permissions</span></span>
<span data-ttu-id="69f86-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="69f86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69f86-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="69f86-108">Permission type</span></span>      | <span data-ttu-id="69f86-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="69f86-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="69f86-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="69f86-110">Delegated (work or school account)</span></span> | <span data-ttu-id="69f86-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69f86-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="69f86-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="69f86-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69f86-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="69f86-113">Not supported.</span></span>    |
|<span data-ttu-id="69f86-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="69f86-114">Application</span></span> | <span data-ttu-id="69f86-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69f86-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="69f86-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="69f86-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="69f86-117">グループの[会話](../resources/conversation.md)に属する[スレッド](../resources/conversationthread.md)内の[投稿](../resources/post.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="69f86-117">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="69f86-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="69f86-118">Optional query parameters</span></span>
<span data-ttu-id="69f86-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="69f86-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="69f86-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="69f86-120">Request headers</span></span>
| <span data-ttu-id="69f86-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="69f86-121">Header</span></span>       | <span data-ttu-id="69f86-122">値</span><span class="sxs-lookup"><span data-stu-id="69f86-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="69f86-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="69f86-123">Authorization</span></span>  | <span data-ttu-id="69f86-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="69f86-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="69f86-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="69f86-126">Request body</span></span>
<span data-ttu-id="69f86-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="69f86-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="69f86-128">応答</span><span class="sxs-lookup"><span data-stu-id="69f86-128">Response</span></span>

<span data-ttu-id="69f86-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Attachment](../resources/attachment.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="69f86-129">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="69f86-130">例</span><span class="sxs-lookup"><span data-stu-id="69f86-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="69f86-131">要求</span><span class="sxs-lookup"><span data-stu-id="69f86-131">Request</span></span>
<span data-ttu-id="69f86-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="69f86-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="69f86-133">応答</span><span class="sxs-lookup"><span data-stu-id="69f86-133">Response</span></span>
<span data-ttu-id="69f86-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="69f86-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="69f86-137">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="69f86-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="69f86-138">Visual</span><span class="sxs-lookup"><span data-stu-id="69f86-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_attachments-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="69f86-139">Java</span><span class="sxs-lookup"><span data-stu-id="69f86-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_attachments-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/post-list-attachments.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/post-list-attachments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
