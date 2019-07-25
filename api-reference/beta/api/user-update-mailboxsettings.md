---
title: ユーザーのメールボックスの設定を更新する
description: ユーザーのメールボックスの 1 つ以上の設定を更新します。 これには、自動応答の設定 (電子メールの受信時にユーザーに自動的に通知される)、ロケール (言語と国/地域)、タイムゾーン、および稼働時間の設定が含まれます。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7c61a56996d53f3e72b847a627e7140f46cd025a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35866680"
---
# <a name="update-user-mailbox-settings"></a><span data-ttu-id="816a7-104">ユーザーのメールボックスの設定を更新する</span><span class="sxs-lookup"><span data-stu-id="816a7-104">Update user mailbox settings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="816a7-p102">ユーザーのメールボックスの設定を 1 つ以上更新します。これには、[自動応答](../resources/automaticrepliessetting.md) (電子メールの受信時に自動的にユーザーに通知)、[ロケール](../resources/localeinfo.md) (言語と国/地域)、タイム ゾーン、[就業時間](../resources/workinghours.md)の設定が含まれます。</span><span class="sxs-lookup"><span data-stu-id="816a7-p102">Update one or more settings for the user's mailbox. This includes settings for [automatic replies](../resources/automaticrepliessetting.md) (notify people automatically upon receipt of their email), [locale](../resources/localeinfo.md) (language and country/region), time zone, and [working hours](../resources/workinghours.md).</span></span>

<span data-ttu-id="816a7-107">これらの設定の 1 つ以上を、[mailboxSettings](../resources/mailboxsettings.md)の一部として有効化、構成、または無効化できます。</span><span class="sxs-lookup"><span data-stu-id="816a7-107">You can enable, configure, or disable one or more of these settings as part of [mailboxSettings](../resources/mailboxsettings.md).</span></span>

<span data-ttu-id="816a7-108">**注** メールボックス設定は作成または削除できません。</span><span class="sxs-lookup"><span data-stu-id="816a7-108">**Note** You cannot create or delete any mailbox settings.</span></span>

