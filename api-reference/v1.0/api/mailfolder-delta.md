---
title: 'mailFolder: delta'
description: ユーザーのメールボックスで追加または削除された一連のメール フォルダーを取得します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: bf7b935b8354bf01cd3a612dd5178a96ef74d00c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27965720"
---
# <a name="mailfolder-delta"></a><span data-ttu-id="ff9a7-103">mailFolder: delta</span><span class="sxs-lookup"><span data-stu-id="ff9a7-103">mailFolder: delta</span></span>

<span data-ttu-id="ff9a7-104">ユーザーのメールボックスで追加または削除された一連のメール フォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="ff9a7-104">Get a set of mail folders that have been added, deleted, or removed from the user's mailbox.</span></span>

<span data-ttu-id="ff9a7-p101">メールボックス内のメール フォルダーに対する**デルタ**関数の呼び出しと GET 要求とは似ていますが、[状態トークン](/graph/delta-query-overview)をこれらの呼び出しに適切に適用することにより、メール フォルダーの増分の変更をクエリできる点が異なります。これにより、ユーザーのメール フォルダーのローカル ストアの保守と同期を行う際に、そのメールボックスのメール フォルダーすべてを毎回サーバーからフェッチする必要がなくなります。</span><span class="sxs-lookup"><span data-stu-id="ff9a7-p101">A **delta** function call for mail folders in a mailbox is similar to a GET request, except that by appropriately applying [state tokens](/graph/delta-query-overview) in one or more of these calls, you can query for incremental changes in the mail folders. This allows you to maintain and synchronize a local store of a user's mail folders without having to fetch all the mail folders of that mailbox from the server every time.</span></span>

