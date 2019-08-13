---
title: メッセージを取得する
description: Message オブジェクトのプロパティとリレーションシップを取得します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 554de5308b5a485e94c62c3ed1cabde93d4e0ec1
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36346934"
---
# <a name="get-message"></a><span data-ttu-id="d49d3-103">メッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="d49d3-103">Get message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d49d3-104">[Message](../resources/message.md)オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="d49d3-104">Retrieve the properties and relationships of the [message](../resources/message.md) object.</span></span>

<span data-ttu-id="d49d3-105">たとえば、メッセージを取得して、メッセージ内のすべての[言及](../resources/mention.md)インスタンスを展開することができます。</span><span class="sxs-lookup"><span data-stu-id="d49d3-105">For example, you can get a message and expand all the [mention](../resources/mention.md) instances in the message.</span></span>

<span data-ttu-id="d49d3-106">`$value`パラメーターを使用し[て、メッセージの MIME コンテンツを取得](/graph/outlook-get-mime-message)できます。</span><span class="sxs-lookup"><span data-stu-id="d49d3-106">You can use the `$value` parameter to [get the MIME content of a message](/graph/outlook-get-mime-message).</span></span>

<span data-ttu-id="d49d3-107">別のユーザーのメール フォルダーからアプリがメッセージを取得するシナリオは 2 つあります。</span><span class="sxs-lookup"><span data-stu-id="d49d3-107">There are two scenarios where an app can get a message in another user's mail folder:</span></span>

* <span data-ttu-id="d49d3-108">アプリにアプリケーションのアクセス許可がある場合。または</span><span class="sxs-lookup"><span data-stu-id="d49d3-108">If the app has application permissions, or,</span></span>
* <span data-ttu-id="d49d3-109">あるユーザーからアプリに適切な代理[アクセス許可](#permissions)が与えられ、別のユーザーがそのユーザーとメール フォルダーを共有しているか、そのユーザーに代理アクセスを付与している場合。</span><span class="sxs-lookup"><span data-stu-id="d49d3-109">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="d49d3-110">[詳細と例](/graph/outlook-share-messages-folders)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d49d3-110">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

<span data-ttu-id="d49d3-111">**メッセージ** リソースは[拡張機能](/graph/extensibility-overview)をサポートしているため、`GET` 操作を使用して、**メッセージ** インスタンスでカスタム プロパティと拡張機能データを取得することもできます。</span><span class="sxs-lookup"><span data-stu-id="d49d3-111">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **message** instance.</span></span>


## <a name="permissions"></a><span data-ttu-id="d49d3-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d49d3-112">Permissions</span></span>
<span data-ttu-id="d49d3-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d49d3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d49d3-115">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d49d3-115">Permission type</span></span>      | <span data-ttu-id="d49d3-116">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d49d3-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d49d3-117">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d49d3-117">Delegated (work or school account)</span></span> | <span data-ttu-id="d49d3-118">メール ReadBasic、Mail。</span><span class="sxs-lookup"><span data-stu-id="d49d3-118">Mail.ReadBasic, Mail.Read</span></span>    |
|<span data-ttu-id="d49d3-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d49d3-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d49d3-120">メール ReadBasic、Mail。</span><span class="sxs-lookup"><span data-stu-id="d49d3-120">Mail.ReadBasic, Mail.Read</span></span>    |
|<span data-ttu-id="d49d3-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d49d3-121">Application</span></span> | <span data-ttu-id="d49d3-122">メールを取得します。</span><span class="sxs-lookup"><span data-stu-id="d49d3-122">Mail.ReadBasic.All, Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="d49d3-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d49d3-123">HTTP request</span></span>

<span data-ttu-id="d49d3-124">指定したメッセージを取得するには:</span><span class="sxs-lookup"><span data-stu-id="d49d3-124">To get the specified message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}
GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

