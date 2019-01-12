---
title: 添付ファイルを一覧表示する
description: 投稿に添付された添付ファイル オブジェクトのリストを取得します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 690b4ab540982dc9b7febcd1ea302afbcf8429ab
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916300"
---
# <a name="list-attachments"></a><span data-ttu-id="07d1b-103">添付ファイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="07d1b-103">List attachments</span></span>

> <span data-ttu-id="07d1b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="07d1b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="07d1b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="07d1b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="07d1b-106">投稿に添付された[添付ファイル](../resources/attachment.md) オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="07d1b-106">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a post.</span></span>
## <a name="permissions"></a><span data-ttu-id="07d1b-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="07d1b-107">Permissions</span></span>
<span data-ttu-id="07d1b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="07d1b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07d1b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="07d1b-110">Permission type</span></span>      | <span data-ttu-id="07d1b-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="07d1b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="07d1b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="07d1b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="07d1b-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07d1b-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="07d1b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="07d1b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07d1b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="07d1b-115">Not supported.</span></span>    |
|<span data-ttu-id="07d1b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="07d1b-116">Application</span></span> | <span data-ttu-id="07d1b-117">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07d1b-117">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="07d1b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="07d1b-118">HTTP request</span></span>
<span data-ttu-id="07d1b-119"><!-- { "blockType": "ignored" } -->[転記](../resources/post.md)グループの[会話](../resources/conversation.md)に属している[スレッド](../resources/conversationthread.md)での添付ファイルです。</span><span class="sxs-lookup"><span data-stu-id="07d1b-119"><!-- { "blockType": "ignored" } --> Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="07d1b-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="07d1b-120">Optional query parameters</span></span>
<span data-ttu-id="07d1b-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="07d1b-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="07d1b-122">$ を使用する具体的には、すべての投稿のプロパティの残りの部分と投稿の添付ファイルのインラインを含むようにクエリ パラメーターを展開します。</span><span class="sxs-lookup"><span data-stu-id="07d1b-122">In particular, you can use the $expand query parameter to include all of the post attachments inline with the rest of the post properties.</span></span> <span data-ttu-id="07d1b-123">例:</span><span class="sxs-lookup"><span data-stu-id="07d1b-123">For example:</span></span>

```
GET https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}?$expand=attachments
```
## <a name="request-headers"></a><span data-ttu-id="07d1b-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="07d1b-124">Request headers</span></span>
| <span data-ttu-id="07d1b-125">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="07d1b-125">Header</span></span>       | <span data-ttu-id="07d1b-126">値</span><span class="sxs-lookup"><span data-stu-id="07d1b-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="07d1b-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="07d1b-127">Authorization</span></span>  | <span data-ttu-id="07d1b-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="07d1b-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="07d1b-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="07d1b-130">Request body</span></span>
<span data-ttu-id="07d1b-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="07d1b-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="07d1b-132">応答</span><span class="sxs-lookup"><span data-stu-id="07d1b-132">Response</span></span>

<span data-ttu-id="07d1b-133">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Attachment](../resources/attachment.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="07d1b-133">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="07d1b-134">例</span><span class="sxs-lookup"><span data-stu-id="07d1b-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="07d1b-135">要求</span><span class="sxs-lookup"><span data-stu-id="07d1b-135">Request</span></span>
<span data-ttu-id="07d1b-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="07d1b-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="07d1b-137">応答</span><span class="sxs-lookup"><span data-stu-id="07d1b-137">Response</span></span>
<span data-ttu-id="07d1b-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="07d1b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
