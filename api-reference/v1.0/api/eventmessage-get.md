---
title: eventMessage の取得
description: '**イベント**ナビゲーションプロパティの [パラメーター] を展開して、出席者の予定表にある関連イベントを取得します。'
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 48460738e5330af0ca79d6e702667db31430b39d
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35277442"
---
# <a name="get-eventmessage"></a><span data-ttu-id="f1462-103">eventMessage の取得</span><span class="sxs-lookup"><span data-stu-id="f1462-103">Get eventMessage</span></span>

<span data-ttu-id="f1462-104">[eventMessage](../resources/eventmessage.md) オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="f1462-104">Get the properties and relationships of the [eventMessage](../resources/eventmessage.md) object.</span></span> <span data-ttu-id="f1462-105">$expand パラメーターを **event** ナビゲーション プロパティに適用して、出席者の予定表で関連付けられている[イベント](../resources/event.md)を取得します。</span><span class="sxs-lookup"><span data-stu-id="f1462-105">Apply the $expand parameter on the **event** navigation property to get the associated [event](../resources/event.md) in an attendee's calendar.</span></span>

<span data-ttu-id="f1462-106">現在、この操作によって返されるイベント メッセージの本文は HTML 形式のみです。</span><span class="sxs-lookup"><span data-stu-id="f1462-106">Currently, this operation returns event message bodies in only HTML format.</span></span>

## <a name="permissions"></a><span data-ttu-id="f1462-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f1462-107">Permissions</span></span>
<span data-ttu-id="f1462-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f1462-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1462-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f1462-110">Permission type</span></span>      | <span data-ttu-id="f1462-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f1462-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1462-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f1462-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f1462-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="f1462-113">Mail.Read</span></span>    |
|<span data-ttu-id="f1462-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f1462-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1462-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="f1462-115">Mail.Read</span></span>    |
|<span data-ttu-id="f1462-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f1462-116">Application</span></span> | <span data-ttu-id="f1462-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="f1462-117">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1462-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f1462-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}

GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f1462-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f1462-119">Optional query parameters</span></span>
<span data-ttu-id="f1462-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="f1462-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f1462-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f1462-121">Request headers</span></span>
| <span data-ttu-id="f1462-122">名前</span><span class="sxs-lookup"><span data-stu-id="f1462-122">Name</span></span>       | <span data-ttu-id="f1462-123">型</span><span class="sxs-lookup"><span data-stu-id="f1462-123">Type</span></span> | <span data-ttu-id="f1462-124">説明</span><span class="sxs-lookup"><span data-stu-id="f1462-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f1462-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1462-125">Authorization</span></span>  | <span data-ttu-id="f1462-126">string</span><span class="sxs-lookup"><span data-stu-id="f1462-126">string</span></span>  | <span data-ttu-id="f1462-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f1462-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f1462-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="f1462-129">Request body</span></span>
<span data-ttu-id="f1462-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f1462-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1462-131">応答</span><span class="sxs-lookup"><span data-stu-id="f1462-131">Response</span></span>

