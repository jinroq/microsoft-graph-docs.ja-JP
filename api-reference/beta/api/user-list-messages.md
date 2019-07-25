---
title: メッセージを一覧表示する
description: 'サインイン中のユーザーのメールボックス内のメッセージを取得します (削除済みアイテムと低優先メール フォルダーを含む)。 '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 96913cb62520e215a171220bae777630f34f5f45
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867209"
---
# <a name="list-messages"></a><span data-ttu-id="65371-103">メッセージを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="65371-103">List messages</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65371-104">サインイン中のユーザーのメールボックス内のメッセージを取得します (削除済みアイテムと低優先メール フォルダーを含む)。</span><span class="sxs-lookup"><span data-stu-id="65371-104">Get the messages in the signed-in user's mailbox (including the Deleted Items and Clutter folders).</span></span> 

<span data-ttu-id="65371-105">ページ サイズとメールボックスのデータに応じ、メールボックスから取得するメッセージは複数の要求を発生します。</span><span class="sxs-lookup"><span data-stu-id="65371-105">Depending on the page size and mailbox data, getting messages from a mailbox can incur multiple requests.</span></span> <span data-ttu-id="65371-106">ページ サイズの規定値は、10 件のメッセージです。</span><span class="sxs-lookup"><span data-stu-id="65371-106">The default page size is 10 messages.</span></span> <span data-ttu-id="65371-107">メッセージの次のページを取得するには、`@odata.nextLink`で返される URL 全体を単に次のメッセージ要求に適用するだけです。</span><span class="sxs-lookup"><span data-stu-id="65371-107">To get the next page of messages, simply apply the entire URL returned in `@odata.nextLink` to the next get-messages request.</span></span> <span data-ttu-id="65371-108">この URL は、最初の要求で指定された全てのクエリ パラメーターを含みます。</span><span class="sxs-lookup"><span data-stu-id="65371-108">This URL includes any query parameters you may have specified in the initial request.</span></span> 

<span data-ttu-id="65371-109">応答を操作するために`@odata.nextLink` URL から`$skip` 値を抽出しようとしないでください。</span><span class="sxs-lookup"><span data-stu-id="65371-109">Do not try to extract the `$skip` value from the `@odata.nextLink` URL to manipulate responses.</span></span> <span data-ttu-id="65371-110">この API は`$skip` 値を使用し、メッセージの種類の項目のページを返すためにユーザーのメールボックス内で確認された全ての項目をカウントし続けます。</span><span class="sxs-lookup"><span data-stu-id="65371-110">This API uses the `$skip` value to keep count of all the items it has gone through in the user's mailbox to return a page of message-type items.</span></span> <span data-ttu-id="65371-111">そのため、最初の要求の場合も`$skip` 値がページ サイズより大きくなる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="65371-111">It's therefore possible that even in the initial response, the `$skip` value is larger than the page size.</span></span> <span data-ttu-id="65371-112">詳細については、[アプリで Microsoft Graph データをページングする](/graph/paging)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="65371-112">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

<span data-ttu-id="65371-113">メッセージにフィルターを適用し、サインインしているユーザーの[メンション](../resources/mention.md)を含むメッセージのみを取得できます。</span><span class="sxs-lookup"><span data-stu-id="65371-113">You can filter on the messages and get only those that include a [mention](../resources/mention.md) of the signed-in user.</span></span>

