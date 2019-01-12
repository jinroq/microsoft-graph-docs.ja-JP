---
title: 'message: delta'
description: 指定したフォルダーで追加、削除、更新されたメッセージのセットを取得します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7344b53e69916870e1c2705d6b251be2fff61721
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980525"
---
# <a name="message-delta"></a><span data-ttu-id="2f597-103">message: delta</span><span class="sxs-lookup"><span data-stu-id="2f597-103">message: delta</span></span>

> <span data-ttu-id="2f597-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2f597-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2f597-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2f597-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2f597-106">指定したフォルダーで追加、削除、更新されたメッセージのセットを取得します。</span><span class="sxs-lookup"><span data-stu-id="2f597-106">Get a set of messages that have been added, deleted, or updated in a specified folder.</span></span>

<span data-ttu-id="2f597-p102">フォルダー内のメッセージに対する**デルタ**関数呼び出しと GET 要求とは似ていますが、[状態トークン](/graph/delta-query-overview)をこれらの 1 つ以上の呼び出しに適切に適用することにより、[そのフォルダーのメッセージの増分の変更をクエリできる](/graph/delta-query-messages)点が異なります。これにより、ユーザーのメッセージのローカル ストアの保守と同期を行う際に、メッセージのセット全体を毎回サーバーからフェッチする必要がなくなります。</span><span class="sxs-lookup"><span data-stu-id="2f597-p102">A **delta** function call for messages in a folder is similar to a GET request, except that by appropriately applying [state tokens](/graph/delta-query-overview) in one or more of these calls, you can [query for incremental changes in the messages in that folder](/graph/delta-query-messages). This allows you to maintain and synchronize a local store of a user's messages without having to fetch the entire set of messages from the server every time.</span></span>  

