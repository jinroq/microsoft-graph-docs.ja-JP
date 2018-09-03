# <a name="user-getmailtips"></a><span data-ttu-id="9a9e2-101">ユーザー: getMailTips</span><span class="sxs-lookup"><span data-stu-id="9a9e2-101">user: getMailTips</span></span>

<span data-ttu-id="9a9e2-102">サインイン中の[ユーザー](../resources/user.md)が利用できる、1 人以上の受信者に対するメール ヒントを取得します。</span><span class="sxs-lookup"><span data-stu-id="9a9e2-102">Return the MailTips of one or more recipients as available to the signed-in user.</span></span>

<span data-ttu-id="9a9e2-103">`getMailTips` アクションに対して`POST` 呼び出しを行うことで、特定の種類のメール ヒントを一度に複数の受信者に返す要求ができることにご注意ください。</span><span class="sxs-lookup"><span data-stu-id="9a9e2-103">Note that by making a `POST` call to the `getMailTips` action, you can request specific types of MailTips to be returned for more than one recipient at one time.</span></span> <span data-ttu-id="9a9e2-104">要求されたメール ヒントは、[mailTips](../resources/mailtips.md) コレクションに返されます。</span><span class="sxs-lookup"><span data-stu-id="9a9e2-104">The requested MailTips are returned in a [mailTips](../resources/mailtips.md) collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a9e2-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9a9e2-105">Permissions</span></span>
<span data-ttu-id="9a9e2-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9a9e2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9a9e2-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9a9e2-108">Permission type</span></span>      | <span data-ttu-id="9a9e2-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9a9e2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a9e2-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9a9e2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9a9e2-111">Mail.Read、Mail.Read.Shared</span><span class="sxs-lookup"><span data-stu-id="9a9e2-111">Mail.Read, Mail.Read.Shared</span></span>    |
|<span data-ttu-id="9a9e2-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9a9e2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a9e2-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="9a9e2-113">Mail.Read</span></span>    |
|<span data-ttu-id="9a9e2-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9a9e2-114">Application</span></span> | <span data-ttu-id="9a9e2-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="9a9e2-115">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a9e2-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9a9e2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMailTips
POST /users/{id|userPrincipalName}/getMailTips
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9a9e2-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="9a9e2-117">Optional query parameters</span></span>
<span data-ttu-id="9a9e2-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="9a9e2-118">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9a9e2-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9a9e2-119">Request headers</span></span>
| <span data-ttu-id="9a9e2-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9a9e2-120">Header</span></span>       | <span data-ttu-id="9a9e2-121">値</span><span class="sxs-lookup"><span data-stu-id="9a9e2-121">Value</span></span>|
|:-----------  |:------|
| <span data-ttu-id="9a9e2-122">承認</span><span class="sxs-lookup"><span data-stu-id="9a9e2-122">Authorization</span></span> | <span data-ttu-id="9a9e2-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9a9e2-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9a9e2-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9a9e2-125">Content-Type</span></span>  | <span data-ttu-id="9a9e2-126">アプリケーション /json</span><span class="sxs-lookup"><span data-stu-id="9a9e2-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9a9e2-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="9a9e2-127">Request body</span></span>
<span data-ttu-id="9a9e2-128">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="9a9e2-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9a9e2-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9a9e2-129">Property</span></span>     | <span data-ttu-id="9a9e2-130">タイプ</span><span class="sxs-lookup"><span data-stu-id="9a9e2-130">Type</span></span>   |<span data-ttu-id="9a9e2-131">説明</span><span class="sxs-lookup"><span data-stu-id="9a9e2-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9a9e2-132">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="9a9e2-132">EmailAddresses</span></span>|<span data-ttu-id="9a9e2-133">String コレクション</span><span class="sxs-lookup"><span data-stu-id="9a9e2-133">String collection</span></span>|<span data-ttu-id="9a9e2-134">メール ヒントを取得する受信者の SMTP アドレスのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="9a9e2-134">A collection of SMTP addresses of recipients to get MailTips for.</span></span>|
|<span data-ttu-id="9a9e2-135">MailTipsOptions</span><span class="sxs-lookup"><span data-stu-id="9a9e2-135">MailTipsOptions</span></span>|<span data-ttu-id="9a9e2-136">String</span><span class="sxs-lookup"><span data-stu-id="9a9e2-136">String</span></span>|<span data-ttu-id="9a9e2-137">要求されたメールヒントを表すフラグの列挙型。</span><span class="sxs-lookup"><span data-stu-id="9a9e2-137">A enumeration of flags that represents the requested mailtips.</span></span> <span data-ttu-id="9a9e2-138">使用可能な値は、 `automaticReplies`、 `customMailTip`、 `deliveryRestriction`、 `externalMemberCount`、 `mailboxFullStatus`、 `maxMessageSize`、 `moderationStatus`、 `recipientScope`、 `recipientSuggestions`、 `totalMemberCount` です。</span><span class="sxs-lookup"><span data-stu-id="9a9e2-138">Possible values are: `automaticReplies`, `customMailTip`, `deliveryRestriction`, `externalMemberCount`,`mailboxFullStatus`, `maxMessageSize`, `moderationStatus`, `recipientScope`, `recipientSuggestions`, `totalMemberCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="9a9e2-139">応答</span><span class="sxs-lookup"><span data-stu-id="9a9e2-139">Response</span></span>

<span data-ttu-id="9a9e2-140">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [mailTips](../resources/mailtips.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="9a9e2-140">If successful, this method returns a `200 OK` response code and a collection of [macOSCompliancePolicy](../resources/mailtips.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9a9e2-141">例</span><span class="sxs-lookup"><span data-stu-id="9a9e2-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9a9e2-142">要求</span><span class="sxs-lookup"><span data-stu-id="9a9e2-142">Request</span></span>
<span data-ttu-id="9a9e2-143">次の使用例では、指定した受信者に対して、自動応答設定やメールボックスのフル状態を示すメール ヒントを取得します。</span><span class="sxs-lookup"><span data-stu-id="9a9e2-143">The following example gets MailTips for the specified recipients, for any automatic reply settings and mailbox full status.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_getmailtips"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/getMailTips
Content-Type: application/json

{
    "EmailAddresses": [
        "danas@contoso.onmicrosoft.com", 
        "fannyd@contoso.onmicrosoft.com"
    ],
    "MailTipsOptions": "automaticReplies, mailboxFullStatus"
}
```

