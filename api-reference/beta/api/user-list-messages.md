---
title: メッセージを一覧表示する
description: 'サインイン中のユーザーのメールボックス内のメッセージを取得します (削除済みアイテムと低優先メール フォルダーを含む)。 '
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 828dac4a345eaba3bb902ba5d96dec4852501033
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523569"
---
# <a name="list-messages"></a><span data-ttu-id="2f2f4-103">メッセージを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="2f2f4-103">List messages</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f2f4-104">サインイン中のユーザーのメールボックス内のメッセージを取得します (削除済みアイテムと低優先メール フォルダーを含む)。</span><span class="sxs-lookup"><span data-stu-id="2f2f4-104">Get the messages in the signed-in user's mailbox (including the Deleted Items and Clutter folders).</span></span> 

<span data-ttu-id="2f2f4-105">具体的には、メッセージにフィルターを適用し、のみが含まれるもの、[説明](../resources/mention.md)サインイン中のユーザーの取得できます。</span><span class="sxs-lookup"><span data-stu-id="2f2f4-105">In particular, you can filter on the messages and get only those that include a [mention](../resources/mention.md) of the signed-in user.</span></span>

<span data-ttu-id="2f2f4-106">既定では、注意してください、`GET /me/messages`操作**に関する**プロパティを返しません。</span><span class="sxs-lookup"><span data-stu-id="2f2f4-106">Note that by default, the `GET /me/messages` operation does not return the **mentions** property.</span></span> <span data-ttu-id="2f2f4-107">使用して、 `$expand` [メッセージに記載されているそれぞれの詳細情報を検索](../api/message-get.md#request-2)するパラメーター クエリを実行します。</span><span class="sxs-lookup"><span data-stu-id="2f2f4-107">Use the `$expand` query parameter to [find details of each mention in a message](../api/message-get.md#request-2).</span></span>

<span data-ttu-id="2f2f4-108">2 つシナリオは、アプリケーションが別のユーザーのメール フォルダーにメッセージを取得する場所です。</span><span class="sxs-lookup"><span data-stu-id="2f2f4-108">There are two scenarios where an app can get messages in another user's mail folder:</span></span>

* <span data-ttu-id="2f2f4-109">アプリケーションは、アプリケーションの権限を持つ場合、または、</span><span class="sxs-lookup"><span data-stu-id="2f2f4-109">If the app has application permissions, or,</span></span>
* <span data-ttu-id="2f2f4-110">アプリケーションがある場合、適切な 1 人のユーザーから[アクセス許可](#permissions)を委任を実行し、別のユーザーは、そのユーザーのメール フォルダーを共有するにはまたは、そのユーザーに代理アクセスを与えを実行します。</span><span class="sxs-lookup"><span data-stu-id="2f2f4-110">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="2f2f4-111">[詳細と例](/graph/outlook-share-messages-folders)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2f2f4-111">See [details and an example](/graph/outlook-share-messages-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="2f2f4-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2f2f4-112">Permissions</span></span>
<span data-ttu-id="2f2f4-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2f2f4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f2f4-115">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2f2f4-115">Permission type</span></span>      | <span data-ttu-id="2f2f4-116">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2f2f4-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2f2f4-117">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2f2f4-117">Delegated (work or school account)</span></span> | <span data-ttu-id="2f2f4-118">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2f2f4-118">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="2f2f4-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2f2f4-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f2f4-120">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2f2f4-120">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="2f2f4-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2f2f4-121">Application</span></span> | <span data-ttu-id="2f2f4-122">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2f2f4-122">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="2f2f4-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2f2f4-123">HTTP request</span></span>

<span data-ttu-id="2f2f4-124">ユーザーのメールボックス内のすべてのメッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="2f2f4-124">To get all the messages in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
GET /users/{id | userPrincipalName}/messages
```

<span data-ttu-id="2f2f4-125">ユーザーのメールボックス内の特定のフォルダーにあるメッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="2f2f4-125">To get messages in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```

<span data-ttu-id="2f2f4-126">**説明**のユーザーは、ユーザーのメールボックス内には、すべてのメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="2f2f4-126">To get all the messages in the user's mailbox that include a **mention** of the user:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages?$filter=mentionsPreview/isMentioned eq true
GET /users/{id | userPrincipalName}/messages?$filter=mentionsPreview/isMentioned eq true
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2f2f4-127">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="2f2f4-127">Optional query parameters</span></span>
<span data-ttu-id="2f2f4-128">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="2f2f4-128">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="2f2f4-129">使用することができます、 `$filter` 、サインイン中のユーザーに言及するこれらのメッセージを取得するための**mentionsPreview**プロパティにパラメーター クエリを実行します。</span><span class="sxs-lookup"><span data-stu-id="2f2f4-129">You can use the `$filter` query parameter on the **mentionsPreview** property to get those messages that mention the signed-in user.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2f2f4-130">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2f2f4-130">Request headers</span></span>
| <span data-ttu-id="2f2f4-131">名前</span><span class="sxs-lookup"><span data-stu-id="2f2f4-131">Name</span></span>       | <span data-ttu-id="2f2f4-132">型</span><span class="sxs-lookup"><span data-stu-id="2f2f4-132">Type</span></span> | <span data-ttu-id="2f2f4-133">説明</span><span class="sxs-lookup"><span data-stu-id="2f2f4-133">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2f2f4-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f2f4-134">Authorization</span></span>  | <span data-ttu-id="2f2f4-135">string</span><span class="sxs-lookup"><span data-stu-id="2f2f4-135">string</span></span>  | <span data-ttu-id="2f2f4-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2f2f4-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2f2f4-138">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="2f2f4-138">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="2f2f4-139">string</span><span class="sxs-lookup"><span data-stu-id="2f2f4-139">string</span></span> | <span data-ttu-id="2f2f4-140">**body** プロパティと **uniqueBody** プロパティが返されるときの形式です。</span><span class="sxs-lookup"><span data-stu-id="2f2f4-140">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="2f2f4-141">値は、"text" または "html" になります。</span><span class="sxs-lookup"><span data-stu-id="2f2f4-141">Values can be "text" or "html".</span></span> <span data-ttu-id="2f2f4-142">ヘッダーが指定されていない場合は、**body** プロパティと **uniqueBody** プロパティは HTML 形式で返されます。</span><span class="sxs-lookup"><span data-stu-id="2f2f4-142">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="2f2f4-143">省略可能。</span><span class="sxs-lookup"><span data-stu-id="2f2f4-143">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2f2f4-144">要求本文</span><span class="sxs-lookup"><span data-stu-id="2f2f4-144">Request body</span></span>
<span data-ttu-id="2f2f4-145">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2f2f4-145">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f2f4-146">応答</span><span class="sxs-lookup"><span data-stu-id="2f2f4-146">Response</span></span>

<span data-ttu-id="2f2f4-147">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文の[メッセージ](../resources/message.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="2f2f4-147">If successful, this method returns a `200 OK` response code and collection of [message](../resources/message.md) objects in the response body.</span></span>

<span data-ttu-id="2f2f4-148">この要求の既定のページ サイズは、メッセージ 10 個です。</span><span class="sxs-lookup"><span data-stu-id="2f2f4-148">The default page size for this request is 10 messages.</span></span> 

## <a name="example"></a><span data-ttu-id="2f2f4-149">例</span><span class="sxs-lookup"><span data-stu-id="2f2f4-149">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="2f2f4-150">要求 1</span><span class="sxs-lookup"><span data-stu-id="2f2f4-150">Request 1</span></span>
<span data-ttu-id="2f2f4-151">最初の例では、サインインしているユーザーのメールボックスに上位 10 個のメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="2f2f4-151">The first example gets the top 10 messages in the signed-in user's mailbox.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages
```
##### <a name="response-1"></a><span data-ttu-id="2f2f4-152">応答 1</span><span class="sxs-lookup"><span data-stu-id="2f2f4-152">Response 1</span></span>
<span data-ttu-id="2f2f4-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2f2f4-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 317

{
  "value": [
    {
      "receivedDateTime": "2016-10-19T10:37:00Z",
      "sentDateTime": "2016-10-19T10:37:00Z",
      "hasAttachments": true,
      "subject": "subject-value",
      "body": {
        "contentType": "",
        "content": "content-value"
      },
      "bodyPreview": "bodyPreview-value"
    }
  ]
}
```


##### <a name="request-2"></a><span data-ttu-id="2f2f4-156">要求 2</span><span class="sxs-lookup"><span data-stu-id="2f2f4-156">Request 2</span></span>
<span data-ttu-id="2f2f4-157">次の例では、ユーザーに言及しているサインインしているユーザーのメールボックス内のすべてのメッセージをフィルター処理します。</span><span class="sxs-lookup"><span data-stu-id="2f2f4-157">The next example filters all messages in the signed-in user's mailbox for those that mention the user.</span></span> <span data-ttu-id="2f2f4-158">使用して`$select`の応答メッセージごとのプロパティのサブセットを返す。</span><span class="sxs-lookup"><span data-stu-id="2f2f4-158">It uses `$select` to return a subset of the properties of each message in the response.</span></span> 

<span data-ttu-id="2f2f4-159">例には、URL のクエリ パラメーターの文字列内のスペース文字のエンコードも組み込まれています。</span><span class="sxs-lookup"><span data-stu-id="2f2f4-159">The example also incorporates URL encoding for the space characters in the query parameter string.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages_with_mentions"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages?$filter=MentionsPreview/IsMentioned%20eq%20true&$select=Subject,Sender,ReceivedDateTime,MentionsPreview
```
##### <a name="response-2"></a><span data-ttu-id="2f2f4-160">応答 2</span><span class="sxs-lookup"><span data-stu-id="2f2f4-160">Response 2</span></span>
<span data-ttu-id="2f2f4-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2f2f4-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 987

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#me/messages(subject,sender,receivedDateTime,mentionsPreview)",
  "value":[
    {
      "@odata.id":"https://graph.microsoft.com/beta/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/messages('AQMkADJmMTUAAAgVZAAAA')",
      "@odata.etag":"W/\"CQAAABYAAAAPFhK2FclcRbABBJhCde8iAAAAAATI\"",
      "id":"AQMkADJmMTUAAAgVZAAAA",
      "receivedDateTime":"2016-07-21T07:40:21Z",
      "subject":"Re: Start planning soon",
      "sender":{
        "emailAddress":{
          "name":"Randi Welch",
          "address":"randiw@contoso.onmicrosoft.com"
        }
      },
      "mentionsPreview":{
        "isMentioned":true
      }
    },
    {
      "@odata.id":"https://graph.microsoft.com/beta/Users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/Messages('AQMkADJmMTUAAAjwVAAAA')",
      "@odata.etag":"W/\"CQAAABYAAAAPFhK2FclcRbABBJhCde8iAAAAAEGj\"",
      "id":"AQMkADJmMTUAAAjwVAAAA",
      "receivedDateTime":"2016-07-21T07:40:20Z",
      "subject":"Re: Start planning soon",
      "sender":{
        "emailAddress":{
          "name":"Randi Welch",
          "address":"randiw@contoso.onmicrosoft.com"
        }
      },
      "mentionsPreview":{
        "isMentioned":true
      }
    }
  ]
}
```

##### <a name="request-3"></a><span data-ttu-id="2f2f4-164">要求 3</span><span class="sxs-lookup"><span data-stu-id="2f2f4-164">Request 3</span></span>
<span data-ttu-id="2f2f4-165">3 番目の例を使用する方法を示しています、`Prefer: outlook.body-content-type="text"`ヘッダーをテキスト形式で各メッセージの**本文**および**uniqueBody**プロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="2f2f4-165">The third example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** and **uniqueBody** properties of each message in text format.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages_in_text"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages?$select=subject,body,bodyPreview,uniqueBody
Prefer: outlook.body-content-type="text"
```
##### <a name="response-3"></a><span data-ttu-id="2f2f4-166">応答 3</span><span class="sxs-lookup"><span data-stu-id="2f2f4-166">Response 3</span></span>
<span data-ttu-id="2f2f4-167">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="2f2f4-167">Here is an example of the response.</span></span> 

<!--
Note: The response includes a `Preference-Applied: outlook.body-content-type` header to acknowledge the `Prefer: outlook.body-content-type` request header.
-->

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 2704

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/messages(subject,body,bodyPreview,uniqueBody)",
    "value":[
        {
            "@odata.type":"#microsoft.graph.eventMessageRequest",
            "@odata.etag":"W/\"CwAAABYAAABmWdbhEgBXTophjCWt81m9AAAoZYj5\"",
            "id":"AAMkAGIAAAoZCfIAAA=",
            "subject":"Orientation ",
            "bodyPreview":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.",
            "body":{
                "contentType":"text",
                "content":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.\r\n"
            },
            "uniqueBody":{
                "contentType":"text",
                "content":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.\r\n"
            }
        },
        {
            "@odata.etag":"W/\"CQAAABYAAABmWdbhEgBXTophjCWt81m9AAAoZYj4\"",
            "id":"AAMkAGIAAAoZCfHAAA=",
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
        },
        {
            "@odata.etag":"W/\"CQAAABYAAABmWdbhEgBXTophjCWt81m9AAAAAAjr\"",
            "id":"AQMkAGIAAAIJTQAAAA==",
            "subject":"Welcome aboard!",
            "bodyPreview":"Welcome to the Support group!",
            "body":{
                "contentType":"text",
                "content":"Welcome to the Support group!\r\n"
            },
            "uniqueBody":{
                "contentType":"text",
                "content":"Welcome to the Support group!\r\n"
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-messages.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
