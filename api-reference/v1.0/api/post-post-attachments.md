---
title: 添付ファイルを追加する
description: 添付ファイルを投稿に追加する場合に、この API を使用します。 そこから
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 87bab38e3d6761a2345202302520aa1bf1699566
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33608547"
---
# <a name="add-attachment"></a><span data-ttu-id="e1235-104">添付ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="e1235-104">Add attachment</span></span>

<span data-ttu-id="e1235-p102">[添付ファイル](../resources/attachment.md)を投稿に追加する場合に、この API を使用します。現在、各 REST 要求の合計サイズは 4 MB に制限されているため、追加できる添付ファイルのサイズは 4 MB 未満に制限されます。</span><span class="sxs-lookup"><span data-stu-id="e1235-p102">Use this API to add an [attachment](../resources/attachment.md) to a post. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>

<span data-ttu-id="e1235-107">添付ファイルは、次の種類のいずれかにできます。</span><span class="sxs-lookup"><span data-stu-id="e1235-107">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="e1235-108">ファイル ([fileAttachment](../resources/fileattachment.md) リソース)。</span><span class="sxs-lookup"><span data-stu-id="e1235-108">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="e1235-109">項目 ([itemAttachment](../resources/itemattachment.md) リソースで表される連絡先、イベント、メッセージ)。</span><span class="sxs-lookup"><span data-stu-id="e1235-109">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="e1235-110">ファイルへのリンク ([referenceAttachment](../resources/referenceattachment.md) リソース)。</span><span class="sxs-lookup"><span data-stu-id="e1235-110">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="e1235-111">これらの添付ファイル リソースのすべての種類は、[attachment](../resources/attachment.md) リソースから派生します。</span><span class="sxs-lookup"><span data-stu-id="e1235-111">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="e1235-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e1235-112">Permissions</span></span>
<span data-ttu-id="e1235-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e1235-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1235-115">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e1235-115">Permission type</span></span>      | <span data-ttu-id="e1235-116">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e1235-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1235-117">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e1235-117">Delegated (work or school account)</span></span> | <span data-ttu-id="e1235-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1235-118">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e1235-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e1235-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1235-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e1235-120">Not supported.</span></span>    |
|<span data-ttu-id="e1235-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e1235-121">Application</span></span> | <span data-ttu-id="e1235-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1235-122">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1235-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e1235-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="e1235-124">グループの[会話](../resources/conversation.md)に属する[スレッド](../resources/conversationthread.md)内の[投稿](../resources/post.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="e1235-124">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
POST /groups/{id}/threads/{id}/posts/{id}/attachments
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="e1235-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e1235-125">Request headers</span></span>
| <span data-ttu-id="e1235-126">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e1235-126">Header</span></span>       | <span data-ttu-id="e1235-127">値</span><span class="sxs-lookup"><span data-stu-id="e1235-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e1235-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1235-128">Authorization</span></span>  | <span data-ttu-id="e1235-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e1235-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e1235-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="e1235-131">Request body</span></span>
<span data-ttu-id="e1235-132">要求本文で、[Attachment](../resources/attachment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e1235-132">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e1235-133">応答</span><span class="sxs-lookup"><span data-stu-id="e1235-133">Response</span></span>

<span data-ttu-id="e1235-134">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [Attachment](../resources/attachment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e1235-134">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="e1235-135">例 (添付ファイル)</span><span class="sxs-lookup"><span data-stu-id="e1235-135">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="e1235-136">要求</span><span class="sxs-lookup"><span data-stu-id="e1235-136">Request</span></span>
<span data-ttu-id="e1235-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e1235-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_post"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/attachments
Content-type: application/json
Content-length: 142

{
  "@odata.type": "#microsoft.graph.fileAttachment",
  "name": "name-value",
  "contentBytes": "base64-contentBytes-value"
}
```

<span data-ttu-id="e1235-138">要求本文で、[Attachment](../resources/attachment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e1235-138">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="e1235-139">応答</span><span class="sxs-lookup"><span data-stu-id="e1235-139">Response</span></span>
<span data-ttu-id="e1235-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e1235-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "lastModifiedDateTime": "datetime-value",
  "name": "name-value",
  "contentType": "contentType-value",
  "size": 99,
  "isInline": true,
  "id": "id-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e1235-143">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="e1235-143">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e1235-144">Java</span><span class="sxs-lookup"><span data-stu-id="e1235-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_file_attachment_from_post-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="example-item-attachment"></a><span data-ttu-id="e1235-145">例 (項目の添付ファイル)</span><span class="sxs-lookup"><span data-stu-id="e1235-145">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="e1235-146">要求</span><span class="sxs-lookup"><span data-stu-id="e1235-146">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_post"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/attachments
Content-type: application/json
Content-length: 100

{
  "@odata.type": "#microsoft.graph.itemAttachment",
  "name": "name-value",
  "item": { }
}
```

##### <a name="response"></a><span data-ttu-id="e1235-147">応答</span><span class="sxs-lookup"><span data-stu-id="e1235-147">Response</span></span>
<span data-ttu-id="e1235-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e1235-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "lastModifiedDateTime": "datetime-value",
  "name": "name-value",
  "contentType": "contentType-value",
  "size": 99,
  "isInline": true,
  "id": "id-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e1235-151">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="e1235-151">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e1235-152">Java</span><span class="sxs-lookup"><span data-stu-id="e1235-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_item_attachment_from_post-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/post-post-attachments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/post-post-attachments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
