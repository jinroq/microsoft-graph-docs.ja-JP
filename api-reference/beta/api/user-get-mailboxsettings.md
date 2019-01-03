---
title: ユーザーのメールボックスの設定を取得する
description: 'ユーザーの mailboxSettings を取得します。 (時に自動的にユーザーに通知する自動返信の設定が含まれます '
ms.openlocfilehash: fae1bb16ec533abf7f29d0aadc0f66ba33f5ec25
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072950"
---
# <a name="get-user-mailbox-settings"></a><span data-ttu-id="32b40-104">ユーザーのメールボックスの設定を取得する</span><span class="sxs-lookup"><span data-stu-id="32b40-104">Get user mailbox settings</span></span>

> <span data-ttu-id="32b40-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="32b40-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="32b40-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="32b40-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="32b40-107">ユーザーの[mailboxSettings](../resources/mailboxsettings.md)を取得します。</span><span class="sxs-lookup"><span data-stu-id="32b40-107">Get the user's [mailboxSettings](../resources/mailboxsettings.md).</span></span> <span data-ttu-id="32b40-108">(自分の電子メールの受信時に自動的にユーザーに通知) の自動返信、ロケール (言語および国/地域)、タイム ゾーン、および作業時間の設定が含まれます。</span><span class="sxs-lookup"><span data-stu-id="32b40-108">This includes settings for automatic replies (notify people automatically upon receipt of their email), locale (language and country/region), time zone, and working hours.</span></span>

<span data-ttu-id="32b40-109">すべてのメールボックス設定を表示することも、特定の設定を取得することもできます。</span><span class="sxs-lookup"><span data-stu-id="32b40-109">You can view all mailbox settings, or, get specific settings.</span></span>