<span data-ttu-id="d49d3-125">指定したメッセージの MIME コンテンツを取得するには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="d49d3-125">To get the MIME content of the specified message:</span></span>
<!-- { "blockType": "ignored" } --> 
```http 
GET /me/messages/{id}/$value 
GET /users/{id | userPrincipalName}/messages/{id}/$value 
GET /me/mailFolders/{id}/messages/{id}/$value 
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/$value 
```

<span data-ttu-id="d49d3-126">メッセージを取得して、メッセージ内のすべてのメンションを展開するには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="d49d3-126">To get a message and expand all mentions in the message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}?$expand=mentions
GET /users/{id | userPrincipalName}/messages/{id}?$expand=mentions
GET /me/mailFolders/{id}/messages/{id}?$expand=mentions
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}?$expand=mentions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d49d3-127">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="d49d3-127">Optional query parameters</span></span>
<span data-ttu-id="d49d3-128">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d49d3-128">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="d49d3-129">`$value`パラメーターを使用して、メッセージの MIME コンテンツを取得します。</span><span class="sxs-lookup"><span data-stu-id="d49d3-129">Use the `$value` parameter to get the MIME content of a message.</span></span>

<span data-ttu-id="d49d3-130">展開さ`$expand`れたメッセージ内の各[メンション](../resources/mention.md)の詳細を含むメッセージを取得するには、**メンション**ナビゲーションプロパティのクエリパラメーターを使用します。</span><span class="sxs-lookup"><span data-stu-id="d49d3-130">Use the `$expand` query parameter on the **mentions** navigation property to get a message with the details of each [mention](../resources/mention.md) in the message expanded.</span></span>



## <a name="request-headers"></a><span data-ttu-id="d49d3-131">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d49d3-131">Request headers</span></span>
| <span data-ttu-id="d49d3-132">名前</span><span class="sxs-lookup"><span data-stu-id="d49d3-132">Name</span></span>       | <span data-ttu-id="d49d3-133">型</span><span class="sxs-lookup"><span data-stu-id="d49d3-133">Type</span></span> | <span data-ttu-id="d49d3-134">説明</span><span class="sxs-lookup"><span data-stu-id="d49d3-134">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d49d3-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="d49d3-135">Authorization</span></span>  | <span data-ttu-id="d49d3-136">string</span><span class="sxs-lookup"><span data-stu-id="d49d3-136">string</span></span>  | <span data-ttu-id="d49d3-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d49d3-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d49d3-139">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="d49d3-139">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="d49d3-140">string</span><span class="sxs-lookup"><span data-stu-id="d49d3-140">string</span></span> | <span data-ttu-id="d49d3-141">**body** プロパティと **uniqueBody** プロパティが返されるときの形式です。</span><span class="sxs-lookup"><span data-stu-id="d49d3-141">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="d49d3-142">値は、"text" または "html" になります。</span><span class="sxs-lookup"><span data-stu-id="d49d3-142">Values can be "text" or "html".</span></span> <span data-ttu-id="d49d3-143">この `Prefer` ヘッダーが指定されている場合、`Preference-Applied` ヘッダーが確認として返されます。</span><span class="sxs-lookup"><span data-stu-id="d49d3-143">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="d49d3-144">ヘッダーが指定されていない場合は、**body** プロパティと **uniqueBody** プロパティは HTML 形式で返されます。</span><span class="sxs-lookup"><span data-stu-id="d49d3-144">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="d49d3-145">省略可能。</span><span class="sxs-lookup"><span data-stu-id="d49d3-145">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d49d3-146">要求本文</span><span class="sxs-lookup"><span data-stu-id="d49d3-146">Request body</span></span>
<span data-ttu-id="d49d3-147">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d49d3-147">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d49d3-148">応答</span><span class="sxs-lookup"><span data-stu-id="d49d3-148">Response</span></span>

