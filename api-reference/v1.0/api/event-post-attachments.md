---
title: 添付ファイルを追加する
description: 添付ファイルをイベントに追加する場合に、この API を使用します。 そこから
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 372842894dccdc5da9d8d4fc7ce3d7442315db55
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33615157"
---
# <a name="add-attachment"></a><span data-ttu-id="0b3d7-104">添付ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="0b3d7-104">Add attachment</span></span>

<span data-ttu-id="0b3d7-p102">[添付ファイル](../resources/attachment.md)をイベントに追加する場合に、この API を使用します。現在、各 REST 要求の合計サイズは 4 MB に制限されているため、追加できる添付ファイルのサイズは 4 MB 未満に制限されます。</span><span class="sxs-lookup"><span data-stu-id="0b3d7-p102">Use this API to add an [attachment](../resources/attachment.md) to an event. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>
## <a name="permissions"></a><span data-ttu-id="0b3d7-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0b3d7-107">Permissions</span></span>
<span data-ttu-id="0b3d7-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0b3d7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b3d7-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0b3d7-110">Permission type</span></span>      | <span data-ttu-id="0b3d7-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0b3d7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b3d7-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0b3d7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0b3d7-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0b3d7-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="0b3d7-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0b3d7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b3d7-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0b3d7-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="0b3d7-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0b3d7-116">Application</span></span> | <span data-ttu-id="0b3d7-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0b3d7-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0b3d7-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0b3d7-118">HTTP request</span></span>
<span data-ttu-id="0b3d7-119">ユーザーの既定の[予定表](../resources/calendar.md)にある[イベント](../resources/event.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="0b3d7-119">Attachments for an [event](../resources/event.md) in the user's default [calendar](../resources/calendar.md).</span></span>

<!--
Attachments for an [event](../resources/event.md) in the user's or group's default [calendar](../resources/calendar.md).
-->
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/attachments
POST /users/{id | userPrincipalName}/events/{id}/attachments

POST /me/calendar/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendar/events/{id}/attachments
```

<!--
POST /groups/{id}/events/{id}/attachments
POST /groups/{id}/calendar/events/{id}/attachments
-->

<span data-ttu-id="0b3d7-120">ユーザーの既定 [calendarGroup](../resources/calendargroup.md) に属する[カレンダー](../resources/calendar.md)内[イベント](../resources/event.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="0b3d7-120">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendars/{id}/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments

POST /me/calendargroup/calendars/{id}/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments
```
<span data-ttu-id="0b3d7-121">ユーザーの [calendarGroup](../resources/calendargroup.md) に属する[カレンダー](../resources/calendar.md)内[イベント](../resources/event.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="0b3d7-121">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="0b3d7-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0b3d7-122">Request headers</span></span>
| <span data-ttu-id="0b3d7-123">名前</span><span class="sxs-lookup"><span data-stu-id="0b3d7-123">Name</span></span>       | <span data-ttu-id="0b3d7-124">型</span><span class="sxs-lookup"><span data-stu-id="0b3d7-124">Type</span></span> | <span data-ttu-id="0b3d7-125">説明</span><span class="sxs-lookup"><span data-stu-id="0b3d7-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0b3d7-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b3d7-126">Authorization</span></span>  | <span data-ttu-id="0b3d7-127">string</span><span class="sxs-lookup"><span data-stu-id="0b3d7-127">string</span></span>  | <span data-ttu-id="0b3d7-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0b3d7-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0b3d7-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0b3d7-130">Content-Type</span></span> | <span data-ttu-id="0b3d7-131">string</span><span class="sxs-lookup"><span data-stu-id="0b3d7-131">string</span></span>  | <span data-ttu-id="0b3d7-p105">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="0b3d7-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0b3d7-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="0b3d7-134">Request body</span></span>
<span data-ttu-id="0b3d7-135">要求本文で、[attachment](../resources/attachment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0b3d7-135">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="0b3d7-136">応答</span><span class="sxs-lookup"><span data-stu-id="0b3d7-136">Response</span></span>

<span data-ttu-id="0b3d7-137">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [attachment](../resources/attachment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0b3d7-137">If successful, this method returns `201 Created` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="0b3d7-138">例 (添付ファイル)</span><span class="sxs-lookup"><span data-stu-id="0b3d7-138">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="0b3d7-139">要求</span><span class="sxs-lookup"><span data-stu-id="0b3d7-139">Request</span></span>
<span data-ttu-id="0b3d7-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0b3d7-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGI1AAAt9AHjAAA="],
  "name": "create_file_attachment_from_event"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/AAMkAGI1AAAt9AHjAAA=/attachments
Content-type: application/json
Content-length: 151

{
    "@odata.type": "#microsoft.graph.fileAttachment",
    "name": "menu.txt",
    "contentBytes": "base64bWFjIGFuZCBjaGVlc2UgdG9kYXk="   
}
```

<span data-ttu-id="0b3d7-141">要求本文で、[Attachment](../resources/attachment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0b3d7-141">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="0b3d7-142">応答</span><span class="sxs-lookup"><span data-stu-id="0b3d7-142">Response</span></span>
<span data-ttu-id="0b3d7-143">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="0b3d7-143">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events('AAMkAGI1AAAt9AHjAAA%3D')/attachments/$entity",
    "@odata.type":"#microsoft.graph.fileAttachment",
    "id":"AAMkAGI1AAAt9AHjAAABEgAQAEdBogju-MJEu6Ngg-1_W0g=",
    "lastModifiedDateTime":"2017-04-15T03:21:49Z",
    "name":"menu.txt",
    "contentType":"text/plain",
    "size":178,
    "isInline":false,
    "contentId":null,
    "contentLocation":null,
    "contentBytes":"base64bWFjIGFuZCBjaGVlc2UgdG9kYXk="
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="0b3d7-144">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="0b3d7-144">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0b3d7-145">Java</span><span class="sxs-lookup"><span data-stu-id="0b3d7-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_file_attachment_from_event-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="example-item-attachment"></a><span data-ttu-id="0b3d7-146">例 (項目の添付ファイル)</span><span class="sxs-lookup"><span data-stu-id="0b3d7-146">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="0b3d7-147">要求</span><span class="sxs-lookup"><span data-stu-id="0b3d7-147">Request</span></span>

<span data-ttu-id="0b3d7-148">以下は、アイテムの添付ファイルとしてイベントを別のイベントに添付する例です。</span><span class="sxs-lookup"><span data-stu-id="0b3d7-148">Here is an example which attaches an event with another event as an item attachment.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGI1AAAt9AHjAAA="],
  "name": "create_item_attachment_from_event"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/AAMkAGI1AAAt9AHjAAA=/attachments
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

##### <a name="response"></a><span data-ttu-id="0b3d7-149">応答</span><span class="sxs-lookup"><span data-stu-id="0b3d7-149">Response</span></span>
<span data-ttu-id="0b3d7-150">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="0b3d7-150">Here is an example of the response.</span></span>
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
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#me/events('AAMkAGI1AAAt9AHjAAA=')/attachments/$entity",
    "@odata.type":"#microsoft.graph.itemAttachment",
    "@odata.id":"https://graph.microsoft.com/v1.0/users('fdcbcf34-2505-4d07-be5b-0a55b699d157@41a5b830-45ac-4f1b-9bfc-baafa3b7db2e')/events('AAMkAGI1AAAt9AHjAAA=')/attachments('AAMkADNkN2Jp5JVnQIe9r0=')",
    "id":"AAMkADNkNJp5JVnQIe9r0=",
    "lastModifiedDateTime":"2016-12-01T22:27:13Z",
    "name":"Holiday event",
    "contentType":null,
    "size":2473,
    "isInline":false
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="0b3d7-151">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="0b3d7-151">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0b3d7-152">Java</span><span class="sxs-lookup"><span data-stu-id="0b3d7-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_item_attachment_from_event-Javascript-snippets.md)]

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
    "Error: /api-reference/v1.0/api/event-post-attachments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/event-post-attachments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