<span data-ttu-id="32b40-110">タイム ゾーンは、ユーザーが自分のメールボックスに設定できる優先設定のうちの 1 つです。</span><span class="sxs-lookup"><span data-stu-id="32b40-110">Time zone is one of the preferred settings a user can set up for the user's mailbox.</span></span> <span data-ttu-id="32b40-111">ユーザーを設定すると、[タイム ゾーンがサポートされている](outlookuser-supportedtimezones.md)ユーザーのメールボックス サーバーの管理者が設定することを選択します。</span><span class="sxs-lookup"><span data-stu-id="32b40-111">The user chooses it from the [supported time zones](outlookuser-supportedtimezones.md) that an administrator has set up for the user's mailbox server.</span></span> <span data-ttu-id="32b40-112">管理者は、Windows タイム ゾーンの形式または[インターネット割り当て番号機関 (IANA) タイム ゾーン](https://www.iana.org/time-zones)(Olson タイム ・ ゾーンとも呼ばれます) の形式でタイムゾーンを設定します。</span><span class="sxs-lookup"><span data-stu-id="32b40-112">The administrator sets up time zones in the Windows time zone format or  [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="32b40-113">既定値は Windows 形式です。</span><span class="sxs-lookup"><span data-stu-id="32b40-113">The Windows format is the default.</span></span> 

<span data-ttu-id="32b40-114">ユーザーの優先タイム ゾーンを取得するとき、そのタイム ゾーンは設定された形式で返されます。</span><span class="sxs-lookup"><span data-stu-id="32b40-114">When you get a user's preferred time zone, the time zone is returned in the format that it was set up.</span></span> <span data-ttu-id="32b40-115">タイム ゾーンを特定の形式 (Windows または IANA) にする場合は、最初に[メールボックス設定としてその形式の優先タイム ゾーンを更新](user-update-mailboxsettings.md)します。</span><span class="sxs-lookup"><span data-stu-id="32b40-115">If you want that time zone to be in a specific format (Windows or IANA), you can first [update the preferred time zone in that format as a mailbox setting](user-update-mailboxsettings.md).</span></span> <span data-ttu-id="32b40-116">その後は、その形式でタイム ゾーンを取得できるようになります。</span><span class="sxs-lookup"><span data-stu-id="32b40-116">Subsequently you will be able to get the time zone in that format.</span></span> <span data-ttu-id="32b40-117">または、アプリ内で形式変換を個別に管理することもできます。</span><span class="sxs-lookup"><span data-stu-id="32b40-117">Alternatively, you can manage the format conversion separately in your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="32b40-118">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="32b40-118">Permissions</span></span>
<span data-ttu-id="32b40-p106">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="32b40-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32b40-121">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="32b40-121">Permission type</span></span>      | <span data-ttu-id="32b40-122">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="32b40-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="32b40-123">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="32b40-123">Delegated (work or school account)</span></span> | <span data-ttu-id="32b40-124">MailboxSettings.Read、MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="32b40-124">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="32b40-125">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="32b40-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32b40-126">MailboxSettings.Read、MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="32b40-126">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="32b40-127">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="32b40-127">Application</span></span> | <span data-ttu-id="32b40-128">MailboxSettings.Read、MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="32b40-128">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="32b40-129">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="32b40-129">HTTP request</span></span>
<span data-ttu-id="32b40-130">ユーザーのすべてのメールボックスの設定を取得するには。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="32b40-130">To get all the mailbox settings for a user: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/mailboxSettings
GET /users/{id|userPrincipalName}/mailboxSettings
```

<span data-ttu-id="32b40-131">-自動返信の設定、ロケール、タイム ゾーン、または作業時間だけの特定の設定を取得するには。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="32b40-131">To get specific settings - only the automatic replies settings, locale, time zone, or working hours: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/mailboxSettings/automaticRepliesSetting
GET /users/{id|userPrincipalName}/mailboxSettings/automaticRepliesSetting

GET /me/mailboxSettings/language
GET /users/{id|userPrincipalName}/mailboxSettings/language

GET /me/mailboxSettings/timeZone
GET /users/{id|userPrincipalName}/mailboxSettings/timeZone

GET /me/mailboxSettings/workingHours
GET /users/{id|userPrincipalName}/mailboxSettings/workingHours
```
## <a name="optional-query-parameters"></a><span data-ttu-id="32b40-132">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="32b40-132">Optional query parameters</span></span>
<span data-ttu-id="32b40-133">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="32b40-133">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="32b40-134">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="32b40-134">Request headers</span></span>
| <span data-ttu-id="32b40-135">名前</span><span class="sxs-lookup"><span data-stu-id="32b40-135">Name</span></span>       | <span data-ttu-id="32b40-136">型</span><span class="sxs-lookup"><span data-stu-id="32b40-136">Type</span></span> | <span data-ttu-id="32b40-137">説明</span><span class="sxs-lookup"><span data-stu-id="32b40-137">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="32b40-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="32b40-138">Authorization</span></span>  | <span data-ttu-id="32b40-139">string</span><span class="sxs-lookup"><span data-stu-id="32b40-139">string</span></span>  | <span data-ttu-id="32b40-p107">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="32b40-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="32b40-142">要求本文</span><span class="sxs-lookup"><span data-stu-id="32b40-142">Request body</span></span>
<span data-ttu-id="32b40-143">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="32b40-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="32b40-144">応答</span><span class="sxs-lookup"><span data-stu-id="32b40-144">Response</span></span>

<span data-ttu-id="32b40-145">成功した場合、このメソッドは `200 OK` 応答コードと、次に示す要求されたオブジェクトのいずれかを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="32b40-145">If successful, this method returns a `200 OK` response code and one of the following requested objects in the response body:</span></span>

- <span data-ttu-id="32b40-146">[mailboxSettings](../resources/mailboxsettings.md) オブジェクト</span><span class="sxs-lookup"><span data-stu-id="32b40-146">[mailboxSettings](../resources/mailboxsettings.md) object</span></span>
- <span data-ttu-id="32b40-147">[automaticRepliesSetting](../resources/automaticrepliessetting.md) オブジェクト</span><span class="sxs-lookup"><span data-stu-id="32b40-147">[automaticRepliesSetting](../resources/automaticrepliessetting.md) object</span></span>
- <span data-ttu-id="32b40-148">[localeInfo](../resources/localeinfo.md) オブジェクト</span><span class="sxs-lookup"><span data-stu-id="32b40-148">[localeInfo](../resources/localeinfo.md) object</span></span>
- <span data-ttu-id="32b40-149">string (**timeZone** の場合)</span><span class="sxs-lookup"><span data-stu-id="32b40-149">string (for **timeZone**)</span></span>
- [<span data-ttu-id="32b40-150">workingHours</span><span class="sxs-lookup"><span data-stu-id="32b40-150">workingHours</span></span>](../resources/workinghours.md)

## <a name="example"></a><span data-ttu-id="32b40-151">例</span><span class="sxs-lookup"><span data-stu-id="32b40-151">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="32b40-152">要求 1</span><span class="sxs-lookup"><span data-stu-id="32b40-152">Request 1</span></span>
<span data-ttu-id="32b40-153">最初の例では、サインインしているユーザーのメールボックスのすべてのメールボックス設定を取得します。取得される設定には、自動応答、ロケール (言語と国/地域)、タイム ゾーン、就業時間の設定が含まれます。</span><span class="sxs-lookup"><span data-stu-id="32b40-153">The first example gets all the mailbox settings of the signed-in user's mailbox, which include settings for time zone, automatic replies, locale (language and country/region), and working hours.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_1"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailboxSettings
```
##### <a name="response-1"></a><span data-ttu-id="32b40-154">応答 1</span><span class="sxs-lookup"><span data-stu-id="32b40-154">Response 1</span></span>
<span data-ttu-id="32b40-155">応答には、サインイン中のユーザーのすべてのメールボックスの設定が含まれています。</span><span class="sxs-lookup"><span data-stu-id="32b40-155">The response includes all the mailbox settings of the signed-in user.</span></span> <span data-ttu-id="32b40-156">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="32b40-156">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="32b40-157">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="32b40-157">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxSettings"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/mailboxSettings",
    "automaticRepliesSetting": {
        "status": "Scheduled",
        "externalAudience": "All",
        "scheduledStartDateTime": {
            "dateTime": "2016-03-14T07:00:00.0000000",
            "timeZone": "UTC"
        },
        "scheduledEndDateTime": {
            "dateTime": "2016-03-28T07:00:00.0000000",
            "timeZone": "UTC"
        },
        "internalReplyMessage": "<html>\n<body>\n<p>I'm at our company's worldwide reunion and will respond to your message as soon as I return.<br>\n</p></body>\n</html>\n",
        "externalReplyMessage": "<html>\n<body>\n<p>I'm at the Contoso worldwide reunion and will respond to your message as soon as I return.<br>\n</p></body>\n</html>\n"
    },
    "timeZone":"UTC",
    "language":{
      "locale":"en-US",
      "displayName":"English (United States)"
    },
    "workingHours":{
        "daysOfWeek":[
            "monday",
            "tuesday",
            "wednesday",
            "thursday",
            "friday"
        ],
        "startTime":"08:00:00.0000000",
        "endTime":"17:00:00.0000000",
        "timeZone":{
            "name":"Pacific Standard Time"
        }
    }
}
```

##### <a name="request-2"></a><span data-ttu-id="32b40-158">要求 2</span><span class="sxs-lookup"><span data-stu-id="32b40-158">Request 2</span></span>
<span data-ttu-id="32b40-159">2 番目の例では、具体的にサインインしているユーザーのメールボックスの自動応答設定を取得します。</span><span class="sxs-lookup"><span data-stu-id="32b40-159">The second example gets specifically the automatic replies settings of the signed-in user's mailbox.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_2"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailboxSettings/automaticRepliesSetting
```
##### <a name="response-2"></a><span data-ttu-id="32b40-160">応答 2</span><span class="sxs-lookup"><span data-stu-id="32b40-160">Response 2</span></span>
<span data-ttu-id="32b40-p109">この応答には自動とうとう設定のみが含まれます。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="32b40-p109">The response includes only the automatic replies settings. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.automaticRepliesSetting"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/mailboxSettings/automaticRepliesSetting",
    "status": "alwaysEnabled",
    "externalAudience": "None",
    "scheduledStartDateTime": {
        "dateTime": "2016-03-19T02:00:00.0000000",
        "timeZone": "UTC"
    },
    "scheduledEndDateTime": {
        "dateTime": "2016-03-20T02:00:00.0000000",
        "timeZone": "UTC"
    },
    "internalReplyMessage": "<html>\n<body>\n<p>I'm at our company's worldwide reunion and will respond to your message as soon as I return.<br>\n</p></body>\n</html>\n",
    "externalReplyMessage": "<html>\n<body>\n<p>I'm at the Contoso worldwide reunion and will respond to your message as soon as I return.<br>\n</p></body>\n</html>\n"
}
```


##### <a name="request-3"></a><span data-ttu-id="32b40-164">要求 3</span><span class="sxs-lookup"><span data-stu-id="32b40-164">Request 3</span></span>
<span data-ttu-id="32b40-165">3 番目の例では、サインインしているユーザーのメールボックスの自動応答の設定を具体的に指定して取得します。</span><span class="sxs-lookup"><span data-stu-id="32b40-165">The third example gets specifically the working hour settings of the signed-in user's mailbox.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_mailboxsettings_3"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailboxSettings/workingHours
```
##### <a name="response-3"></a><span data-ttu-id="32b40-166">応答 3</span><span class="sxs-lookup"><span data-stu-id="32b40-166">Response 3</span></span>
<span data-ttu-id="32b40-167">この応答には、自動応答の設定のみが含まれます。</span><span class="sxs-lookup"><span data-stu-id="32b40-167">The response includes only the working hours settings.</span></span> <span data-ttu-id="32b40-168">ユーザーの就業時間には、[カスタム タイム ゾーン](../resources/customtimezone.md)が適用されていることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="32b40-168">Notice that the user's work hours are in a [custom time zone](../resources/customtimezone.md).</span></span> <span data-ttu-id="32b40-169">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="32b40-169">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="32b40-170">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="32b40-170">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_mailboxsettings_3",
  "truncated": true,
  "@odata.type": "microsoft.graph.workingHours"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('94447c6e-ea4c-494c-a9ed-d905e366c5cb')/mailboxSettings/workingHours",
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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get mailbox settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->