## <a name="permissions"></a><span data-ttu-id="ff9a7-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ff9a7-107">Permissions</span></span>
<span data-ttu-id="ff9a7-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ff9a7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ff9a7-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ff9a7-110">Permission type</span></span>      | <span data-ttu-id="ff9a7-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ff9a7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ff9a7-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ff9a7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ff9a7-113">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ff9a7-113">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ff9a7-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ff9a7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff9a7-115">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ff9a7-115">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ff9a7-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ff9a7-116">Application</span></span> | <span data-ttu-id="ff9a7-117">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ff9a7-117">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff9a7-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ff9a7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/delta
GET /users/{id}/mailFolders/delta
```

## <a name="query-parameters"></a><span data-ttu-id="ff9a7-119">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ff9a7-119">Query parameters</span></span>

<span data-ttu-id="ff9a7-p103">メール フォルダーの変更を追跡すると、1 つ以上の **デルタ**関数呼び出しのラウンドが発生します。任意のクエリ パラメーター (`$deltatoken` と `$skiptoken` 以外) を使用する場合は、最初の**デルタ**要求でこれを指定する必要があります。Microsoft Graph は、応答で提供される `nextLink` や `deltaLink` の URL のトークン部分に指定したパラメーターを自動的にエンコードします。必要なクエリ パラメーターを前もって指定しておくだけで済みます。それ以降の要求では、前の応答で `nextLink` や `deltaLink` の URL に必要なパラメーターが既にエンコードされ、含まれているため、この URL をコピーして適用するだけです。</span><span class="sxs-lookup"><span data-stu-id="ff9a7-p103">Tracking changes in mail folders incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response. You only need to specify any desired query parameters once upfront. In subsequent requests, simply copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="ff9a7-125">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ff9a7-125">Query parameter</span></span>      | <span data-ttu-id="ff9a7-126">種類</span><span class="sxs-lookup"><span data-stu-id="ff9a7-126">Type</span></span>   |<span data-ttu-id="ff9a7-127">説明</span><span class="sxs-lookup"><span data-stu-id="ff9a7-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ff9a7-128">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="ff9a7-128">$deltatoken</span></span> | <span data-ttu-id="ff9a7-129">文字列</span><span class="sxs-lookup"><span data-stu-id="ff9a7-129">string</span></span> | <span data-ttu-id="ff9a7-p104">同じメール フォルダー コレクションの前の**デルタ**関数呼び出しの `deltaLink` URL で[状態トークン](/graph/delta-query-overview)が返され、その変更追跡のラウンドが完了したことを示します。このコレクションについて、このトークンを含む、`deltaLink` URL 全体を次の変更追跡のラウンドの最初の要求に保存し、適用します。</span><span class="sxs-lookup"><span data-stu-id="ff9a7-p104">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same mail folder collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="ff9a7-132">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="ff9a7-132">$skiptoken</span></span> | <span data-ttu-id="ff9a7-133">文字列</span><span class="sxs-lookup"><span data-stu-id="ff9a7-133">string</span></span> | <span data-ttu-id="ff9a7-134">前の**デルタ**関数呼び出しの `nextLink` URL で[状態トークン](/graph/delta-query-overview)が返され、同じメール フォルダー コレクションに追跡すべき変更が他にもあることを示します。</span><span class="sxs-lookup"><span data-stu-id="ff9a7-134">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same mail folder collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="ff9a7-135">OData クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ff9a7-135">OData query parameters</span></span>

<span data-ttu-id="ff9a7-p105">任意の GET リクエストと同様に `$select` クエリ パラメーターを使用して、最善のパフォーマンスを得るために必要なプロパティのみを指定することができます。_Id_ プロパティは常に返されます。</span><span class="sxs-lookup"><span data-stu-id="ff9a7-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="ff9a7-138">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ff9a7-138">Request headers</span></span>
| <span data-ttu-id="ff9a7-139">名前</span><span class="sxs-lookup"><span data-stu-id="ff9a7-139">Name</span></span>       | <span data-ttu-id="ff9a7-140">型</span><span class="sxs-lookup"><span data-stu-id="ff9a7-140">Type</span></span> | <span data-ttu-id="ff9a7-141">説明</span><span class="sxs-lookup"><span data-stu-id="ff9a7-141">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="ff9a7-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff9a7-142">Authorization</span></span>  | <span data-ttu-id="ff9a7-143">string</span><span class="sxs-lookup"><span data-stu-id="ff9a7-143">string</span></span>  | <span data-ttu-id="ff9a7-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ff9a7-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ff9a7-146">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ff9a7-146">Content-Type</span></span>  | <span data-ttu-id="ff9a7-147">string</span><span class="sxs-lookup"><span data-stu-id="ff9a7-147">string</span></span>  | <span data-ttu-id="ff9a7-p107">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="ff9a7-p107">application/json. Required.</span></span> |
| <span data-ttu-id="ff9a7-150">Prefer</span><span class="sxs-lookup"><span data-stu-id="ff9a7-150">Prefer</span></span> | <span data-ttu-id="ff9a7-151">文字列</span><span class="sxs-lookup"><span data-stu-id="ff9a7-151">string</span></span>  | <span data-ttu-id="ff9a7-p108">odata.maxpagesize={x}.省略可能。</span><span class="sxs-lookup"><span data-stu-id="ff9a7-p108">odata.maxpagesize={x}. Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="ff9a7-154">応答</span><span class="sxs-lookup"><span data-stu-id="ff9a7-154">Response</span></span>

<span data-ttu-id="ff9a7-155">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [mailFolder](../resources/mailfolder.md) コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ff9a7-155">If successful, this method returns a `200 OK` response code and [mailFolder](../resources/mailfolder.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff9a7-156">例</span><span class="sxs-lookup"><span data-stu-id="ff9a7-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ff9a7-157">要求</span><span class="sxs-lookup"><span data-stu-id="ff9a7-157">Request</span></span>
<span data-ttu-id="ff9a7-158">次の例に、**デルタ**関数呼び出しを 1 つ作成し、応答本文に含まれるメール フォルダーの最大数を 2 に制限する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="ff9a7-158">The following example shows how to make a single **delta** function call, and limit the maximum number of mail folders in the response body to 2.</span></span>

<span data-ttu-id="ff9a7-159">メールボックスのメール フォルダー内の変更を追跡するには、1 つ以上の**デルタ**関数呼び出しを作成し、適切な状態トークンを使用して、前回のデルタ クエリ以降になされた一連の増分の変更を取得します。</span><span class="sxs-lookup"><span data-stu-id="ff9a7-159">To track changes in the mail folders of a mailbox, you would make one or more **delta** function calls, with appropriate state tokens, to get the set of incremental changes since the last delta query.</span></span> 

<span data-ttu-id="ff9a7-p109">メール フォルダー内のメッセージ変更を追跡するために状態トークンを使用する方法を示す同様の例については、次をご覧ください。「[フォルダー内のメッセージへの増分の変更を取得する](/graph/delta-query-messages)」。メール フォルダーの追跡とフォルダー内のメッセージの追跡の主な違いは、デルタ クエリ要求 URL と、**message** コレクションではなく **mailFolder** を返すクエリ応答にあります。</span><span class="sxs-lookup"><span data-stu-id="ff9a7-p109">You can find a similar example that shows how to use the state tokens to track changes in the messages of a mail folder: [Get incremental changes to messages in a folder](/graph/delta-query-messages). The main differences between tracking mail folders and tracking messages in a folder are in the delta query request URLs, and the query responses returning **mailFolder** rather than **message** collections.</span></span>

<!-- {
  "blockType": "request",
  "name": "mailfolder_delta"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/delta

Prefer: odata.maxpagesize=2
```