## <a name="permissions"></a><span data-ttu-id="2f597-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2f597-109">Permissions</span></span>
<span data-ttu-id="2f597-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2f597-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f597-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2f597-112">Permission type</span></span>      | <span data-ttu-id="2f597-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2f597-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2f597-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2f597-114">Delegated (work or school account)</span></span> | <span data-ttu-id="2f597-115">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2f597-115">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="2f597-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2f597-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f597-117">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2f597-117">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="2f597-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2f597-118">Application</span></span> | <span data-ttu-id="2f597-119">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2f597-119">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="2f597-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2f597-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages/delta
GET /users/<id>/mailFolders/{id}/messages/delta
```

## <a name="query-parameters"></a><span data-ttu-id="2f597-121">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="2f597-121">Query parameters</span></span>

<span data-ttu-id="2f597-p104">メッセージの変更を追跡すると、1 つ以上の**デルタ**関数呼び出しのラウンドが発生します。任意のクエリ パラメーター (`$deltatoken` と `$skiptoken` 以外) を使用する場合は、最初の**デルタ**要求でこれを指定する必要があります。Microsoft Graph は、応答で提供される `nextLink` や `deltaLink` の URL のトークン部分に指定したパラメーターを自動的にエンコードします。必要なクエリ パラメーターを前もって指定しておくだけで済みます。それ以降の要求では、前の応答で `nextLink` や `deltaLink` の URL に必要なパラメーターが既にエンコードされ、含まれているため、この URL をコピーして適用するだけです。</span><span class="sxs-lookup"><span data-stu-id="2f597-p104">Tracking changes in messages incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response. You only need to specify any desired query parameters once upfront. In subsequent requests, simply copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="2f597-127">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="2f597-127">Query parameter</span></span>      | <span data-ttu-id="2f597-128">種類</span><span class="sxs-lookup"><span data-stu-id="2f597-128">Type</span></span>   |<span data-ttu-id="2f597-129">説明</span><span class="sxs-lookup"><span data-stu-id="2f597-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2f597-130">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="2f597-130">$deltatoken</span></span> | <span data-ttu-id="2f597-131">string</span><span class="sxs-lookup"><span data-stu-id="2f597-131">string</span></span> | <span data-ttu-id="2f597-p105">同じメッセージ コレクションの前の**デルタ**関数呼び出しの `deltaLink` URL で[状態トークン](/graph/delta-query-overview)が返され、その変更追跡のラウンドが完了したことを示します。このコレクションについて、このトークンを含む、`deltaLink` URL 全体を次の変更追跡のラウンドの最初の要求に保存し、適用します。</span><span class="sxs-lookup"><span data-stu-id="2f597-p105">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same message collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="2f597-134">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="2f597-134">$skiptoken</span></span> | <span data-ttu-id="2f597-135">string</span><span class="sxs-lookup"><span data-stu-id="2f597-135">string</span></span> | <span data-ttu-id="2f597-136">前の**デルタ**関数呼び出しの `nextLink` URL で[状態トークン](/graph/delta-query-overview)が返され、同じメッセージ コレクションに追跡すべき変更が他にもあることを示します。</span><span class="sxs-lookup"><span data-stu-id="2f597-136">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same message collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="2f597-137">OData クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="2f597-137">OData query parameters</span></span>

- <span data-ttu-id="2f597-p106">任意の GET リクエストと同様に `$select` クエリ パラメーターを使用して、最善のパフォーマンスを得るために必要なプロパティのみを指定することができます。_Id_ プロパティは常に返されます。</span><span class="sxs-lookup"><span data-stu-id="2f597-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 
- <span data-ttu-id="2f597-140">デルタ クエリは、メッセージの `$select`、`$top`、および `$expand` をサポートします。</span><span class="sxs-lookup"><span data-stu-id="2f597-140">Delta query support `$select`, `$top`, and `$expand` for messages.</span></span> 
- <span data-ttu-id="2f597-141">`$filter` と `$orderby` に対するサポートには制限があります。</span><span class="sxs-lookup"><span data-stu-id="2f597-141">There is limited support for `$filter` and `$orderby`:</span></span>
  * <span data-ttu-id="2f597-142">サポートされている唯一の `$filter` 式は、`$filter=receivedDateTime+ge+{value}` または `$filter=receivedDateTime+gt+{value}` です。</span><span class="sxs-lookup"><span data-stu-id="2f597-142">The only supported `$filter` expresssions are `$filter=receivedDateTime+ge+{value}` or `$filter=receivedDateTime+gt+{value}`.</span></span>
  * <span data-ttu-id="2f597-p107">サポートされている唯一の `$orderby` 式は、`$orderby=receivedDateTime+desc` です。`$orderby` 式を含めない場合、戻り値の順序は保証されません。</span><span class="sxs-lookup"><span data-stu-id="2f597-p107">The only supported `$orderby` expression is `$orderby=receivedDateTime+desc`. If you do not include an `$orderby` expression, the return order is not guaranteed.</span></span> 
- <span data-ttu-id="2f597-145">`$search` はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2f597-145">There is no support for `$search`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2f597-146">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2f597-146">Request headers</span></span>
| <span data-ttu-id="2f597-147">名前</span><span class="sxs-lookup"><span data-stu-id="2f597-147">Name</span></span>       | <span data-ttu-id="2f597-148">型</span><span class="sxs-lookup"><span data-stu-id="2f597-148">Type</span></span> | <span data-ttu-id="2f597-149">説明</span><span class="sxs-lookup"><span data-stu-id="2f597-149">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="2f597-150">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f597-150">Authorization</span></span>  | <span data-ttu-id="2f597-151">string</span><span class="sxs-lookup"><span data-stu-id="2f597-151">string</span></span>  | <span data-ttu-id="2f597-p108">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2f597-p108">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2f597-154">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2f597-154">Content-Type</span></span>  | <span data-ttu-id="2f597-155">string</span><span class="sxs-lookup"><span data-stu-id="2f597-155">string</span></span>  | <span data-ttu-id="2f597-p109">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="2f597-p109">application/json. Required.</span></span> |
| <span data-ttu-id="2f597-158">Prefer</span><span class="sxs-lookup"><span data-stu-id="2f597-158">Prefer</span></span> | <span data-ttu-id="2f597-159">文字列</span><span class="sxs-lookup"><span data-stu-id="2f597-159">string</span></span>  | <span data-ttu-id="2f597-p110">odata.maxpagesize={x}.省略可能。</span><span class="sxs-lookup"><span data-stu-id="2f597-p110">odata.maxpagesize={x}. Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="2f597-162">応答</span><span class="sxs-lookup"><span data-stu-id="2f597-162">Response</span></span>

<span data-ttu-id="2f597-163">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [message](../resources/message.md) コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2f597-163">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f597-164">例</span><span class="sxs-lookup"><span data-stu-id="2f597-164">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2f597-165">要求</span><span class="sxs-lookup"><span data-stu-id="2f597-165">Request</span></span>
<span data-ttu-id="2f597-166">次の例に、**デルタ**関数呼び出しを 1 つ作成し、応答本文に含まれるメッセージの最大数を 2 に制限する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="2f597-166">The following example shows how to make a single **delta** function call, and limit the maximum number of messages in the response body to 2.</span></span>

<span data-ttu-id="2f597-p111">フォルダー内のメッセージの変更を追跡するには、1 つ以上の**デルタ**関数呼び出しを作成し、前回のデルタ クエリ以降になされた一連の増分の変更を取得します。デルタ クエリ呼び出しのラウンドを示す例については、「[フォルダー内のメッセージへの増分の変更を取得する](/graph/delta-query-messages)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="2f597-p111">To track changes in the messages in a folder, you would make one or more **delta** function calls to get the set of incremental changes since the last delta query. For an example that shows a round of delta query calls, see [Get incremental changes to messages in a folder](/graph/delta-query-messages).</span></span>
 
<!-- {
  "blockType": "request",
  "name": "message_delta"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders/{id}/messages/delta

Prefer: odata.maxpagesize=2
```