<span data-ttu-id="d49d3-149">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [message](../resources/message.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d49d3-149">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d49d3-150">例</span><span class="sxs-lookup"><span data-stu-id="d49d3-150">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="d49d3-151">要求 1</span><span class="sxs-lookup"><span data-stu-id="d49d3-151">Request 1</span></span>
<span data-ttu-id="d49d3-152">最初の例では、指定されたメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="d49d3-152">The first example gets the specified message.</span></span> <span data-ttu-id="d49d3-153">返される本文の形式を示すヘッダーは指定されていません。</span><span class="sxs-lookup"><span data-stu-id="d49d3-153">It does not specify any header to indicate the desired format of the body to be returned.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d49d3-154">プロトコル</span><span class="sxs-lookup"><span data-stu-id="d49d3-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGI1AAAoZCfHAAA="],
  "name": "get_message"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages/AAMkAGI1AAAoZCfHAAA=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d49d3-155">C#</span><span class="sxs-lookup"><span data-stu-id="d49d3-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d49d3-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d49d3-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d49d3-157">目的-C</span><span class="sxs-lookup"><span data-stu-id="d49d3-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d49d3-158">Java</span><span class="sxs-lookup"><span data-stu-id="d49d3-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-1"></a><span data-ttu-id="d49d3-159">応答 1</span><span class="sxs-lookup"><span data-stu-id="d49d3-159">Response 1</span></span>
<span data-ttu-id="d49d3-160">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="d49d3-160">Here is an example of the response.</span></span> <span data-ttu-id="d49d3-161">**Body**プロパティと**uniqueBody**プロパティは、既定の HTML 形式で返されます。</span><span class="sxs-lookup"><span data-stu-id="d49d3-161">The **body** and **uniqueBody** properties are returned in the default HTML format.</span></span>
<span data-ttu-id="d49d3-162">注: 簡潔にするために、ここに示す response オブジェクトは切り詰められています。</span><span class="sxs-lookup"><span data-stu-id="d49d3-162">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="d49d3-163">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="d49d3-163">All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request-2"></a><span data-ttu-id="d49d3-164">要求 2</span><span class="sxs-lookup"><span data-stu-id="d49d3-164">Request 2</span></span>
<span data-ttu-id="d49d3-165">次の例では、サインインしているユーザーは Dana Swope です。</span><span class="sxs-lookup"><span data-stu-id="d49d3-165">In the next example, the signed-in user is Dana Swope.</span></span> <span data-ttu-id="d49d3-166">この例では、Dana のメールボックス内の指定されたメッセージ内のすべてのメンションの詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="d49d3-166">The example shows getting the details of all the mentions in the specified message in Dana's mailbox.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d49d3-167">プロトコル</span><span class="sxs-lookup"><span data-stu-id="d49d3-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AQMkADJmMTUAAAgVZAAAA"],
  "name": "get_mentions_in_message"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages/AQMkADJmMTUAAAgVZAAAA/?$expand=mentions
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d49d3-168">C#</span><span class="sxs-lookup"><span data-stu-id="d49d3-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mentions-in-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d49d3-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d49d3-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mentions-in-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d49d3-170">目的-C</span><span class="sxs-lookup"><span data-stu-id="d49d3-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mentions-in-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d49d3-171">Java</span><span class="sxs-lookup"><span data-stu-id="d49d3-171">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mentions-in-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-2"></a><span data-ttu-id="d49d3-172">応答 2</span><span class="sxs-lookup"><span data-stu-id="d49d3-172">Response 2</span></span>
<span data-ttu-id="d49d3-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d49d3-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


##### <a name="request-3"></a><span data-ttu-id="d49d3-176">要求 3</span><span class="sxs-lookup"><span data-stu-id="d49d3-176">Request 3</span></span>

<span data-ttu-id="d49d3-177">3番目の例では、 `Prefer: outlook.body-content-type="text"`ヘッダーを使用して、指定したメッセージの**本文**と**uniqueBody**をテキスト形式で取得する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="d49d3-177">The third example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** and **uniqueBody** of the specified message in text format.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d49d3-178">プロトコル</span><span class="sxs-lookup"><span data-stu-id="d49d3-178">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGI1AAAoZCfHAAA="],
  "name": "get_message_in_text"
}-->

