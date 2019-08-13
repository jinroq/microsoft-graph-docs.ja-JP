---
title: ユーザーのメールボックスの設定を取得する
description: 'ユーザーの mailboxSettings を取得します。 これには、自動応答 (自動的にユーザーに通知) の設定が含まれます。 '
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 25285820bebbd2a7c22f88bc6347c073f17fda87
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36362450"
---
# <a name="get-user-mailbox-settings"></a><span data-ttu-id="75f39-104">ユーザーのメールボックスの設定を取得する</span><span class="sxs-lookup"><span data-stu-id="75f39-104">Get user mailbox settings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75f39-105">ユーザーの [mailboxSettings](../resources/mailboxsettings.md) を取得します。</span><span class="sxs-lookup"><span data-stu-id="75f39-105">Get the user's [mailboxSettings](../resources/mailboxsettings.md).</span></span> <span data-ttu-id="75f39-106">これには、自動応答の設定 (電子メールの受信時にユーザーに自動的に通知される)、ロケール (言語と国/地域)、タイムゾーン、および稼働時間の設定が含まれます。</span><span class="sxs-lookup"><span data-stu-id="75f39-106">This includes settings for automatic replies (notify people automatically upon receipt of their email), locale (language and country/region), time zone, and working hours.</span></span>

<span data-ttu-id="75f39-107">すべてのメールボックス設定を表示することも、特定の設定を取得することもできます。</span><span class="sxs-lookup"><span data-stu-id="75f39-107">You can view all mailbox settings, or, get specific settings.</span></span>

