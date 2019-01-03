---
title: ユーザーのメールボックスの設定を更新する
description: ユーザーのメールボックスの設定を 1 つ以上更新します。これには、自動応答 (電子メールの受信時に自動的にユーザーに通知)、ロケール (言語と国/地域)、タイム ゾーン、就業時間の設定が含まれます。
ms.openlocfilehash: b5d52771e67bb79abb7c325c908e0c5f155fff15
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020345"
---
# <a name="update-user-mailbox-settings"></a><span data-ttu-id="119ca-104">ユーザーのメールボックスの設定を更新する</span><span class="sxs-lookup"><span data-stu-id="119ca-104">Update user mailbox settings</span></span>

<span data-ttu-id="119ca-p102">ユーザーのメールボックスの設定を 1 つ以上更新します。これには、[自動応答](../resources/automaticrepliessetting.md) (電子メールの受信時に自動的にユーザーに通知)、[ロケール](../resources/localeinfo.md) (言語と国/地域)、タイム ゾーン、[就業時間](../resources/workinghours.md)の設定が含まれます。</span><span class="sxs-lookup"><span data-stu-id="119ca-p102">Update one or more settings for the user's mailbox. This includes settings for [automatic replies](../resources/automaticrepliessetting.md) (notify people automatically upon receipt of their email), [locale](../resources/localeinfo.md) (language and country/region), time zone, and [working hours](../resources/workinghours.md).</span></span>

<span data-ttu-id="119ca-107">これらの設定の 1 つ以上を、[mailboxSettings](../resources/mailboxsettings.md)の一部として有効化、構成、または無効化できます。</span><span class="sxs-lookup"><span data-stu-id="119ca-107">You can enable, configure, or disable one or more of these settings as part of [mailboxSettings](../resources/mailboxsettings.md).</span></span>

<span data-ttu-id="119ca-108">**注** メールボックス設定は作成または削除できません。</span><span class="sxs-lookup"><span data-stu-id="119ca-108">**Note** You cannot create or delete any mailbox settings.</span></span>

