---
title: eventMessage の取得
description: 展開 '**イベント**のパラメーター
ms.openlocfilehash: 8f0498864a9d71846fec3854257789d6641d57e6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066976"
---
# <a name="get-eventmessage"></a><span data-ttu-id="56246-103">eventMessage の取得</span><span class="sxs-lookup"><span data-stu-id="56246-103">Get eventMessage</span></span>

> <span data-ttu-id="56246-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="56246-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="56246-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="56246-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="56246-106">[eventMessage](../resources/eventmessage.md) オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="56246-106">Get the properties and relationships of the [eventMessage](../resources/eventmessage.md) object.</span></span> <span data-ttu-id="56246-107">適用、 `$expand` 、出席者の予定表に関連する[イベント](../resources/event.md)を取得する**イベント**のナビゲーション プロパティのパラメーターです。</span><span class="sxs-lookup"><span data-stu-id="56246-107">Apply the `$expand` parameter on the **event** navigation property to get the associated [event](../resources/event.md) in an attendee's calendar.</span></span>

### <a name="get-the-event-message-body-in-html-or-text-format"></a><span data-ttu-id="56246-108">イベント メッセージの本文を html 形式またはテキスト形式で取得します。</span><span class="sxs-lookup"><span data-stu-id="56246-108">Get the event message body in HTML or text format</span></span>

<span data-ttu-id="56246-109">イベント メッセージの本文は、html 形式またはテキスト形式で指定できます。</span><span class="sxs-lookup"><span data-stu-id="56246-109">Event message bodies can be in HTML or text format.</span></span>

<span data-ttu-id="56246-110">使用することができます、`Prefer: outlook.body-content-type`の**本体**と**uniqueBody**のプロパティで、目的の形式を指定するのにはヘッダーが返されます、`GET`の要求。</span><span class="sxs-lookup"><span data-stu-id="56246-110">You can use the `Prefer: outlook.body-content-type` header to specify the desired format returned in the **body** and **uniqueBody** properties in a `GET` request:</span></span>

- <span data-ttu-id="56246-111">指定`Prefer: outlook.body-content-type="text"`テキスト形式で返されるイベント メッセージの本文を取得します。</span><span class="sxs-lookup"><span data-stu-id="56246-111">Specify `Prefer: outlook.body-content-type="text"` to get a event message body returned in text format.</span></span>
- <span data-ttu-id="56246-112">指定`Prefer: outlook.body-content-type="html"`、または、イベント メッセージの本文を HTML 形式で取得するのには、ヘッダーをスキップしています。</span><span class="sxs-lookup"><span data-stu-id="56246-112">Specify `Prefer: outlook.body-content-type="html"`, or just skip the header, to return the event message body in HTML format.</span></span>

<span data-ttu-id="56246-113">いずれかのヘッダーを指定すると、応答には対応する `Preference-Applied` ヘッダーが確認として含まれます。</span><span class="sxs-lookup"><span data-stu-id="56246-113">If you specify either header, the response will include the corresponding `Preference-Applied` header as confirmation:</span></span>

- <span data-ttu-id="56246-114">テキスト形式要求の場合: `Preference-Applied: outlook.body-content-type="text"`</span><span class="sxs-lookup"><span data-stu-id="56246-114">For text format requests: `Preference-Applied: outlook.body-content-type="text"`</span></span>
- <span data-ttu-id="56246-115">HTML 形式要求の場合: `Preference-Applied: outlook.body-content-type="html"`</span><span class="sxs-lookup"><span data-stu-id="56246-115">For HTML format requests: `Preference-Applied: outlook.body-content-type="html"`</span></span>

