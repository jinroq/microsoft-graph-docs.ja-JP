---
title: メッセージを取得する
description: プロパティと、メッセージ オブジェクトの関係を取得します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: e5f7b8c73ac9e121a1f0cbe1bf4200326d2d4e29
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643200"
---
# <a name="get-message"></a><span data-ttu-id="766d3-103">メッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="766d3-103">Get message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="766d3-104">プロパティと、[メッセージ](../resources/message.md)オブジェクトの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="766d3-104">Retrieve the properties and relationships of the [message](../resources/message.md) object.</span></span>

<span data-ttu-id="766d3-105">たとえば、メッセージを取得し、メッセージ内にある、[説明](../resources/mention.md)のすべてのインスタンスを展開できます。</span><span class="sxs-lookup"><span data-stu-id="766d3-105">For example, you can get a message and expand all the [mention](../resources/mention.md) instances in the message.</span></span>

<span data-ttu-id="766d3-106">2 つシナリオは、アプリケーションが別のユーザーのメール フォルダーにメッセージを取得する場所です。</span><span class="sxs-lookup"><span data-stu-id="766d3-106">There are two scenarios where an app can get a message in another user's mail folder:</span></span>

* <span data-ttu-id="766d3-107">アプリケーションは、アプリケーションの権限を持つ場合、または、</span><span class="sxs-lookup"><span data-stu-id="766d3-107">If the app has application permissions, or,</span></span>
* <span data-ttu-id="766d3-108">アプリケーションがある場合、適切な 1 人のユーザーから[アクセス許可](#permissions)を委任を実行し、別のユーザーは、そのユーザーのメール フォルダーを共有するにはまたは、そのユーザーに代理アクセスを与えを実行します。</span><span class="sxs-lookup"><span data-stu-id="766d3-108">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="766d3-109">[詳細と例](/graph/outlook-share-messages-folders)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="766d3-109">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

<span data-ttu-id="766d3-110">**メッセージ** リソースは[拡張機能](/graph/extensibility-overview)をサポートしているため、`GET` 操作を使用して、**メッセージ** インスタンスでカスタム プロパティと拡張機能データを取得することもできます。</span><span class="sxs-lookup"><span data-stu-id="766d3-110">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **message** instance.</span></span>


## <a name="permissions"></a><span data-ttu-id="766d3-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="766d3-111">Permissions</span></span>
<span data-ttu-id="766d3-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="766d3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="766d3-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="766d3-114">Permission type</span></span>      | <span data-ttu-id="766d3-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="766d3-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="766d3-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="766d3-116">Delegated (work or school account)</span></span> | <span data-ttu-id="766d3-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="766d3-117">Mail.Read</span></span>    |
|<span data-ttu-id="766d3-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="766d3-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="766d3-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="766d3-119">Mail.Read</span></span>    |
|<span data-ttu-id="766d3-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="766d3-120">Application</span></span> | <span data-ttu-id="766d3-121">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="766d3-121">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="766d3-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="766d3-122">HTTP request</span></span>

<span data-ttu-id="766d3-123">指定したメッセージを取得するには。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="766d3-123">To get the specified message: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}
GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

<span data-ttu-id="766d3-124">メッセージを取得し、メッセージ内のすべての記述を展開します。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="766d3-124">To get a message and expand all mentions in the message: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/messages/{id}?$expand=mentions
GET /users/{id | userPrincipalName}/messages/{id}?$expand=mentions
GET /me/mailFolders/{id}/messages/{id}?$expand=mentions
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}?$expand=mentions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="766d3-125">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="766d3-125">Optional query parameters</span></span>
<span data-ttu-id="766d3-126">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="766d3-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="766d3-127">使用することができます、 `$expand` 、**紹介**ナビゲーション プロパティにメッセージのそれぞれの[説明](../resources/mention.md)の詳細を含むメッセージを取得するクエリ パラメーターを展開します。</span><span class="sxs-lookup"><span data-stu-id="766d3-127">You can use the `$expand` query parameter on the **mentions** navigation property to get a message with the details of each [mention](../resources/mention.md) in the message expanded.</span></span>



