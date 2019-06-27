---
title: 'user: reminderView'
description: '指定した開始時刻と終了時刻内の予定表のアラームの一覧を返します。 '
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 00f2f2b9ab96e8776e3e082c1ad296ddfc4be9b3
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35278681"
---
# <a name="user-reminderview"></a><span data-ttu-id="87107-103">user: reminderView</span><span class="sxs-lookup"><span data-stu-id="87107-103">user: reminderView</span></span>
<span data-ttu-id="87107-104">指定した開始時刻と終了時刻内の、ユーザーの予定表にあるイベントリマインダーの一覧を返します。</span><span class="sxs-lookup"><span data-stu-id="87107-104">Return a list of event reminders in a user calendar within the specified start and end times.</span></span> 

## <a name="permissions"></a><span data-ttu-id="87107-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="87107-105">Permissions</span></span>
<span data-ttu-id="87107-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="87107-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87107-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="87107-108">Permission type</span></span>      | <span data-ttu-id="87107-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="87107-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87107-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="87107-110">Delegated (work or school account)</span></span> | <span data-ttu-id="87107-111">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="87107-111">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="87107-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="87107-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87107-113">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="87107-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="87107-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="87107-114">Application</span></span> | <span data-ttu-id="87107-115">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="87107-115">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="87107-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="87107-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/reminderView(startDateTime=startDateTime-value,endDateTime=endDateTime-value)
```

## <a name="function-parameters"></a><span data-ttu-id="87107-117">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="87107-117">Function parameters</span></span>
<span data-ttu-id="87107-118">要求 URL に、次の関数パラメーターを値で指定します。</span><span class="sxs-lookup"><span data-stu-id="87107-118">In the request URL, provide the following function parameters with values.</span></span>

| <span data-ttu-id="87107-119">パラメーター</span><span class="sxs-lookup"><span data-stu-id="87107-119">Parameter</span></span>    | <span data-ttu-id="87107-120">型</span><span class="sxs-lookup"><span data-stu-id="87107-120">Type</span></span>   |<span data-ttu-id="87107-121">説明</span><span class="sxs-lookup"><span data-stu-id="87107-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="87107-122">startDateTime</span><span class="sxs-lookup"><span data-stu-id="87107-122">startDateTime</span></span>|<span data-ttu-id="87107-123">String</span><span class="sxs-lookup"><span data-stu-id="87107-123">String</span></span>|<span data-ttu-id="87107-p102">アラームを設定するイベントの開始日時です。値は ISO 8601 形式で表されます。例: "2015-11-08T19:00:00.0000000"。</span><span class="sxs-lookup"><span data-stu-id="87107-p102">The start date and time of the event for which the reminder is set up. The value is represented in ISO 8601 format, for example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="87107-126">endDateTime</span><span class="sxs-lookup"><span data-stu-id="87107-126">endDateTime</span></span>|<span data-ttu-id="87107-127">String</span><span class="sxs-lookup"><span data-stu-id="87107-127">String</span></span>|<span data-ttu-id="87107-p103">アラームを設定するイベントの終了日時です。値は ISO 8601 形式で表されます。例: "2015-11-08T20:00:00.0000000"。</span><span class="sxs-lookup"><span data-stu-id="87107-p103">The end date and time of the event for which the reminder is set up. The value is represented in ISO 8601 format, for example, "2015-11-08T20:00:00.0000000".</span></span>|

## <a name="request-headers"></a><span data-ttu-id="87107-130">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="87107-130">Request headers</span></span>
| <span data-ttu-id="87107-131">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="87107-131">Header</span></span>       | <span data-ttu-id="87107-132">値</span><span class="sxs-lookup"><span data-stu-id="87107-132">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="87107-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="87107-133">Authorization</span></span>  | <span data-ttu-id="87107-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="87107-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="87107-136">Content-Type</span><span class="sxs-lookup"><span data-stu-id="87107-136">Content-Type</span></span>   | <span data-ttu-id="87107-137">application/json</span><span class="sxs-lookup"><span data-stu-id="87107-137">application/json</span></span> |
| <span data-ttu-id="87107-138">Prefer</span><span class="sxs-lookup"><span data-stu-id="87107-138">Prefer</span></span> | <span data-ttu-id="87107-p105">{Time-zone}。省略可能。指定しない場合、UTC が使用されます。</span><span class="sxs-lookup"><span data-stu-id="87107-p105">{Time-zone}. Optional, UTC assumed if absent.</span></span>|

## <a name="request-body"></a><span data-ttu-id="87107-141">要求本文</span><span class="sxs-lookup"><span data-stu-id="87107-141">Request body</span></span>
<span data-ttu-id="87107-142">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="87107-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87107-143">応答</span><span class="sxs-lookup"><span data-stu-id="87107-143">Response</span></span>

<span data-ttu-id="87107-144">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[アラーム](../resources/reminder.md) コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="87107-144">If successful, this method returns `200 OK` response code and [reminder](../resources/reminder.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87107-145">例</span><span class="sxs-lookup"><span data-stu-id="87107-145">Example</span></span>
<span data-ttu-id="87107-146">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="87107-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="87107-147">要求</span><span class="sxs-lookup"><span data-stu-id="87107-147">Request</span></span>
<span data-ttu-id="87107-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="87107-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_reminderview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/reminderView(startDateTime='2017-06-05T10:00:00.0000000',endDateTime='2017-06-11T11:00:00.0000000')
```

##### <a name="response"></a><span data-ttu-id="87107-149">応答</span><span class="sxs-lookup"><span data-stu-id="87107-149">Response</span></span>
<span data-ttu-id="87107-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="87107-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.reminder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 673

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.reminder)",
    "value": [
        {
            "eventId": "AAMkADNsvAAA=",
            "changeKey": "SuFHwDRP1EeXJUopWbSLlgAAmBvk2g==",
            "eventSubject": "Plan summer company picnic",
            "eventWebLink": "https://outlook.office365.com/owa/?itemid=AAMkADNsvAAA%3D&exvsurl=1&path=/calendar/item",
            "eventStartTime": {
                "dateTime": "2017-06-09T18:00:00.0000000",
                "timeZone": "UTC"
            },
            "eventEndTime": {
                "dateTime": "2017-06-09T19:00:00.0000000",
                "timeZone": "UTC"
            },
            "eventLocation": {
                "displayName": "Conf Room 3"
            },
            "reminderFireTime": {
                "dateTime": "2017-06-09T17:45:00.0000000",
                "timeZone": "UTC"
            }
        }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="87107-153">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="87107-153">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="87107-154">C#</span><span class="sxs-lookup"><span data-stu-id="87107-154">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_reminderview-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="87107-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="87107-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_reminderview-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="87107-156">目的-C</span><span class="sxs-lookup"><span data-stu-id="87107-156">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/user_reminderview-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: reminderView",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/user-reminderview.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/user-reminderview.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/user-reminderview.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
