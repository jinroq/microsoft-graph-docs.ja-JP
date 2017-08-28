# <a name="update-user-mailbox-settings"></a><span data-ttu-id="bc526-101">ユーザーのメールボックスの設定を更新する</span><span class="sxs-lookup"><span data-stu-id="bc526-101">Update user mailbox settings</span></span>

<span data-ttu-id="bc526-p101">ユーザーのメールボックスの 1 つ以上の設定を更新します。これには、自動応答 (ユーザーが電子メールを受信したときに自動的にユーザーに通知)、ロケール、またはタイム ゾーンの設定が含まれます。</span><span class="sxs-lookup"><span data-stu-id="bc526-p101">Update one or more settings for the user's mailbox. This includes settings for automatic replies (notify people automatically upon receipt of their email), locale, or time zone.</span></span>

<span data-ttu-id="bc526-104">これらの設定の 1 つ以上を、[mailboxSettings](../resources/mailboxsettings.md)の一部として有効化、構成、または無効化できます。</span><span class="sxs-lookup"><span data-stu-id="bc526-104">You can enable, configure, or disable one or more of these settings as part of [mailboxSettings](../resources/mailboxsettings.md).</span></span>

<span data-ttu-id="bc526-105">**注** メールボックス設定は作成または削除できません。</span><span class="sxs-lookup"><span data-stu-id="bc526-105">**Note** You cannot create or delete any mailbox settings.</span></span>

## <a name="permissions"></a><span data-ttu-id="bc526-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bc526-106">Permissions</span></span>
<span data-ttu-id="bc526-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bc526-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="bc526-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bc526-109">Permission type</span></span>      | <span data-ttu-id="bc526-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bc526-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc526-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bc526-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bc526-112">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc526-112">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="bc526-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bc526-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc526-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc526-114">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="bc526-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bc526-115">Application</span></span> | <span data-ttu-id="bc526-116">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc526-116">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc526-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bc526-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailboxSettings
PATCH /users/{id|userPrincipalName}/mailboxSettings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bc526-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="bc526-118">Optional query parameters</span></span>
<span data-ttu-id="bc526-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="bc526-119">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="bc526-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bc526-120">Request headers</span></span>
| <span data-ttu-id="bc526-121">名前</span><span class="sxs-lookup"><span data-stu-id="bc526-121">Name</span></span>       | <span data-ttu-id="bc526-122">型</span><span class="sxs-lookup"><span data-stu-id="bc526-122">Type</span></span> | <span data-ttu-id="bc526-123">説明</span><span class="sxs-lookup"><span data-stu-id="bc526-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="bc526-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc526-124">Authorization</span></span>  | <span data-ttu-id="bc526-125">string</span><span class="sxs-lookup"><span data-stu-id="bc526-125">string</span></span>  | <span data-ttu-id="bc526-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="bc526-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bc526-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="bc526-128">Request body</span></span>
<span data-ttu-id="bc526-p104">要求本文で、更新する関連プロパティの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。書き込み可能または更新可能なプロパティを次に示します。</span><span class="sxs-lookup"><span data-stu-id="bc526-p104">In the request body, supply the values for the relevant properties that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. The following are the writable/updatable properties:</span></span>

| <span data-ttu-id="bc526-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bc526-133">Property</span></span>     | <span data-ttu-id="bc526-134">型</span><span class="sxs-lookup"><span data-stu-id="bc526-134">Type</span></span>   |<span data-ttu-id="bc526-135">説明</span><span class="sxs-lookup"><span data-stu-id="bc526-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bc526-136">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="bc526-136">automaticRepliesSetting</span></span>|[<span data-ttu-id="bc526-137">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="bc526-137">automaticRepliesSetting</span></span>](../resources/automaticrepliessetting.md)|<span data-ttu-id="bc526-138">サインイン ユーザーからのメッセージを使用して、着信メールの送信者に自動的に通知する構成設定。</span><span class="sxs-lookup"><span data-stu-id="bc526-138">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span>|
|<span data-ttu-id="bc526-139">language</span><span class="sxs-lookup"><span data-stu-id="bc526-139">language</span></span>|[<span data-ttu-id="bc526-140">localeInfo</span><span class="sxs-lookup"><span data-stu-id="bc526-140">localeInfo</span></span>](../resources/localeinfo.md)|<span data-ttu-id="bc526-141">優先言語および国/地域を含むユーザーのロケール情報。</span><span class="sxs-lookup"><span data-stu-id="bc526-141">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="bc526-142">timeZone</span><span class="sxs-lookup"><span data-stu-id="bc526-142">timeZone</span></span>|<span data-ttu-id="bc526-143">string</span><span class="sxs-lookup"><span data-stu-id="bc526-143">string</span></span>|<span data-ttu-id="bc526-144">ユーザーのメールボックスの既定のタイム ゾーン。</span><span class="sxs-lookup"><span data-stu-id="bc526-144">The default time zone for the user's mailbox.</span></span>|

## <a name="response"></a><span data-ttu-id="bc526-145">応答</span><span class="sxs-lookup"><span data-stu-id="bc526-145">Response</span></span>

<span data-ttu-id="bc526-146">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [mailboxSettings](../resources/mailboxSettings.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="bc526-146">If successful, this method returns a `200 OK` response code and [mailboxSettings](../resources/mailboxSettings.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bc526-147">例</span><span class="sxs-lookup"><span data-stu-id="bc526-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bc526-148">要求</span><span class="sxs-lookup"><span data-stu-id="bc526-148">Request</span></span>
<span data-ttu-id="bc526-149">次の例では、**automaticRepliesSetting** プロパティの **status**、**scheduledStartDateTime** および **scheduledEndDateTime** プロパティを設定することにより、日付の範囲の自動応答を有効にします。</span><span class="sxs-lookup"><span data-stu-id="bc526-149">The following example enables automatic replies for a date range, by setting the following properties of the **automaticRepliesSetting** property: **status**, **scheduledStartDateTime** and **scheduledEndDateTime**.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_mailboxsettings"
}-->
```http
PATCH https://graph.microsoft.com/api/v1.0/me/mailboxSettings
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/api/v1.0/$metadata#Me/mailboxSettings",
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
##### <a name="response"></a><span data-ttu-id="bc526-150">応答</span><span class="sxs-lookup"><span data-stu-id="bc526-150">Response</span></span>
<span data-ttu-id="bc526-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bc526-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxSettings"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/api/v1.0/$metadata#Me/mailboxSettings",
    "automaticRepliesSetting": {
        "status": "scheduled",
        "externalAudience": "none",
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
    },
    "timeZone":"UTC",
    "language":{
      "locale":"en-US",
      "displayName":"English (United States)"
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