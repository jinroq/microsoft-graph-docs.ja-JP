---
title: 'ユーザー: getMailTips ヒント'
description: サインインしているユーザーが使用できる1人以上の受信者のメールヒントを取得します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5ba3c606f9e54a27f46586ecc13b008a761a7d85
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637333"
---
# <a name="user-getmailtips"></a><span data-ttu-id="c54d3-103">ユーザー: getMailTips ヒント</span><span class="sxs-lookup"><span data-stu-id="c54d3-103">user: getMailTips</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c54d3-104">サインインしている[ユーザー](../resources/user.md)が使用できる1人以上の受信者のメールヒントを取得します。</span><span class="sxs-lookup"><span data-stu-id="c54d3-104">Get the MailTips of one or more recipients as available to the signed-in [user](../resources/user.md).</span></span>

<span data-ttu-id="c54d3-105">`getMailTips`アクションを`POST`呼び出すことによって、複数の受信者に対して特定の種類のメールヒントが一度に返されるように要求することができることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="c54d3-105">Note that by making a `POST` call to the `getMailTips` action, you can request specific types of MailTips to be returned for more than one recipient at one time.</span></span> <span data-ttu-id="c54d3-106">要求されたメールヒントが[メールヒント](../resources/mailtips.md)コレクションに返されます。</span><span class="sxs-lookup"><span data-stu-id="c54d3-106">The requested MailTips are returned in a [mailTips](../resources/mailtips.md) collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="c54d3-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c54d3-107">Permissions</span></span>
<span data-ttu-id="c54d3-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c54d3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c54d3-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c54d3-110">Permission type</span></span>      | <span data-ttu-id="c54d3-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c54d3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c54d3-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c54d3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c54d3-113">メール。読み取り、共有</span><span class="sxs-lookup"><span data-stu-id="c54d3-113">Mail.Read, Mail.Read.Shared</span></span>    |
|<span data-ttu-id="c54d3-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c54d3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c54d3-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c54d3-115">Mail.Read</span></span>    |
|<span data-ttu-id="c54d3-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c54d3-116">Application</span></span> | <span data-ttu-id="c54d3-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c54d3-117">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="c54d3-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c54d3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMailTips
POST /users/{id|userPrincipalName}/getMailTips
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c54d3-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c54d3-119">Optional query parameters</span></span>
<span data-ttu-id="c54d3-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c54d3-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c54d3-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c54d3-121">Request headers</span></span>
| <span data-ttu-id="c54d3-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c54d3-122">Header</span></span>       | <span data-ttu-id="c54d3-123">値</span><span class="sxs-lookup"><span data-stu-id="c54d3-123">Value</span></span>|
|:-----------  |:------|
| <span data-ttu-id="c54d3-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c54d3-124">Authorization</span></span> | <span data-ttu-id="c54d3-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c54d3-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c54d3-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c54d3-127">Content-Type</span></span>  | <span data-ttu-id="c54d3-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c54d3-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c54d3-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="c54d3-129">Request body</span></span>
<span data-ttu-id="c54d3-130">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="c54d3-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c54d3-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c54d3-131">Property</span></span>     | <span data-ttu-id="c54d3-132">型</span><span class="sxs-lookup"><span data-stu-id="c54d3-132">Type</span></span>   |<span data-ttu-id="c54d3-133">説明</span><span class="sxs-lookup"><span data-stu-id="c54d3-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c54d3-134">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="c54d3-134">EmailAddresses</span></span>|<span data-ttu-id="c54d3-135">String collection</span><span class="sxs-lookup"><span data-stu-id="c54d3-135">String collection</span></span>|<span data-ttu-id="c54d3-136">メール ヒントを取得する受信者の SMTP アドレスのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="c54d3-136">A collection of SMTP addresses of recipients to get MailTips for.</span></span>|
|<span data-ttu-id="c54d3-137">MailTipsOptions</span><span class="sxs-lookup"><span data-stu-id="c54d3-137">MailTipsOptions</span></span>|<span data-ttu-id="c54d3-138">String</span><span class="sxs-lookup"><span data-stu-id="c54d3-138">String</span></span>|<span data-ttu-id="c54d3-139">要求されたメールヒントを表すフラグの列挙。</span><span class="sxs-lookup"><span data-stu-id="c54d3-139">A enumeration of flags that represents the requested mailtips.</span></span> <span data-ttu-id="c54d3-140">可能な値は`automaticReplies`、 `customMailTip`、 `deliveryRestriction` `externalMemberCount` `mailboxFullStatus` `maxMessageSize` `moderationStatus` `recipientScope`、、、、、、、、および`totalMemberCount` `recipientSuggestions`です。</span><span class="sxs-lookup"><span data-stu-id="c54d3-140">Possible values are: `automaticReplies`, `customMailTip`, `deliveryRestriction`, `externalMemberCount`, `mailboxFullStatus`, `maxMessageSize`, `moderationStatus`, `recipientScope`, `recipientSuggestions`, and `totalMemberCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="c54d3-141">応答</span><span class="sxs-lookup"><span data-stu-id="c54d3-141">Response</span></span>

<span data-ttu-id="c54d3-142">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[メールヒント](../resources/mailtips.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="c54d3-142">If successful, this method returns a `200 OK` response code and a collection of [mailTips](../resources/mailtips.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c54d3-143">例</span><span class="sxs-lookup"><span data-stu-id="c54d3-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c54d3-144">要求</span><span class="sxs-lookup"><span data-stu-id="c54d3-144">Request</span></span>
<span data-ttu-id="c54d3-145">次の例では、指定された受信者のメールヒントを取得します。すべての自動応答の設定と、メールボックスの状態が [完全] になっています。</span><span class="sxs-lookup"><span data-stu-id="c54d3-145">The following example gets MailTips for the specified recipients, for any automatic reply settings and the mailbox full status.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_getmailtips"
}-->
```http
POST https://graph.microsoft.com/beta/me/getMailTips
Content-Type: application/json

{
    "EmailAddresses": [
        "danas@contoso.onmicrosoft.com", 
        "fannyd@contoso.onmicrosoft.com"
    ],
    "MailTipsOptions": "automaticReplies, mailboxFullStatus"
}
```

##### <a name="response"></a><span data-ttu-id="c54d3-146">応答</span><span class="sxs-lookup"><span data-stu-id="c54d3-146">Response</span></span>
<span data-ttu-id="c54d3-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c54d3-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.mailTips)",
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="c54d3-150">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="c54d3-150">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c54d3-151">Visual</span><span class="sxs-lookup"><span data-stu-id="c54d3-151">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_getmailtips-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c54d3-152">Java</span><span class="sxs-lookup"><span data-stu-id="c54d3-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_getmailtips-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: getMailTips",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-getmailtips.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-getmailtips.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
