---
title: ユーザーのメールボックスの設定を更新する
description: ユーザーのメールボックスの設定を 1 つ以上更新します。これには、自動応答 (電子メールの受信時に自動的にユーザーに通知)、ロケール (言語と国/地域)、タイム ゾーン、就業時間の設定が含まれます。
ms.openlocfilehash: fb4e3f49c014b9bebee3076db49594eb1aee0fa8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070982"
---
# <a name="update-user-mailbox-settings"></a><span data-ttu-id="163b1-104">ユーザーのメールボックスの設定を更新する</span><span class="sxs-lookup"><span data-stu-id="163b1-104">Update user mailbox settings</span></span>

> <span data-ttu-id="163b1-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="163b1-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="163b1-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="163b1-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="163b1-p103">ユーザーのメールボックスの設定を 1 つ以上更新します。これには、[自動応答](../resources/automaticrepliessetting.md) (電子メールの受信時に自動的にユーザーに通知)、[ロケール](../resources/localeinfo.md) (言語と国/地域)、タイム ゾーン、[就業時間](../resources/workinghours.md)の設定が含まれます。</span><span class="sxs-lookup"><span data-stu-id="163b1-p103">Update one or more settings for the user's mailbox. This includes settings for [automatic replies](../resources/automaticrepliessetting.md) (notify people automatically upon receipt of their email), [locale](../resources/localeinfo.md) (language and country/region), time zone, and [working hours](../resources/workinghours.md).</span></span>

<span data-ttu-id="163b1-109">これらの設定の 1 つ以上を、[mailboxSettings](../resources/mailboxsettings.md)の一部として有効化、構成、または無効化できます。</span><span class="sxs-lookup"><span data-stu-id="163b1-109">You can enable, configure, or disable one or more of these settings as part of [mailboxSettings](../resources/mailboxsettings.md).</span></span>

<span data-ttu-id="163b1-110">**注** メールボックス設定は作成または削除できません。</span><span class="sxs-lookup"><span data-stu-id="163b1-110">**Note** You cannot create or delete any mailbox settings.</span></span>

