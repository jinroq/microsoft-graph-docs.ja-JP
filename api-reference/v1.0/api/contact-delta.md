---
title: 'contact: delta'
description: 指定したフォルダーで追加、削除、更新された連絡先のセットを取得します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: bc919b40cbfb8b669ea4ad926e1bf166be610823
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35443141"
---
# <a name="contact-delta"></a><span data-ttu-id="8f24a-103">contact: delta</span><span class="sxs-lookup"><span data-stu-id="8f24a-103">contact: delta</span></span>

<span data-ttu-id="8f24a-104">指定したフォルダーで追加、削除、更新された連絡先のセットを取得します。</span><span class="sxs-lookup"><span data-stu-id="8f24a-104">Get a set of contacts that have been added, deleted, or updated in a specified folder.</span></span>

<span data-ttu-id="8f24a-p101">フォルダー内の連絡先に対する **デルタ** 関数呼び出しと GET 要求とは似ていますが、[状態トークン](/graph/delta-query-overview)をこれらの呼び出しに適切に適用することにより、そのフォルダーの連絡先の増分変更をクエリできる点が異なります。これにより、ユーザーの連絡先のローカル ストアの保守と同期を行う際に、連絡先のセット全体を毎回サーバーからフェッチする必要がなくなります。</span><span class="sxs-lookup"><span data-stu-id="8f24a-p101">A **delta** function call for contacts in a folder is similar to a GET request, except that by appropriately applying [state tokens](/graph/delta-query-overview) in one or more of these calls, you can query for incremental changes in the contacts in that folder. This allows you to maintain and synchronize a local store of a user's contacts without having to fetch the entire set of contacts from the server every time.</span></span>  

