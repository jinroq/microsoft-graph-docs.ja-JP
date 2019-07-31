---
title: 添付ファイルを追加する
description: 添付ファイルを投稿に追加する場合に、この API を使用します。 そこから
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 2b54818d602d9226303c96cb002cf72e453cae13
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35983419"
---
# <a name="add-attachment"></a><span data-ttu-id="cc967-104">添付ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="cc967-104">Add attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc967-p102">[添付ファイル](../resources/attachment.md)を投稿に追加する場合に、この API を使用します。現在、各 REST 要求の合計サイズは 4 MB に制限されているため、追加できる添付ファイルのサイズは 4 MB 未満に制限されます。</span><span class="sxs-lookup"><span data-stu-id="cc967-p102">Use this API to add an [attachment](../resources/attachment.md) to a post. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>

<span data-ttu-id="cc967-107">添付ファイルは、次の種類のいずれかにできます。</span><span class="sxs-lookup"><span data-stu-id="cc967-107">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="cc967-108">ファイル ([fileAttachment](../resources/fileattachment.md) リソース)。</span><span class="sxs-lookup"><span data-stu-id="cc967-108">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="cc967-109">項目 ([itemAttachment](../resources/itemattachment.md) リソースで表される連絡先、イベント、メッセージ)。</span><span class="sxs-lookup"><span data-stu-id="cc967-109">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="cc967-110">ファイルへのリンク ([referenceAttachment](../resources/referenceattachment.md) リソース)。</span><span class="sxs-lookup"><span data-stu-id="cc967-110">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="cc967-111">これらの添付ファイル リソースのすべての種類は、[attachment](../resources/attachment.md) リソースから派生します。</span><span class="sxs-lookup"><span data-stu-id="cc967-111">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="cc967-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cc967-112">Permissions</span></span>
<span data-ttu-id="cc967-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cc967-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc967-115">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cc967-115">Permission type</span></span>      | <span data-ttu-id="cc967-116">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cc967-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc967-117">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cc967-117">Delegated (work or school account)</span></span> | <span data-ttu-id="cc967-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc967-118">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="cc967-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cc967-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc967-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cc967-120">Not supported.</span></span>    |
|<span data-ttu-id="cc967-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cc967-121">Application</span></span> | <span data-ttu-id="cc967-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc967-122">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cc967-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cc967-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="cc967-124">グループの[会話](../resources/conversation.md)に属する[スレッド](../resources/conversationthread.md)内の[投稿](../resources/post.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="cc967-124">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
POST /groups/{id}/threads/{id}/posts/{id}/attachments
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="cc967-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cc967-125">Request headers</span></span>
| <span data-ttu-id="cc967-126">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cc967-126">Header</span></span>       | <span data-ttu-id="cc967-127">値</span><span class="sxs-lookup"><span data-stu-id="cc967-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cc967-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc967-128">Authorization</span></span>  | <span data-ttu-id="cc967-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="cc967-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cc967-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="cc967-131">Request body</span></span>
<span data-ttu-id="cc967-132">要求本文で、[Attachment](../resources/attachment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="cc967-132">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="cc967-133">応答</span><span class="sxs-lookup"><span data-stu-id="cc967-133">Response</span></span>

<span data-ttu-id="cc967-134">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [Attachment](../resources/attachment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="cc967-134">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="cc967-135">例 (添付ファイル)</span><span class="sxs-lookup"><span data-stu-id="cc967-135">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="cc967-136">要求</span><span class="sxs-lookup"><span data-stu-id="cc967-136">Request</span></span>
<span data-ttu-id="cc967-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cc967-137">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="cc967-138">プロトコル</span><span class="sxs-lookup"><span data-stu-id="cc967-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_post"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}/attachments
Content-type: application/json
Content-length: 142

{
  "@odata.type": "#microsoft.graph.fileAttachment",
  "name": "name-value",
  "contentBytes": "contentBytes-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cc967-139">C#</span><span class="sxs-lookup"><span data-stu-id="cc967-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-file-attachment-from-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cc967-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="cc967-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-file-attachment-from-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cc967-141">目的-C</span><span class="sxs-lookup"><span data-stu-id="cc967-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-file-attachment-from-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="cc967-142">Java</span><span class="sxs-lookup"><span data-stu-id="cc967-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-file-attachment-from-post-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="cc967-143">要求本文で、[Attachment](../resources/attachment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="cc967-143">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="cc967-144">応答</span><span class="sxs-lookup"><span data-stu-id="cc967-144">Response</span></span>
<span data-ttu-id="cc967-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cc967-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 162

{
  "lastModifiedDateTime": "2016-10-19T10:37:00Z",
  "name": "name-value",
  "contentType": "contentType-value",
  "size": 99,
  "isInline": true,
  "id": "id-value"
}
```

## <a name="example-item-attachment"></a><span data-ttu-id="cc967-148">例 (項目の添付ファイル)</span><span class="sxs-lookup"><span data-stu-id="cc967-148">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="cc967-149">要求</span><span class="sxs-lookup"><span data-stu-id="cc967-149">Request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}/attachments
Content-type: application/json
Content-length: 100

{
  "@odata.type": "#microsoft.graph.itemAttachment",
  "name": "name-value",
  "item": { }
}
```


##### <a name="response"></a><span data-ttu-id="cc967-150">応答</span><span class="sxs-lookup"><span data-stu-id="cc967-150">Response</span></span>
<span data-ttu-id="cc967-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cc967-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 162

{
  "lastModifiedDateTime": "2016-10-19T10:37:00Z",
  "name": "name-value",
  "contentType": "contentType-value",
  "size": 99,
  "isInline": true,
  "id": "id-value"
}
```

## <a name="example-reference-attachment"></a><span data-ttu-id="cc967-154">例 (添付ファイルの参照)</span><span class="sxs-lookup"><span data-stu-id="cc967-154">Example (reference attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="cc967-155">要求</span><span class="sxs-lookup"><span data-stu-id="cc967-155">Request</span></span>
<span data-ttu-id="cc967-156">既存の投稿に参照添付ファイルを追加する要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cc967-156">Here is an example of a request that adds a reference attachment to an existing post.</span></span>
<span data-ttu-id="cc967-157">添付ファイルは、OneDrive 上のフォルダーを指します。</span><span class="sxs-lookup"><span data-stu-id="cc967-157">The attachment points to a folder on OneDrive.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="cc967-158">プロトコル</span><span class="sxs-lookup"><span data-stu-id="cc967-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_reference_attachment_from_post",
  "@odata.type": "microsoft.graph.referenceAttachment"
}-->

```
POST https://graph.microsoft.com/beta/groups/c75831bdfad/threads/AAQkAGF97XEKhULw/posts/AAMkAGFcAAA/attachments
Content-type: application/json
Content-length: 319

{ 
    "@odata.type": "#microsoft.graph.referenceAttachment", 
    "name": "Personal pictures", 
    "sourceUrl": "https://contoso.com/personal/mario_contoso_net/Documents/Pics", 
    "providerType": "oneDriveConsumer", 
    "permission": "Edit", 
    "isFolder": "True" 
} 
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cc967-159">C#</span><span class="sxs-lookup"><span data-stu-id="cc967-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-reference-attachment-from-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cc967-160">Javascript</span><span class="sxs-lookup"><span data-stu-id="cc967-160">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-reference-attachment-from-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cc967-161">目的-C</span><span class="sxs-lookup"><span data-stu-id="cc967-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-reference-attachment-from-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="cc967-162">Java</span><span class="sxs-lookup"><span data-stu-id="cc967-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-reference-attachment-from-post-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="cc967-163">応答</span><span class="sxs-lookup"><span data-stu-id="cc967-163">Response</span></span>
<span data-ttu-id="cc967-164">完全な応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cc967-164">Here is an example of a full response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.referenceAttachment"
} -->
```http
HTTP 201 Created

{
  "@odata.context": "https://graph.microsoft.com/beta/groups/c75831bdfad/threads/AAQkAGF97XEKhULw/posts/AAMkAGFcAAA/attachments/$entity",
  "@odata.type": "#microsoft.graph.referenceAttachment",
  "id": "AAMkAGE1Mg72tgf7hJp0PICVGCc0g=",
  "lastModifiedDateTime": "2016-03-12T06:04:38Z",
  "name": "Personal pictures",
  "contentType": null,
  "size": 382,
  "isInline": false,
  "sourceUrl": "https://contoso.com/personal/mario_contoso_net/Documents/Pics",
  "providerType": "oneDriveConsumer",
  "thumbnailUrl": null,
  "previewUrl": null,
  "permission": "edit",
  "isFolder": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
