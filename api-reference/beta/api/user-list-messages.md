---
title: メッセージを一覧表示する
description: 'サインイン中のユーザーのメールボックス内のメッセージを取得します (削除済みアイテムと低優先メール フォルダーを含む)。 '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 19cb2dc1dd1e86cd697319a0dc8a729cb712e463
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31792189"
---
# <a name="list-messages"></a><span data-ttu-id="3416e-103">メッセージを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="3416e-103">List messages</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3416e-104">サインイン中のユーザーのメールボックス内のメッセージを取得します (削除済みアイテムと低優先メール フォルダーを含む)。</span><span class="sxs-lookup"><span data-stu-id="3416e-104">Get the messages in the signed-in user's mailbox (including the Deleted Items and Clutter folders).</span></span> 

<span data-ttu-id="3416e-105">ページサイズとメールボックスのデータによっては、メールボックスからメッセージを取得すると、複数の要求が発生することがあります。</span><span class="sxs-lookup"><span data-stu-id="3416e-105">Depending on the page size and mailbox data, getting messages from a mailbox can incur multiple requests.</span></span> <span data-ttu-id="3416e-106">既定のページサイズは10個のメッセージです。</span><span class="sxs-lookup"><span data-stu-id="3416e-106">The default page size is 10 messages.</span></span> <span data-ttu-id="3416e-107">メッセージの次のページを取得するには、返される URL 全体`@odata.nextLink`を次のメッセージの取得要求に適用するだけです。</span><span class="sxs-lookup"><span data-stu-id="3416e-107">To get the next page of messages, simply apply the entire URL returned in `@odata.nextLink` to the next get-messages request.</span></span> <span data-ttu-id="3416e-108">この URL には、最初の要求で指定されたすべてのクエリパラメーターが含まれています。</span><span class="sxs-lookup"><span data-stu-id="3416e-108">This URL includes any query parameters you may have specified in the initial request.</span></span> 

<span data-ttu-id="3416e-109">応答を操作するために`$skip` 、 `@odata.nextLink` URL から値を抽出しようとしないでください。</span><span class="sxs-lookup"><span data-stu-id="3416e-109">Do not try to extract the `$skip` value from the `@odata.nextLink` URL to manipulate responses.</span></span> <span data-ttu-id="3416e-110">この API は、 `$skip`値を使用して、ユーザーのメールボックスで削除されたすべてのアイテムのカウントを保持し、メッセージタイプのアイテムのページを返します。</span><span class="sxs-lookup"><span data-stu-id="3416e-110">This API uses the `$skip` value to keep count of all the items it has gone through in the user's mailbox to return a page of message-type items.</span></span> <span data-ttu-id="3416e-111">最初の応答でも、この`$skip`値がページサイズよりも大きくなる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="3416e-111">It's therefore possible that even in the initial response, the `$skip` value is larger than the page size.</span></span> <span data-ttu-id="3416e-112">詳細については、「[アプリで Microsoft Graph データをページングする](/graph/paging)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3416e-112">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

<span data-ttu-id="3416e-113">メッセージにフィルターを適用し、サインインしているユーザーの[メンション](../resources/mention.md)を含むメッセージのみを取得できます。</span><span class="sxs-lookup"><span data-stu-id="3416e-113">You can filter on the messages and get only those that include a [mention](../resources/mention.md) of the signed-in user.</span></span>