##### <a name="response"></a><span data-ttu-id="ff9a7-162">応答</span><span class="sxs-lookup"><span data-stu-id="ff9a7-162">Response</span></span>

<span data-ttu-id="ff9a7-163">要求が成功すると、応答には状態トークンが含まれます。これは、_skipToken_</span><span class="sxs-lookup"><span data-stu-id="ff9a7-163">If the request is successful, the response would include a state token, which is either a _skipToken_</span></span>  
<span data-ttu-id="ff9a7-p110">(_@odata.nextLink_ 応答ヘッダーに含まれる) か、_deltaToken_ (_@odata.deltaLink_ 応答ヘッダーに含まれる) のいずれかになります。前者はその回を続行する必要があることを示し、後者はその回のすべての変更の取得が完了したことを示します。</span><span class="sxs-lookup"><span data-stu-id="ff9a7-p110">(in an _@odata.nextLink_ response header) or a _deltaToken_ (in an _@odata.deltaLink_ response header). Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="ff9a7-166">以下の応答は、_@odata.nextLink_ 応答ヘッダーに含まれる _skipToken_ を示しています。</span><span class="sxs-lookup"><span data-stu-id="ff9a7-166">The response below shows a _skipToken_ in an _@odata.nextLink_ response header.</span></span>

<span data-ttu-id="ff9a7-p111">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ff9a7-p111">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 254

{
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/me/mailfolders/delta?$skiptoken={_skipToken_}",
  "value": [
    {
      "displayName": "displayName-value",
      "parentFolderId": "parentFolderId-value",
      "childFolderCount": 99,
      "unreadItemCount": 99,
      "totalItemCount": 99
    }
  ]
}
```

### <a name="see-also"></a><span data-ttu-id="ff9a7-169">関連項目</span><span class="sxs-lookup"><span data-stu-id="ff9a7-169">See also</span></span>

- [<span data-ttu-id="ff9a7-170">デルタ クエリを使用して、Microsoft Graph データの変更を追跡する</span><span class="sxs-lookup"><span data-stu-id="ff9a7-170">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="ff9a7-171">フォルダー内のメッセージへの増分の変更を取得する</span><span class="sxs-lookup"><span data-stu-id="ff9a7-171">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
