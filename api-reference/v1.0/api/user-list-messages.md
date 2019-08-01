---
title: メッセージを一覧表示する
description: サインイン中のユーザーのメールボックス内のメッセージを取得します (削除済みアイテムと低優先メール フォルダーを含む)。
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: b53ec824e5dd368b0f563c5040270feef0f3ea7d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36026832"
---
# <a name="list-messages"></a><span data-ttu-id="84359-103">メッセージを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="84359-103">List messages</span></span>

<span data-ttu-id="84359-104">サインイン中のユーザーのメールボックス内のメッセージを取得します (削除済みアイテムと低優先メール フォルダーを含む)。</span><span class="sxs-lookup"><span data-stu-id="84359-104">Get the messages in the signed-in user's mailbox (including the Deleted Items and Clutter folders).</span></span>

<span data-ttu-id="84359-105">ページ サイズとメールボックスのデータに応じ、メールボックスから取得するメッセージは複数の要求を発生します。</span><span class="sxs-lookup"><span data-stu-id="84359-105">Depending on the page size and mailbox data, getting messages from a mailbox can incur multiple requests.</span></span> <span data-ttu-id="84359-106">ページ サイズの規定値は、10 件のメッセージです。</span><span class="sxs-lookup"><span data-stu-id="84359-106">The default page size is 10 messages.</span></span> <span data-ttu-id="84359-107">メッセージの次のページを取得するには、`@odata.nextLink`で返される URL 全体を単に次のメッセージ要求に適用するだけです。</span><span class="sxs-lookup"><span data-stu-id="84359-107">To get the next page of messages, simply apply the entire URL returned in `@odata.nextLink` to the next get-messages request.</span></span> <span data-ttu-id="84359-108">この URL は、最初の要求で指定された全てのクエリ パラメーターを含みます。</span><span class="sxs-lookup"><span data-stu-id="84359-108">This URL includes any query parameters you may have specified in the initial request.</span></span> 

<span data-ttu-id="84359-109">応答を操作するために`@odata.nextLink` URL から`$skip` 値を抽出しようとしないでください。</span><span class="sxs-lookup"><span data-stu-id="84359-109">Do not try to extract the `$skip` value from the `@odata.nextLink` URL to manipulate responses.</span></span> <span data-ttu-id="84359-110">この API は`$skip` 値を使用し、メッセージの種類の項目のページを返すためにユーザーのメールボックス内で確認された全ての項目をカウントし続けます。</span><span class="sxs-lookup"><span data-stu-id="84359-110">This API uses the `$skip` value to keep count of all the items it has gone through in the user's mailbox to return a page of message-type items.</span></span> <span data-ttu-id="84359-111">そのため、最初の要求の場合も`$skip` 値がページ サイズより大きくなる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="84359-111">It's therefore possible that even in the initial response, the `$skip` value is larger than the page size.</span></span> <span data-ttu-id="84359-112">詳細については、[アプリで Microsoft Graph データをページングする](/graph/paging)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="84359-112">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

<span data-ttu-id="84359-113">現在、この操作によって返されるメッセージの本文は HTML 形式のみです。</span><span class="sxs-lookup"><span data-stu-id="84359-113">Currently, this operation returns message bodies in only HTML format.</span></span>

<span data-ttu-id="84359-114">別のユーザーのメール フォルダーからアプリがメッセージを取得するシナリオは 2 つあります。</span><span class="sxs-lookup"><span data-stu-id="84359-114">There are two scenarios where an app can get messages in another user's mail folder:</span></span>