## <a name="permissions"></a><span data-ttu-id="8f24a-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8f24a-107">Permissions</span></span>
<span data-ttu-id="8f24a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8f24a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f24a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8f24a-110">Permission type</span></span>      | <span data-ttu-id="8f24a-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8f24a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8f24a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8f24a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8f24a-113">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8f24a-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="8f24a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8f24a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f24a-115">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8f24a-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="8f24a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8f24a-116">Application</span></span> | <span data-ttu-id="8f24a-117">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8f24a-117">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f24a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8f24a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}/contacts/delta
GET /users/{id}/contactFolders/{id}/contacts/delta
```

## <a name="query-parameters"></a><span data-ttu-id="8f24a-119">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="8f24a-119">Query parameters</span></span>

<span data-ttu-id="8f24a-p103">連絡先の変更を追跡すると、一連の**デルタ**関数呼び出しが発生します。任意のクエリ パラメーター (`$deltatoken` と `$skiptoken` 以外) を使用する場合は、最初の**デルタ**要求でこれを指定する必要があります。Microsoft Graph は、応答で提供される `nextLink` または `deltaLink` の URL のトークン部分に指定したパラメーターを自動的にエンコードします。必要なクエリ パラメーターを前もって指定しておくだけで済みます。それ以降の要求では、前の応答で `nextLink` または `deltaLink` の URL に必要なパラメーターが既にエンコードされ、含まれているため、この URL をコピーして適用します。</span><span class="sxs-lookup"><span data-stu-id="8f24a-p103">Tracking changes in contacts incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response. You only need to specify any desired query parameters once upfront. In subsequent requests, simply copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="8f24a-125">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="8f24a-125">Query parameter</span></span>      | <span data-ttu-id="8f24a-126">種類</span><span class="sxs-lookup"><span data-stu-id="8f24a-126">Type</span></span>   |<span data-ttu-id="8f24a-127">説明</span><span class="sxs-lookup"><span data-stu-id="8f24a-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8f24a-128">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="8f24a-128">$deltatoken</span></span> | <span data-ttu-id="8f24a-129">string</span><span class="sxs-lookup"><span data-stu-id="8f24a-129">string</span></span> | <span data-ttu-id="8f24a-p104">同じ連絡先コレクションの前の**デルタ**関数呼び出しの `deltaLink` URL で[状態トークン](/graph/delta-query-overview)が返され、変更追跡のその回が完了したことを示します。このコレクションについて、このトークンを含む `deltaLink` URL 全体を、変更追跡の次の回の最初の要求に保存し、適用します。</span><span class="sxs-lookup"><span data-stu-id="8f24a-p104">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same contact collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="8f24a-132">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="8f24a-132">$skiptoken</span></span> | <span data-ttu-id="8f24a-133">string</span><span class="sxs-lookup"><span data-stu-id="8f24a-133">string</span></span> | <span data-ttu-id="8f24a-134">前の**デルタ**関数呼び出しの `nextLink` URL で[状態トークン](/graph/delta-query-overview)が返され、同じ連絡先コレクションに追跡すべき変更が他にもあることを示します。</span><span class="sxs-lookup"><span data-stu-id="8f24a-134">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same contact collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="8f24a-135">OData クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="8f24a-135">OData query parameters</span></span>

- <span data-ttu-id="8f24a-p105">任意の GET リクエストと同様に `$select` クエリ パラメーターを使用して、最善のパフォーマンスを得るために必要なプロパティのみを指定することができます。_Id_ プロパティは常に返されます。</span><span class="sxs-lookup"><span data-stu-id="8f24a-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 


## <a name="request-headers"></a><span data-ttu-id="8f24a-138">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8f24a-138">Request headers</span></span>
| <span data-ttu-id="8f24a-139">名前</span><span class="sxs-lookup"><span data-stu-id="8f24a-139">Name</span></span>       | <span data-ttu-id="8f24a-140">型</span><span class="sxs-lookup"><span data-stu-id="8f24a-140">Type</span></span> | <span data-ttu-id="8f24a-141">説明</span><span class="sxs-lookup"><span data-stu-id="8f24a-141">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="8f24a-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f24a-142">Authorization</span></span>  | <span data-ttu-id="8f24a-143">string</span><span class="sxs-lookup"><span data-stu-id="8f24a-143">string</span></span>  | <span data-ttu-id="8f24a-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8f24a-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8f24a-146">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8f24a-146">Content-Type</span></span>  | <span data-ttu-id="8f24a-147">string</span><span class="sxs-lookup"><span data-stu-id="8f24a-147">string</span></span>  | <span data-ttu-id="8f24a-p107">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="8f24a-p107">application/json. Required.</span></span> |
| <span data-ttu-id="8f24a-150">Prefer</span><span class="sxs-lookup"><span data-stu-id="8f24a-150">Prefer</span></span> | <span data-ttu-id="8f24a-151">string</span><span class="sxs-lookup"><span data-stu-id="8f24a-151">string</span></span>  | <span data-ttu-id="8f24a-p108">odata.maxpagesize={x}.省略可能。</span><span class="sxs-lookup"><span data-stu-id="8f24a-p108">odata.maxpagesize={x}. Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="8f24a-154">応答</span><span class="sxs-lookup"><span data-stu-id="8f24a-154">Response</span></span>

<span data-ttu-id="8f24a-155">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [contact](../resources/contact.md) コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8f24a-155">If successful, this method returns a `200 OK` response code and [contact](../resources/contact.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f24a-156">例</span><span class="sxs-lookup"><span data-stu-id="8f24a-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8f24a-157">要求</span><span class="sxs-lookup"><span data-stu-id="8f24a-157">Request</span></span>
<span data-ttu-id="8f24a-158">**デルタ**関数の呼び出しを 1 つ作成し、`$select` パラメーターを使用して各連絡先の**displayName** プロパティのみを取得し、応答本文に含まれる連絡先の最大数を 2 に制限する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="8f24a-158">The following example shows how to make a single **delta** function call, use the `$select` parameter to get only each contact's **displayName** property, and limit the maximum number of contacts in the response body to 2.</span></span>

<span data-ttu-id="8f24a-159">フォルダー内の連絡先の変更を追跡するには、1 つ以上の**デルタ**関数呼び出しを作成し、適切な状態トークンを使用して、前回のデルタ クエリ以降になされた一連の増分変更を取得します。</span><span class="sxs-lookup"><span data-stu-id="8f24a-159">To track changes in the contacts in a folder, you would make one or more **delta** function calls, with appropriate state tokens, to get the set of incremental changes since the last delta query.</span></span> 

<span data-ttu-id="8f24a-p109">メール フォルダー内のメッセージ変更を追跡するために状態トークンを使用する方法を示す同様の例については、次をご覧ください。[フォルダー内のメッセージへの増分の変更を取得する](/graph/delta-query-messages)。フォルダー内の連絡先の追跡とメッセージの追跡の主な違いは、デルタ クエリ要求 URL のほかに、クエリ応答で**メッセージ** コレクションではなく **contact** が返されることです。</span><span class="sxs-lookup"><span data-stu-id="8f24a-p109">You can find a similar example that shows how to use the state tokens to track changes in the messages of a mail folder: [Get incremental changes to messages in a folder](/graph/delta-query-messages). The main differences between tracking contacts and tracking messages in a folder are in the delta query request URLs, and the query responses returning **contact** rather than **message** collections.</span></span>
 

# <a name="httptabhttp"></a>[<span data-ttu-id="8f24a-162">プロトコル</span><span class="sxs-lookup"><span data-stu-id="8f24a-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contact_delta"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contactFolders/{id}/contacts/delta?$select=displayName
Prefer: odata.maxpagesize=2
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8f24a-163">C#</span><span class="sxs-lookup"><span data-stu-id="8f24a-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contact-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8f24a-164">Javascript</span><span class="sxs-lookup"><span data-stu-id="8f24a-164">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contact-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8f24a-165">目的-C</span><span class="sxs-lookup"><span data-stu-id="8f24a-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contact-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8f24a-166">応答</span><span class="sxs-lookup"><span data-stu-id="8f24a-166">Response</span></span>
<span data-ttu-id="8f24a-167">要求が成功すると、応答には状態トークンが含まれます。これは、_skipToken_</span><span class="sxs-lookup"><span data-stu-id="8f24a-167">If the request is successful, the response would include a state token, which is either a _skipToken_</span></span>  
<span data-ttu-id="8f24a-p110">(_@odata.nextLink_ 応答ヘッダーに含まれる) か、_deltaToken_ (_@odata.deltaLink_ 応答ヘッダーに含まれる) のいずれかになります。前者はその回を続行する必要があることを示し、後者はその回のすべての変更の取得が完了したことを示します。</span><span class="sxs-lookup"><span data-stu-id="8f24a-p110">(in an _@odata.nextLink_ response header) or a _deltaToken_ (in an _@odata.deltaLink_ response header). Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="8f24a-170">以下の応答は、_@odata.nextLink_ 応答ヘッダーに含まれる _skipToken_ を示しています。</span><span class="sxs-lookup"><span data-stu-id="8f24a-170">The response below shows a _skipToken_ in an _@odata.nextLink_ response header.</span></span>

<span data-ttu-id="8f24a-p111">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8f24a-p111">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 337

{
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/me/contactfolders('{id}')/contacts/delta?$skiptoken={_skipToken_}",
  "value": [
    {
      "parentFolderId": "parentFolderId-value",
      "birthday": "2016-10-19T10:37:00Z",
      "fileAs": "fileAs-value",
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "initials": "initials-value"
    }
  ]
}
```

### <a name="see-also"></a><span data-ttu-id="8f24a-173">関連項目</span><span class="sxs-lookup"><span data-stu-id="8f24a-173">See also</span></span>

- [<span data-ttu-id="8f24a-174">デルタ クエリを使用して、Microsoft Graph データの変更を追跡する</span><span class="sxs-lookup"><span data-stu-id="8f24a-174">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="8f24a-175">フォルダー内のメッセージへの増分の変更を取得する</span><span class="sxs-lookup"><span data-stu-id="8f24a-175">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contact: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
