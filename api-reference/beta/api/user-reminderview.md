---
title: 'user: reminderView'
description: '指定した開始時刻と終了時刻内の予定表のアラームの一覧を返します。 '
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3fb0283aaae4f814f06b59a8a6ad6183cc18fec1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918211"
---
# <a name="user-reminderview"></a><span data-ttu-id="9b112-103">user: reminderView</span><span class="sxs-lookup"><span data-stu-id="9b112-103">user: reminderView</span></span>

> <span data-ttu-id="9b112-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9b112-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9b112-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9b112-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9b112-106">内の指定した開始時刻と終了時刻、ユーザーの予定表のイベント通知の一覧を返します。</span><span class="sxs-lookup"><span data-stu-id="9b112-106">Return a list of event reminders in a user calendar within the specified start and end times.</span></span> 

## <a name="permissions"></a><span data-ttu-id="9b112-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9b112-107">Permissions</span></span>
<span data-ttu-id="9b112-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9b112-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b112-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9b112-110">Permission type</span></span>      | <span data-ttu-id="9b112-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9b112-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9b112-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9b112-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9b112-113">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9b112-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="9b112-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9b112-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b112-115">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9b112-115">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="9b112-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9b112-116">Application</span></span> | <span data-ttu-id="9b112-117">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9b112-117">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9b112-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9b112-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/reminderView(startDateTime=startDateTime-value,endDateTime=endDateTime-value)
```

## <a name="function-parameters"></a><span data-ttu-id="9b112-119">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="9b112-119">Function parameters</span></span>
<span data-ttu-id="9b112-120">要求 URL に、次の関数パラメーターを値で指定します。</span><span class="sxs-lookup"><span data-stu-id="9b112-120">In the request URL, provide the following function parameters with values.</span></span>

| <span data-ttu-id="9b112-121">パラメーター</span><span class="sxs-lookup"><span data-stu-id="9b112-121">Parameter</span></span>    | <span data-ttu-id="9b112-122">型</span><span class="sxs-lookup"><span data-stu-id="9b112-122">Type</span></span>   |<span data-ttu-id="9b112-123">説明</span><span class="sxs-lookup"><span data-stu-id="9b112-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9b112-124">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9b112-124">startDateTime</span></span>|<span data-ttu-id="9b112-125">String</span><span class="sxs-lookup"><span data-stu-id="9b112-125">String</span></span>|<span data-ttu-id="9b112-p103">アラームを設定するイベントの開始日時です。値は ISO 8601 形式で表されます。例: "2015-11-08T19:00:00.0000000"。</span><span class="sxs-lookup"><span data-stu-id="9b112-p103">The start date and time of the event for which the reminder is set up. The value is represented in ISO 8601 format, for example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="9b112-128">endDateTime</span><span class="sxs-lookup"><span data-stu-id="9b112-128">endDateTime</span></span>|<span data-ttu-id="9b112-129">String</span><span class="sxs-lookup"><span data-stu-id="9b112-129">String</span></span>|<span data-ttu-id="9b112-p104">アラームを設定するイベントの終了日時です。値は ISO 8601 形式で表されます。例: "2015-11-08T20:00:00.0000000"。</span><span class="sxs-lookup"><span data-stu-id="9b112-p104">The end date and time of the event for which the reminder is set up. The value is represented in ISO 8601 format, for example, "2015-11-08T20:00:00.0000000".</span></span>|

## <a name="request-headers"></a><span data-ttu-id="9b112-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9b112-132">Request headers</span></span>
| <span data-ttu-id="9b112-133">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9b112-133">Header</span></span>       | <span data-ttu-id="9b112-134">値</span><span class="sxs-lookup"><span data-stu-id="9b112-134">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="9b112-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b112-135">Authorization</span></span>  | <span data-ttu-id="9b112-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9b112-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9b112-138">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9b112-138">Content-Type</span></span>   | <span data-ttu-id="9b112-139">application/json</span><span class="sxs-lookup"><span data-stu-id="9b112-139">application/json</span></span> |
| <span data-ttu-id="9b112-140">Prefer</span><span class="sxs-lookup"><span data-stu-id="9b112-140">Prefer</span></span> | <span data-ttu-id="9b112-p106">{Time-zone}。省略可能。指定しない場合、UTC が使用されます。</span><span class="sxs-lookup"><span data-stu-id="9b112-p106">{Time-zone}. Optional, UTC assumed if absent.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b112-143">要求本文</span><span class="sxs-lookup"><span data-stu-id="9b112-143">Request body</span></span>
<span data-ttu-id="9b112-144">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="9b112-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9b112-145">応答</span><span class="sxs-lookup"><span data-stu-id="9b112-145">Response</span></span>

<span data-ttu-id="9b112-146">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[アラーム](../resources/reminder.md) コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9b112-146">If successful, this method returns `200 OK` response code and [reminder](../resources/reminder.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b112-147">例</span><span class="sxs-lookup"><span data-stu-id="9b112-147">Example</span></span>
<span data-ttu-id="9b112-148">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="9b112-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9b112-149">要求</span><span class="sxs-lookup"><span data-stu-id="9b112-149">Request</span></span>
<span data-ttu-id="9b112-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9b112-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_reminderview"
}-->
```http
GET https://graph.microsoft.com/beta/me/reminderView(startDateTime='2017-06-05T10:00:00.0000000',endDateTime='2017-06-11T11:00:00.0000000')
```

##### <a name="response"></a><span data-ttu-id="9b112-151">応答</span><span class="sxs-lookup"><span data-stu-id="9b112-151">Response</span></span>
<span data-ttu-id="9b112-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9b112-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.reminder)",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: reminderView",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
