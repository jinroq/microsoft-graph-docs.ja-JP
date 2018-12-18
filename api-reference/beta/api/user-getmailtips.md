---
title: 'ユーザー: getMailTips'
description: サインイン中のユーザーに利用可能な 1 つまたは複数の受信者のメール ヒントを取得します。
author: dkershaw10
ms.openlocfilehash: 039d86c728c2394153ebe1a5aebba1243d40d726
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304047"
---
# <a name="user-getmailtips"></a><span data-ttu-id="cf005-103">ユーザー: getMailTips</span><span class="sxs-lookup"><span data-stu-id="cf005-103">user: getMailTips</span></span>

> <span data-ttu-id="cf005-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cf005-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cf005-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cf005-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cf005-106">サインインしている[ユーザー](../resources/user.md)に利用可能な 1 つまたは複数の受信者のメール ヒントを取得します。</span><span class="sxs-lookup"><span data-stu-id="cf005-106">Get the MailTips of one or more recipients as available to the signed-in [user](../resources/user.md).</span></span>

<span data-ttu-id="cf005-107">注意することにより、`POST`を呼び出して、`getMailTips`アクション、同時に複数の受信者に返されるメール ヒントの特定の種類を要求することができます。</span><span class="sxs-lookup"><span data-stu-id="cf005-107">Note that by making a `POST` call to the `getMailTips` action, you can request specific types of MailTips to be returned for more than one recipient at one time.</span></span> <span data-ttu-id="cf005-108">[メール ヒント](../resources/mailtips.md)のコレクションでは、要求されたメール ヒントが返されます。</span><span class="sxs-lookup"><span data-stu-id="cf005-108">The requested MailTips are returned in a [mailTips](../resources/mailtips.md) collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="cf005-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cf005-109">Permissions</span></span>
<span data-ttu-id="cf005-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cf005-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf005-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cf005-112">Permission type</span></span>      | <span data-ttu-id="cf005-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cf005-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cf005-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cf005-114">Delegated (work or school account)</span></span> | <span data-ttu-id="cf005-115">Mail.Read、Mail.Read.Shared</span><span class="sxs-lookup"><span data-stu-id="cf005-115">Mail.Read, Mail.Read.Shared</span></span>    |
|<span data-ttu-id="cf005-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cf005-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf005-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="cf005-117">Mail.Read</span></span>    |
|<span data-ttu-id="cf005-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cf005-118">Application</span></span> | <span data-ttu-id="cf005-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="cf005-119">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="cf005-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cf005-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMailTips
POST /users/{id|userPrincipalName}/getMailTips
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cf005-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="cf005-121">Optional query parameters</span></span>
<span data-ttu-id="cf005-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="cf005-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="cf005-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cf005-123">Request headers</span></span>
| <span data-ttu-id="cf005-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cf005-124">Header</span></span>       | <span data-ttu-id="cf005-125">値</span><span class="sxs-lookup"><span data-stu-id="cf005-125">Value</span></span>|
|:-----------  |:------|
| <span data-ttu-id="cf005-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf005-126">Authorization</span></span> | <span data-ttu-id="cf005-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="cf005-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cf005-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cf005-129">Content-Type</span></span>  | <span data-ttu-id="cf005-130">application/json</span><span class="sxs-lookup"><span data-stu-id="cf005-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cf005-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="cf005-131">Request body</span></span>
<span data-ttu-id="cf005-132">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="cf005-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cf005-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cf005-133">Property</span></span>     | <span data-ttu-id="cf005-134">種類</span><span class="sxs-lookup"><span data-stu-id="cf005-134">Type</span></span>   |<span data-ttu-id="cf005-135">説明</span><span class="sxs-lookup"><span data-stu-id="cf005-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cf005-136">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="cf005-136">EmailAddresses</span></span>|<span data-ttu-id="cf005-137">String コレクション</span><span class="sxs-lookup"><span data-stu-id="cf005-137">String collection</span></span>|<span data-ttu-id="cf005-138">メール ヒントを取得する受信者の SMTP アドレスのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="cf005-138">A collection of SMTP addresses of recipients to get MailTips for.</span></span>|
|<span data-ttu-id="cf005-139">MailTipsOptions</span><span class="sxs-lookup"><span data-stu-id="cf005-139">MailTipsOptions</span></span>|<span data-ttu-id="cf005-140">String</span><span class="sxs-lookup"><span data-stu-id="cf005-140">String</span></span>|<span data-ttu-id="cf005-141">要求されたメールヒントを表すフラグの列挙型。</span><span class="sxs-lookup"><span data-stu-id="cf005-141">A enumeration of flags that represents the requested mailtips.</span></span> <span data-ttu-id="cf005-142">使用可能な値: `automaticReplies`、 `customMailTip`、 `deliveryRestriction`、 `externalMemberCount`、 `mailboxFullStatus`、 `maxMessageSize`、 `moderationStatus`、 `recipientScope`、`recipientSuggestions`と`totalMemberCount`。</span><span class="sxs-lookup"><span data-stu-id="cf005-142">Possible values are: `automaticReplies`, `customMailTip`, `deliveryRestriction`, `externalMemberCount`, `mailboxFullStatus`, `maxMessageSize`, `moderationStatus`, `recipientScope`, `recipientSuggestions`, and `totalMemberCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="cf005-143">応答</span><span class="sxs-lookup"><span data-stu-id="cf005-143">Response</span></span>

<span data-ttu-id="cf005-144">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文の[メール ヒント](../resources/mailtips.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="cf005-144">If successful, this method returns a `200 OK` response code and a collection of [mailTips](../resources/mailtips.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cf005-145">例</span><span class="sxs-lookup"><span data-stu-id="cf005-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cf005-146">要求</span><span class="sxs-lookup"><span data-stu-id="cf005-146">Request</span></span>
<span data-ttu-id="cf005-147">次の使用例は、自動応答の設定、およびメールボックスのすべての状態を指定された受信者のメール ヒントを取得します。</span><span class="sxs-lookup"><span data-stu-id="cf005-147">The following example gets MailTips for the specified recipients, for any automatic reply settings and the mailbox full status.</span></span>

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

##### <a name="response"></a><span data-ttu-id="cf005-148">応答</span><span class="sxs-lookup"><span data-stu-id="cf005-148">Response</span></span>
<span data-ttu-id="cf005-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cf005-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: getMailTips",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
