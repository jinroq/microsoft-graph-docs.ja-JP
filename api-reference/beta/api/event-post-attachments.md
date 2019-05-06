---
title: 添付ファイルを追加する
description: 添付ファイルをイベントに追加する場合に、この API を使用します。 そこから
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 238afc378ac7e49cb39a07308c8b1e176cbd11ae
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33586737"
---
# <a name="add-attachment"></a><span data-ttu-id="56e55-104">添付ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="56e55-104">Add attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56e55-p102">[添付ファイル](../resources/attachment.md)をイベントに追加する場合に、この API を使用します。現在、各 REST 要求の合計サイズは 4 MB に制限されているため、追加できる添付ファイルのサイズは 4 MB 未満に制限されます。</span><span class="sxs-lookup"><span data-stu-id="56e55-p102">Use this API to add an [attachment](../resources/attachment.md) to an event. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>

## <a name="permissions"></a><span data-ttu-id="56e55-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="56e55-107">Permissions</span></span>

<span data-ttu-id="56e55-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="56e55-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56e55-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="56e55-110">Permission type</span></span>      | <span data-ttu-id="56e55-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="56e55-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="56e55-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="56e55-112">Delegated (work or school account)</span></span> | <span data-ttu-id="56e55-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="56e55-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="56e55-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="56e55-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56e55-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="56e55-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="56e55-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="56e55-116">Application</span></span> | <span data-ttu-id="56e55-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="56e55-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="56e55-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="56e55-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/events/{id}/attachments
POST /users/{id | userPrincipalName}/events/{id}/attachments
```

<!--
POST /groups/{id}/events/{id}/attachments
-->

## <a name="request-headers"></a><span data-ttu-id="56e55-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="56e55-119">Request headers</span></span>

| <span data-ttu-id="56e55-120">名前</span><span class="sxs-lookup"><span data-stu-id="56e55-120">Name</span></span>       | <span data-ttu-id="56e55-121">型</span><span class="sxs-lookup"><span data-stu-id="56e55-121">Type</span></span> | <span data-ttu-id="56e55-122">説明</span><span class="sxs-lookup"><span data-stu-id="56e55-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="56e55-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="56e55-123">Authorization</span></span>  | <span data-ttu-id="56e55-124">string</span><span class="sxs-lookup"><span data-stu-id="56e55-124">string</span></span>  | <span data-ttu-id="56e55-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="56e55-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="56e55-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="56e55-127">Content-Type</span></span> | <span data-ttu-id="56e55-128">string</span><span class="sxs-lookup"><span data-stu-id="56e55-128">string</span></span>  | <span data-ttu-id="56e55-p105">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="56e55-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="56e55-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="56e55-131">Request body</span></span>

<span data-ttu-id="56e55-132">要求本文で、[attachment](../resources/attachment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="56e55-132">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="56e55-133">応答</span><span class="sxs-lookup"><span data-stu-id="56e55-133">Response</span></span>

<span data-ttu-id="56e55-134">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [attachment](../resources/attachment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="56e55-134">If successful, this method returns `201 Created` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="56e55-135">例 (添付ファイル)</span><span class="sxs-lookup"><span data-stu-id="56e55-135">Example (file attachment)</span></span>

### <a name="request"></a><span data-ttu-id="56e55-136">要求</span><span class="sxs-lookup"><span data-stu-id="56e55-136">Request</span></span>

<span data-ttu-id="56e55-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="56e55-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_event"
}-->

```http
POST https://graph.microsoft.com/beta/me/events('AAMkAGI1AAAt9AHjAAA=')/attachments
Content-type: application/json
Content-length: 151

{
    "@odata.type": "#microsoft.graph.fileAttachment",
    "name": "menu.txt",
    "contentBytes": "bWFjIGFuZCBjaGVlc2UgdG9kYXk="
}
```

<span data-ttu-id="56e55-138">要求本文で、[Attachment](../resources/attachment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="56e55-138">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="56e55-139">応答</span><span class="sxs-lookup"><span data-stu-id="56e55-139">Response</span></span>

<span data-ttu-id="56e55-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="56e55-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->

```http
HTTP 201 Created
Content-Length: 735

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events('AAMkAGI1AAAt9AHjAAA%3D')/attachments/$entity",
    "@odata.type":"#microsoft.graph.fileAttachment",
    "id":"AAMkAGI1AAAt9AHjAAABEgAQAEdBogju-MJEu6Ngg-1_W0g=",
    "lastModifiedDateTime":"2017-04-15T03:21:49Z",
    "name":"menu.txt",
    "contentType":"text/plain",
    "size":178,
    "isInline":false,
    "contentId":null,
    "contentLocation":null,
    "contentBytes":"bWFjIGFuZCBjaGVlc2UgdG9kYXk="
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="56e55-143">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="56e55-143">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="56e55-144">Java</span><span class="sxs-lookup"><span data-stu-id="56e55-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_file_attachment_from_event-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="example-item-attachment"></a><span data-ttu-id="56e55-145">例 (項目の添付ファイル)</span><span class="sxs-lookup"><span data-stu-id="56e55-145">Example (item attachment)</span></span>