## <a name="permissions"></a><span data-ttu-id="56246-116">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="56246-116">Permissions</span></span>
<span data-ttu-id="56246-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="56246-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56246-119">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="56246-119">Permission type</span></span>      | <span data-ttu-id="56246-120">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="56246-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="56246-121">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="56246-121">Delegated (work or school account)</span></span> | <span data-ttu-id="56246-122">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="56246-122">Mail.Read</span></span>    |
|<span data-ttu-id="56246-123">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="56246-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56246-124">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="56246-124">Mail.Read</span></span>    |
|<span data-ttu-id="56246-125">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="56246-125">Application</span></span> | <span data-ttu-id="56246-126">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="56246-126">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="56246-127">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="56246-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}

GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="56246-128">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="56246-128">Optional query parameters</span></span>
<span data-ttu-id="56246-129">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="56246-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="56246-130">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="56246-130">Request headers</span></span>
| <span data-ttu-id="56246-131">名前</span><span class="sxs-lookup"><span data-stu-id="56246-131">Name</span></span>       | <span data-ttu-id="56246-132">型</span><span class="sxs-lookup"><span data-stu-id="56246-132">Type</span></span> | <span data-ttu-id="56246-133">説明</span><span class="sxs-lookup"><span data-stu-id="56246-133">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="56246-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="56246-134">Authorization</span></span>  | <span data-ttu-id="56246-135">string</span><span class="sxs-lookup"><span data-stu-id="56246-135">string</span></span>  | <span data-ttu-id="56246-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="56246-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="56246-138">要求本文</span><span class="sxs-lookup"><span data-stu-id="56246-138">Request body</span></span>
<span data-ttu-id="56246-139">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="56246-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="56246-140">応答</span><span class="sxs-lookup"><span data-stu-id="56246-140">Response</span></span>

