---
title: メッセージを取得する
description: プロパティと、メッセージ オブジェクトの関係を取得します。
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 5c83d0e9a59a69ebf0e20cfa0f883301b827c84f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852389"
---
# <a name="get-message"></a><span data-ttu-id="c4cba-103">メッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="c4cba-103">Get message</span></span>

> <span data-ttu-id="c4cba-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c4cba-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c4cba-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c4cba-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c4cba-106">プロパティと、[メッセージ](../resources/message.md)オブジェクトの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="c4cba-106">Retrieve the properties and relationships of the [message](../resources/message.md) object.</span></span>

<span data-ttu-id="c4cba-107">たとえば、メッセージを取得し、メッセージ内にある、[説明](../resources/mention.md)のすべてのインスタンスを展開できます。</span><span class="sxs-lookup"><span data-stu-id="c4cba-107">For example, you can get a message and expand all the [mention](../resources/mention.md) instances in the message.</span></span>

<span data-ttu-id="c4cba-108">2 つシナリオは、アプリケーションが別のユーザーのメール フォルダーにメッセージを取得する場所です。</span><span class="sxs-lookup"><span data-stu-id="c4cba-108">There are two scenarios where an app can get a message in another user's mail folder:</span></span>

* <span data-ttu-id="c4cba-109">アプリケーションは、アプリケーションの権限を持つ場合、または、</span><span class="sxs-lookup"><span data-stu-id="c4cba-109">If the app has application permissions, or,</span></span>
* <span data-ttu-id="c4cba-110">アプリケーションがある場合、適切な 1 人のユーザーから[アクセス許可](#permissions)を委任を実行し、別のユーザーは、そのユーザーのメール フォルダーを共有するにはまたは、そのユーザーに代理アクセスを与えを実行します。</span><span class="sxs-lookup"><span data-stu-id="c4cba-110">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="c4cba-111">[詳細と例](/graph/outlook-share-messages-folders)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c4cba-111">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

<span data-ttu-id="c4cba-112">**メッセージ** リソースは[拡張機能](/graph/extensibility-overview)をサポートしているため、`GET` 操作を使用して、**メッセージ** インスタンスでカスタム プロパティと拡張機能データを取得することもできます。</span><span class="sxs-lookup"><span data-stu-id="c4cba-112">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **message** instance.</span></span>


## <a name="permissions"></a><span data-ttu-id="c4cba-113">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c4cba-113">Permissions</span></span>
<span data-ttu-id="c4cba-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c4cba-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4cba-116">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c4cba-116">Permission type</span></span>      | <span data-ttu-id="c4cba-117">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c4cba-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c4cba-118">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c4cba-118">Delegated (work or school account)</span></span> | <span data-ttu-id="c4cba-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c4cba-119">Mail.Read</span></span>    |
|<span data-ttu-id="c4cba-120">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c4cba-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4cba-121">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c4cba-121">Mail.Read</span></span>    |
|<span data-ttu-id="c4cba-122">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c4cba-122">Application</span></span> | <span data-ttu-id="c4cba-123">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c4cba-123">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4cba-124">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c4cba-124">HTTP request</span></span>

<span data-ttu-id="c4cba-125">指定したメッセージを取得するには。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="c4cba-125">To get the specified message: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}
GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

<span data-ttu-id="c4cba-126">メッセージを取得し、メッセージ内のすべての記述を展開します。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="c4cba-126">To get a message and expand all mentions in the message: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/messages/{id}?$expand=mentions
GET /users/{id | userPrincipalName}/messages/{id}?$expand=mentions
GET /me/mailFolders/{id}/messages/{id}?$expand=mentions
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}?$expand=mentions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c4cba-127">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c4cba-127">Optional query parameters</span></span>
<span data-ttu-id="c4cba-128">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c4cba-128">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="c4cba-129">使用することができます、 `$expand` 、**紹介**ナビゲーション プロパティにメッセージのそれぞれの[説明](../resources/mention.md)の詳細を含むメッセージを取得するクエリ パラメーターを展開します。</span><span class="sxs-lookup"><span data-stu-id="c4cba-129">You can use the `$expand` query parameter on the **mentions** navigation property to get a message with the details of each [mention](../resources/mention.md) in the message expanded.</span></span>