<span data-ttu-id="f1462-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [eventMessage](../resources/eventmessage.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f1462-132">If successful, this method returns a `200 OK` response code and [eventMessage](../resources/eventmessage.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f1462-133">例</span><span class="sxs-lookup"><span data-stu-id="f1462-133">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="f1462-134">要求 1</span><span class="sxs-lookup"><span data-stu-id="f1462-134">Request 1</span></span>
<span data-ttu-id="f1462-135">最初の例では、イベント メッセージ ID に基づいてイベント メッセージのプロパティを取得する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="f1462-135">The first example shows how to get the properties of an event message based on the event message ID.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADYAAAImV_lAAA="],
  "name": "get_eventmessage"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADYAAAImV_lAAA=
```
##### <a name="response-1"></a><span data-ttu-id="f1462-136">応答 1</span><span class="sxs-lookup"><span data-stu-id="f1462-136">Response 1</span></span>
<span data-ttu-id="f1462-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f1462-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_eventmessage",
  "truncated": true,
  "@odata.type": "microsoft.graph.eventMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('8fd6e83b-3cc0-4bf0-8b26-950f4d7110f6')/messages/$entity",
    "@odata.type":"#microsoft.graph.eventMessage",
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
    "isDeliveryReceiptRequested":null,
    "isReadReceiptRequested":false,
    "isRead":false,
    "isDraft":false,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADYAAAImV%2BlAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification":"focused",
    "meetingMessageType":"meetingRequest",
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

    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f1462-140">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="f1462-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f1462-141">C#</span><span class="sxs-lookup"><span data-stu-id="f1462-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_eventmessage-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f1462-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="f1462-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_eventmessage-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f1462-143">目的-C</span><span class="sxs-lookup"><span data-stu-id="f1462-143">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_eventmessage-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request-2"></a><span data-ttu-id="f1462-144">要求 2</span><span class="sxs-lookup"><span data-stu-id="f1462-144">Request 2</span></span>
<span data-ttu-id="f1462-145">2 番目の例では、イベント メッセージに関連付けられているイベントを取得する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="f1462-145">The second example shows how to get the event associated with an event message.</span></span> <span data-ttu-id="f1462-146">イベント メッセージ ID を使用してイベントのメッセージを取得し、イベント メッセージ上に明示的にキャストを提供してその **event** ナビゲーション プロパティにアクセスし、$expand パラメーターを適用してそのイベントのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="f1462-146">It uses the event message ID to get the event message, explicitly provides a cast on the event message to access its **event** navigation property, and apply an $expand parameter to get the properties of the event.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADYAAAImV_jAAA="],
  "name": "get_event_based_on_eventmessage"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADYAAAImV_jAAA=?$expand=microsoft.graph.eventMessage/event
```
##### <a name="response-2"></a><span data-ttu-id="f1462-147">応答 2</span><span class="sxs-lookup"><span data-stu-id="f1462-147">Response 2</span></span>
<span data-ttu-id="f1462-148">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="f1462-148">Here is an example of the response.</span></span> <span data-ttu-id="f1462-149">関連付けられているイベントのプロパティは、応答で返されます。</span><span class="sxs-lookup"><span data-stu-id="f1462-149">The properties of the associated event are returned in the response.</span></span> <span data-ttu-id="f1462-150">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="f1462-150">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f1462-151">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f1462-151">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_event_based_on_eventmessage",
  "truncated": true,
  "@odata.type": "microsoft.graph.eventMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
   "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('8fd6e83b-3cc0-4bf0-8b26-950f4d7110f6')/messages/$entity",
   "@odata.type":"#microsoft.graph.eventMessage",
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
   "internetMessageId":"<MWHPR1301MB211042CF@MWHPR1301MB2110.namprd13.prod.outlook.com>",
   "subject":"Kick off planning",
   "bodyPreview":"Let's collect opinions from our teams and organize action items.",
   "importance":"normal",
    "parentFolderId":"AQMkADYAS4AAAIBDAAAAA==",
    "conversationId":"AAQkADYRuffB3wDlPn-ReFZarI60=",
   "isDeliveryReceiptRequested":null,
   "isReadReceiptRequested":false,
   "isRead":false,
   "isDraft":false,
   "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADYAAAImV%2BjAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
   "inferenceClassification":"focused",
   "meetingMessageType":"meetingRequest",
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
   "event@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('8fd6e83b-3cc0-4bf0-8b26-950f4d7110f6')/messages('AAMkADYAAAImV_jAAA%3D')/microsoft.graph.eventMessage/event/$entity",
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
      "iCalUId":"040000008200E00074C5B7101A82E00800000000A2A6F3535D7FD3010000000000000000100000003D770E2E8974F44B9471BDB348097FE3",
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
         "displayName":"Mt. Hood"
      },
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
      }
   }
}
``` 
#### <a name="sdk-sample-code"></a><span data-ttu-id="f1462-152">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="f1462-152">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f1462-153">C#</span><span class="sxs-lookup"><span data-stu-id="f1462-153">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_event_based_on_eventmessage-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f1462-154">Javascript</span><span class="sxs-lookup"><span data-stu-id="f1462-154">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_event_based_on_eventmessage-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f1462-155">目的-C</span><span class="sxs-lookup"><span data-stu-id="f1462-155">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_event_based_on_eventmessage-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get eventMessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/eventmessage-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/eventmessage-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/eventmessage-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/eventmessage-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/eventmessage-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