## <a name="request-headers"></a><span data-ttu-id="766d3-128">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="766d3-128">Request headers</span></span>
| <span data-ttu-id="766d3-129">名前</span><span class="sxs-lookup"><span data-stu-id="766d3-129">Name</span></span>       | <span data-ttu-id="766d3-130">型</span><span class="sxs-lookup"><span data-stu-id="766d3-130">Type</span></span> | <span data-ttu-id="766d3-131">説明</span><span class="sxs-lookup"><span data-stu-id="766d3-131">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="766d3-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="766d3-132">Authorization</span></span>  | <span data-ttu-id="766d3-133">string</span><span class="sxs-lookup"><span data-stu-id="766d3-133">string</span></span>  | <span data-ttu-id="766d3-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="766d3-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="766d3-136">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="766d3-136">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="766d3-137">string</span><span class="sxs-lookup"><span data-stu-id="766d3-137">string</span></span> | <span data-ttu-id="766d3-138">**body** プロパティと **uniqueBody** プロパティが返されるときの形式です。</span><span class="sxs-lookup"><span data-stu-id="766d3-138">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="766d3-139">値は、"text" または "html" になります。</span><span class="sxs-lookup"><span data-stu-id="766d3-139">Values can be "text" or "html".</span></span> <span data-ttu-id="766d3-140">この `Prefer` ヘッダーが指定されている場合、`Preference-Applied` ヘッダーが確認として返されます。</span><span class="sxs-lookup"><span data-stu-id="766d3-140">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="766d3-141">ヘッダーが指定されていない場合は、**body** プロパティと **uniqueBody** プロパティは HTML 形式で返されます。</span><span class="sxs-lookup"><span data-stu-id="766d3-141">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="766d3-142">省略可能。</span><span class="sxs-lookup"><span data-stu-id="766d3-142">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="766d3-143">要求本文</span><span class="sxs-lookup"><span data-stu-id="766d3-143">Request body</span></span>
<span data-ttu-id="766d3-144">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="766d3-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="766d3-145">応答</span><span class="sxs-lookup"><span data-stu-id="766d3-145">Response</span></span>