##### <a name="response"></a><span data-ttu-id="9a9e2-144">応答</span><span class="sxs-lookup"><span data-stu-id="9a9e2-144">Response</span></span>
<span data-ttu-id="9a9e2-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9a9e2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailTips",
  isCollection: true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.mailTips)",
    "value":[
        {
            "emailAddress":{
                "name":"",
                "address":"danas@contoso.onmicrosoft.com"
            },
            "automaticReplies":{
                "message":"<style type=\"text/css\" style=\"\">\r\n<!--\r\np\r\n\t{margin-top:0;\r\n\tmargin-bottom:0}\r\n-->\r\n</style>\r\n<div dir=\"ltr\">\r\n<div id=\"x_divtagdefaultwrapper\" style=\"font-size:12pt; color:#000000; background-color:#FFFFFF; font-family:Calibri,Arial,Helvetica,sans-serif\">\r\n<p>Hi, I am on vacation right now. I'll get back to you after I return.<br>\r\n</p>\r\n</div>\r\n</div>",
                "messageLanguage":{
                    "locale":"en-US",
                    "displayName":"English (United States)"
                },
                "scheduledStartTime": {
                    "dateTime": "2018-08-07T02:00:00.0000000",
                    "timeZone": "UTC"
                },
                "scheduledEndTime": {
                    "dateTime": "2018-08-09T02:00:00.0000000",
                    "timeZone": "UTC"
                }
            },
            "mailboxFull":false
        },
        {
            "emailAddress":{
                "name":"",
                "address":"fannyd@contoso.onmicrosoft.com"
            },
            "automaticReplies":{
                "message":""
            },
            "mailboxFull":false
        }
    ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: getMailTips",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
