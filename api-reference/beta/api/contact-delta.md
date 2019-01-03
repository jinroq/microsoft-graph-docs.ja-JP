---
title: 'contact: delta'
description: 指定したフォルダーで追加、削除、更新された連絡先のセットを取得します。
ms.openlocfilehash: 1e97a59de7abec0c69a5e02559081f7b344ebad0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071045"
---
# <a name="contact-delta"></a><span data-ttu-id="a03c0-103">contact: delta</span><span class="sxs-lookup"><span data-stu-id="a03c0-103">contact: delta</span></span>

> <span data-ttu-id="a03c0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a03c0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a03c0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a03c0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a03c0-106">指定したフォルダーで追加、削除、更新された連絡先のセットを取得します。</span><span class="sxs-lookup"><span data-stu-id="a03c0-106">Get a set of contacts that have been added, deleted, or updated in a specified folder.</span></span>

<span data-ttu-id="a03c0-p102">フォルダー内の連絡先に対する **デルタ** 関数呼び出しと GET 要求とは似ていますが、[状態トークン](/graph/delta-query-overview)をこれらの呼び出しに適切に適用することにより、そのフォルダーの連絡先の増分変更をクエリできる点が異なります。これにより、ユーザーの連絡先のローカル ストアの保守と同期を行う際に、連絡先のセット全体を毎回サーバーからフェッチする必要がなくなります。</span><span class="sxs-lookup"><span data-stu-id="a03c0-p102">A **delta** function call for contacts in a folder is similar to a GET request, except that by appropriately applying [state tokens](/graph/delta-query-overview) in one or more of these calls, you can query for incremental changes in the contacts in that folder. This allows you to maintain and synchronize a local store of a user's contacts without having to fetch the entire set of contacts from the server every time.</span></span>  

