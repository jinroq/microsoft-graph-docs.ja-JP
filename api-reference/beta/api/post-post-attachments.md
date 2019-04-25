---
title: 添付ファイルを追加する
description: 添付ファイルを投稿に追加する場合に、この API を使用します。 存在するため
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 4349673b5400674394db33540f09a407a0a6af33
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32538739"
---
# <a name="add-attachment"></a><span data-ttu-id="36dbe-104">添付ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="36dbe-104">Add attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36dbe-p102">[添付ファイル](../resources/attachment.md)を投稿に追加する場合に、この API を使用します。現在、各 REST 要求の合計サイズは 4 MB に制限されているため、追加できる添付ファイルのサイズは 4 MB 未満に制限されます。</span><span class="sxs-lookup"><span data-stu-id="36dbe-p102">Use this API to add an [attachment](../resources/attachment.md) to a post. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>

<span data-ttu-id="36dbe-107">添付ファイルは、次の種類のいずれかにできます。</span><span class="sxs-lookup"><span data-stu-id="36dbe-107">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="36dbe-108">ファイル ([fileAttachment](../resources/fileattachment.md) リソース)。</span><span class="sxs-lookup"><span data-stu-id="36dbe-108">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="36dbe-109">項目 ([itemAttachment](../resources/itemattachment.md) リソースで表される連絡先、イベント、メッセージ)。</span><span class="sxs-lookup"><span data-stu-id="36dbe-109">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="36dbe-110">ファイルへのリンク ([referenceAttachment](../resources/referenceattachment.md) リソース)。</span><span class="sxs-lookup"><span data-stu-id="36dbe-110">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="36dbe-111">これらの添付ファイル リソースのすべての種類は、[attachment](../resources/attachment.md) リソースから派生します。</span><span class="sxs-lookup"><span data-stu-id="36dbe-111">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="36dbe-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="36dbe-112">Permissions</span></span>
<span data-ttu-id="36dbe-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="36dbe-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36dbe-115">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="36dbe-115">Permission type</span></span>      | <span data-ttu-id="36dbe-116">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="36dbe-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36dbe-117">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="36dbe-117">Delegated (work or school account)</span></span> | <span data-ttu-id="36dbe-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36dbe-118">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="36dbe-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="36dbe-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36dbe-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="36dbe-120">Not supported.</span></span>    |
|<span data-ttu-id="36dbe-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="36dbe-121">Application</span></span> | <span data-ttu-id="36dbe-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36dbe-122">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="36dbe-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="36dbe-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="36dbe-124">グループの[会話](../resources/conversation.md)に属する[スレッド](../resources/conversationthread.md)内の[投稿](../resources/post.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="36dbe-124">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
POST /groups/{id}/threads/{id}/posts/{id}/attachments
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="36dbe-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="36dbe-125">Request headers</span></span>
| <span data-ttu-id="36dbe-126">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="36dbe-126">Header</span></span>       | <span data-ttu-id="36dbe-127">値</span><span class="sxs-lookup"><span data-stu-id="36dbe-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="36dbe-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="36dbe-128">Authorization</span></span>  | <span data-ttu-id="36dbe-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="36dbe-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="36dbe-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="36dbe-131">Request body</span></span>
<span data-ttu-id="36dbe-132">要求本文で、[Attachment](../resources/attachment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="36dbe-132">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="36dbe-133">応答</span><span class="sxs-lookup"><span data-stu-id="36dbe-133">Response</span></span>

<span data-ttu-id="36dbe-134">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [Attachment](../resources/attachment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="36dbe-134">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="36dbe-135">例 (添付ファイル)</span><span class="sxs-lookup"><span data-stu-id="36dbe-135">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="36dbe-136">要求</span><span class="sxs-lookup"><span data-stu-id="36dbe-136">Request</span></span>
<span data-ttu-id="36dbe-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="36dbe-137">Here is an example of the request.</span></span>
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

<span data-ttu-id="36dbe-138">要求本文で、[Attachment](../resources/attachment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="36dbe-138">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="36dbe-139">応答</span><span class="sxs-lookup"><span data-stu-id="36dbe-139">Response</span></span>
<span data-ttu-id="36dbe-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="36dbe-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="example-item-attachment"></a><span data-ttu-id="36dbe-143">例 (項目の添付ファイル)</span><span class="sxs-lookup"><span data-stu-id="36dbe-143">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="36dbe-144">要求</span><span class="sxs-lookup"><span data-stu-id="36dbe-144">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_post"
}-->
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

##### <a name="response"></a><span data-ttu-id="36dbe-145">応答</span><span class="sxs-lookup"><span data-stu-id="36dbe-145">Response</span></span>
<span data-ttu-id="36dbe-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="36dbe-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


## <a name="example-reference-attachment"></a><span data-ttu-id="36dbe-149">例 (添付ファイルの参照)</span><span class="sxs-lookup"><span data-stu-id="36dbe-149">Example (reference attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="36dbe-150">要求</span><span class="sxs-lookup"><span data-stu-id="36dbe-150">Request</span></span>
<span data-ttu-id="36dbe-151">既存の投稿に参照添付ファイルを追加する要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="36dbe-151">Here is an example of a request that adds a reference attachment to an existing post.</span></span>
<span data-ttu-id="36dbe-152">添付ファイルは、OneDrive 上のフォルダーを指します。</span><span class="sxs-lookup"><span data-stu-id="36dbe-152">The attachment points to a folder on OneDrive.</span></span>
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

##### <a name="response"></a><span data-ttu-id="36dbe-153">応答</span><span class="sxs-lookup"><span data-stu-id="36dbe-153">Response</span></span>
<span data-ttu-id="36dbe-154">完全な応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="36dbe-154">Here is an example of a full response.</span></span>
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
    "Error: /api-reference/beta/api/post-post-attachments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