<span data-ttu-id="766d3-146">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [message](../resources/message.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="766d3-146">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="766d3-147">例</span><span class="sxs-lookup"><span data-stu-id="766d3-147">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="766d3-148">要求 1</span><span class="sxs-lookup"><span data-stu-id="766d3-148">Request 1</span></span>
<span data-ttu-id="766d3-149">最初の例では、指定されたメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="766d3-149">The first example gets the specified message.</span></span> <span data-ttu-id="766d3-150">返される本文の適切な形式を指定する任意のヘッダーは指定しません。</span><span class="sxs-lookup"><span data-stu-id="766d3-150">It does not specify any header to indicate the desired format of the body to be returned.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGI1AAAoZCfHAAA="],
  "name": "get_message"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages('AAMkAGI1AAAoZCfHAAA=')
```
##### <a name="response-1"></a><span data-ttu-id="766d3-151">応答 1</span><span class="sxs-lookup"><span data-stu-id="766d3-151">Response 1</span></span>
<span data-ttu-id="766d3-152">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="766d3-152">Here is an example of the response.</span></span> <span data-ttu-id="766d3-153">**本文**および**uniqueBody**プロパティは、既定の HTML 形式で返されます。</span><span class="sxs-lookup"><span data-stu-id="766d3-153">The **body** and **uniqueBody** properties are returned in the default HTML format.</span></span>
<span data-ttu-id="766d3-154">注: ここに示す応答オブジェクトは、簡潔にするため切り捨てられます。</span><span class="sxs-lookup"><span data-stu-id="766d3-154">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="766d3-155">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="766d3-155">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 523

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/messages/$entity",
    "@odata.etag":"W/\"CQAAABYAAABmWdbhEgBXTophjCWt81m9AAAoZYj4\"",
    "id":"AAMkAGI1AAAoZCfHAAA=",
    "subject":"Welcome to our group!",
    "bodyPreview":"Welcome to our group, Dana! Hope you will enjoy working with us !\r\n",
    "body":{
        "contentType":"html",
        "content":"<html>\r\n<head></head><body><p>Welcome to our group, Dana! Hope you will enjoy working with us </p></body></html>\r\n"
    },
    "uniqueBody":{
        "contentType":"html",
        "content":"<html>\r\n<head></head><body><p>Welcome to our group, Dana! Hope you will enjoy working with us </p></body></html>\r\n"
    }
}
```

##### <a name="request-2"></a><span data-ttu-id="766d3-156">要求 2</span><span class="sxs-lookup"><span data-stu-id="766d3-156">Request 2</span></span>
<span data-ttu-id="766d3-157">次の例では、サインイン中のユーザーとは、Dana Swope です。</span><span class="sxs-lookup"><span data-stu-id="766d3-157">In the next example, the signed-in user is Dana Swope.</span></span> <span data-ttu-id="766d3-158">Dana のメールボックス内の指定されたメッセージですべての記述の詳細を取得する例を示しています。</span><span class="sxs-lookup"><span data-stu-id="766d3-158">The example shows getting the details of all the mentions in the specified message in Dana's mailbox.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AQMkADJmMTUAAAgVZAAAA"],
  "name": "get_mentions_in_message"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages/('AQMkADJmMTUAAAgVZAAAA')?$expand=mentions
```
##### <a name="response-2"></a><span data-ttu-id="766d3-159">応答 2</span><span class="sxs-lookup"><span data-stu-id="766d3-159">Response 2</span></span>
<span data-ttu-id="766d3-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="766d3-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 2248

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#me/messages/$entity",
  "@odata.id":"https://graph.microsoft.com/beta/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/messages('AQMkADJmMTUAAAgVZAAAA')",
  "@odata.etag":"W/\"CQAAABYAAAAPFhK2FclcRbABBJhCde8iAAAAAATI\"",
  "id":"AQMkADJmMTUAAAgVZAAAA",
  "subject":"Start planning soon",
  "body":{
    "contentType":"HTML",
    "content":"<html><head></head><body><p><a href=\"mailto:danas@contoso.onmicrosoft.com\">@Dana Swope</a>,<a href=\"mailto:randiw@contoso.onmicrosoft.com\">@Randi Welch</a>, forgot to mention, I will be away&nbsp;this weekend. I can start on Monday though.</p></body></html>"
  },
  "bodyPreview":"@Dana Swope<mailto:danas@contoso.onmicrosoft.com>, @Randi Welch, forgot to mention, I will be away this weekend. I can start on Monday though.",
  "sender":{
    "emailAddress":{
      "name":"Samantha Booth",
      "address":"samanthab@contoso.onmicrosoft.com"
    }
  },
  "from":{
    "emailAddress":{
      "name":"Samantha Booth",
      "address":"samanthab@contoso.onmicrosoft.com"
    }
  },
  "toRecipients":[
    {
      "emailAddress":{
        "name":"Dana Swope",
        "address":"danas@contoso.onmicrosoft.com"
      }
    },
    {
      "emailAddress":{
        "name":"Randi Welch",
        "address":"randiw@contoso.onmicrosoft.com"
      }
    }
  ],
  "ccRecipients":[
  ],
  "bccRecipients":[
  ],
  "mentionsPreview":{
    "isMentioned":true
  },
  "mentions@odata.context":"https://graph.microsoft.com/beta/$metadata#me/messages('AQMkADJmMTUAAAgVZAAAA')/mentions",
  "mentions":[
    {
      "@odata.id":"https://graph.microsoft.com/beta/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/messages('AQMkADJmMTUAAAgVZAAAA')/mentions('138f4c0a-1130-4776-b780-bf79d73abb3f')",
      "id":"138f4c0a-1130-4776-b780-bf79d73abb3f",
      "mentioned":{
        "name":"Dana Swope",
        "address":"danas@contoso.onmicrosoft.com"
      },
      "mentionText":null,
      "clientReference":null,
      "createdBy":{
        "name":"Samantha Booth",
        "address":"samanthab@contoso.onmicrosoft.com"
      },
      "createdDateTime":"2016-07-21T07:40:20.152Z",
      "serverCreatedDateTime":"2016-07-21T07:40:20.152Z",
      "deepLink":null,
      "application":null
    },
    {
      "@odata.id":"https://graph.microsoft.com/beta/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/messages('AQMkADJmMTUAAAgVZAAAA')/mentions('7b94df1a-0086-482a-b0da-e62fae12f983')",
      "id":"7b94df1a-0086-482a-b0da-e62fae12f983",
      "mentioned":{
        "name":"Randi Welch",
        "address":"randiw@contoso.onmicrosoft.com"
      },
      "mentionText":null,
      "clientReference":null,
      "createdBy":{
        "name":"Samantha Booth",
        "address":"samanthab@contoso.onmicrosoft.com"
      },
      "createdDateTime":"2016-07-21T07:40:20.158Z",
      "serverCreatedDateTime":"2016-07-21T07:40:20.158Z",
      "deepLink":null,
      "application":null
    }
  ]
}
```


##### <a name="request-3"></a><span data-ttu-id="766d3-163">要求 3</span><span class="sxs-lookup"><span data-stu-id="766d3-163">Request 3</span></span>

<span data-ttu-id="766d3-164">3 番目の例を使用する方法を示しています、`Prefer: outlook.body-content-type="text"`ヘッダーをテキスト形式の**本文**と指定されたメッセージの**uniqueBody**を取得します。</span><span class="sxs-lookup"><span data-stu-id="766d3-164">The third example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** and **uniqueBody** of the specified message in text format.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGI1AAAoZCfHAAA="],
  "name": "get_message_in_text"
}-->

```http
GET https://graph.microsoft.com/beta/me/messages('AAMkAGI1AAAoZCfHAAA=')?$select=subject,body,bodyPreview,uniqueBody
Prefer: outlook.body-content-type="text"
```