<span data-ttu-id="816a7-109">ユーザーの優先タイム ゾーンを更新する場合、Windows または [Internet Assigned Numbers Authority (IANA) のタイム ゾーン](https://www.iana.org/time-zones) (別称: Olson タイム ゾーン) 形式で指定することができます。</span><span class="sxs-lookup"><span data-stu-id="816a7-109">When you update the preferred time zone for a user, you can specify it in the Windows or  [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="816a7-110">また、次の[例 2](#request-2)に示すように、タイムゾーンをさらにカスタマイズすることもできます。</span><span class="sxs-lookup"><span data-stu-id="816a7-110">You can also further customize the time zone as shown in [example 2](#request-2) below.</span></span>

## <a name="permissions"></a><span data-ttu-id="816a7-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="816a7-111">Permissions</span></span>
<span data-ttu-id="816a7-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="816a7-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="816a7-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="816a7-114">Permission type</span></span>      | <span data-ttu-id="816a7-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="816a7-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="816a7-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="816a7-116">Delegated (work or school account)</span></span> | <span data-ttu-id="816a7-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="816a7-117">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="816a7-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="816a7-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="816a7-119">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="816a7-119">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="816a7-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="816a7-120">Application</span></span> | <span data-ttu-id="816a7-121">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="816a7-121">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="816a7-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="816a7-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailboxSettings
PATCH /users/{id|userPrincipalName}/mailboxSettings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="816a7-123">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="816a7-123">Optional query parameters</span></span>
<span data-ttu-id="816a7-124">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="816a7-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="816a7-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="816a7-125">Request headers</span></span>
| <span data-ttu-id="816a7-126">名前</span><span class="sxs-lookup"><span data-stu-id="816a7-126">Name</span></span>       | <span data-ttu-id="816a7-127">型</span><span class="sxs-lookup"><span data-stu-id="816a7-127">Type</span></span> | <span data-ttu-id="816a7-128">説明</span><span class="sxs-lookup"><span data-stu-id="816a7-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="816a7-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="816a7-129">Authorization</span></span>  | <span data-ttu-id="816a7-130">string</span><span class="sxs-lookup"><span data-stu-id="816a7-130">string</span></span>  | <span data-ttu-id="816a7-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="816a7-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="816a7-133">要求本文</span><span class="sxs-lookup"><span data-stu-id="816a7-133">Request body</span></span>
<span data-ttu-id="816a7-p106">要求本文で、更新する関連プロパティの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。書き込み可能または更新可能なプロパティを次に示します。</span><span class="sxs-lookup"><span data-stu-id="816a7-p106">In the request body, supply the values for the relevant properties that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. The following are the writable/updatable properties:</span></span>

| <span data-ttu-id="816a7-138">プロパティ</span><span class="sxs-lookup"><span data-stu-id="816a7-138">Property</span></span>     | <span data-ttu-id="816a7-139">型</span><span class="sxs-lookup"><span data-stu-id="816a7-139">Type</span></span>   |<span data-ttu-id="816a7-140">説明</span><span class="sxs-lookup"><span data-stu-id="816a7-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="816a7-141">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="816a7-141">automaticRepliesSetting</span></span>|[<span data-ttu-id="816a7-142">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="816a7-142">automaticRepliesSetting</span></span>](../resources/automaticrepliessetting.md)|<span data-ttu-id="816a7-143">サインイン ユーザーからのメッセージを使用して、着信メールの送信者に自動的に通知する構成設定。</span><span class="sxs-lookup"><span data-stu-id="816a7-143">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span> <span data-ttu-id="816a7-144">このような通知は、将来の日付範囲に対してのみ設定できます。</span><span class="sxs-lookup"><span data-stu-id="816a7-144">You can set such notifications for only a future date range.</span></span>|
|<span data-ttu-id="816a7-145">language</span><span class="sxs-lookup"><span data-stu-id="816a7-145">language</span></span>|[<span data-ttu-id="816a7-146">localeInfo</span><span class="sxs-lookup"><span data-stu-id="816a7-146">localeInfo</span></span>](../resources/localeinfo.md)|<span data-ttu-id="816a7-147">優先言語および国/地域を含むユーザーのロケール情報。</span><span class="sxs-lookup"><span data-stu-id="816a7-147">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="816a7-148">timeZone</span><span class="sxs-lookup"><span data-stu-id="816a7-148">timeZone</span></span>|<span data-ttu-id="816a7-149">string</span><span class="sxs-lookup"><span data-stu-id="816a7-149">string</span></span>|<span data-ttu-id="816a7-150">ユーザーのメールボックスの既定のタイム ゾーン。</span><span class="sxs-lookup"><span data-stu-id="816a7-150">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="816a7-151">workingHours</span><span class="sxs-lookup"><span data-stu-id="816a7-151">workingHours</span></span>|[<span data-ttu-id="816a7-152">workingHours</span><span class="sxs-lookup"><span data-stu-id="816a7-152">workingHours</span></span>](../resources/workinghours.md)|<span data-ttu-id="816a7-153">ユーザーが働く時間、曜日、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="816a7-153">The hours, days of a week, and time zone that the user works.</span></span>|

## <a name="response"></a><span data-ttu-id="816a7-154">応答</span><span class="sxs-lookup"><span data-stu-id="816a7-154">Response</span></span>

<span data-ttu-id="816a7-155">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文に [mailboxSettings](../resources/mailboxsettings.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="816a7-155">If successful, this method returns a `200 OK` response code and [mailboxSettings](../resources/mailboxsettings.md) object in the response body.</span></span>

## <a name="errors"></a><span data-ttu-id="816a7-156">エラー</span><span class="sxs-lookup"><span data-stu-id="816a7-156">Errors</span></span>

<span data-ttu-id="816a7-157">不適切な値で就労時間を設定すると、次のエラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="816a7-157">Setting working hours with inappropriate values may return the following errors.</span></span>

| <span data-ttu-id="816a7-158">シナリオ</span><span class="sxs-lookup"><span data-stu-id="816a7-158">Scenario</span></span>   | <span data-ttu-id="816a7-159">HTTP ステータス コード</span><span class="sxs-lookup"><span data-stu-id="816a7-159">HTTP status code</span></span> | <span data-ttu-id="816a7-160">エラー コード</span><span class="sxs-lookup"><span data-stu-id="816a7-160">Error code</span></span> | <span data-ttu-id="816a7-161">エラー メッセージ</span><span class="sxs-lookup"><span data-stu-id="816a7-161">Error message</span></span> |
|:-----------|:------|:----------|:----------|
| <span data-ttu-id="816a7-162">無効な **startTime** または **endTime**</span><span class="sxs-lookup"><span data-stu-id="816a7-162">Invalid **startTime** or **endTime**</span></span> | <span data-ttu-id="816a7-163">400</span><span class="sxs-lookup"><span data-stu-id="816a7-163">400</span></span> | <span data-ttu-id="816a7-164">RequestBodyRead</span><span class="sxs-lookup"><span data-stu-id="816a7-164">RequestBodyRead</span></span> | <span data-ttu-id="816a7-165">リテラル '08' を期待される型 'Edm.TimeOfDay' に変換できません。</span><span class="sxs-lookup"><span data-stu-id="816a7-165">Cannot convert the literal '08' to the expected type 'Edm.TimeOfDay'.</span></span>|
| <span data-ttu-id="816a7-166">終了時刻の後に設定されている開始時刻</span><span class="sxs-lookup"><span data-stu-id="816a7-166">Start time is greater than end time</span></span> | <span data-ttu-id="816a7-167">400</span><span class="sxs-lookup"><span data-stu-id="816a7-167">400</span></span> | <span data-ttu-id="816a7-168">ErrorInvalidTimeSettings</span><span class="sxs-lookup"><span data-stu-id="816a7-168">ErrorInvalidTimeSettings</span></span> | <span data-ttu-id="816a7-169">開始時刻は、終了時刻の前でなければなりません。</span><span class="sxs-lookup"><span data-stu-id="816a7-169">Start Time should occur before End Time.</span></span> |
| <span data-ttu-id="816a7-170">**daysOfWeek** に設定された無効な曜日</span><span class="sxs-lookup"><span data-stu-id="816a7-170">Invalid day in **daysOfWeek**</span></span> | <span data-ttu-id="816a7-171">400</span><span class="sxs-lookup"><span data-stu-id="816a7-171">400</span></span> | <span data-ttu-id="816a7-172">InvalidArguments</span><span class="sxs-lookup"><span data-stu-id="816a7-172">InvalidArguments</span></span> | <span data-ttu-id="816a7-173">要求された値 'RandomDay' が見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="816a7-173">Requested value 'RandomDay' was not found.</span></span>|
| <span data-ttu-id="816a7-174">無効な **timeZone**</span><span class="sxs-lookup"><span data-stu-id="816a7-174">Invalid **timeZone**</span></span> | <span data-ttu-id="816a7-175">400</span><span class="sxs-lookup"><span data-stu-id="816a7-175">400</span></span> | <span data-ttu-id="816a7-176">InvalidTimeZone</span><span class="sxs-lookup"><span data-stu-id="816a7-176">InvalidTimeZone</span></span> | <span data-ttu-id="816a7-177">指定されているタイム ゾーンの設定は無効です。</span><span class="sxs-lookup"><span data-stu-id="816a7-177">Time Zone settings provided are invalid.</span></span>|


## <a name="example"></a><span data-ttu-id="816a7-178">例</span><span class="sxs-lookup"><span data-stu-id="816a7-178">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="816a7-179">要求 1</span><span class="sxs-lookup"><span data-stu-id="816a7-179">Request 1</span></span>
<span data-ttu-id="816a7-180">最初の例では、**automaticRepliesSetting** プロパティの **status**、**scheduledStartDateTime** および **scheduledEndDateTime** プロパティを設定して、該当する日付範囲に対して自動応答を有効にします。</span><span class="sxs-lookup"><span data-stu-id="816a7-180">The first example enables automatic replies for a date range, by setting the following properties of the **automaticRepliesSetting** property: **status**, **scheduledStartDateTime** and **scheduledEndDateTime**.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="816a7-181">プロトコル</span><span class="sxs-lookup"><span data-stu-id="816a7-181">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="816a7-182">C#</span><span class="sxs-lookup"><span data-stu-id="816a7-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-mailboxsettings-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="816a7-183">Javascript</span><span class="sxs-lookup"><span data-stu-id="816a7-183">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-mailboxsettings-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="816a7-184">目的-C</span><span class="sxs-lookup"><span data-stu-id="816a7-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-mailboxsettings-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="816a7-185">Java</span><span class="sxs-lookup"><span data-stu-id="816a7-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-mailboxsettings-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-1"></a><span data-ttu-id="816a7-186">応答 1</span><span class="sxs-lookup"><span data-stu-id="816a7-186">Response 1</span></span>
<span data-ttu-id="816a7-187">この応答には、自動応答の設定が含まれます。</span><span class="sxs-lookup"><span data-stu-id="816a7-187">The response includes the updated settings for automatic replies.</span></span> <span data-ttu-id="816a7-188">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="816a7-188">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="816a7-189">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="816a7-189">All of the properties will be returned from an actual call.</span></span>
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


##### <a name="request-2"></a><span data-ttu-id="816a7-190">要求 2</span><span class="sxs-lookup"><span data-stu-id="816a7-190">Request 2</span></span>
<span data-ttu-id="816a7-191">2 番目の例では、サインインしているユーザーの就業時間のタイム ゾーンをカスタマイズするために、**timeZone** プロパティを[カスタム タイム ゾーン](../resources/customtimezone.md)に設定します。</span><span class="sxs-lookup"><span data-stu-id="816a7-191">The second example customizes the time zone for the working hours of the signed-in user, by setting the **timeZone** property to a [custom time zone](../resources/customtimezone.md).</span></span>

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
##### <a name="response-2"></a><span data-ttu-id="816a7-192">応答 2</span><span class="sxs-lookup"><span data-stu-id="816a7-192">Response 2</span></span>
<span data-ttu-id="816a7-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="816a7-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update mailbox settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