## <a name="request-headers"></a><span data-ttu-id="c4cba-130">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c4cba-130">Request headers</span></span>
| <span data-ttu-id="c4cba-131">名前</span><span class="sxs-lookup"><span data-stu-id="c4cba-131">Name</span></span>       | <span data-ttu-id="c4cba-132">種類</span><span class="sxs-lookup"><span data-stu-id="c4cba-132">Type</span></span> | <span data-ttu-id="c4cba-133">説明</span><span class="sxs-lookup"><span data-stu-id="c4cba-133">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c4cba-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4cba-134">Authorization</span></span>  | <span data-ttu-id="c4cba-135">string</span><span class="sxs-lookup"><span data-stu-id="c4cba-135">string</span></span>  | <span data-ttu-id="c4cba-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c4cba-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c4cba-138">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="c4cba-138">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="c4cba-139">文字列</span><span class="sxs-lookup"><span data-stu-id="c4cba-139">string</span></span> | <span data-ttu-id="c4cba-140">**body** プロパティと **uniqueBody** プロパティが返されるときの形式です。</span><span class="sxs-lookup"><span data-stu-id="c4cba-140">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="c4cba-141">値は、"text" または "html" になります。</span><span class="sxs-lookup"><span data-stu-id="c4cba-141">Values can be "text" or "html".</span></span> <span data-ttu-id="c4cba-142">この `Prefer` ヘッダーが指定されている場合、`Preference-Applied` ヘッダーが確認として返されます。</span><span class="sxs-lookup"><span data-stu-id="c4cba-142">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="c4cba-143">ヘッダーが指定されていない場合は、**body** プロパティと **uniqueBody** プロパティは HTML 形式で返されます。</span><span class="sxs-lookup"><span data-stu-id="c4cba-143">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="c4cba-144">省略可能。</span><span class="sxs-lookup"><span data-stu-id="c4cba-144">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c4cba-145">要求本文</span><span class="sxs-lookup"><span data-stu-id="c4cba-145">Request body</span></span>
<span data-ttu-id="c4cba-146">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c4cba-146">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4cba-147">応答</span><span class="sxs-lookup"><span data-stu-id="c4cba-147">Response</span></span>

<span data-ttu-id="c4cba-148">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [message](../resources/message.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c4cba-148">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c4cba-149">例</span><span class="sxs-lookup"><span data-stu-id="c4cba-149">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="c4cba-150">要求 1</span><span class="sxs-lookup"><span data-stu-id="c4cba-150">Request 1</span></span>
<span data-ttu-id="c4cba-151">最初の例では、指定されたメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="c4cba-151">The first example gets the specified message.</span></span> <span data-ttu-id="c4cba-152">返される本文の適切な形式を指定する任意のヘッダーは指定しません。</span><span class="sxs-lookup"><span data-stu-id="c4cba-152">It does not specify any header to indicate the desired format of the body to be returned.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGI1AAAoZCfHAAA="],
  "name": "get_message"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages('AAMkAGI1AAAoZCfHAAA=')
```
##### <a name="response-1"></a><span data-ttu-id="c4cba-153">応答 1</span><span class="sxs-lookup"><span data-stu-id="c4cba-153">Response 1</span></span>
<span data-ttu-id="c4cba-154">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="c4cba-154">Here is an example of the response.</span></span> <span data-ttu-id="c4cba-155">**本文**および**uniqueBody**プロパティは、既定の HTML 形式で返されます。</span><span class="sxs-lookup"><span data-stu-id="c4cba-155">The **body** and **uniqueBody** properties are returned in the default HTML format.</span></span>
<span data-ttu-id="c4cba-156">注: ここに示す応答オブジェクトは、簡潔にするため切り捨てられます。</span><span class="sxs-lookup"><span data-stu-id="c4cba-156">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="c4cba-157">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="c4cba-157">All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request-2"></a><span data-ttu-id="c4cba-158">要求 2</span><span class="sxs-lookup"><span data-stu-id="c4cba-158">Request 2</span></span>
<span data-ttu-id="c4cba-159">次の例では、サインイン中のユーザーとは、Dana Swope です。</span><span class="sxs-lookup"><span data-stu-id="c4cba-159">In the next example, the signed-in user is Dana Swope.</span></span> <span data-ttu-id="c4cba-160">Dana のメールボックス内の指定されたメッセージですべての記述の詳細を取得する例を示しています。</span><span class="sxs-lookup"><span data-stu-id="c4cba-160">The example shows getting the details of all the mentions in the specified message in Dana's mailbox.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AQMkADJmMTUAAAgVZAAAA"],
  "name": "get_mentions_in_message"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages/('AQMkADJmMTUAAAgVZAAAA')?$expand=mentions
```
##### <a name="response-2"></a><span data-ttu-id="c4cba-161">応答 2</span><span class="sxs-lookup"><span data-stu-id="c4cba-161">Response 2</span></span>
<span data-ttu-id="c4cba-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c4cba-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


##### <a name="request-3"></a><span data-ttu-id="c4cba-165">要求 3</span><span class="sxs-lookup"><span data-stu-id="c4cba-165">Request 3</span></span>

<span data-ttu-id="c4cba-166">3 番目の例を使用する方法を示しています、`Prefer: outlook.body-content-type="text"`ヘッダーをテキスト形式の**本文**と指定されたメッセージの**uniqueBody**を取得します。</span><span class="sxs-lookup"><span data-stu-id="c4cba-166">The third example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** and **uniqueBody** of the specified message in text format.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGI1AAAoZCfHAAA="],
  "name": "get_message_in_text"
}-->