<span data-ttu-id="119ca-109">ユーザーの優先タイム ゾーンを更新する場合、Windows または [Internet Assigned Numbers Authority (IANA) のタイム ゾーン](https://www.iana.org/time-zones) (別称: Olson タイム ゾーン) 形式で指定することができます。</span><span class="sxs-lookup"><span data-stu-id="119ca-109">When you update the preferred time zone for a user, you can specify it in the Windows or  [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span>

## <a name="permissions"></a><span data-ttu-id="119ca-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="119ca-110">Permissions</span></span>
<span data-ttu-id="119ca-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="119ca-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="119ca-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="119ca-113">Permission type</span></span>      | <span data-ttu-id="119ca-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="119ca-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="119ca-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="119ca-115">Delegated (work or school account)</span></span> | <span data-ttu-id="119ca-116">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="119ca-116">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="119ca-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="119ca-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="119ca-118">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="119ca-118">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="119ca-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="119ca-119">Application</span></span> | <span data-ttu-id="119ca-120">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="119ca-120">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="119ca-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="119ca-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailboxSettings
PATCH /users/{id|userPrincipalName}/mailboxSettings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="119ca-122">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="119ca-122">Optional query parameters</span></span>
<span data-ttu-id="119ca-123">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="119ca-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="119ca-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="119ca-124">Request headers</span></span>
| <span data-ttu-id="119ca-125">名前</span><span class="sxs-lookup"><span data-stu-id="119ca-125">Name</span></span>       | <span data-ttu-id="119ca-126">型</span><span class="sxs-lookup"><span data-stu-id="119ca-126">Type</span></span> | <span data-ttu-id="119ca-127">説明</span><span class="sxs-lookup"><span data-stu-id="119ca-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="119ca-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="119ca-128">Authorization</span></span>  | <span data-ttu-id="119ca-129">string</span><span class="sxs-lookup"><span data-stu-id="119ca-129">string</span></span>  | <span data-ttu-id="119ca-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="119ca-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="119ca-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="119ca-132">Request body</span></span>
<span data-ttu-id="119ca-p105">要求本文で、更新する関連プロパティの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。書き込み可能または更新可能なプロパティを次に示します。</span><span class="sxs-lookup"><span data-stu-id="119ca-p105">In the request body, supply the values for the relevant properties that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. The following are the writable/updatable properties:</span></span>

| <span data-ttu-id="119ca-137">プロパティ</span><span class="sxs-lookup"><span data-stu-id="119ca-137">Property</span></span>     | <span data-ttu-id="119ca-138">型</span><span class="sxs-lookup"><span data-stu-id="119ca-138">Type</span></span>   |<span data-ttu-id="119ca-139">説明</span><span class="sxs-lookup"><span data-stu-id="119ca-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="119ca-140">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="119ca-140">automaticRepliesSetting</span></span>|[<span data-ttu-id="119ca-141">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="119ca-141">automaticRepliesSetting</span></span>](../resources/automaticrepliessetting.md)|<span data-ttu-id="119ca-142">サインイン ユーザーからのメッセージを使用して、着信メールの送信者に自動的に通知する構成設定。</span><span class="sxs-lookup"><span data-stu-id="119ca-142">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span> <span data-ttu-id="119ca-143">将来の日付の範囲だけにこのような通知を設定することができます。</span><span class="sxs-lookup"><span data-stu-id="119ca-143">You can set such notifications for only a future date range.</span></span>|
|<span data-ttu-id="119ca-144">language</span><span class="sxs-lookup"><span data-stu-id="119ca-144">language</span></span>|[<span data-ttu-id="119ca-145">localeInfo</span><span class="sxs-lookup"><span data-stu-id="119ca-145">localeInfo</span></span>](../resources/localeinfo.md)|<span data-ttu-id="119ca-146">優先言語および国/地域を含むユーザーのロケール情報。</span><span class="sxs-lookup"><span data-stu-id="119ca-146">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="119ca-147">timeZone</span><span class="sxs-lookup"><span data-stu-id="119ca-147">timeZone</span></span>|<span data-ttu-id="119ca-148">文字列</span><span class="sxs-lookup"><span data-stu-id="119ca-148">string</span></span>|<span data-ttu-id="119ca-149">ユーザーのメールボックスの既定のタイム ゾーン。</span><span class="sxs-lookup"><span data-stu-id="119ca-149">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="119ca-150">workingHours</span><span class="sxs-lookup"><span data-stu-id="119ca-150">workingHours</span></span>|[<span data-ttu-id="119ca-151">workingHours</span><span class="sxs-lookup"><span data-stu-id="119ca-151">workingHours</span></span>](../resources/workinghours.md)|<span data-ttu-id="119ca-152">ユーザーが働く時間、曜日、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="119ca-152">The hours, days of a week, and time zone that the user works.</span></span>|

## <a name="response"></a><span data-ttu-id="119ca-153">応答</span><span class="sxs-lookup"><span data-stu-id="119ca-153">Response</span></span>

<span data-ttu-id="119ca-154">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文に [mailboxSettings](../resources/mailboxsettings.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="119ca-154">If successful, this method returns a `200 OK` response code and [mailboxSettings](../resources/mailboxsettings.md) object in the response body.</span></span>


## <a name="errors"></a><span data-ttu-id="119ca-155">エラー</span><span class="sxs-lookup"><span data-stu-id="119ca-155">Errors</span></span>

<span data-ttu-id="119ca-156">不適切な値で就労時間を設定すると、次のエラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="119ca-156">Setting working hours with inappropriate values may return the following errors.</span></span>

| <span data-ttu-id="119ca-157">シナリオ</span><span class="sxs-lookup"><span data-stu-id="119ca-157">Scenario</span></span>   | <span data-ttu-id="119ca-158">HTTP ステータス コード</span><span class="sxs-lookup"><span data-stu-id="119ca-158">HTTP status code</span></span> | <span data-ttu-id="119ca-159">エラー コード</span><span class="sxs-lookup"><span data-stu-id="119ca-159">Error code</span></span> | <span data-ttu-id="119ca-160">エラー メッセージ</span><span class="sxs-lookup"><span data-stu-id="119ca-160">Error message</span></span> |
|:-----------|:------|:----------|:----------|
| <span data-ttu-id="119ca-161">無効な **startTime** または **endTime**</span><span class="sxs-lookup"><span data-stu-id="119ca-161">Invalid **startTime** or **endTime**</span></span> | <span data-ttu-id="119ca-162">400</span><span class="sxs-lookup"><span data-stu-id="119ca-162">400</span></span> | <span data-ttu-id="119ca-163">RequestBodyRead</span><span class="sxs-lookup"><span data-stu-id="119ca-163">RequestBodyRead</span></span> | <span data-ttu-id="119ca-164">リテラル '08' を期待される型 'Edm.TimeOfDay' に変換できません。</span><span class="sxs-lookup"><span data-stu-id="119ca-164">Cannot convert the literal '08' to the expected type 'Edm.TimeOfDay'.</span></span>|
| <span data-ttu-id="119ca-165">終了時刻の後に設定されている開始時刻</span><span class="sxs-lookup"><span data-stu-id="119ca-165">Start time is greater than end time</span></span> | <span data-ttu-id="119ca-166">400</span><span class="sxs-lookup"><span data-stu-id="119ca-166">400</span></span> | <span data-ttu-id="119ca-167">ErrorInvalidTimeSettings</span><span class="sxs-lookup"><span data-stu-id="119ca-167">ErrorInvalidTimeSettings</span></span> | <span data-ttu-id="119ca-168">開始時刻は、終了時刻の前でなければなりません。</span><span class="sxs-lookup"><span data-stu-id="119ca-168">Start Time should occur before End Time.</span></span> |
| <span data-ttu-id="119ca-169">**daysOfWeek** に設定された無効な曜日</span><span class="sxs-lookup"><span data-stu-id="119ca-169">Invalid day in **daysOfWeek**</span></span> | <span data-ttu-id="119ca-170">400</span><span class="sxs-lookup"><span data-stu-id="119ca-170">400</span></span> | <span data-ttu-id="119ca-171">InvalidArguments</span><span class="sxs-lookup"><span data-stu-id="119ca-171">InvalidArguments</span></span> | <span data-ttu-id="119ca-172">要求された値 'RandomDay' が見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="119ca-172">Requested value 'RandomDay' was not found.</span></span>|
| <span data-ttu-id="119ca-173">無効な **timeZone**</span><span class="sxs-lookup"><span data-stu-id="119ca-173">Invalid **timeZone**</span></span> | <span data-ttu-id="119ca-174">400</span><span class="sxs-lookup"><span data-stu-id="119ca-174">400</span></span> | <span data-ttu-id="119ca-175">InvalidTimeZone</span><span class="sxs-lookup"><span data-stu-id="119ca-175">InvalidTimeZone</span></span> | <span data-ttu-id="119ca-176">指定されているタイム ゾーンの設定は無効です。</span><span class="sxs-lookup"><span data-stu-id="119ca-176">Time Zone settings provided are invalid.</span></span>|


## <a name="example"></a><span data-ttu-id="119ca-177">例</span><span class="sxs-lookup"><span data-stu-id="119ca-177">Example</span></span>
##### <a name="request"></a><span data-ttu-id="119ca-178">要求</span><span class="sxs-lookup"><span data-stu-id="119ca-178">Request</span></span>
<span data-ttu-id="119ca-179">最初の例では、**automaticRepliesSetting** プロパティの **status**、**scheduledStartDateTime** および **scheduledEndDateTime** プロパティを設定して、該当する日付範囲に対して自動応答を有効にします。</span><span class="sxs-lookup"><span data-stu-id="119ca-179">The first example enables automatic replies for a date range, by setting the following properties of the **automaticRepliesSetting** property: **status**, **scheduledStartDateTime** and **scheduledEndDateTime**.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_mailboxsettings"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/mailboxSettings
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/mailboxSettings",
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
##### <a name="response"></a><span data-ttu-id="119ca-180">応答</span><span class="sxs-lookup"><span data-stu-id="119ca-180">Response</span></span>
<span data-ttu-id="119ca-181">この応答には、自動応答の設定が含まれます。</span><span class="sxs-lookup"><span data-stu-id="119ca-181">The response includes the updated settings for automatic replies.</span></span> <span data-ttu-id="119ca-182">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="119ca-182">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="119ca-183">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="119ca-183">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxSettings"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/mailboxSettings",
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


##### <a name="request-2"></a><span data-ttu-id="119ca-184">要求 2</span><span class="sxs-lookup"><span data-stu-id="119ca-184">Request 2</span></span>
<span data-ttu-id="119ca-185">2 番目の例では、サインインしているユーザーの就業時間のタイム ゾーンをカスタマイズするために、**timeZone** プロパティを[カスタム タイム ゾーン](../resources/customtimezone.md)に設定します。</span><span class="sxs-lookup"><span data-stu-id="119ca-185">The second example customizes the time zone for the working hours of the signed-in user, by setting the **timeZone** property to a [custom time zone](../resources/customtimezone.md).</span></span>

<!-- {
  "blockType": "ignored",
  "name": "update_mailboxsettings_2"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/mailboxSettings
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
##### <a name="response-2"></a><span data-ttu-id="119ca-186">応答 2</span><span class="sxs-lookup"><span data-stu-id="119ca-186">Response 2</span></span>
<span data-ttu-id="119ca-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="119ca-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('94447c6e-ea4c-494c-a9ed-d905e366c5cb')/mailboxSettings",
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