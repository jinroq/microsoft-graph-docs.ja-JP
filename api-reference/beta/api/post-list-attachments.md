---
title: 添付ファイルを一覧表示する
description: 投稿に添付された添付ファイル オブジェクトのリストを取得します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 910e269fb860ff21ecb80b8bcd247f9f9d43c947
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527013"
---
# <a name="list-attachments"></a><span data-ttu-id="c5e2b-103">添付ファイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="c5e2b-103">List attachments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5e2b-104">投稿に添付された[添付ファイル](../resources/attachment.md) オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="c5e2b-104">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a post.</span></span>
## <a name="permissions"></a><span data-ttu-id="c5e2b-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c5e2b-105">Permissions</span></span>
<span data-ttu-id="c5e2b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c5e2b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5e2b-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c5e2b-108">Permission type</span></span>      | <span data-ttu-id="c5e2b-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c5e2b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5e2b-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c5e2b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c5e2b-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5e2b-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c5e2b-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c5e2b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5e2b-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c5e2b-113">Not supported.</span></span>    |
|<span data-ttu-id="c5e2b-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c5e2b-114">Application</span></span> | <span data-ttu-id="c5e2b-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5e2b-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c5e2b-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c5e2b-116">HTTP request</span></span>
<span data-ttu-id="c5e2b-117"><!-- { "blockType": "ignored" } -->[転記](../resources/post.md)グループの[会話](../resources/conversation.md)に属している[スレッド](../resources/conversationthread.md)での添付ファイルです。</span><span class="sxs-lookup"><span data-stu-id="c5e2b-117"><!-- { "blockType": "ignored" } --> Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c5e2b-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c5e2b-118">Optional query parameters</span></span>
<span data-ttu-id="c5e2b-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c5e2b-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="c5e2b-120">$ を使用する具体的には、すべての投稿のプロパティの残りの部分と投稿の添付ファイルのインラインを含むようにクエリ パラメーターを展開します。</span><span class="sxs-lookup"><span data-stu-id="c5e2b-120">In particular, you can use the $expand query parameter to include all of the post attachments inline with the rest of the post properties.</span></span> <span data-ttu-id="c5e2b-121">次に例を示します。</span><span class="sxs-lookup"><span data-stu-id="c5e2b-121">For example:</span></span>

```
GET https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}?$expand=attachments
```
## <a name="request-headers"></a><span data-ttu-id="c5e2b-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c5e2b-122">Request headers</span></span>
| <span data-ttu-id="c5e2b-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c5e2b-123">Header</span></span>       | <span data-ttu-id="c5e2b-124">値</span><span class="sxs-lookup"><span data-stu-id="c5e2b-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c5e2b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5e2b-125">Authorization</span></span>  | <span data-ttu-id="c5e2b-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c5e2b-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c5e2b-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="c5e2b-128">Request body</span></span>
<span data-ttu-id="c5e2b-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c5e2b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5e2b-130">応答</span><span class="sxs-lookup"><span data-stu-id="c5e2b-130">Response</span></span>

<span data-ttu-id="c5e2b-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Attachment](../resources/attachment.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="c5e2b-131">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c5e2b-132">例</span><span class="sxs-lookup"><span data-stu-id="c5e2b-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c5e2b-133">要求</span><span class="sxs-lookup"><span data-stu-id="c5e2b-133">Request</span></span>
<span data-ttu-id="c5e2b-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c5e2b-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="c5e2b-135">応答</span><span class="sxs-lookup"><span data-stu-id="c5e2b-135">Response</span></span>
<span data-ttu-id="c5e2b-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c5e2b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/post-list-attachments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