##### <a name="response"></a><span data-ttu-id="2f597-169">応答</span><span class="sxs-lookup"><span data-stu-id="2f597-169">Response</span></span>
<span data-ttu-id="2f597-170">要求が成功すると、応答には状態トークンが含まれます。これは、_skipToken_</span><span class="sxs-lookup"><span data-stu-id="2f597-170">If the request is successful, the response would include a state token, which is either a _skipToken_</span></span>  
<span data-ttu-id="2f597-p112">(_@odata.nextLink_ 応答ヘッダーに含まれる) か、_deltaToken_ (_@odata.deltaLink_ 応答ヘッダーに含まれる) のいずれかになります。前者はその回を続行する必要があることを示し、後者はその回のすべての変更の取得が完了したことを示します。</span><span class="sxs-lookup"><span data-stu-id="2f597-p112">(in an _@odata.nextLink_ response header) or a _deltaToken_ (in an _@odata.deltaLink_ response header). Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="2f597-173">以下の応答は、_@odata.nextLink_ 応答ヘッダーに含まれる _skipToken_ を示しています。</span><span class="sxs-lookup"><span data-stu-id="2f597-173">The response below shows a _skipToken_ in an _@odata.nextLink_ response header.</span></span>

<span data-ttu-id="2f597-p113">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2f597-p113">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 337

{
  "@odata.nextLink":"https://graph.microsoft.com/beta/me/mailfolders('{id}')/messages/delta?$skiptoken={_skipToken_}",
  "value": [
    {
      "receivedDateTime": "datetime-value",
      "sentDateTime": "datetime-value",
      "hasAttachments": true,
      "internetMessageId": "internetMessageId-value",
      "subject": "subject-value",
      "body": {
        "contentType": "contentType-value",
        "content": "content-value"
      }
    }
  ]
}
```

### <a name="see-also"></a><span data-ttu-id="2f597-176">関連項目</span><span class="sxs-lookup"><span data-stu-id="2f597-176">See also</span></span>

- [<span data-ttu-id="2f597-177">Microsoft Graph デルタ クエリ</span><span class="sxs-lookup"><span data-stu-id="2f597-177">Microsoft Graph delta query</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="2f597-178">フォルダー内のメッセージへの増分の変更を取得する</span><span class="sxs-lookup"><span data-stu-id="2f597-178">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
