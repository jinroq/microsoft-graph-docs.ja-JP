---
title: 添付ファイルを追加する
description: イベントの添付ファイルを追加するのにには、この API を使用します。 そこから
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: ece15b579bae9e439eb9303c8b594631ce9b9b31
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525228"
---
# <a name="add-attachment"></a><span data-ttu-id="063b4-104">添付ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="063b4-104">Add attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="063b4-p102">[添付ファイル](../resources/attachment.md)をイベントに追加する場合に、この API を使用します。現在、各 REST 要求の合計サイズは 4 MB に制限されているため、追加できる添付ファイルのサイズは 4 MB 未満に制限されます。</span><span class="sxs-lookup"><span data-stu-id="063b4-p102">Use this API to add an [attachment](../resources/attachment.md) to an event. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>

## <a name="permissions"></a><span data-ttu-id="063b4-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="063b4-107">Permissions</span></span>

<span data-ttu-id="063b4-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="063b4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="063b4-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="063b4-110">Permission type</span></span>      | <span data-ttu-id="063b4-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="063b4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="063b4-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="063b4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="063b4-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="063b4-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="063b4-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="063b4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="063b4-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="063b4-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="063b4-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="063b4-116">Application</span></span> | <span data-ttu-id="063b4-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="063b4-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="063b4-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="063b4-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/events/{id}/attachments
POST /users/{id | userPrincipalName}/events/{id}/attachments
```

<!--
POST /groups/{id}/events/{id}/attachments
-->

## <a name="request-headers"></a><span data-ttu-id="063b4-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="063b4-119">Request headers</span></span>

| <span data-ttu-id="063b4-120">名前</span><span class="sxs-lookup"><span data-stu-id="063b4-120">Name</span></span>       | <span data-ttu-id="063b4-121">型</span><span class="sxs-lookup"><span data-stu-id="063b4-121">Type</span></span> | <span data-ttu-id="063b4-122">説明</span><span class="sxs-lookup"><span data-stu-id="063b4-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="063b4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="063b4-123">Authorization</span></span>  | <span data-ttu-id="063b4-124">string</span><span class="sxs-lookup"><span data-stu-id="063b4-124">string</span></span>  | <span data-ttu-id="063b4-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="063b4-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="063b4-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="063b4-127">Content-Type</span></span> | <span data-ttu-id="063b4-128">string</span><span class="sxs-lookup"><span data-stu-id="063b4-128">string</span></span>  | <span data-ttu-id="063b4-p105">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="063b4-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="063b4-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="063b4-131">Request body</span></span>

<span data-ttu-id="063b4-132">要求本文で、[attachment](../resources/attachment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="063b4-132">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="063b4-133">応答</span><span class="sxs-lookup"><span data-stu-id="063b4-133">Response</span></span>

<span data-ttu-id="063b4-134">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [attachment](../resources/attachment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="063b4-134">If successful, this method returns `201 Created` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="063b4-135">例 (添付ファイル)</span><span class="sxs-lookup"><span data-stu-id="063b4-135">Example (file attachment)</span></span>

### <a name="request"></a><span data-ttu-id="063b4-136">要求</span><span class="sxs-lookup"><span data-stu-id="063b4-136">Request</span></span>

<span data-ttu-id="063b4-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="063b4-137">Here is an example of the request.</span></span>
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

<span data-ttu-id="063b4-138">要求本文で、[Attachment](../resources/attachment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="063b4-138">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="063b4-139">応答</span><span class="sxs-lookup"><span data-stu-id="063b4-139">Response</span></span>

<span data-ttu-id="063b4-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="063b4-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="example-item-attachment"></a><span data-ttu-id="063b4-143">例 (項目の添付ファイル)</span><span class="sxs-lookup"><span data-stu-id="063b4-143">Example (item attachment)</span></span>

### <a name="request"></a><span data-ttu-id="063b4-144">要求</span><span class="sxs-lookup"><span data-stu-id="063b4-144">Request</span></span>

<span data-ttu-id="063b4-145">以下は、アイテムの添付ファイルとしてイベントを別のイベントに添付する例です。</span><span class="sxs-lookup"><span data-stu-id="063b4-145">Here is an example which attaches an event with another event as an item attachment.</span></span>

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

### <a name="response"></a><span data-ttu-id="063b4-146">応答</span><span class="sxs-lookup"><span data-stu-id="063b4-146">Response</span></span>

<span data-ttu-id="063b4-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="063b4-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="example-reference-attachment"></a><span data-ttu-id="063b4-150">例 (添付ファイルの参照)</span><span class="sxs-lookup"><span data-stu-id="063b4-150">Example (reference attachment)</span></span>

### <a name="request"></a><span data-ttu-id="063b4-151">要求</span><span class="sxs-lookup"><span data-stu-id="063b4-151">Request</span></span>

<span data-ttu-id="063b4-152">ここでは、既存のイベントへの参照の添付ファイルを追加する要求の例です。</span><span class="sxs-lookup"><span data-stu-id="063b4-152">Here is an example of a request that adds a reference attachment to an existing event.</span></span>
<span data-ttu-id="063b4-153">添付ファイルは、OneDrive 上のフォルダーをポイントします。</span><span class="sxs-lookup"><span data-stu-id="063b4-153">The attachment points to a folder on OneDrive.</span></span>
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

### <a name="response"></a><span data-ttu-id="063b4-154">応答</span><span class="sxs-lookup"><span data-stu-id="063b4-154">Response</span></span>

<span data-ttu-id="063b4-155">ここでは、完全な応答の例です。</span><span class="sxs-lookup"><span data-stu-id="063b4-155">Here is an example of a full response.</span></span>
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
    "Error: /api-reference/beta/api/event-post-attachments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