## <a name="permissions"></a><span data-ttu-id="a03c0-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a03c0-109">Permissions</span></span>
<span data-ttu-id="a03c0-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a03c0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a03c0-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a03c0-112">Permission type</span></span>      | <span data-ttu-id="a03c0-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a03c0-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a03c0-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a03c0-114">Delegated (work or school account)</span></span> | <span data-ttu-id="a03c0-115">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a03c0-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a03c0-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a03c0-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a03c0-117">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a03c0-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a03c0-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a03c0-118">Application</span></span> | <span data-ttu-id="a03c0-119">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a03c0-119">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a03c0-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a03c0-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}/contacts/delta
GET /users/<id>/contactFolders/{id}/contacts/delta
```

## <a name="query-parameters"></a><span data-ttu-id="a03c0-121">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="a03c0-121">Query parameters</span></span>

<span data-ttu-id="a03c0-p104">連絡先の変更を追跡すると、一連の**デルタ**関数呼び出しが発生します。任意のクエリ パラメーター (`$deltatoken` と `$skiptoken` 以外) を使用する場合は、最初の**デルタ**要求でこれを指定する必要があります。Microsoft Graph は、応答で提供される `nextLink` または `deltaLink` の URL のトークン部分に指定したパラメーターを自動的にエンコードします。必要なクエリ パラメーターを前もって指定しておくだけで済みます。それ以降の要求では、前の応答で `nextLink` または `deltaLink` の URL に必要なパラメーターが既にエンコードされ、含まれているため、この URL をコピーして適用します。</span><span class="sxs-lookup"><span data-stu-id="a03c0-p104">Tracking changes in contacts incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response. You only need to specify any desired query parameters once upfront. In subsequent requests, simply copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="a03c0-127">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="a03c0-127">Query parameter</span></span>      | <span data-ttu-id="a03c0-128">種類</span><span class="sxs-lookup"><span data-stu-id="a03c0-128">Type</span></span>   |<span data-ttu-id="a03c0-129">説明</span><span class="sxs-lookup"><span data-stu-id="a03c0-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a03c0-130">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="a03c0-130">$deltatoken</span></span> | <span data-ttu-id="a03c0-131">文字列</span><span class="sxs-lookup"><span data-stu-id="a03c0-131">string</span></span> | <span data-ttu-id="a03c0-p105">同じ連絡先コレクションの前の**デルタ**関数呼び出しの `deltaLink` URL で[状態トークン](/graph/delta-query-overview)が返され、変更追跡のその回が完了したことを示します。このコレクションについて、このトークンを含む `deltaLink` URL 全体を、変更追跡の次の回の最初の要求に保存し、適用します。</span><span class="sxs-lookup"><span data-stu-id="a03c0-p105">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same contact collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="a03c0-134">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="a03c0-134">$skiptoken</span></span> | <span data-ttu-id="a03c0-135">文字列</span><span class="sxs-lookup"><span data-stu-id="a03c0-135">string</span></span> | <span data-ttu-id="a03c0-136">前の**デルタ**関数呼び出しの `nextLink` URL で[状態トークン](/graph/delta-query-overview)が返され、同じ連絡先コレクションに追跡すべき変更が他にもあることを示します。</span><span class="sxs-lookup"><span data-stu-id="a03c0-136">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same contact collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="a03c0-137">OData クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="a03c0-137">OData query parameters</span></span>

- <span data-ttu-id="a03c0-p106">任意の GET リクエストと同様に `$select` クエリ パラメーターを使用して、最善のパフォーマンスを得るために必要なプロパティのみを指定することができます。_Id_ プロパティは常に返されます。</span><span class="sxs-lookup"><span data-stu-id="a03c0-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 


## <a name="request-headers"></a><span data-ttu-id="a03c0-140">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a03c0-140">Request headers</span></span>
| <span data-ttu-id="a03c0-141">名前</span><span class="sxs-lookup"><span data-stu-id="a03c0-141">Name</span></span>       | <span data-ttu-id="a03c0-142">型</span><span class="sxs-lookup"><span data-stu-id="a03c0-142">Type</span></span> | <span data-ttu-id="a03c0-143">説明</span><span class="sxs-lookup"><span data-stu-id="a03c0-143">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="a03c0-144">Authorization</span><span class="sxs-lookup"><span data-stu-id="a03c0-144">Authorization</span></span>  | <span data-ttu-id="a03c0-145">string</span><span class="sxs-lookup"><span data-stu-id="a03c0-145">string</span></span>  | <span data-ttu-id="a03c0-p107">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a03c0-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a03c0-148">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a03c0-148">Content-Type</span></span>  | <span data-ttu-id="a03c0-149">string</span><span class="sxs-lookup"><span data-stu-id="a03c0-149">string</span></span>  | <span data-ttu-id="a03c0-p108">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="a03c0-p108">application/json. Required.</span></span> |
| <span data-ttu-id="a03c0-152">Prefer</span><span class="sxs-lookup"><span data-stu-id="a03c0-152">Prefer</span></span> | <span data-ttu-id="a03c0-153">文字列</span><span class="sxs-lookup"><span data-stu-id="a03c0-153">string</span></span>  | <span data-ttu-id="a03c0-p109">odata.maxpagesize={x}.省略可能。</span><span class="sxs-lookup"><span data-stu-id="a03c0-p109">odata.maxpagesize={x}. Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="a03c0-156">応答</span><span class="sxs-lookup"><span data-stu-id="a03c0-156">Response</span></span>

<span data-ttu-id="a03c0-157">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [contact](../resources/contact.md) コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a03c0-157">If successful, this method returns a `200 OK` response code and [contact](../resources/contact.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a03c0-158">例</span><span class="sxs-lookup"><span data-stu-id="a03c0-158">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a03c0-159">要求</span><span class="sxs-lookup"><span data-stu-id="a03c0-159">Request</span></span>
<span data-ttu-id="a03c0-160">**デルタ**関数の呼び出しを 1 つ作成し、`$select` パラメーターを使用して各連絡先の**displayName** プロパティのみを取得し、応答本文に含まれる連絡先の最大数を 2 に制限する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="a03c0-160">The following example shows how to make a single **delta** function call, use the `$select` parameter to get only each contact's **displayName** property, and limit the maximum number of contacts in the response body to 2.</span></span>

<span data-ttu-id="a03c0-161">フォルダー内の連絡先の変更を追跡するには、1 つ以上の**デルタ**関数呼び出しを作成し、適切な状態トークンを使用して、前回のデルタ クエリ以降になされた一連の増分変更を取得します。</span><span class="sxs-lookup"><span data-stu-id="a03c0-161">To track changes in the contacts in a folder, you would make one or more **delta** function calls, with appropriate state tokens, to get the set of incremental changes since the last delta query.</span></span> 

<span data-ttu-id="a03c0-p110">メール フォルダー内のメッセージ変更を追跡するために状態トークンを使用する方法を示す同様の例については、次をご覧ください。[フォルダー内のメッセージへの増分の変更を取得する](/graph/delta-query-messages)。フォルダー内の連絡先の追跡とメッセージの追跡の主な違いは、デルタ クエリ要求 URL のほかに、クエリ応答で**メッセージ** コレクションではなく **contact** が返されることです。</span><span class="sxs-lookup"><span data-stu-id="a03c0-p110">You can find a similar example that shows how to use the state tokens to track changes in the messages of a mail folder: [Get incremental changes to messages in a folder](/graph/delta-query-messages). The main differences between tracking contacts and tracking messages in a folder are in the delta query request URLs, and the query responses returning **contact** rather than **message** collections.</span></span>
 
<!-- {
  "blockType": "request",
  "name": "contact_delta"
}-->
```http
GET https://graph.microsoft.com/beta/me/contactFolders/{id}/contacts/delta?$select=displayName