<span data-ttu-id="75f39-108">タイム ゾーンは、ユーザーが自分のメールボックスに設定できる優先設定のうちの 1 つです。</span><span class="sxs-lookup"><span data-stu-id="75f39-108">Time zone is one of the preferred settings a user can set up for the user's mailbox.</span></span> <span data-ttu-id="75f39-109">ユーザーは、ユーザーのメールボックスサーバーに対して管理者が設定した、サポートされている[タイムゾーン](outlookuser-supportedtimezones.md)からそれを選択します。</span><span class="sxs-lookup"><span data-stu-id="75f39-109">The user chooses it from the [supported time zones](outlookuser-supportedtimezones.md) that an administrator has set up for the user's mailbox server.</span></span> <span data-ttu-id="75f39-110">管理者は、Windows タイムゾーン形式または[インターネット割り当て番号オーソリティ (IANA) タイムゾーン](https://www.iana.org/time-zones)(olson タイムゾーンとも呼ばれる) 形式でタイムゾーンを設定します。</span><span class="sxs-lookup"><span data-stu-id="75f39-110">The administrator sets up time zones in the Windows time zone format or  [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="75f39-111">既定値は Windows 形式です。</span><span class="sxs-lookup"><span data-stu-id="75f39-111">The Windows format is the default.</span></span> 

<span data-ttu-id="75f39-112">ユーザーの優先タイム ゾーンを取得するとき、そのタイム ゾーンは設定された形式で返されます。</span><span class="sxs-lookup"><span data-stu-id="75f39-112">When you get a user's preferred time zone, the time zone is returned in the format that it was set up.</span></span> <span data-ttu-id="75f39-113">タイム ゾーンを特定の形式 (Windows または IANA) にする場合は、最初に[メールボックス設定としてその形式の優先タイム ゾーンを更新](user-update-mailboxsettings.md)します。</span><span class="sxs-lookup"><span data-stu-id="75f39-113">If you want that time zone to be in a specific format (Windows or IANA), you can first [update the preferred time zone in that format as a mailbox setting](user-update-mailboxsettings.md).</span></span> <span data-ttu-id="75f39-114">その後は、その形式でタイム ゾーンを取得できるようになります。</span><span class="sxs-lookup"><span data-stu-id="75f39-114">Subsequently you will be able to get the time zone in that format.</span></span> <span data-ttu-id="75f39-115">または、アプリ内で形式変換を個別に管理することもできます。</span><span class="sxs-lookup"><span data-stu-id="75f39-115">Alternatively, you can manage the format conversion separately in your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="75f39-116">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="75f39-116">Permissions</span></span>
<span data-ttu-id="75f39-p105">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="75f39-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75f39-119">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="75f39-119">Permission type</span></span>      | <span data-ttu-id="75f39-120">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="75f39-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="75f39-121">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="75f39-121">Delegated (work or school account)</span></span> | <span data-ttu-id="75f39-122">MailboxSettings.Read、MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="75f39-122">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="75f39-123">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="75f39-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75f39-124">MailboxSettings.Read、MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="75f39-124">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="75f39-125">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="75f39-125">Application</span></span> | <span data-ttu-id="75f39-126">MailboxSettings.Read、MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="75f39-126">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="75f39-127">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="75f39-127">HTTP request</span></span>
<span data-ttu-id="75f39-128">ユーザーのすべてのメールボックス設定を取得するには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="75f39-128">To get all the mailbox settings for a user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings
GET /users/{id|userPrincipalName}/mailboxSettings
```

<span data-ttu-id="75f39-129">特定の設定を取得するには、自動応答の設定、ロケール、タイムゾーン、または稼働時間のみを取得します。</span><span class="sxs-lookup"><span data-stu-id="75f39-129">To get specific settings - only the automatic replies settings, locale, time zone, or working hours:</span></span>
<!-- { "blockType": "ignored" } -->
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
## <a name="optional-query-parameters"></a><span data-ttu-id="75f39-130">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="75f39-130">Optional query parameters</span></span>
<span data-ttu-id="75f39-131">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="75f39-131">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="75f39-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="75f39-132">Request headers</span></span>
| <span data-ttu-id="75f39-133">名前</span><span class="sxs-lookup"><span data-stu-id="75f39-133">Name</span></span>       | <span data-ttu-id="75f39-134">型</span><span class="sxs-lookup"><span data-stu-id="75f39-134">Type</span></span> | <span data-ttu-id="75f39-135">説明</span><span class="sxs-lookup"><span data-stu-id="75f39-135">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="75f39-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="75f39-136">Authorization</span></span>  | <span data-ttu-id="75f39-137">string</span><span class="sxs-lookup"><span data-stu-id="75f39-137">string</span></span>  | <span data-ttu-id="75f39-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="75f39-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="75f39-140">要求本文</span><span class="sxs-lookup"><span data-stu-id="75f39-140">Request body</span></span>
<span data-ttu-id="75f39-141">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="75f39-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="75f39-142">応答</span><span class="sxs-lookup"><span data-stu-id="75f39-142">Response</span></span>

<span data-ttu-id="75f39-143">成功した場合、このメソッドは `200 OK` 応答コードと、次に示す要求されたオブジェクトのいずれかを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="75f39-143">If successful, this method returns a `200 OK` response code and one of the following requested objects in the response body:</span></span>

- <span data-ttu-id="75f39-144">[mailboxSettings](../resources/mailboxsettings.md) オブジェクト</span><span class="sxs-lookup"><span data-stu-id="75f39-144">[mailboxSettings](../resources/mailboxsettings.md) object</span></span>
- <span data-ttu-id="75f39-145">[automaticRepliesSetting](../resources/automaticrepliessetting.md) オブジェクト</span><span class="sxs-lookup"><span data-stu-id="75f39-145">[automaticRepliesSetting](../resources/automaticrepliessetting.md) object</span></span>
- <span data-ttu-id="75f39-146">[localeInfo](../resources/localeinfo.md) オブジェクト</span><span class="sxs-lookup"><span data-stu-id="75f39-146">[localeInfo](../resources/localeinfo.md) object</span></span>
- <span data-ttu-id="75f39-147">string (**timeZone** の場合)</span><span class="sxs-lookup"><span data-stu-id="75f39-147">string (for **timeZone**)</span></span>
- [<span data-ttu-id="75f39-148">workingHours</span><span class="sxs-lookup"><span data-stu-id="75f39-148">workingHours</span></span>](../resources/workinghours.md)

## <a name="example"></a><span data-ttu-id="75f39-149">例</span><span class="sxs-lookup"><span data-stu-id="75f39-149">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="75f39-150">要求 1</span><span class="sxs-lookup"><span data-stu-id="75f39-150">Request 1</span></span>
<span data-ttu-id="75f39-151">最初の例では、サインインしているユーザーのメールボックスのすべてのメールボックス設定を取得します。取得される設定には、自動応答、ロケール (言語と国/地域)、タイム ゾーン、就業時間の設定が含まれます。</span><span class="sxs-lookup"><span data-stu-id="75f39-151">The first example gets all the mailbox settings of the signed-in user's mailbox, which include settings for time zone, automatic replies, locale (language and country/region), and working hours.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="75f39-152">プロトコル</span><span class="sxs-lookup"><span data-stu-id="75f39-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_1"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailboxSettings
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="75f39-153">C#</span><span class="sxs-lookup"><span data-stu-id="75f39-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailboxsettings-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="75f39-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="75f39-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailboxsettings-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="75f39-155">目的-C</span><span class="sxs-lookup"><span data-stu-id="75f39-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailboxsettings-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="75f39-156">Java</span><span class="sxs-lookup"><span data-stu-id="75f39-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailboxsettings-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-1"></a><span data-ttu-id="75f39-157">応答 1</span><span class="sxs-lookup"><span data-stu-id="75f39-157">Response 1</span></span>
<span data-ttu-id="75f39-158">応答には、サインインしているユーザーのすべてのメールボックス設定が含まれます。</span><span class="sxs-lookup"><span data-stu-id="75f39-158">The response includes all the mailbox settings of the signed-in user.</span></span> <span data-ttu-id="75f39-159">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="75f39-159">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="75f39-160">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="75f39-160">All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request-2"></a><span data-ttu-id="75f39-161">要求 2</span><span class="sxs-lookup"><span data-stu-id="75f39-161">Request 2</span></span>
<span data-ttu-id="75f39-162">2 番目の例では、具体的にサインインしているユーザーのメールボックスの自動応答設定を取得します。</span><span class="sxs-lookup"><span data-stu-id="75f39-162">The second example gets specifically the automatic replies settings of the signed-in user's mailbox.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="75f39-163">プロトコル</span><span class="sxs-lookup"><span data-stu-id="75f39-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_2"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailboxSettings/automaticRepliesSetting
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="75f39-164">C#</span><span class="sxs-lookup"><span data-stu-id="75f39-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailboxsettings-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="75f39-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="75f39-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailboxsettings-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="75f39-166">目的-C</span><span class="sxs-lookup"><span data-stu-id="75f39-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailboxsettings-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="75f39-167">Java</span><span class="sxs-lookup"><span data-stu-id="75f39-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailboxsettings-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-2"></a><span data-ttu-id="75f39-168">応答 2</span><span class="sxs-lookup"><span data-stu-id="75f39-168">Response 2</span></span>
<span data-ttu-id="75f39-p108">この応答には自動とうとう設定のみが含まれます。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="75f39-p108">The response includes only the automatic replies settings. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


##### <a name="request-3"></a><span data-ttu-id="75f39-172">要求 3</span><span class="sxs-lookup"><span data-stu-id="75f39-172">Request 3</span></span>
<span data-ttu-id="75f39-173">3 番目の例では、サインインしているユーザーのメールボックスの自動応答の設定を具体的に指定して取得します。</span><span class="sxs-lookup"><span data-stu-id="75f39-173">The third example gets specifically the working hour settings of the signed-in user's mailbox.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_mailboxsettings_3"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailboxSettings/workingHours
```
##### <a name="response-3"></a><span data-ttu-id="75f39-174">応答 3</span><span class="sxs-lookup"><span data-stu-id="75f39-174">Response 3</span></span>
<span data-ttu-id="75f39-175">この応答には、自動応答の設定のみが含まれます。</span><span class="sxs-lookup"><span data-stu-id="75f39-175">The response includes only the working hours settings.</span></span> <span data-ttu-id="75f39-176">ユーザーの就業時間には、[カスタム タイム ゾーン](../resources/customtimezone.md)が適用されていることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="75f39-176">Notice that the user's work hours are in a [custom time zone](../resources/customtimezone.md).</span></span> <span data-ttu-id="75f39-177">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="75f39-177">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="75f39-178">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="75f39-178">All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get mailbox settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