```http
GET https://graph.microsoft.com/beta/me/messages/AAMkAGI1AAAoZCfHAAA=/?$select=subject,body,bodyPreview,uniqueBody
Prefer: outlook.body-content-type="text"
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d49d3-179">C#</span><span class="sxs-lookup"><span data-stu-id="d49d3-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-in-text-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d49d3-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d49d3-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-in-text-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d49d3-181">目的-C</span><span class="sxs-lookup"><span data-stu-id="d49d3-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-in-text-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d49d3-182">Java</span><span class="sxs-lookup"><span data-stu-id="d49d3-182">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-message-in-text-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-3"></a><span data-ttu-id="d49d3-183">応答 3</span><span class="sxs-lookup"><span data-stu-id="d49d3-183">Response 3</span></span>

<span data-ttu-id="d49d3-184">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="d49d3-184">Here is an example of the response.</span></span> <span data-ttu-id="d49d3-185">注: 応答には、 `Preference-Applied: outlook.body-content-type` `Prefer: outlook.body-content-type`要求ヘッダーを認識するためのヘッダーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="d49d3-185">Note: The response includes a `Preference-Applied: outlook.body-content-type` header to acknowledge the `Prefer: outlook.body-content-type` request header.</span></span>
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

##### <a name="request-4"></a><span data-ttu-id="d49d3-186">要求 4</span><span class="sxs-lookup"><span data-stu-id="d49d3-186">Request 4</span></span>

<span data-ttu-id="d49d3-187">4番目の例は、特定のメッセージのインターネットメッセージヘッダーを取得する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="d49d3-187">The fourth example shows how to get the Internet message headers of a specific message.</span></span>  


# <a name="httptabhttp"></a>[<span data-ttu-id="d49d3-188">プロトコル</span><span class="sxs-lookup"><span data-stu-id="d49d3-188">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGVmMDEz"],
  "name": "get_message_internet_headers"
}-->

```http
GET https://graph.microsoft.com/beta/me/messages/AAMkAGVmMDEz/?$select=internetMessageHeaders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d49d3-189">C#</span><span class="sxs-lookup"><span data-stu-id="d49d3-189">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-internet-headers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d49d3-190">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d49d3-190">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-internet-headers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d49d3-191">目的-C</span><span class="sxs-lookup"><span data-stu-id="d49d3-191">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-internet-headers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d49d3-192">Java</span><span class="sxs-lookup"><span data-stu-id="d49d3-192">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-message-internet-headers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-4"></a><span data-ttu-id="d49d3-193">応答 4</span><span class="sxs-lookup"><span data-stu-id="d49d3-193">Response 4</span></span>

<span data-ttu-id="d49d3-194">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="d49d3-194">Here is an example of the response.</span></span> <span data-ttu-id="d49d3-195">注: 簡潔にするために、response オブジェクトのインターネットメッセージヘッダーの数は短縮されています。</span><span class="sxs-lookup"><span data-stu-id="d49d3-195">Note: The number of Internet message headers in the response object has been reduced for brevity.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="d49d3-196">関連項目</span><span class="sxs-lookup"><span data-stu-id="d49d3-196">See also</span></span>

- [<span data-ttu-id="d49d3-197">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="d49d3-197">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="d49d3-198">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="d49d3-198">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="d49d3-199">スキーマ拡張機能を使用したグループへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="d49d3-199">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
    "Error: get_message_internet_headers/internetMessageHeaders/member/value:\r\n       Expected type String but actual was Binary. Property: value, actual value: 'binary'"
  ]
}
-->