Prefer: odata.maxpagesize=2
```

##### <a name="response"></a><span data-ttu-id="a03c0-164">応答</span><span class="sxs-lookup"><span data-stu-id="a03c0-164">Response</span></span>
<span data-ttu-id="a03c0-165">要求が成功すると、応答には状態トークンが含まれます。これは、_skipToken_</span><span class="sxs-lookup"><span data-stu-id="a03c0-165">If the request is successful, the response would include a state token, which is either a _skipToken_</span></span>  
<span data-ttu-id="a03c0-p111">(_@odata.nextLink_ 応答ヘッダーに含まれる) か、_deltaToken_ (_@odata.deltaLink_ 応答ヘッダーに含まれる) のいずれかになります。前者はその回を続行する必要があることを示し、後者はその回のすべての変更の取得が完了したことを示します。</span><span class="sxs-lookup"><span data-stu-id="a03c0-p111">(in an _@odata.nextLink_ response header) or a _deltaToken_ (in an _@odata.deltaLink_ response header). Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="a03c0-168">以下の応答は、_@odata.nextLink_ 応答ヘッダーに含まれる _skipToken_ を示しています。</span><span class="sxs-lookup"><span data-stu-id="a03c0-168">The response below shows a _skipToken_ in an _@odata.nextLink_ response header.</span></span>

<span data-ttu-id="a03c0-p112">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a03c0-p112">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.nextLink":"https://graph.microsoft.com/beta/me/contactfolders('{id}')/contacts/delta?$skiptoken={_skipToken_}",
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

### <a name="see-also"></a><span data-ttu-id="a03c0-171">関連項目</span><span class="sxs-lookup"><span data-stu-id="a03c0-171">See also</span></span>

- [<span data-ttu-id="a03c0-172">Microsoft Graph デルタ クエリ</span><span class="sxs-lookup"><span data-stu-id="a03c0-172">Microsoft Graph delta query</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="a03c0-173">フォルダー内のメッセージへの増分の変更を取得する</span><span class="sxs-lookup"><span data-stu-id="a03c0-173">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contact: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->