```http
GET https://graph.microsoft.com/beta/me/messages('AAMkAGI1AAAoZCfHAAA=')?$select=subject,body,bodyPreview,uniqueBody
Prefer: outlook.body-content-type="text"
```

##### <a name="response-3"></a><span data-ttu-id="c4cba-167">応答 3</span><span class="sxs-lookup"><span data-stu-id="c4cba-167">Response 3</span></span>

<span data-ttu-id="c4cba-168">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="c4cba-168">Here is an example of the response.</span></span> <span data-ttu-id="c4cba-169">注: 応答が含まれています、`Preference-Applied: outlook.body-content-type`ヘッダーを確認するのには、`Prefer: outlook.body-content-type`要求ヘッダー。</span><span class="sxs-lookup"><span data-stu-id="c4cba-169">Note: The response includes a `Preference-Applied: outlook.body-content-type` header to acknowledge the `Prefer: outlook.body-content-type` request header.</span></span>
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

##### <a name="request-4"></a><span data-ttu-id="c4cba-170">要求 4</span><span class="sxs-lookup"><span data-stu-id="c4cba-170">Request 4</span></span>

<span data-ttu-id="c4cba-171">4 番目の例では、特定のメッセージのインターネット メッセージ ヘッダーを取得する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="c4cba-171">The fourth example shows how to get the Internet message headers of a specific message.</span></span>  

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGVmMDEz"],
  "name": "get_message_internet_headers"
}-->

```http
GET https://graph.microsoft.com/beta/me/messages('AAMkAGVmMDEz')?$select=internetMessageHeaders
```

##### <a name="response-4"></a><span data-ttu-id="c4cba-172">応答 4</span><span class="sxs-lookup"><span data-stu-id="c4cba-172">Response 4</span></span>

<span data-ttu-id="c4cba-173">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="c4cba-173">Here is an example of the response.</span></span> <span data-ttu-id="c4cba-174">注: わかりやすくするための応答オブジェクト内のインターネット メッセージ ヘッダーの数が削減されました。</span><span class="sxs-lookup"><span data-stu-id="c4cba-174">Note: The number of Internet message headers in the response object has been reduced for brevity.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="c4cba-175">関連項目</span><span class="sxs-lookup"><span data-stu-id="c4cba-175">See also</span></span>

- [<span data-ttu-id="c4cba-176">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="c4cba-176">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="c4cba-177">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="c4cba-177">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="c4cba-178">スキーマ拡張機能を使用したグループへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="c4cba-178">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