<span data-ttu-id="56246-141">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [eventMessage](../resources/eventmessage.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="56246-141">If successful, this method returns a `200 OK` response code and [eventMessage](../resources/eventmessage.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="56246-142">例</span><span class="sxs-lookup"><span data-stu-id="56246-142">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="56246-143">要求 1</span><span class="sxs-lookup"><span data-stu-id="56246-143">Request 1</span></span>
<span data-ttu-id="56246-144">最初の例では、イベント メッセージ ID に基づいてイベント メッセージのプロパティを取得する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="56246-144">The first example shows how to get the properties of an event message based on the event message ID.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_eventmessage"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages('AAMkADYAAAImV_lAAA=')
```
##### <a name="response-1"></a><span data-ttu-id="56246-145">応答 1</span><span class="sxs-lookup"><span data-stu-id="56246-145">Response 1</span></span>
<span data-ttu-id="56246-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="56246-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_eventmessage",
  "truncated": true,
  "@odata.type": "microsoft.graph.eventMessageRequest"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('8fd6e83b-3cc0-4bf0-8b26-950f4d7110f6')/messages/$entity",
    "@odata.type":"#microsoft.graph.eventMessageRequest",
    "@odata.etag":"W/\"CwAAABYAAABXlB/SL0N4Q6g6o+jSYAEuAAAImkVD\"",
    "id":"AAMkADYAAAImV_lAAA=",
    "createdDateTime":"2017-12-27T21:58:36Z",
    "lastModifiedDateTime":"2017-12-27T23:26:38Z",
    "changeKey":"CwAAABYAAABXlB/SL0N4Q6g6o+jSYAEuAAAImkVD",
    "categories":[

    ],
    "receivedDateTime":"2017-12-27T21:58:36Z",
    "sentDateTime":"2017-12-27T21:58:36Z",
    "hasAttachments":false,
    "internetMessageId":"<MWHPR1301MB2110DCFC@MWHPR1301MB2110.namprd13.prod.outlook.com>",
    "subject":"Debrief from meetup",
    "bodyPreview":"Let's debrief after community meetup.",
    "importance":"normal",
    "parentFolderId":"AQMkADYAAAIBDAAAAA==",
    "conversationId":"AAQkADYCipTiRjXQORU=",
    "conversationIndex":"AdN/Xdgnql4N9FlrT0KKlOJGNdA5FQ==",
    "isDeliveryReceiptRequested":null,
    "isReadReceiptRequested":false,
    "isRead":false,
    "isDraft":false,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADYAAAImV%2BlAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification":"focused",
    "unsubscribeData":[

    ],
    "unsubscribeEnabled":false,
    "meetingMessageType":"meetingRequest",
    "type":"singleInstance",
    "isOutOfDate":false,
    "isAllDay":false,
    "isDelegated":false,
    "responseRequested":true,
    "body":{
        "contentType":"html",
        "content":"<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n<style type=\"text/css\" style=\"display:none\">\r\n<!--\r\np\r\n\t{margin-top:0;\r\n\tmargin-bottom:0}\r\n-->\r\n</style>\r\n</head>\r\n<body dir=\"ltr\">\r\n<div id=\"divtagdefaultwrapper\" dir=\"ltr\" style=\"font-size:12pt; color:#000000; font-family:Calibri,Helvetica,sans-serif\">\r\n<p style=\"margin-top:0; margin-bottom:0\">Let's debrief after community meetup.<br>\r\n</p>\r\n</div>\r\n</body>\r\n</html>\r\n"
    },
    "sender":{
        "emailAddress":{
            "name":"Administrator",
            "address":"admin@contoso.onmicrosoft.com"
        }
    },
    "from":{
        "emailAddress":{
            "name":"Administrator",
            "address":"admin@contoso.onmicrosoft.com"
        }
    },
    "toRecipients":[
        {
            "emailAddress":{
                "name":"Alex Wilber",
                "address":"AlexW@contoso.onmicrosoft.com"
            }
        }
    ],
    "ccRecipients":[

    ],
    "bccRecipients":[

    ],
    "replyTo":[

    ],
    "mentionsPreview":null,
    "flag":{
        "flagStatus":"notFlagged"
    },
    "startDateTime":{
        "dateTime":"2018-02-19T19:00:00.0000000",
        "timeZone":"UTC"
    },
    "endDateTime":{
        "dateTime":"2018-02-19T19:30:00.0000000",
        "timeZone":"UTC"
    },
    "location":{
        "displayName":"Mt. Hood",
        "locationType":"default",
        "uniqueIdType":"unknown"
    },
    "recurrence":null,
    "previousLocation":null,
    "previousStartDateTime":null,
    "previousEndDateTime":null
}
```


##### <a name="request-2"></a><span data-ttu-id="56246-149">要求 2</span><span class="sxs-lookup"><span data-stu-id="56246-149">Request 2</span></span>
<span data-ttu-id="56246-150">2 番目の例では、イベント メッセージに関連付けられているイベントを取得する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="56246-150">The second example shows how to get the event associated with an event message.</span></span> <span data-ttu-id="56246-151">イベント メッセージ ID を使用してイベントのメッセージを取得し、イベント メッセージ上に明示的にキャストを提供してその **event** ナビゲーション プロパティにアクセスし、$expand パラメーターを適用してそのイベントのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="56246-151">It uses the event message ID to get the event message, explicitly provides a cast on the event message to access its **event** navigation property, and apply an $expand parameter to get the properties of the event.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_event_based_on_eventmessage"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages('AAMkADYAAAImV_jAAA=')?$expand=microsoft.graph.eventMessage/event
```
##### <a name="response-2"></a><span data-ttu-id="56246-152">応答 2</span><span class="sxs-lookup"><span data-stu-id="56246-152">Response 2</span></span>
<span data-ttu-id="56246-153">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="56246-153">Here is an example of the response.</span></span> <span data-ttu-id="56246-154">関連付けられているイベントのプロパティは、応答で返されます。</span><span class="sxs-lookup"><span data-stu-id="56246-154">The properties of the associated event are returned in the response.</span></span>
<span data-ttu-id="56246-155">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="56246-155">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="56246-156">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="56246-156">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_event_based_on_eventmessage",
  "truncated": true,
  "@odata.type": "microsoft.graph.eventMessageRequest"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('8fd6e83b-3cc0-4bf0-8b26-950f4d7110f6')/messages/$entity",
    "@odata.type":"#microsoft.graph.eventMessageRequest",
    "@odata.etag":"W/\"CwAAABYAAABXlB/SL0N4Q6g6o+jSYAEuAAAImkVF\"",
    "id":"AAMkADYAAAImV_jAAA=",
    "createdDateTime":"2017-12-27T21:54:55Z",
    "lastModifiedDateTime":"2017-12-27T23:26:38Z",
    "changeKey":"CwAAABYAAABXlB/SL0N4Q6g6o+jSYAEuAAAImkVF",
    "categories":[

    ],
    "receivedDateTime":"2017-12-27T21:54:55Z",
    "sentDateTime":"2017-12-27T21:54:54Z",
    "hasAttachments":false,
    "internetMessageId":"<MWHPR1301MB211042CFBF@MWHPR1301MB2110.namprd13.prod.outlook.com>",
    "subject":"Kick off planning",
    "bodyPreview":"Let's collect opinions from our teams and organize action items.",
    "importance":"normal",
    "parentFolderId":"AQMkADYAS4AAAIBDAAAAA==",
    "conversationId":"AAQkADYRuffB3wDlPn-ReFZarI60=",
    "conversationIndex":"AdN/XVP4JG598HfAOU+f9F4VlqsjrQ==",
    "isDeliveryReceiptRequested":null,
    "isReadReceiptRequested":false,
    "isRead":false,
    "isDraft":false,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADYAAAImV%2BjAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification":"focused",
    "unsubscribeData":[

    ],
    "unsubscribeEnabled":false,
    "meetingMessageType":"meetingRequest",
    "type":"singleInstance",
    "isOutOfDate":false,
    "isAllDay":false,
    "isDelegated":false,
    "responseRequested":true,
    "body":{
        "contentType":"html",
        "content":"<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n<style type=\"text/css\" style=\"display:none\">\r\n<!--\r\np\r\n\t{margin-top:0;\r\n\tmargin-bottom:0}\r\n-->\r\n</style>\r\n</head>\r\n<body dir=\"ltr\">\r\n<div id=\"divtagdefaultwrapper\" dir=\"ltr\" style=\"font-size:12pt; color:#000000; font-family:Calibri,Helvetica,sans-serif\">\r\n<p style=\"margin-top:0; margin-bottom:0\">Let's collect opinions from our teams and organize action items.<br>\r\n</p>\r\n</div>\r\n</body>\r\n</html>\r\n"
    },
    "sender":{
        "emailAddress":{
            "name":"Administrator",
            "address":"admin@contoso.onmicrosoft.com"
        }
    },
    "from":{
        "emailAddress":{
            "name":"Administrator",
            "address":"admin@contoso.onmicrosoft.com"
        }
    },
    "toRecipients":[
        {
            "emailAddress":{
                "name":"Alex Wilber",
                "address":"AlexW@contoso.onmicrosoft.com"
            }
        }
    ],
    "ccRecipients":[

    ],
    "bccRecipients":[

    ],
    "replyTo":[

    ],
    "mentionsPreview":null,
    "flag":{
        "flagStatus":"notFlagged"
    },
    "startDateTime":{
        "dateTime":"2018-02-02T22:00:00.0000000",
        "timeZone":"UTC"
    },
    "endDateTime":{
        "dateTime":"2018-02-02T23:00:00.0000000",
        "timeZone":"UTC"
    },
    "location":{
        "displayName":"Mt. Hood",
        "locationType":"default",
        "uniqueIdType":"unknown"
    },
    "recurrence":null,
    "previousLocation":null,
    "previousStartDateTime":null,
    "previousEndDateTime":null,
    "event@odata.context":"https://graph.microsoft.com/beta/$metadata#users('8fd6e83b-3cc0-4bf0-8b26-950f4d7110f6')/messages('AAMkADYAAAImV_jAAA%3D')/microsoft.graph.eventMessage/event/$entity",
    "event":{
        "@odata.etag":"W/\"V5Qf0i9DeEOoOqPo0mABLgAACJpBWg==\"",
        "id":"AAMkADYAAAImVu6AAA=",
        "createdDateTime":"2017-12-27T21:54:55.2624551Z",
        "lastModifiedDateTime":"2017-12-27T22:19:16.6667889Z",
        "changeKey":"V5Qf0i9DeEOoOqPo0mABLgAACJpBWg==",
        "categories":[

        ],
        "originalStartTimeZone":"Pacific Standard Time",
        "originalEndTimeZone":"Pacific Standard Time",
        "uid":"040000008200E00074C5B7101A82E00800000000A2A6F3535D7FD3010000000000000000100000003D770E2E8974F44B9471BDB348097FE3",
        "reminderMinutesBeforeStart":15,
        "isReminderOn":true,
        "hasAttachments":false,
        "subject":"Kick off planning",
        "bodyPreview":"Let's collect opinions from our teams and organize action items.",
        "importance":"normal",
        "sensitivity":"normal",
        "isAllDay":false,
        "isCancelled":false,
        "isOrganizer":false,
        "responseRequested":true,
        "seriesMasterId":null,
        "showAs":"tentative",
        "type":"singleInstance",
        "webLink":"https://outlook.office365.com/owa/?itemid=AAMkADYAAAImVu6AAA%3D&exvsurl=1&path=/calendar/item",
        "onlineMeetingUrl":null,
        "responseStatus":{
            "response":"tentativelyAccepted",
            "time":"2017-12-27T22:19:12.6197462Z"
        },
        "body":{
            "contentType":"html",
            "content":"<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n<style type=\"text/css\" style=\"display:none\">\r\n<!--\r\np\r\n\t{margin-top:0;\r\n\tmargin-bottom:0}\r\n-->\r\n</style>\r\n</head>\r\n<body dir=\"ltr\">\r\n<div id=\"divtagdefaultwrapper\" dir=\"ltr\" style=\"font-size:12pt; color:#000000; font-family:Calibri,Helvetica,sans-serif\">\r\n<p style=\"margin-top:0; margin-bottom:0\">Let's collect opinions from our teams and organize action items.<br>\r\n</p>\r\n</div>\r\n</body>\r\n</html>\r\n"
        },
        "start":{
            "dateTime":"2018-02-02T22:00:00.0000000",
            "timeZone":"UTC"
        },
        "end":{
            "dateTime":"2018-02-02T23:00:00.0000000",
            "timeZone":"UTC"
        },
        "location":{
            "displayName":"Mt. Hood",
            "locationType":"default",
            "uniqueId":"Mt. Hood",
            "uniqueIdType":"private"
        },
        "locations":[
            {
                "displayName":"Mt. Hood",
                "locationType":"default",
                "uniqueId":"Mt. Hood",
                "uniqueIdType":"private"
            }
        ],
        "recurrence":null,
        "attendees":[
            {
                "type":"required",
                "status":{
                    "response":"none",
                    "time":"0001-01-01T00:00:00Z"
                },
                "emailAddress":{
                    "name":"Administrator",
                    "address":"admin@contoso.onmicrosoft.com"
                }
            },
            {
                "type":"required",
                "status":{
                    "response":"tentativelyAccepted",
                    "time":"0001-01-01T00:00:00Z"
                },
                "emailAddress":{
                    "name":"Alex Wilber",
                    "address":"AlexW@contoso.onmicrosoft.com"
                }
            }
        ],
        "organizer":{
            "emailAddress":{
                "name":"Administrator",
                "address":"admin@contoso.onmicrosoft.com"
            }
        },
        "OnlineMeeting":null
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get eventMessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