<span data-ttu-id="65371-114">既定では、操作に`GET /me/messages`よって**メンション**プロパティは返されないことに注意してください。</span><span class="sxs-lookup"><span data-stu-id="65371-114">Note that by default, the `GET /me/messages` operation does not return the **mentions** property.</span></span> <span data-ttu-id="65371-115">`$expand` [メッセージ内の各メンションの詳細を検索](../api/message-get.md#request-2)するには、クエリパラメーターを使用します。</span><span class="sxs-lookup"><span data-stu-id="65371-115">Use the `$expand` query parameter to [find details of each mention in a message](../api/message-get.md#request-2).</span></span>

<span data-ttu-id="65371-116">別のユーザーのメール フォルダーからアプリがメッセージを取得するシナリオは 2 つあります。</span><span class="sxs-lookup"><span data-stu-id="65371-116">There are two scenarios where an app can get messages in another user's mail folder:</span></span>

* <span data-ttu-id="65371-117">アプリにアプリケーションのアクセス許可がある場合。または</span><span class="sxs-lookup"><span data-stu-id="65371-117">If the app has application permissions, or,</span></span>
* <span data-ttu-id="65371-118">あるユーザーからアプリに適切な代理[アクセス許可](#permissions)が与えられ、別のユーザーがそのユーザーとメール フォルダーを共有しているか、そのユーザーに代理アクセスを付与している場合。</span><span class="sxs-lookup"><span data-stu-id="65371-118">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="65371-119">[詳細と例](/graph/outlook-share-messages-folders)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="65371-119">See [details and an example](/graph/outlook-share-messages-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="65371-120">権限</span><span class="sxs-lookup"><span data-stu-id="65371-120">Permissions</span></span>
<span data-ttu-id="65371-p105">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="65371-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65371-123">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="65371-123">Permission type</span></span>      | <span data-ttu-id="65371-124">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="65371-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="65371-125">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="65371-125">Delegated (work or school account)</span></span> | <span data-ttu-id="65371-126">メール ReadBasic、Mail. 読み取り、ReadWrite</span><span class="sxs-lookup"><span data-stu-id="65371-126">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="65371-127">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="65371-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65371-128">メール ReadBasic、Mail. 読み取り、ReadWrite</span><span class="sxs-lookup"><span data-stu-id="65371-128">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="65371-129">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="65371-129">Application</span></span> | <span data-ttu-id="65371-130">-ReadBasic、mail. 読み取り、および書き込み</span><span class="sxs-lookup"><span data-stu-id="65371-130">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="65371-131">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="65371-131">HTTP request</span></span>

<span data-ttu-id="65371-132">ユーザーのメールボックス内のすべてのメッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="65371-132">To get all the messages in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
GET /users/{id | userPrincipalName}/messages
```

<span data-ttu-id="65371-133">ユーザーのメールボックス内の特定のフォルダーにあるメッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="65371-133">To get messages in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```

<span data-ttu-id="65371-134">ユーザーのメールボックス内のすべてのメッセージを取得するに\*\*\*\* は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="65371-134">To get all the messages in the user's mailbox that include a **mention** of the user:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages?$filter=mentionsPreview/isMentioned eq true
GET /users/{id | userPrincipalName}/messages?$filter=mentionsPreview/isMentioned eq true
```

## <a name="optional-query-parameters"></a><span data-ttu-id="65371-135">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="65371-135">Optional query parameters</span></span>
<span data-ttu-id="65371-136">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="65371-136">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="65371-137">`$filter` **MentionsPreview**プロパティの query パラメーターを使用すると、サインインしているユーザーを言及するメッセージを取得できます。</span><span class="sxs-lookup"><span data-stu-id="65371-137">You can use the `$filter` query parameter on the **mentionsPreview** property to get those messages that mention the signed-in user.</span></span>

## <a name="request-headers"></a><span data-ttu-id="65371-138">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="65371-138">Request headers</span></span>
| <span data-ttu-id="65371-139">名前</span><span class="sxs-lookup"><span data-stu-id="65371-139">Name</span></span>       | <span data-ttu-id="65371-140">型</span><span class="sxs-lookup"><span data-stu-id="65371-140">Type</span></span> | <span data-ttu-id="65371-141">説明</span><span class="sxs-lookup"><span data-stu-id="65371-141">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="65371-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="65371-142">Authorization</span></span>  | <span data-ttu-id="65371-143">string</span><span class="sxs-lookup"><span data-stu-id="65371-143">string</span></span>  | <span data-ttu-id="65371-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="65371-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="65371-146">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="65371-146">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="65371-147">string</span><span class="sxs-lookup"><span data-stu-id="65371-147">string</span></span> | <span data-ttu-id="65371-148">**body** プロパティと **uniqueBody** プロパティが返されるときの形式です。</span><span class="sxs-lookup"><span data-stu-id="65371-148">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="65371-149">値は、"text" または "html" になります。</span><span class="sxs-lookup"><span data-stu-id="65371-149">Values can be "text" or "html".</span></span> <span data-ttu-id="65371-150">ヘッダーが指定されていない場合は、**body** プロパティと **uniqueBody** プロパティは HTML 形式で返されます。</span><span class="sxs-lookup"><span data-stu-id="65371-150">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="65371-151">省略可能。</span><span class="sxs-lookup"><span data-stu-id="65371-151">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="65371-152">要求本文</span><span class="sxs-lookup"><span data-stu-id="65371-152">Request body</span></span>
<span data-ttu-id="65371-153">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="65371-153">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="65371-154">応答</span><span class="sxs-lookup"><span data-stu-id="65371-154">Response</span></span>

<span data-ttu-id="65371-155">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[message](../resources/message.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="65371-155">If successful, this method returns a `200 OK` response code and collection of [message](../resources/message.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65371-156">例</span><span class="sxs-lookup"><span data-stu-id="65371-156">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="65371-157">要求 1</span><span class="sxs-lookup"><span data-stu-id="65371-157">Request 1</span></span>
<span data-ttu-id="65371-158">最初の例では、サインインしているユーザーのメールボックス内の既定の上位10個のメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="65371-158">The first example gets the default, top 10 messages in the signed-in user's mailbox.</span></span> <span data-ttu-id="65371-159">`$select` を使用し、応答にメッセージごとのプロパティのサブセットを返します。</span><span class="sxs-lookup"><span data-stu-id="65371-159">It uses `$select` to return a subset of the properties of each message in the response.</span></span> 

# <a name="httptabhttp"></a>[<span data-ttu-id="65371-160">プロトコル</span><span class="sxs-lookup"><span data-stu-id="65371-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages?$select=sender,subject
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="65371-161">C#</span><span class="sxs-lookup"><span data-stu-id="65371-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-messages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="65371-162">Javascript</span><span class="sxs-lookup"><span data-stu-id="65371-162">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-messages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="65371-163">目的-C</span><span class="sxs-lookup"><span data-stu-id="65371-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-messages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="65371-164">Java</span><span class="sxs-lookup"><span data-stu-id="65371-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-messages-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-1"></a><span data-ttu-id="65371-165">応答 1</span><span class="sxs-lookup"><span data-stu-id="65371-165">Response 1</span></span>
<span data-ttu-id="65371-166">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="65371-166">Here is an example of the response.</span></span> <span data-ttu-id="65371-167">メッセージの次のページを取得するには、`@odata.nextLink`で返されるURL を後続の Get 要求に適用します。</span><span class="sxs-lookup"><span data-stu-id="65371-167">To get the next page of messages, apply the URL returned in `@odata.nextLink` to a subsequent GET request.</span></span>

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


##### <a name="request-2"></a><span data-ttu-id="65371-168">要求 2</span><span class="sxs-lookup"><span data-stu-id="65371-168">Request 2</span></span>
<span data-ttu-id="65371-169">次の例では、サインインしているユーザーのメールボックス内のすべてのメッセージに対して、ユーザーに言及するメッセージをフィルター処理します。</span><span class="sxs-lookup"><span data-stu-id="65371-169">The next example filters all messages in the signed-in user's mailbox for those that mention the user.</span></span> <span data-ttu-id="65371-170">また、を`$select`使用して、応答内の各メッセージのプロパティのサブセットを返します。</span><span class="sxs-lookup"><span data-stu-id="65371-170">It also uses `$select` to return a subset of the properties of each message in the response.</span></span> 

<span data-ttu-id="65371-171">この例では、クエリパラメーター文字列にスペース文字の URL エンコーディングも組み込まれています。</span><span class="sxs-lookup"><span data-stu-id="65371-171">The example also incorporates URL encoding for the space characters in the query parameter string.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="65371-172">プロトコル</span><span class="sxs-lookup"><span data-stu-id="65371-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_messages_with_mentions"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages?$filter=MentionsPreview/IsMentioned%20eq%20true&$select=Subject,Sender,ReceivedDateTime,MentionsPreview
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="65371-173">C#</span><span class="sxs-lookup"><span data-stu-id="65371-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-messages-with-mentions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="65371-174">Javascript</span><span class="sxs-lookup"><span data-stu-id="65371-174">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-messages-with-mentions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="65371-175">目的-C</span><span class="sxs-lookup"><span data-stu-id="65371-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-messages-with-mentions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="65371-176">Java</span><span class="sxs-lookup"><span data-stu-id="65371-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-messages-with-mentions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-2"></a><span data-ttu-id="65371-177">応答 2</span><span class="sxs-lookup"><span data-stu-id="65371-177">Response 2</span></span>
<span data-ttu-id="65371-p111">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="65371-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request-3"></a><span data-ttu-id="65371-181">要求 3</span><span class="sxs-lookup"><span data-stu-id="65371-181">Request 3</span></span>
<span data-ttu-id="65371-182">3番目の例では、 `Prefer: outlook.body-content-type="text"`ヘッダーを使用して、各メッセージの**本文**および**uniqueBody**プロパティをテキスト形式で取得する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="65371-182">The third example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** and **uniqueBody** properties of each message in text format.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="65371-183">プロトコル</span><span class="sxs-lookup"><span data-stu-id="65371-183">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_messages_in_text"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages?$select=subject,body,bodyPreview,uniqueBody
Prefer: outlook.body-content-type="text"
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="65371-184">C#</span><span class="sxs-lookup"><span data-stu-id="65371-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-messages-in-text-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="65371-185">Javascript</span><span class="sxs-lookup"><span data-stu-id="65371-185">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-messages-in-text-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="65371-186">目的-C</span><span class="sxs-lookup"><span data-stu-id="65371-186">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-messages-in-text-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="65371-187">Java</span><span class="sxs-lookup"><span data-stu-id="65371-187">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-messages-in-text-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-3"></a><span data-ttu-id="65371-188">応答 3</span><span class="sxs-lookup"><span data-stu-id="65371-188">Response 3</span></span>
<span data-ttu-id="65371-189">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="65371-189">Here is an example of the response.</span></span> 

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
  ]
}
-->
