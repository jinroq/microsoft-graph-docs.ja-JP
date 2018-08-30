# <a name="add-attachment"></a><span data-ttu-id="5501c-101">添付ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="5501c-101">Add attachment</span></span>

<span data-ttu-id="5501c-p101">[添付ファイル](../resources/attachment.md)をイベントに追加する場合に、この API を使用します。現在、各 REST 要求の合計サイズは 4 MB に制限されているため、追加できる添付ファイルのサイズは 4 MB 未満に制限されます。</span><span class="sxs-lookup"><span data-stu-id="5501c-p101">Use this API to add an [attachment](../resources/attachment.md) to an event. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>
## <a name="permissions"></a><span data-ttu-id="5501c-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5501c-104">Permissions</span></span>
<span data-ttu-id="5501c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5501c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5501c-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5501c-107">Permission type</span></span>      | <span data-ttu-id="5501c-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5501c-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5501c-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5501c-109">Delegated (work or school account)</span></span> | <span data-ttu-id="5501c-110">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5501c-110">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="5501c-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5501c-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5501c-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5501c-112">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="5501c-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5501c-113">Application</span></span> | <span data-ttu-id="5501c-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5501c-114">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5501c-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5501c-115">HTTP request</span></span>
<span data-ttu-id="5501c-116">ユーザーの既定[ カレンダー](../resources/event.md)内の[ イベント](../resources/calendar.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="5501c-116">Attachments for an [event](../resources/event.md) in the user's or group's default [calendar](../resources/calendar.md).</span></span>

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

<span data-ttu-id="5501c-117">ユーザーの既定[  calendarGroup](../resources/event.md) に属する[カレンダー](../resources/calendar.md)内[ イベント](../resources/calendargroup.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="5501c-117">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendars/{id}/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments

POST /me/calendargroup/calendars/{id}/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments
```
<span data-ttu-id="5501c-118">ユーザーの [calendarGroup](../resources/calendargroup.md) に属する[カレンダー](../resources/calendar.md)内[イベント](../resources/event.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="5501c-118">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="5501c-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5501c-119">Request headers</span></span>
| <span data-ttu-id="5501c-120">名前</span><span class="sxs-lookup"><span data-stu-id="5501c-120">Name</span></span>       | <span data-ttu-id="5501c-121">型</span><span class="sxs-lookup"><span data-stu-id="5501c-121">Type</span></span> | <span data-ttu-id="5501c-122">説明</span><span class="sxs-lookup"><span data-stu-id="5501c-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5501c-123">承認</span><span class="sxs-lookup"><span data-stu-id="5501c-123">Authorization</span></span>  | <span data-ttu-id="5501c-124">文字列</span><span class="sxs-lookup"><span data-stu-id="5501c-124">string</span></span>  | <span data-ttu-id="5501c-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5501c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5501c-127">コンテンツ - タイプ</span><span class="sxs-lookup"><span data-stu-id="5501c-127">Content-Type</span></span> | <span data-ttu-id="5501c-128">文字列</span><span class="sxs-lookup"><span data-stu-id="5501c-128">string</span></span>  | <span data-ttu-id="5501c-p104">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="5501c-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5501c-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="5501c-131">Request body</span></span>
<span data-ttu-id="5501c-132">要求本文で、[attachment](../resources/attachment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="5501c-132">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="5501c-133">応答</span><span class="sxs-lookup"><span data-stu-id="5501c-133">Response</span></span>

<span data-ttu-id="5501c-134">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [attachment](../resources/attachment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5501c-134">If successful, this method returns `201 Created` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="5501c-135">例 (添付ファイル)</span><span class="sxs-lookup"><span data-stu-id="5501c-135">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="5501c-136">要求</span><span class="sxs-lookup"><span data-stu-id="5501c-136">Request</span></span>
<span data-ttu-id="5501c-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5501c-137">Here is an example of the request.</span></span>
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

<span data-ttu-id="5501c-138">要求本文で、[Attachment](../resources/attachment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="5501c-138">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="5501c-139">応答</span><span class="sxs-lookup"><span data-stu-id="5501c-139">Response</span></span>
<span data-ttu-id="5501c-140">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="5501c-140">Here is an example of the response.</span></span>
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

## <a name="example-item-attachment"></a><span data-ttu-id="5501c-141">例 (項目の添付ファイル)</span><span class="sxs-lookup"><span data-stu-id="5501c-141">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="5501c-142">要求</span><span class="sxs-lookup"><span data-stu-id="5501c-142">Request</span></span>

<span data-ttu-id="5501c-143">以下は、アイテムの添付ファイルとしてイベントを別のイベントに添付する例です。</span><span class="sxs-lookup"><span data-stu-id="5501c-143">Here is an example which attaches an event with another event as an item attachment.</span></span>

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

##### <a name="response"></a><span data-ttu-id="5501c-144">応答</span><span class="sxs-lookup"><span data-stu-id="5501c-144">Response</span></span>
<span data-ttu-id="5501c-145">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="5501c-145">Here is an example of the response.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