* <span data-ttu-id="84359-115">アプリにアプリケーションのアクセス許可がある場合。または</span><span class="sxs-lookup"><span data-stu-id="84359-115">If the app has application permissions, or,</span></span>
* <span data-ttu-id="84359-116">あるユーザーからアプリに適切な代理[アクセス許可](#permissions)が与えられ、別のユーザーがそのユーザーとメール フォルダーを共有しているか、そのユーザーに代理アクセスを付与している場合。</span><span class="sxs-lookup"><span data-stu-id="84359-116">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="84359-117">[詳細と例](/graph/outlook-share-messages-folders)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="84359-117">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

## <a name="permissions"></a><span data-ttu-id="84359-118">権限</span><span class="sxs-lookup"><span data-stu-id="84359-118">Permissions</span></span>
<span data-ttu-id="84359-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="84359-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84359-121">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="84359-121">Permission type</span></span>      | <span data-ttu-id="84359-122">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="84359-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="84359-123">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="84359-123">Delegated (work or school account)</span></span> | <span data-ttu-id="84359-124">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84359-124">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="84359-125">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="84359-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84359-126">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84359-126">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="84359-127">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="84359-127">Application</span></span> | <span data-ttu-id="84359-128">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84359-128">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="84359-129">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="84359-129">HTTP request</span></span>

<span data-ttu-id="84359-130">ユーザーのメールボックス内のすべてのメッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="84359-130">To get all the messages in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
GET /users/{id | userPrincipalName}/messages
```

<span data-ttu-id="84359-131">ユーザーのメールボックス内の特定のフォルダーにあるメッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="84359-131">To get messages in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="84359-132">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="84359-132">Optional query parameters</span></span>
<span data-ttu-id="84359-133">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="84359-133">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="84359-134">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="84359-134">Request headers</span></span>
| <span data-ttu-id="84359-135">名前</span><span class="sxs-lookup"><span data-stu-id="84359-135">Name</span></span>       | <span data-ttu-id="84359-136">種類</span><span class="sxs-lookup"><span data-stu-id="84359-136">Type</span></span> | <span data-ttu-id="84359-137">説明</span><span class="sxs-lookup"><span data-stu-id="84359-137">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="84359-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="84359-138">Authorization</span></span>  | <span data-ttu-id="84359-139">string</span><span class="sxs-lookup"><span data-stu-id="84359-139">string</span></span>  | <span data-ttu-id="84359-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="84359-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="84359-142">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="84359-142">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="84359-143">string</span><span class="sxs-lookup"><span data-stu-id="84359-143">string</span></span> | <span data-ttu-id="84359-144">**body** プロパティと **uniqueBody** プロパティが返されるときの形式です。</span><span class="sxs-lookup"><span data-stu-id="84359-144">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="84359-145">値は、"text" または "html" になります。</span><span class="sxs-lookup"><span data-stu-id="84359-145">Values can be "text" or "html".</span></span> <span data-ttu-id="84359-146">ヘッダーが指定されていない場合は、**body** プロパティと **uniqueBody** プロパティは HTML 形式で返されます。</span><span class="sxs-lookup"><span data-stu-id="84359-146">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="84359-147">省略可能。</span><span class="sxs-lookup"><span data-stu-id="84359-147">Optional.</span></span> |


## <a name="request-body"></a><span data-ttu-id="84359-148">要求本文</span><span class="sxs-lookup"><span data-stu-id="84359-148">Request body</span></span>
<span data-ttu-id="84359-149">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="84359-149">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="84359-150">応答</span><span class="sxs-lookup"><span data-stu-id="84359-150">Response</span></span>

<span data-ttu-id="84359-151">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Message](../resources/message.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="84359-151">If successful, this method returns a `200 OK` response code and collection of [Message](../resources/message.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84359-152">例</span><span class="sxs-lookup"><span data-stu-id="84359-152">Example</span></span>
##### <a name="request"></a><span data-ttu-id="84359-153">要求</span><span class="sxs-lookup"><span data-stu-id="84359-153">Request</span></span>
<span data-ttu-id="84359-154">この例では、サインイン済みのユーザーのメールボックスで、既定の上位10件のメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="84359-154">This example gets the default, top 10 messages in the signed-in user's mailbox.</span></span> <span data-ttu-id="84359-155">`$select` を使用し、応答にメッセージごとのプロパティのサブセットを返します。</span><span class="sxs-lookup"><span data-stu-id="84359-155">It uses `$select` to return a subset of the properties of each message in the response.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="84359-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="84359-156">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages?$select=sender,subject
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="84359-157">C#</span><span class="sxs-lookup"><span data-stu-id="84359-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-messages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="84359-158">Javascript</span><span class="sxs-lookup"><span data-stu-id="84359-158">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-messages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="84359-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="84359-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-messages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="84359-160">Java</span><span class="sxs-lookup"><span data-stu-id="84359-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-messages-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="84359-161">応答</span><span class="sxs-lookup"><span data-stu-id="84359-161">Response</span></span>
<span data-ttu-id="84359-162">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="84359-162">Here is an example of the response.</span></span> <span data-ttu-id="84359-163">メッセージの次のページを取得するには、`@odata.nextLink`で返されるURL を後続の Get 要求に適用します。</span><span class="sxs-lookup"><span data-stu-id="84359-163">To get the next page of messages, apply the URL returned in `@odata.nextLink` to a subsequent GET request.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('bb8775a4-4d8c-42cf-a1d4-4d58c2bb668f')/messages(sender,subject)",
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/messages?$select=sender%2csubject&$skip=14",
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
            "@odata.type": "#microsoft.graph.eventMessage",
            "@odata.etag": "W/\"DAAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAq4Dft\"",
            "id": "AAMkAGUAAAq5UMVAAA=",
            "subject": "Accepted: Review strategy for Q3",
            "sender": {
                "emailAddress": {
                    "name": "Adele Vance",
                    "address": "/O=EXCHANGELABS/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=A17A02BCF30C4937A87B14273385667C-ADELEV"
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.eventMessage",
            "@odata.etag": "W/\"DAAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAq4DfF\"",
            "id": "AAMkAGUAAAq5UMUAAA=",
            "subject": "Accepted: Review strategy for Q3",
            "sender": {
                "emailAddress": {
                    "name": "Adele Vance",
                    "address": "/O=EXCHANGELABS/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=A17A02BCF30C4937A87B14273385667C-ADELEV"
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.eventMessage",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