<span data-ttu-id="163b1-111">ユーザーの優先タイム ゾーンを更新する場合、Windows または [Internet Assigned Numbers Authority (IANA) のタイム ゾーン](https://www.iana.org/time-zones) (別称: Olson タイム ゾーン) 形式で指定することができます。</span><span class="sxs-lookup"><span data-stu-id="163b1-111">When you update the preferred time zone for a user, you can specify it in the Windows or  [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="163b1-112">タイム ゾーンは次の[例 2](#request-2)に示すようにもさらにカスタマイズできます。</span><span class="sxs-lookup"><span data-stu-id="163b1-112">You can also further customize the time zone as shown in [example 2](#request-2) below.</span></span>

## <a name="permissions"></a><span data-ttu-id="163b1-113">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="163b1-113">Permissions</span></span>
<span data-ttu-id="163b1-p105">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="163b1-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="163b1-116">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="163b1-116">Permission type</span></span>      | <span data-ttu-id="163b1-117">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="163b1-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="163b1-118">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="163b1-118">Delegated (work or school account)</span></span> | <span data-ttu-id="163b1-119">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="163b1-119">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="163b1-120">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="163b1-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="163b1-121">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="163b1-121">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="163b1-122">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="163b1-122">Application</span></span> | <span data-ttu-id="163b1-123">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="163b1-123">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="163b1-124">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="163b1-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailboxSettings
PATCH /users/{id|userPrincipalName}/mailboxSettings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="163b1-125">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="163b1-125">Optional query parameters</span></span>
<span data-ttu-id="163b1-126">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="163b1-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="163b1-127">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="163b1-127">Request headers</span></span>
| <span data-ttu-id="163b1-128">名前</span><span class="sxs-lookup"><span data-stu-id="163b1-128">Name</span></span>       | <span data-ttu-id="163b1-129">型</span><span class="sxs-lookup"><span data-stu-id="163b1-129">Type</span></span> | <span data-ttu-id="163b1-130">説明</span><span class="sxs-lookup"><span data-stu-id="163b1-130">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="163b1-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="163b1-131">Authorization</span></span>  | <span data-ttu-id="163b1-132">string</span><span class="sxs-lookup"><span data-stu-id="163b1-132">string</span></span>  | <span data-ttu-id="163b1-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="163b1-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="163b1-135">要求本文</span><span class="sxs-lookup"><span data-stu-id="163b1-135">Request body</span></span>
<span data-ttu-id="163b1-p107">要求本文で、更新する関連プロパティの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。書き込み可能または更新可能なプロパティを次に示します。</span><span class="sxs-lookup"><span data-stu-id="163b1-p107">In the request body, supply the values for the relevant properties that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. The following are the writable/updatable properties:</span></span>

| <span data-ttu-id="163b1-140">プロパティ</span><span class="sxs-lookup"><span data-stu-id="163b1-140">Property</span></span>     | <span data-ttu-id="163b1-141">型</span><span class="sxs-lookup"><span data-stu-id="163b1-141">Type</span></span>   |<span data-ttu-id="163b1-142">説明</span><span class="sxs-lookup"><span data-stu-id="163b1-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="163b1-143">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="163b1-143">automaticRepliesSetting</span></span>|[<span data-ttu-id="163b1-144">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="163b1-144">automaticRepliesSetting</span></span>](../resources/automaticrepliessetting.md)|<span data-ttu-id="163b1-145">サインイン ユーザーからのメッセージを使用して、着信メールの送信者に自動的に通知する構成設定。</span><span class="sxs-lookup"><span data-stu-id="163b1-145">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span> <span data-ttu-id="163b1-146">将来の日付の範囲だけにこのような通知を設定することができます。</span><span class="sxs-lookup"><span data-stu-id="163b1-146">You can set such notifications for only a future date range.</span></span>|
|<span data-ttu-id="163b1-147">language</span><span class="sxs-lookup"><span data-stu-id="163b1-147">language</span></span>|[<span data-ttu-id="163b1-148">localeInfo</span><span class="sxs-lookup"><span data-stu-id="163b1-148">localeInfo</span></span>](../resources/localeinfo.md)|<span data-ttu-id="163b1-149">優先言語および国/地域を含むユーザーのロケール情報。</span><span class="sxs-lookup"><span data-stu-id="163b1-149">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="163b1-150">timeZone</span><span class="sxs-lookup"><span data-stu-id="163b1-150">timeZone</span></span>|<span data-ttu-id="163b1-151">文字列</span><span class="sxs-lookup"><span data-stu-id="163b1-151">string</span></span>|<span data-ttu-id="163b1-152">ユーザーのメールボックスの既定のタイム ゾーン。</span><span class="sxs-lookup"><span data-stu-id="163b1-152">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="163b1-153">workingHours</span><span class="sxs-lookup"><span data-stu-id="163b1-153">workingHours</span></span>|[<span data-ttu-id="163b1-154">workingHours</span><span class="sxs-lookup"><span data-stu-id="163b1-154">workingHours</span></span>](../resources/workinghours.md)|<span data-ttu-id="163b1-155">ユーザーが働く時間、曜日、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="163b1-155">The hours, days of a week, and time zone that the user works.</span></span>|

## <a name="response"></a><span data-ttu-id="163b1-156">応答</span><span class="sxs-lookup"><span data-stu-id="163b1-156">Response</span></span>

<span data-ttu-id="163b1-157">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文に [mailboxSettings](../resources/mailboxsettings.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="163b1-157">If successful, this method returns a `200 OK` response code and [mailboxSettings](../resources/mailboxsettings.md) object in the response body.</span></span>

## <a name="errors"></a><span data-ttu-id="163b1-158">エラー</span><span class="sxs-lookup"><span data-stu-id="163b1-158">Errors</span></span>

<span data-ttu-id="163b1-159">不適切な値で就労時間を設定すると、次のエラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="163b1-159">Setting working hours with inappropriate values may return the following errors.</span></span>

| <span data-ttu-id="163b1-160">シナリオ</span><span class="sxs-lookup"><span data-stu-id="163b1-160">Scenario</span></span>   | <span data-ttu-id="163b1-161">HTTP ステータス コード</span><span class="sxs-lookup"><span data-stu-id="163b1-161">HTTP status code</span></span> | <span data-ttu-id="163b1-162">エラー コード</span><span class="sxs-lookup"><span data-stu-id="163b1-162">Error code</span></span> | <span data-ttu-id="163b1-163">エラー メッセージ</span><span class="sxs-lookup"><span data-stu-id="163b1-163">Error message</span></span> |
|:-----------|:------|:----------|:----------|
| <span data-ttu-id="163b1-164">無効な **startTime** または **endTime**</span><span class="sxs-lookup"><span data-stu-id="163b1-164">Invalid **startTime** or **endTime**</span></span> | <span data-ttu-id="163b1-165">400</span><span class="sxs-lookup"><span data-stu-id="163b1-165">400</span></span> | <span data-ttu-id="163b1-166">RequestBodyRead</span><span class="sxs-lookup"><span data-stu-id="163b1-166">RequestBodyRead</span></span> | <span data-ttu-id="163b1-167">リテラル '08' を期待される型 'Edm.TimeOfDay' に変換できません。</span><span class="sxs-lookup"><span data-stu-id="163b1-167">Cannot convert the literal '08' to the expected type 'Edm.TimeOfDay'.</span></span>|
| <span data-ttu-id="163b1-168">終了時刻の後に設定されている開始時刻</span><span class="sxs-lookup"><span data-stu-id="163b1-168">Start time is greater than end time</span></span> | <span data-ttu-id="163b1-169">400</span><span class="sxs-lookup"><span data-stu-id="163b1-169">400</span></span> | <span data-ttu-id="163b1-170">ErrorInvalidTimeSettings</span><span class="sxs-lookup"><span data-stu-id="163b1-170">ErrorInvalidTimeSettings</span></span> | <span data-ttu-id="163b1-171">開始時刻は、終了時刻の前でなければなりません。</span><span class="sxs-lookup"><span data-stu-id="163b1-171">Start Time should occur before End Time.</span></span> |
| <span data-ttu-id="163b1-172">**daysOfWeek** に設定された無効な曜日</span><span class="sxs-lookup"><span data-stu-id="163b1-172">Invalid day in **daysOfWeek**</span></span> | <span data-ttu-id="163b1-173">400</span><span class="sxs-lookup"><span data-stu-id="163b1-173">400</span></span> | <span data-ttu-id="163b1-174">InvalidArguments</span><span class="sxs-lookup"><span data-stu-id="163b1-174">InvalidArguments</span></span> | <span data-ttu-id="163b1-175">要求された値 'RandomDay' が見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="163b1-175">Requested value 'RandomDay' was not found.</span></span>|
| <span data-ttu-id="163b1-176">無効な **timeZone**</span><span class="sxs-lookup"><span data-stu-id="163b1-176">Invalid **timeZone**</span></span> | <span data-ttu-id="163b1-177">400</span><span class="sxs-lookup"><span data-stu-id="163b1-177">400</span></span> | <span data-ttu-id="163b1-178">InvalidTimeZone</span><span class="sxs-lookup"><span data-stu-id="163b1-178">InvalidTimeZone</span></span> | <span data-ttu-id="163b1-179">指定されているタイム ゾーンの設定は無効です。</span><span class="sxs-lookup"><span data-stu-id="163b1-179">Time Zone settings provided are invalid.</span></span>|


## <a name="example"></a><span data-ttu-id="163b1-180">例</span><span class="sxs-lookup"><span data-stu-id="163b1-180">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="163b1-181">要求 1</span><span class="sxs-lookup"><span data-stu-id="163b1-181">Request 1</span></span>
<span data-ttu-id="163b1-182">最初の例では、**automaticRepliesSetting** プロパティの **status**、**scheduledStartDateTime** および **scheduledEndDateTime** プロパティを設定して、該当する日付範囲に対して自動応答を有効にします。</span><span class="sxs-lookup"><span data-stu-id="163b1-182">The first example enables automatic replies for a date range, by setting the following properties of the **automaticRepliesSetting** property: **status**, **scheduledStartDateTime** and **scheduledEndDateTime**.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_mailboxsettings_1"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/mailboxSettings
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/mailboxSettings",
    "automaticRepliesSetting": {
        "status": "Scheduled",
        "scheduledStartDateTime": {
          "dateTime": "2016-03-20T18:00:00.0000000",
          "timeZone": "UTC"
        },
        "scheduledEndDateTime": {
          "dateTime": "2016-03-28T18:00:00.0000000",
          "timeZone": "UTC"
        }
    }
}
```
##### <a name="response-1"></a><span data-ttu-id="163b1-183">応答 1</span><span class="sxs-lookup"><span data-stu-id="163b1-183">Response 1</span></span>
<span data-ttu-id="163b1-184">この応答には、自動応答の設定が含まれます。</span><span class="sxs-lookup"><span data-stu-id="163b1-184">The response includes the updated settings for automatic replies.</span></span> <span data-ttu-id="163b1-185">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="163b1-185">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="163b1-186">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="163b1-186">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "update_mailboxsettings_1",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxSettings"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/mailboxSettings",
    "automaticRepliesSetting": {
        "status": "scheduled",
        "externalAudience": "all",
        "scheduledStartDateTime": {
            "dateTime": "2016-03-20T02:00:00.0000000",
            "timeZone": "UTC"
        },
        "scheduledEndDateTime": {
            "dateTime": "2016-03-28T02:00:00.0000000",
            "timeZone": "UTC"
        },
    "internalReplyMessage": "<html>\n<body>\n<p>I'm at our company's worldwide reunion and will respond to your message as soon as I return.<br>\n</p></body>\n</html>\n",
    "externalReplyMessage": "<html>\n<body>\n<p>I'm at the Contoso worldwide reunion and will respond to your message as soon as I return.<br>\n</p></body>\n</html>\n"
    }
}
```


##### <a name="request-2"></a><span data-ttu-id="163b1-187">要求 2</span><span class="sxs-lookup"><span data-stu-id="163b1-187">Request 2</span></span>
<span data-ttu-id="163b1-188">2 番目の例では、サインインしているユーザーの就業時間のタイム ゾーンをカスタマイズするために、**timeZone** プロパティを[カスタム タイム ゾーン](../resources/customtimezone.md)に設定します。</span><span class="sxs-lookup"><span data-stu-id="163b1-188">The second example customizes the time zone for the working hours of the signed-in user, by setting the **timeZone** property to a [custom time zone](../resources/customtimezone.md).</span></span>

<!-- {
  "blockType": "ignored",
  "name": "update_mailboxsettings_2"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/mailboxSettings
Content-Type: application/json

{
  "workingHours": {
      "endTime" : "18:30:00.0000000", 
      "daysOfWeek": [ 
          "Monday", 
          "Tuesday", 
          "Wednesday", 
          "Thursday", 
          "Friday", 
          "Saturday" 
      ], 
      "timeZone" : { 
         "@odata.type": "#microsoft.graph.customTimeZone", 
         "bias":-300, 
         "name": "Customized Time Zone",
         "standardOffset":{   
           "time":"02:00:00.0000000", 
           "dayOccurrence":2, 
           "dayOfWeek":"Sunday", 
           "month":10, 
           "year":0 
         }, 
         "daylightOffset":{   
           "daylightBias":100, 
           "time":"02:00:00.0000000", 
           "dayOccurrence":4, 
           "dayOfWeek":"Sunday", 
           "month":5, 
           "year":0 
         } 
      } 
  }
} 
```
##### <a name="response-2"></a><span data-ttu-id="163b1-189">応答 2</span><span class="sxs-lookup"><span data-stu-id="163b1-189">Response 2</span></span>
<span data-ttu-id="163b1-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="163b1-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "update_mailboxsettings_2",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxSettings"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('94447c6e-ea4c-494c-a9ed-d905e366c5cb')/mailboxSettings",
    "workingHours":{
        "daysOfWeek":[
            "monday",
            "tuesday",
            "wednesday",
            "thursday",
            "friday",
            "saturday"
        ],
        "startTime":"09:00:00.0000000",
        "endTime":"18:30:00.0000000",
        "timeZone":{
            "@odata.type":"#microsoft.graph.customTimeZone",
            "bias":-200,
            "name":"Customized Time Zone",
            "standardOffset":{
                "time":"02:00:00.0000000",
                "dayOccurrence":4,
                "dayOfWeek":"sunday",
                "month":5,
                "year":0
            },
            "daylightOffset":{
                "daylightBias":-100,
                "time":"02:00:00.0000000",
                "dayOccurrence":2,
                "dayOfWeek":"sunday",
                "month":10,
                "year":0
            }
        }
    }
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update mailbox settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->