### <a name="request"></a><span data-ttu-id="56e55-146">要求</span><span class="sxs-lookup"><span data-stu-id="56e55-146">Request</span></span>

<span data-ttu-id="56e55-147">以下は、アイテムの添付ファイルとしてイベントを別のイベントに添付する例です。</span><span class="sxs-lookup"><span data-stu-id="56e55-147">Here is an example which attaches an event with another event as an item attachment.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_event"
}-->

```http
POST https://graph.microsoft.com/beta/me/events/{AAMkAGI1AAAt9AHjAAA=}/attachments
Content-type: application/json
Content-length: 600

{
  "@odata.type": "#microsoft.graph.itemAttachment",
  "name": "Holiday event",
  "item": {
        "@odata.type": "microsoft.graph.event",
        "subject": "Discuss gifts for children",
        "body": {
            "contentType": "HTML",
            "content": "Let's look for funding!"
         },
         "start": {
             "dateTime": "2016-12-02T18:00:00",
             "timeZone": "Pacific Standard Time"
          },
          "end": {
             "dateTime": "2016-12-02T19:00:00",
             "timeZone": "Pacific Standard Time"
          }
    }
}
```

### <a name="response"></a><span data-ttu-id="56e55-148">応答</span><span class="sxs-lookup"><span data-stu-id="56e55-148">Response</span></span>

<span data-ttu-id="56e55-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="56e55-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->

```http
HTTP 201 Created
Content-type: application/json
Content-length: 162

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#me/events('AAMkAGI1AAAt9AHjAAA=')/attachments/$entity",
    "@odata.type":"#microsoft.graph.itemAttachment",
    "@odata.id":"https://graph.microsoft.com/beta/users('fdcbcf34-2505-4d07-be5b-0a55b699d157@41a5b830-45ac-4f1b-9bfc-baafa3b7db2e')/events('AAMkAGI1AAAt9AHjAAA=')/attachments('AAMkADNkN2Jp5JVnQIe9r0=')",
    "id":"AAMkADNkNJp5JVnQIe9r0=",
    "lastModifiedDateTime":"2016-12-01T22:27:13Z",
    "name":"Holiday event",
    "contentType":null,
    "size":2473,
    "isInline":false
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="56e55-152">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="56e55-152">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="56e55-153">Java</span><span class="sxs-lookup"><span data-stu-id="56e55-153">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_item_attachment_from_event-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="example-reference-attachment"></a><span data-ttu-id="56e55-154">例 (添付ファイルの参照)</span><span class="sxs-lookup"><span data-stu-id="56e55-154">Example (reference attachment)</span></span>

### <a name="request"></a><span data-ttu-id="56e55-155">要求</span><span class="sxs-lookup"><span data-stu-id="56e55-155">Request</span></span>

<span data-ttu-id="56e55-156">以下は、既存のイベントに参照添付ファイルを追加する要求の例です。</span><span class="sxs-lookup"><span data-stu-id="56e55-156">Here is an example of a request that adds a reference attachment to an existing event.</span></span>
<span data-ttu-id="56e55-157">添付ファイルは、OneDrive 上のフォルダーを指します。</span><span class="sxs-lookup"><span data-stu-id="56e55-157">The attachment points to a folder on OneDrive.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_reference_attachment_from_event",
  "@odata.type": "microsoft.graph.referenceAttachment"
}-->

```http
POST https://graph.microsoft.com/beta/me/events/AAMkAGE1M88AADUv0uAAAG=/attachments
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

### <a name="response"></a><span data-ttu-id="56e55-158">応答</span><span class="sxs-lookup"><span data-stu-id="56e55-158">Response</span></span>

<span data-ttu-id="56e55-159">完全な応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="56e55-159">Here is an example of a full response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.referenceAttachment"
} -->

```http
HTTP 201 Created

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users/ddfcd489-628b-40d7-b48b-57002df800e5/events/AAMkAGE1M88AADUv0uAAAG%3D/attachments/$entity",
  "@odata.type": "#microsoft.graph.referenceAttachment",
  "id": "AAMkAGE1Mg72tgf7hJp0PCGVCIc0g=",
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="56e55-160">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="56e55-160">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="56e55-161">Java</span><span class="sxs-lookup"><span data-stu-id="56e55-161">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_reference_attachment_from_event-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/event-post-attachments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/event-post-attachments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/event-post-attachments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: create_file_attachment_from_event/contentBytes:\r\n      Expected type Binary but actual was String. Property: contentBytes, actual value: 'bWFjIGFuZCBjaGVlc2UgdG9kYXk='"
  ]
}
-->