<span data-ttu-id="3416e-114">既定では、操作に`GET /me/messages`よって**メンション**プロパティは返されないことに注意してください。</span><span class="sxs-lookup"><span data-stu-id="3416e-114">Note that by default, the `GET /me/messages` operation does not return the **mentions** property.</span></span> <span data-ttu-id="3416e-115">`$expand` [メッセージ内の各メンションの詳細を検索](../api/message-get.md#request-2)するには、クエリパラメーターを使用します。</span><span class="sxs-lookup"><span data-stu-id="3416e-115">Use the `$expand` query parameter to [find details of each mention in a message](../api/message-get.md#request-2).</span></span>

<span data-ttu-id="3416e-116">アプリが別のユーザーのメールフォルダーでメッセージを取得できるシナリオは2つあります。</span><span class="sxs-lookup"><span data-stu-id="3416e-116">There are two scenarios where an app can get messages in another user's mail folder:</span></span>

* <span data-ttu-id="3416e-117">アプリにアプリケーションのアクセス許可がある場合。または</span><span class="sxs-lookup"><span data-stu-id="3416e-117">If the app has application permissions, or,</span></span>
* <span data-ttu-id="3416e-118">アプリに1人のユーザーから適切に委任された[アクセス許可](#permissions)がある場合、別のユーザーがそのユーザーとのメールフォルダーを共有しているか、または、そのユーザーに対してアクセスを委任されている。</span><span class="sxs-lookup"><span data-stu-id="3416e-118">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="3416e-119">[詳細と例](/graph/outlook-share-messages-folders)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3416e-119">See [details and an example](/graph/outlook-share-messages-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="3416e-120">権限</span><span class="sxs-lookup"><span data-stu-id="3416e-120">Permissions</span></span>
<span data-ttu-id="3416e-p105">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3416e-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3416e-123">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3416e-123">Permission type</span></span>      | <span data-ttu-id="3416e-124">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3416e-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3416e-125">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3416e-125">Delegated (work or school account)</span></span> | <span data-ttu-id="3416e-126">メール readbasic、mail. 読み取り、ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3416e-126">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="3416e-127">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3416e-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3416e-128">メール readbasic、mail. 読み取り、ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3416e-128">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="3416e-129">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3416e-129">Application</span></span> | <span data-ttu-id="3416e-130">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3416e-130">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3416e-131">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3416e-131">HTTP request</span></span>

<span data-ttu-id="3416e-132">ユーザーのメールボックス内のすべてのメッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="3416e-132">To get all the messages in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
GET /users/{id | userPrincipalName}/messages
```

<span data-ttu-id="3416e-133">ユーザーのメールボックス内の特定のフォルダーにあるメッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="3416e-133">To get messages in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```

<span data-ttu-id="3416e-134">ユーザーのメールボックス内のすべてのメッセージを取得するに\*\*\*\* は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="3416e-134">To get all the messages in the user's mailbox that include a **mention** of the user:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages?$filter=mentionsPreview/isMentioned eq true
GET /users/{id | userPrincipalName}/messages?$filter=mentionsPreview/isMentioned eq true
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3416e-135">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="3416e-135">Optional query parameters</span></span>
<span data-ttu-id="3416e-136">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="3416e-136">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="3416e-137">`$filter` **mentionsPreview**プロパティの query パラメーターを使用すると、サインインしているユーザーを言及するメッセージを取得できます。</span><span class="sxs-lookup"><span data-stu-id="3416e-137">You can use the `$filter` query parameter on the **mentionsPreview** property to get those messages that mention the signed-in user.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3416e-138">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3416e-138">Request headers</span></span>
| <span data-ttu-id="3416e-139">名前</span><span class="sxs-lookup"><span data-stu-id="3416e-139">Name</span></span>       | <span data-ttu-id="3416e-140">型</span><span class="sxs-lookup"><span data-stu-id="3416e-140">Type</span></span> | <span data-ttu-id="3416e-141">説明</span><span class="sxs-lookup"><span data-stu-id="3416e-141">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3416e-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="3416e-142">Authorization</span></span>  | <span data-ttu-id="3416e-143">string</span><span class="sxs-lookup"><span data-stu-id="3416e-143">string</span></span>  | <span data-ttu-id="3416e-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3416e-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3416e-146">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="3416e-146">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="3416e-147">string</span><span class="sxs-lookup"><span data-stu-id="3416e-147">string</span></span> | <span data-ttu-id="3416e-148">**body** プロパティと **uniqueBody** プロパティが返されるときの形式です。</span><span class="sxs-lookup"><span data-stu-id="3416e-148">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="3416e-149">値は、"text" または "html" になります。</span><span class="sxs-lookup"><span data-stu-id="3416e-149">Values can be "text" or "html".</span></span> <span data-ttu-id="3416e-150">ヘッダーが指定されていない場合は、**body** プロパティと **uniqueBody** プロパティは HTML 形式で返されます。</span><span class="sxs-lookup"><span data-stu-id="3416e-150">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="3416e-151">省略可能。</span><span class="sxs-lookup"><span data-stu-id="3416e-151">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3416e-152">要求本文</span><span class="sxs-lookup"><span data-stu-id="3416e-152">Request body</span></span>
<span data-ttu-id="3416e-153">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="3416e-153">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3416e-154">応答</span><span class="sxs-lookup"><span data-stu-id="3416e-154">Response</span></span>

<span data-ttu-id="3416e-155">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[message](../resources/message.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="3416e-155">If successful, this method returns a `200 OK` response code and collection of [message](../resources/message.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3416e-156">例</span><span class="sxs-lookup"><span data-stu-id="3416e-156">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="3416e-157">要求 1</span><span class="sxs-lookup"><span data-stu-id="3416e-157">Request 1</span></span>
<span data-ttu-id="3416e-158">最初の例では、サインインしているユーザーのメールボックス内の既定の上位10個のメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="3416e-158">The first example gets the default, top 10 messages in the signed-in user's mailbox.</span></span> <span data-ttu-id="3416e-159">を使用`$select`して、応答内の各メッセージのプロパティのサブセットを返します。</span><span class="sxs-lookup"><span data-stu-id="3416e-159">It uses `$select` to return a subset of the properties of each message in the response.</span></span> 
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages?$select=sender,subject
```
##### <a name="response-1"></a><span data-ttu-id="3416e-160">応答 1</span><span class="sxs-lookup"><span data-stu-id="3416e-160">Response 1</span></span>
<span data-ttu-id="3416e-161">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="3416e-161">Here is an example of the response.</span></span> <span data-ttu-id="3416e-162">メッセージの次のページを取得するには、で`@odata.nextLink`返される URL を後続の get 要求に適用します。</span><span class="sxs-lookup"><span data-stu-id="3416e-162">To get the next page of messages, apply the URL returned in `@odata.nextLink` to a subsequent GET request.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('bb8775a4-4d8c-42cf-a1d4-4d58c2bb668f')/messages(sender,subject)",
    "@odata.nextLink": "https://graph.microsoft.com/beta/me/messages?$select=sender%2csubject&$skip=14",
    "value": [
        {
            "@odata.etag": "W/\"CQAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAwR4Hg\"",
            "id": "AAMkAGUAAAwTW09AAA=",
            "subject": "You have late tasks!",
            "sender": {
                "emailAddress": {
                    "name": "Microsoft Planner",
                    "address": "noreply@Planner.Office365.com"
                }
            }
        },
        {
            "@odata.etag": "W/\"CQAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAq4D1e\"",
            "id": "AAMkAGUAAAq5QKlAAA=",
            "subject": "You have late tasks!",
            "sender": {
                "emailAddress": {
                    "name": "Microsoft Planner",
                    "address": "noreply@Planner.Office365.com"
                }
            }
        },
        {
            "@odata.etag": "W/\"CQAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAq4D0v\"",
            "id": "AAMkAGUAAAq5QKkAAA=",
            "subject": "Your Azure AD Identity Protection Weekly Digest",
            "sender": {
                "emailAddress": {
                    "name": "Microsoft Azure",
                    "address": "azure-noreply@microsoft.com"
                }
            }
        },
        {
            "@odata.etag": "W/\"CQAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAq4DsN\"",
            "id": "AAMkAGUAAAq5QKjAAA=",
            "subject": "Use attached file",
            "sender": {
                "emailAddress": {
                    "name": "Megan Bowen",
                    "address": "MeganB@contoso.OnMicrosoft.com"
                }
            }
        },
        {
            "@odata.etag": "W/\"CQAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAq4Dq9\"",
            "id": "AAMkAGUAAAq5QKiAAA=",
            "subject": "Original invitation",
            "sender": {
                "emailAddress": {
                    "name": "Megan Bowen",
                    "address": "MeganB@contoso.OnMicrosoft.com"
                }
            }
        },
        {
            "@odata.etag": "W/\"CQAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAq4Dq1\"",
            "id": "AAMkAGUAAAq5QKhAAA=",
            "subject": "Koala image",
            "sender": {
                "emailAddress": {
                    "name": "Megan Bowen",
                    "address": "MeganB@contoso.OnMicrosoft.com"
                }
            }
        },
        {
            "@odata.etag": "W/\"CQAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAq4Dqp\"",
            "id": "AAMkAGUAAAq5QKgAAA=",
            "subject": "Sales invoice template",
            "sender": {
                "emailAddress": {
                    "name": "Megan Bowen",
                    "address": "MeganB@contoso.OnMicrosoft.com"
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.eventMessageRequest",
            "@odata.etag": "W/\"CwAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAq4Dfa\"",
            "id": "AAMkAGUAAAq5T8tAAA=",
            "subject": "Review strategy for Q3",
            "sender": {
                "emailAddress": {
                    "name": "Megan Bowen",
                    "address": "MeganB@contoso.OnMicrosoft.com"
                }
            }
        }
    ]
}
```


##### <a name="request-2"></a><span data-ttu-id="3416e-163">要求 2</span><span class="sxs-lookup"><span data-stu-id="3416e-163">Request 2</span></span>
<span data-ttu-id="3416e-164">次の例では、サインインしているユーザーのメールボックス内のすべてのメッセージに対して、ユーザーに言及するメッセージをフィルター処理します。</span><span class="sxs-lookup"><span data-stu-id="3416e-164">The next example filters all messages in the signed-in user's mailbox for those that mention the user.</span></span> <span data-ttu-id="3416e-165">また、を`$select`使用して、応答内の各メッセージのプロパティのサブセットを返します。</span><span class="sxs-lookup"><span data-stu-id="3416e-165">It also uses `$select` to return a subset of the properties of each message in the response.</span></span> 

<span data-ttu-id="3416e-166">この例では、クエリパラメーター文字列にスペース文字の URL エンコーディングも組み込まれています。</span><span class="sxs-lookup"><span data-stu-id="3416e-166">The example also incorporates URL encoding for the space characters in the query parameter string.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages_with_mentions"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages?$filter=MentionsPreview/IsMentioned%20eq%20true&$select=Subject,Sender,ReceivedDateTime,MentionsPreview
```
##### <a name="response-2"></a><span data-ttu-id="3416e-167">応答 2</span><span class="sxs-lookup"><span data-stu-id="3416e-167">Response 2</span></span>
<span data-ttu-id="3416e-p111">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3416e-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request-3"></a><span data-ttu-id="3416e-171">要求 3</span><span class="sxs-lookup"><span data-stu-id="3416e-171">Request 3</span></span>
<span data-ttu-id="3416e-172">3番目の例では、 `Prefer: outlook.body-content-type="text"`ヘッダーを使用して、各メッセージの**本文**および**uniqueBody**プロパティをテキスト形式で取得する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="3416e-172">The third example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** and **uniqueBody** properties of each message in text format.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages_in_text"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages?$select=subject,body,bodyPreview,uniqueBody
Prefer: outlook.body-content-type="text"
```
##### <a name="response-3"></a><span data-ttu-id="3416e-173">応答 3</span><span class="sxs-lookup"><span data-stu-id="3416e-173">Response 3</span></span>
<span data-ttu-id="3416e-174">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="3416e-174">Here is an example of the response.</span></span> 

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
