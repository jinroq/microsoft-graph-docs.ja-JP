---
title: イベントを一覧表示する
description: イベント オブジェクトのリストを取得します。
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: d15b5a7b4a781ab98357e0291a112a409eb99c1b
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33614216"
---
# <a name="list-events"></a><span data-ttu-id="1a1fa-103">イベントを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="1a1fa-103">List events</span></span>
<span data-ttu-id="1a1fa-104">[イベント](../resources/event.md) オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="1a1fa-104">Retrieve a list of [event](../resources/event.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="1a1fa-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1a1fa-105">Permissions</span></span>
<span data-ttu-id="1a1fa-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1a1fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a1fa-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1a1fa-108">Permission type</span></span>      | <span data-ttu-id="1a1fa-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1a1fa-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a1fa-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1a1fa-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1a1fa-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a1fa-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1a1fa-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1a1fa-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a1fa-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1a1fa-113">Not supported.</span></span>    |
|<span data-ttu-id="1a1fa-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1a1fa-114">Application</span></span> | <span data-ttu-id="1a1fa-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1a1fa-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a1fa-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1a1fa-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events
GET /groups/{id}/calendar/events
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1a1fa-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="1a1fa-117">Optional query parameters</span></span>
<span data-ttu-id="1a1fa-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="1a1fa-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1a1fa-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1a1fa-119">Request headers</span></span>
| <span data-ttu-id="1a1fa-120">名前</span><span class="sxs-lookup"><span data-stu-id="1a1fa-120">Name</span></span>       | <span data-ttu-id="1a1fa-121">型</span><span class="sxs-lookup"><span data-stu-id="1a1fa-121">Type</span></span> | <span data-ttu-id="1a1fa-122">説明</span><span class="sxs-lookup"><span data-stu-id="1a1fa-122">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="1a1fa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a1fa-123">Authorization</span></span>  | <span data-ttu-id="1a1fa-124">string</span><span class="sxs-lookup"><span data-stu-id="1a1fa-124">string</span></span> | <span data-ttu-id="1a1fa-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1a1fa-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1a1fa-127">優先: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="1a1fa-127">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="1a1fa-128">string</span><span class="sxs-lookup"><span data-stu-id="1a1fa-128">string</span></span> | <span data-ttu-id="1a1fa-129">これを使用して、応答内の開始および終了時刻のタイム ゾーンを指定します。</span><span class="sxs-lookup"><span data-stu-id="1a1fa-129">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="1a1fa-130">指定しない場合、これらの時刻値は UTC で返されます。</span><span class="sxs-lookup"><span data-stu-id="1a1fa-130">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="1a1fa-131">省略可能。</span><span class="sxs-lookup"><span data-stu-id="1a1fa-131">Optional.</span></span> |
| <span data-ttu-id="1a1fa-132">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="1a1fa-132">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="1a1fa-133">string</span><span class="sxs-lookup"><span data-stu-id="1a1fa-133">string</span></span> | <span data-ttu-id="1a1fa-134">**body** プロパティが返されるときの形式です。</span><span class="sxs-lookup"><span data-stu-id="1a1fa-134">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="1a1fa-135">値は、"text" または "html" になります。</span><span class="sxs-lookup"><span data-stu-id="1a1fa-135">Values can be "text" or "html".</span></span> <span data-ttu-id="1a1fa-136">この `Prefer` ヘッダーが指定されている場合、`Preference-Applied` ヘッダーが確認として返されます。</span><span class="sxs-lookup"><span data-stu-id="1a1fa-136">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="1a1fa-137">このヘッダーが指定されていない場合は、**body** プロパティが HTML 形式で返されます。</span><span class="sxs-lookup"><span data-stu-id="1a1fa-137">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="1a1fa-138">省略可能。</span><span class="sxs-lookup"><span data-stu-id="1a1fa-138">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1a1fa-139">要求本文</span><span class="sxs-lookup"><span data-stu-id="1a1fa-139">Request body</span></span>
<span data-ttu-id="1a1fa-140">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1a1fa-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a1fa-141">応答</span><span class="sxs-lookup"><span data-stu-id="1a1fa-141">Response</span></span>
<span data-ttu-id="1a1fa-142">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Event](../resources/event.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="1a1fa-142">If successful, this method returns a `200 OK` response code and a collection of [event](../resources/event.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a1fa-143">例</span><span class="sxs-lookup"><span data-stu-id="1a1fa-143">Example</span></span>
#### <a name="request"></a><span data-ttu-id="1a1fa-144">要求</span><span class="sxs-lookup"><span data-stu-id="1a1fa-144">Request</span></span>
<span data-ttu-id="1a1fa-145">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1a1fa-145">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315"],
  "name": "get_group_events"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/events
```

#### <a name="response"></a><span data-ttu-id="1a1fa-146">応答</span><span class="sxs-lookup"><span data-stu-id="1a1fa-146">Response</span></span>
<span data-ttu-id="1a1fa-147">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1a1fa-147">The following is an example of the response.</span></span>
><span data-ttu-id="1a1fa-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="1a1fa-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 354

{
  "value": [
    {
      "id": "AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOwAAAA==",
      "createdDateTime": "2017-07-31T18:59:01.982289Z",
      "lastModifiedDateTime": "2017-09-06T04:29:38.6647687Z",
      "changeKey": "xPZF2y46pEiVBni87OnrpgAAFq78Xw==",
      "categories": [],
      "originalStartTimeZone": "Eastern Standard Time",
      "originalEndTimeZone": "Eastern Standard Time",
      "iCalUId": "040000008200E00074C5B7101A82E00800000000824DDB122F0AD301000000000000000010000000824A8905B038D54AA7735F117B3442ED",
      "reminderMinutesBeforeStart": 15,
      "isReminderOn": true,
      "hasAttachments": false,
      "subject": "New Training Plans",
      "bodyPreview": "Meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>",
      "importance": "normal",
      "sensitivity": "normal",
      "isAllDay": false,
      "isCancelled": false,
      "isOrganizer": true,
      "responseRequested": true,
      "seriesMasterId": null,
      "showAs": "busy",
      "type": "seriesMaster",
      "webLink": "https://outlook.office365.com/owa/?itemid=AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA%2Bb2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOwAAAA%3D%3D&exvsurl=1&path=/calendar/item",
      "onlineMeetingUrl": null,
      "responseStatus": {
          "response": "organizer",
          "time": "0001-01-01T00:00:00Z"
      },
      "body": {
          "contentType": "html",
          "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n</head>\r\n<body>\r\n<div>Meeting to plan new trainings.</div>\r\n<div><br>\r\n<br>\r\n<br>\r\n<a href=\"https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35\">Join Microsoft Teams Online Meeting</a></div>\r\n</body>\r\n</html>\r\n"
      },
      "start": {
          "dateTime": "2017-08-14T21:00:00.0000000",
          "timeZone": "UTC"
      },
      "end": {
          "dateTime": "2017-08-14T22:00:00.0000000",
          "timeZone": "UTC"
      },
      "location": {
          "displayName": "HR Taskforce / Facilities"
      },
      "recurrence": {
          "pattern": {
              "type": "weekly",
              "interval": 1,
              "month": 0,
              "dayOfMonth": 0,
              "daysOfWeek": [
                  "monday",
                  "wednesday",
                  "friday"
              ],
              "firstDayOfWeek": "sunday",
              "index": "first"
          },
          "range": {
              "type": "noEnd",
              "startDate": "2017-08-14",
              "endDate": "0001-01-01",
              "recurrenceTimeZone": "Eastern Standard Time",
              "numberOfOccurrences": 0
          }
      },
      "attendees": [
          {
              "type": "required",
              "status": {
                  "response": "accepted",
                  "time": "2017-07-31T18:59:06.4180028Z"
              },
              "emailAddress": {
                  "name": "Joni Sherman",
                  "address": "JoniS@contoso.onmicrosoft.com"
              }
          },
          {
              "type": "required",
              "status": {
                  "response": "none",
                  "time": "0001-01-01T00:00:00Z"
              },
              "emailAddress": {
                  "name": "HR Taskforce",
                  "address": "HRTaskforce@contoso.onmicrosoft.com"
              }
          },
          {
              "type": "required",
              "status": {
                  "response": "none",
                  "time": "0001-01-01T00:00:00Z"
              },
              "emailAddress": {
                  "name": "Megan Bowen",
                  "address": "MeganB@contoso.onmicrosoft.com"
              }
          },
          {
              "type": "required",
              "status": {
                  "response": "none",
                  "time": "0001-01-01T00:00:00Z"
              },
              "emailAddress": {
                  "name": "Lidia Holloway",
                  "address": "LidiaH@contoso.onmicrosoft.com"
              }
          },
          {
              "type": "required",
              "status": {
                  "response": "none",
                  "time": "0001-01-01T00:00:00Z"
              },
              "emailAddress": {
                  "name": "Emily Braun",
                  "address": "EmilyB@contoso.onmicrosoft.com"
              }
          }
      ],
      "organizer": {
          "emailAddress": {
              "name": "HR Taskforce",
              "address": "HRTaskforce@contoso.onmicrosoft.com"
          }
      }
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="1a1fa-150">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="1a1fa-150">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1a1fa-151">C#</span><span class="sxs-lookup"><span data-stu-id="1a1fa-151">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_group_events-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1a1fa-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="1a1fa-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_group_events-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List events",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-list-events.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-list-events.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