##### <a name="response-3"></a><span data-ttu-id="766d3-165">応答 3</span><span class="sxs-lookup"><span data-stu-id="766d3-165">Response 3</span></span>

<span data-ttu-id="766d3-166">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="766d3-166">Here is an example of the response.</span></span> <span data-ttu-id="766d3-167">注: 応答が含まれています、`Preference-Applied: outlook.body-content-type`ヘッダーを確認するのには、`Prefer: outlook.body-content-type`要求ヘッダー。</span><span class="sxs-lookup"><span data-stu-id="766d3-167">Note: The response includes a `Preference-Applied: outlook.body-content-type` header to acknowledge the `Prefer: outlook.body-content-type` request header.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.body-content-type="text"
Content-length: 1550

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/messages(subject,body,bodyPreview,uniqueBody)/$entity",
    "@odata.etag":"W/\"CQAAABYAAABmWdbhEgBXTophjCWt81m9AAAoZYj4\"",
    "id":"AAMkAGI1AAAoZCfHAAA=",
    "subject":"Welcome to our group!",
    "bodyPreview":"Welcome to our group, Dana! Hope you will enjoy working with us !\r\n\r\nWould you like to choose a day for our orientation from the available times below:\r\n\r\n\r\nDate\r\n        Time\r\n\r\nApril 14, 2017\r\n        1-3pm\r\n\r\nApril 21, 2017\r\n        10-12noon\r\n\r\n\r\n\r\nTh",
    "body":{
        "contentType":"text",
        "content":"Welcome to our group, Dana! Hope you will enjoy working with us [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] !\r\n\r\nWould you like to choose a day for our orientation from the available times below:\r\n\r\n\r\nDate\r\n        Time\r\n\r\nApril 14, 2017\r\n        1-3pm\r\n\r\nApril 21, 2017\r\n        10-12noon\r\n\r\n\r\n\r\nThanks!\r\n\r\n"
    },
    "uniqueBody":{
        "contentType":"text",
        "content":"Welcome to our group, Dana! Hope you will enjoy working with us [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] !\r\nWould you like to choose a day for our orientation from the available times below:\r\n\r\nDate\r\n        Time\r\n\r\nApril 14, 2017\r\n        1-3pm\r\n\r\nApril 21, 2017\r\n        10-12noon\r\n\r\n\r\nThanks!\r\n"
    }
}
```

##### <a name="request-4"></a><span data-ttu-id="766d3-168">要求 4</span><span class="sxs-lookup"><span data-stu-id="766d3-168">Request 4</span></span>

<span data-ttu-id="766d3-169">4 番目の例では、特定のメッセージのインターネット メッセージ ヘッダーを取得する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="766d3-169">The fourth example shows how to get the Internet message headers of a specific message.</span></span>  

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGVmMDEz"],
  "name": "get_message_internet_headers"
}-->

```http
GET https://graph.microsoft.com/beta/me/messages('AAMkAGVmMDEz')?$select=internetMessageHeaders
```

##### <a name="response-4"></a><span data-ttu-id="766d3-170">応答 4</span><span class="sxs-lookup"><span data-stu-id="766d3-170">Response 4</span></span>

<span data-ttu-id="766d3-171">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="766d3-171">Here is an example of the response.</span></span> <span data-ttu-id="766d3-172">注: わかりやすくするための応答オブジェクト内のインターネット メッセージ ヘッダーの数が削減されました。</span><span class="sxs-lookup"><span data-stu-id="766d3-172">Note: The number of Internet message headers in the response object has been reduced for brevity.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('48d31887-5fad-4d73-a9f5-3c356e68a038')/messages(internetMessageHeaders)/$entity",
  "@odata.type":"#microsoft.graph.eventMessageRequest",
  "@odata.etag":"W/\"CwAAABYAAAAiIsqMbYjsT5e/T7KzowPTAAAa/qUB\"",
  "id":"AAMkAGVmMDEz",
  "internetMessageHeaders":[
    {
      "name":"Content-Type",
      "value":"application/ms-tnef"
    },
    {
      "name":"Content-Transfer-Encoding",
      "value":"binary"
    },
    {
      "name":"Subject",
      "value":"Cloud and Mobile Working Group"
    },
    {
      "name":"x-custom-header-group-name",
      "value":"Washington"
    },
    {
      "name":"x-custom-header-group-id",
      "value":"WA001"
    }
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="766d3-173">関連項目</span><span class="sxs-lookup"><span data-stu-id="766d3-173">See also</span></span>

- [<span data-ttu-id="766d3-174">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="766d3-174">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="766d3-175">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="766d3-175">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="766d3-176">スキーマ拡張機能を使用したグループへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="766d3-176">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/message-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
