---
title: フォルダー内のメッセージへの増分の変更を取得する
description: デルタのクエリは、追加、削除、または一連を使用して、フォルダー内のメッセージへの更新のクエリを実行できます。
ms.openlocfilehash: bae652cc8382ae1b966a24fc4af58f720a2f0c9f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092401"
---
# <a name="get-incremental-changes-to-messages-in-a-folder"></a><span data-ttu-id="882a5-103">フォルダー内のメッセージへの増分の変更を取得する</span><span class="sxs-lookup"><span data-stu-id="882a5-103">Get incremental changes to messages in a folder</span></span>

<span data-ttu-id="882a5-p101">デルタ クエリでは、一連の[デルタ](/graph/api/message-delta?view=graph-rest-1.0)関数呼び出しを使用して、フォルダー内のメッセージへの追加、削除、または更新に対してクエリを実行できます。デルタ データを使用すると、毎回サーバーからユーザーのメッセージのセット全体をフェッチせずに、ユーザーのメッセージのローカル ストアの保守と同期が行えます。</span><span class="sxs-lookup"><span data-stu-id="882a5-p101">Delta query lets you query for additions, deletions, or updates to messages in a folder, by way of a series of [delta](/graph/api/message-delta?view=graph-rest-1.0) function calls. Delta data enables you to maintain and synchronize a local store of a user's messages, without having to fetch the entire set of the user's messages from the server every time.</span></span>

<span data-ttu-id="882a5-p102">デルタ クエリでは、フォルダー内 (ユーザーの受信トレイなど) のすべてのメッセージを取得する完全な同期と、最後の同期以降、そのフォルダー内で変更されたすべてのメッセージを取得する増分同期の両方がサポートされています。通常は、フォルダー内のすべてのメッセージの最初の完全同期を実行して、その後、そのフォルダーの増分の変更を定期的に取得します。</span><span class="sxs-lookup"><span data-stu-id="882a5-p102">Delta query supports both full synchronization that retrieves all of the messages in a folder (for example, the user's Inbox), and incremental synchronization that retrieves all of the messages that have changed in that folder since the last synchronization. Typically, you would do an initial full synchronization of all the messages in a folder, and subsequently, get incremental changes to that folder periodically.</span></span>

## <a name="track-message-changes-in-a-folder"></a><span data-ttu-id="882a5-108">フォルダー内のメッセージの変更を追跡する</span><span class="sxs-lookup"><span data-stu-id="882a5-108">Track message changes in a folder</span></span>

<span data-ttu-id="882a5-p103">デルタ クエリはフォルダー単位の操作です。フォルダー階層内のメッセージの変更を追跡するには、各フォルダーを個別に追跡する必要があります。</span><span class="sxs-lookup"><span data-stu-id="882a5-p103">Delta query is a per-folder operation. To track the changes of the messages in a folder hierarchy, you need to track each folder individually.</span></span>

<span data-ttu-id="882a5-p104">通常、メール フォルダー内のメッセージ変更の追跡は、**デルタ**関数を使用した、1 つ以上の GET 要求のラウンドです。最初の GET 要求は、**デルタ**関数を含めることを除いて、[メッセージの取得](/graph/api/user-list-messages?view=graph-rest-1.0)方法とほぼ同じです。</span><span class="sxs-lookup"><span data-stu-id="882a5-p104">Tracking message changes in a mail folder typically is a round of one or more GET requests with the **delta** function. The initial GET request is very much like the way you [get messages](/graph/api/user-list-messages?view=graph-rest-1.0), except that you include the **delta** function:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/messages/delta
```

<span data-ttu-id="882a5-113">**デルタ**関数を使用した GET 要求は、次のいずれかを返します。</span><span class="sxs-lookup"><span data-stu-id="882a5-113">A GET request with the **delta** function returns either:</span></span>

- <span data-ttu-id="882a5-114">`nextLink` (**デルタ**関数の呼び出しと _skipToken_ を使用した URL を含む)、または</span><span class="sxs-lookup"><span data-stu-id="882a5-114">A `nextLink` (that contains a URL with a **delta** function call and a _skipToken_), or</span></span>
- <span data-ttu-id="882a5-115">`deltaLink` (**デルタ**関数の呼び出しと _deltaToken_ を使用した URL を含む)。</span><span class="sxs-lookup"><span data-stu-id="882a5-115">A `deltaLink` (that contains a URL with a **delta** function call and _deltaToken_).</span></span>

<span data-ttu-id="882a5-p105">これらのトークンは、クライアントに対して完全に不透明な[状態トークン](delta-query-overview.md#state-tokens)です。変更追跡のラウンドを続行する手順は、最後の GET 要求から返された URL を、同じフォルダーの次の**デルタ**関数呼び出しにコピーして適用するだけです。応答で返される `deltaLink` は、変更追跡の現在のラウンドが完了したことを示します。`deltaLink` URL を保存して、次のラウンドを開始する際に使用することができます。</span><span class="sxs-lookup"><span data-stu-id="882a5-p105">These tokens are [state tokens](delta-query-overview.md#state-tokens) that are completely opaque to the client. To proceed with a round of change tracking, simply copy and apply the URL returned from the last GET request to the next **delta** function call for the same folder. A `deltaLink` returned in a response signifies that the current round of change tracking is complete. You can save and use the `deltaLink` URL when you begin the next round.</span></span>

<span data-ttu-id="882a5-120">`nextLink` と `deltaLink` の URL を使用する方法については、以下の[例](#example-to-synchronize-messages-in-a-folder)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="882a5-120">See the [example](#example-to-synchronize-messages-in-a-folder) below to learn how to use the `nextLink` and `deltaLink` URLs.</span></span>

### <a name="use-query-parameters-in-a-delta-query-for-messages"></a><span data-ttu-id="882a5-121">メッセージのデルタ クエリでクエリ パラメーターを使用する</span><span class="sxs-lookup"><span data-stu-id="882a5-121">Use query parameters in a delta query for messages</span></span>

- <span data-ttu-id="882a5-p106">任意の GET リクエストと同様に `$select` クエリ パラメーターを使用して、最善のパフォーマンスを得るために必要なプロパティのみを指定することができます。`id` プロパティは常に返されます。</span><span class="sxs-lookup"><span data-stu-id="882a5-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The `id` property is always returned.</span></span>
- <span data-ttu-id="882a5-124">デルタ クエリは、メッセージの `$select`、`$top`、および `$expand` をサポートします。</span><span class="sxs-lookup"><span data-stu-id="882a5-124">Delta query support `$select`, `$top`, and `$expand` for messages.</span></span>
- <span data-ttu-id="882a5-125">`$filter` と `$orderby` に対するサポートには制限があります。</span><span class="sxs-lookup"><span data-stu-id="882a5-125">There is limited support for `$filter` and `$orderby`:</span></span>
  - <span data-ttu-id="882a5-126">サポートされている唯一の `$filter` 式は、`$filter=receivedDateTime+ge+{value}` または `$filter=receivedDateTime+gt+{value}` です。</span><span class="sxs-lookup"><span data-stu-id="882a5-126">The only supported `$filter` expressions are `$filter=receivedDateTime+ge+{value}` or `$filter=receivedDateTime+gt+{value}`.</span></span>
  - <span data-ttu-id="882a5-p107">サポートされている唯一の `$orderby` 式は、`$orderby=receivedDateTime+desc` です。`$orderby` 式を含めない場合、戻り値の順序は保証されません。</span><span class="sxs-lookup"><span data-stu-id="882a5-p107">The only supported `$orderby` expression is `$orderby=receivedDateTime+desc`. If you do not include an `$orderby` expression, the return order is not guaranteed.</span></span>
- <span data-ttu-id="882a5-129">`$search` に対するサポートはありません。</span><span class="sxs-lookup"><span data-stu-id="882a5-129">There is no support for `$search`.</span></span>

### <a name="optional-request-header"></a><span data-ttu-id="882a5-130">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="882a5-130">Optional request header</span></span>

<span data-ttu-id="882a5-131">各デルタ クエリの GET 要求は、応答で 1 つ以上のメッセージのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="882a5-131">Each delta query GET request returns a collection of one or more messages in the response.</span></span> <span data-ttu-id="882a5-132">必要に応じて、要求ヘッダー `Prefer: odata.maxpagesize={x}` を指定して、応答内の最大メッセージ数を設定できます。</span><span class="sxs-lookup"><span data-stu-id="882a5-132">You can optionally specify the request header, `Prefer: odata.maxpagesize={x}`, to set the maximum number of messages in a response.</span></span>

<!--
### Iterative process

A typical round to track message changes goes like this:

1. Make the initial GET request with the mandatory _Prefer: odata.track-changes_ header. If this is your very first delta query
for messages in that folder, don't provide any state token. If the messages support tracking changes, following the iterative
process (steps 2-6) described below will return the entire set of messages in that folder.

2. Check if the first response returns the _Preference-Applied: odata.track-changes_ header,
which confirms your resource supports tracking changes. Stop if you don't receive the response header.

3. If you receive a _skipToken_ (in an _@odata.nextLink_ response header) in the response, you should continue to track the
   additional messages that have changed (added, deleted, or updated). Make a second GET request, using the URL returned
   in _@odata.nextLink_, which includes a _skipToken_.

4. The second request will return additional messages that have changed, and either a _skipToken_ if there are more changed messages,
  or a _deltaToken_ if all the changed messages have been returned.

5. If you receive a _skipToken_ from the last GET request, continue getting the changes by sending a next GET call, similar to step 3.

6. When you eventually receive a _deltaToken (in an _@odata.deltaLink_ response header) in the response from a GET, stop. This
round of change tracking is complete.

7. Save the _deltaToken_. The next time you track changes for the same folder, make a GET request
similar to step 1, except that now you can use this _deltaToken_ to get just the delta data (messages that have been added, deleted or updated)
since the completion of the very first round.

-->

## <a name="example-to-synchronize-messages-in-a-folder"></a><span data-ttu-id="882a5-133">ファルダー内のメッセージを同期する例</span><span class="sxs-lookup"><span data-stu-id="882a5-133">Example to synchronize messages in a folder</span></span>

<span data-ttu-id="882a5-134">次の例では、最初に 5 つのメッセージを含んでいる特定のフォルダーの同期の 2 つのラウンドを示します。</span><span class="sxs-lookup"><span data-stu-id="882a5-134">The following example shows 2 rounds of synchronization of a specific folder which initially contains 5 messages.</span></span>

<span data-ttu-id="882a5-135">最初のラウンドには、フォルダー内の 5 つのメッセージをすべて同期するための一連の 3 つの要求が含まれます。</span><span class="sxs-lookup"><span data-stu-id="882a5-135">The first round involves a series of 3 requests to synchronize all 5 messages in the folder:</span></span>

- <span data-ttu-id="882a5-136">[サンプルの最初の要求](#sample-initial-request)と[応答](#sample-initial-response)</span><span class="sxs-lookup"><span data-stu-id="882a5-136">[Sample initial request](#sample-initial-request) and [response](#sample-initial-response)</span></span>
- <span data-ttu-id="882a5-137">[サンプルの 2 番目の要求](#sample-second-request)と[応答](#sample-second-response)</span><span class="sxs-lookup"><span data-stu-id="882a5-137">[Sample second request](#sample-second-request) and [response](#sample-second-response)</span></span>
- <span data-ttu-id="882a5-138">[サンプルの 3 番目の要求](#sample-third-request)と[最後の応答](#sample-third-and-final-response)</span><span class="sxs-lookup"><span data-stu-id="882a5-138">[Sample third request](#sample-third-request) and [final response](#sample-third-and-final-response)</span></span>

<span data-ttu-id="882a5-139">最初のラウンドの後、メッセージの 1 つが削除され、別の 1 つのメッセージが既読としてマークされます。</span><span class="sxs-lookup"><span data-stu-id="882a5-139">After the first round, one of the messages is deleted, and another is marked as read.</span></span> <span data-ttu-id="882a5-140">同期の[ 2 回目のラウンド](#synchronize-messages-in-the-same-folder-in-the-next-round)では、変更されていない他のメッセージは返さず、デルタ (削除と更新) のみを返します。</span><span class="sxs-lookup"><span data-stu-id="882a5-140">The [second round](#synchronize-messages-in-the-same-folder-in-the-next-round) of synchronization returns only the delta (the deletion and update), without returning the other messages that have remained the same.</span></span>

### <a name="sample-initial-request"></a><span data-ttu-id="882a5-141">最初の要求のサンプル</span><span class="sxs-lookup"><span data-stu-id="882a5-141">Sample initial request</span></span>

<span data-ttu-id="882a5-p110">この例では、指定されたフォルダーは初めて同期されるため、最初の同期要求には状態トークンは含まれません。このラウンドは、そのフォルダー内のすべてのメッセージを返します。</span><span class="sxs-lookup"><span data-stu-id="882a5-p110">In this example, the specified folder is being synchronized for the first time, so the initial sync request does not include any state token. This round will return all the messages in that folder.</span></span>

<span data-ttu-id="882a5-144">最初の要求では、次のものを指定しています。</span><span class="sxs-lookup"><span data-stu-id="882a5-144">The first request specifies the following:</span></span>

- <span data-ttu-id="882a5-145">応答の各メッセージの `subject` プロパティ、`sender` プロパティ、`isRead` プロパティを返す `$select` パラメーター。</span><span class="sxs-lookup"><span data-stu-id="882a5-145">A `$select` parameter to return the `subject`, `sender`, and `isRead` properties for each message in the response.</span></span>
- <span data-ttu-id="882a5-146">[オプションの要求ヘッダー](#optional-request-header)である _odata.maxpagesize_。一度に 2 通のメッセージを返すよう指定しています。</span><span class="sxs-lookup"><span data-stu-id="882a5-146">The [optional request header](#optional-request-header), _odata.maxpagesize_, returning 2 messages at a time.</span></span>

<!-- {
  "blockType": "ignored",
  "sampleKeys": ["AQMkADNkNAAAgEMAAAA"],
  "name": "get_messages_delta_1"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/mailfolders/AQMkADNkNAAAgEMAAAA/messages/delta?$select=subject,sender,isRead HTTP/1.1
Prefer: odata.maxpagesize=2
```

### <a name="sample-initial-response"></a><span data-ttu-id="882a5-147">最初の応答のサンプル</span><span class="sxs-lookup"><span data-stu-id="882a5-147">Sample initial response</span></span>

<span data-ttu-id="882a5-p111">応答には、2 つのメッセージと `@odata.nextLink` 応答ヘッダーが含まれています。`nextLink` URL は、取得するフォルダーにさらにメッセージがあることを示します。</span><span class="sxs-lookup"><span data-stu-id="882a5-p111">The response includes two messages and an `@odata.nextLink` response header. The `nextLink` URL indicates there are more messages in the folder to get.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->

```json
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(message)",
  "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$skiptoken=GwcBoTmPuoTQWfcsAbkYM",
  "value": [
    {
      "@odata.type": "#microsoft.graph.message",
      "@odata.etag": "W/\"CQAAABYAAAARn2vdzPFjSbaPPxzjlzOTAAASsKZz\"",
      "subject": "Holiday hours update",
      "isRead": "false",
      "sender": {
        "emailAddress": {
          "name": "Dana Swope",
          "address": "danas@contoso.onmicrosoft.com"
        }
      },
      "id": "AAMkADNkNAAASq35xAAA="
    },
    {
      "@odata.type": "#microsoft.graph.message",
      "@odata.etag": "W/\"CQAAABYAAAARn2vdzPFjSbaPPxzjlzOTAAAEfYB/\"",
      "subject": "Holiday promotion sale",
      "isRead": "true",
      "sender": {
        "emailAddress": {
          "name": "Samantha Booth",
          "address": "samanthab@contoso.onmicrosoft.com"
        }
      },
      "id": "AQMkADNkNAAAVRMKAAAAA=="
    }
  ]
}
```

### <a name="sample-second-request"></a><span data-ttu-id="882a5-150">2 番目の要求のサンプル</span><span class="sxs-lookup"><span data-stu-id="882a5-150">Sample second request</span></span>

<span data-ttu-id="882a5-p112">2 番目の要求では、前の応答で返された `nextLink` URL を指定します。最初の要求にあるような同じ `$select` パラメーターを指定する必要はなくなりましたのでご注意ください。これは、`nextLink` URL の `skipToken` によってこのパラメーターがエンコードされて含まれるためです。</span><span class="sxs-lookup"><span data-stu-id="882a5-p112">The second request specifies the `nextLink` URL returned from the previous response. Notice that it no longer has to specify the same `$select` parameter as in the initial request, as the `skipToken` in the `nextLink` URL encodes and includes it.</span></span>

<!-- {
  "blockType": "ignored",
  "sampleKeys": ["AQMkADNkNAAAgEMAAAA"],
  "name": "get_messages_delta_2"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/mailfolders/AQMkADNkNAAAgEMAAAA/messages/delta?$skiptoken=GwcBoTmPuoTQWfcsAbkYM HTTP/1.1
Prefer: odata.maxpagesize=2
```

### <a name="sample-second-response"></a><span data-ttu-id="882a5-153">2 番目の応答のサンプル</span><span class="sxs-lookup"><span data-stu-id="882a5-153">Sample second response</span></span>

<span data-ttu-id="882a5-154">2 番目の応答は、フォルダーから取得するメッセージがまだあることを示す、フォルダー内の次の 2 つのメッセージと別の `nextLink` を返します。</span><span class="sxs-lookup"><span data-stu-id="882a5-154">The second response returns the next 2 messages in the folder and another `nextLink`, indicating there are more messages to get from the folder.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->

```json
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(message)",
  "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$skiptoken=GwcBoTmPKILK4jLH7mAd1lLU",
  "value": [
    {
      "@odata.type": "#microsoft.graph.message",
      "@odata.etag": "W/\"CQAAABYAAAARn2vdzPFjSbaPPxzjlqfdAAAEfYB+\"",
      "subject": "Microsoft Virtual Academy at Contoso",
      "isRead": true,
      "sender": {
        "emailAddress": {
          "name": "Elliot Hyde",
          "address": "elliot-hyde@tailspintoys.com"
        }
      },
      "id": "AQMkADNkNAAAgWkAAAA"
    },
    {
      "@odata.type": "#microsoft.graph.message",
      "@odata.etag": "W/\"CQAAABYAAAARn2vdzPFjSbaPPxzjlzOTAAAEfYB+\"",
      "subject": "New or modified user account information",
      "isRead": true,
      "sender": {
        "emailAddress": {
          "name": "Randi Welch",
          "address": "randiw@contoso.onmicrosoft.com"
        }
      },
      "id": "AQMkADNkNAAAgWJAAAA"
    }
  ]
}
```

### <a name="sample-third-request"></a><span data-ttu-id="882a5-155">3 番目の要求のサンプル</span><span class="sxs-lookup"><span data-stu-id="882a5-155">Sample third request</span></span>

<span data-ttu-id="882a5-156">3 番目の要求は、最後の同期要求から返された最新の `nextLink` URL を引き続き使用します。</span><span class="sxs-lookup"><span data-stu-id="882a5-156">The third request continues to use the latest `nextLink` URL returned from the last sync request.</span></span>

<!-- {
  "blockType": "ignored",
  "sampleKeys": ["AQMkADNkNAAAgEMAAAA"],
  "name": "get_messages_delta_3"
}-->
```
GET https://graph.microsoft.com/v1.0/me/mailFolders/AQMkADNkNAAAgEMAAAA/messages/delta?$skiptoken=GwcBoTmPKILK4jLH7mAd1lLU HTTP/1.1
Prefer: odata.maxpagesize=2
```

### <a name="sample-third-and-final-response"></a><span data-ttu-id="882a5-157">3 番目と最後の応答のサンプル</span><span class="sxs-lookup"><span data-stu-id="882a5-157">Sample third and final response</span></span>

<span data-ttu-id="882a5-p113">3 番目の応答では、フォルダーに残っている 1 つだけのメッセージと、そのフォルダーの同期が当面の間完了していることを示す `deltaLink` URL が返されます。`deltaLink` URL を保存して、[次のラウンドで同じフォルダーを同期するために使用します](#synchronize-messages-in-the-same-folder-in-the-next-round)。</span><span class="sxs-lookup"><span data-stu-id="882a5-p113">The third response returns the only remaining message in the folder, and a `deltaLink` URL which indicates synchronization is complete for the time being for this folder. Save and use the `deltaLink` URL to [synchronize the same folder in the next round](#synchronize-messages-in-the-same-folder-in-the-next-round).</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->

```json
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(message)",
  "@odata.deltaLink": "https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$deltatoken=GwcBoTmPuoGNlgXgF1nyUNMXY",
  "value": [
    {
      "@odata.type": "#microsoft.graph.message",
      "@odata.etag": "W/\"CQAAABYAAAARn2vdzFPjSbaPPxzjlzOTAAAEfYB+\"",
      "subject": "Fabric CDN now available",
      "isRead": true,
      "sender": {
        "emailAddress": {
          "name": "Jodie Sharp",
          "address": "Jodie.Sharp@contoso.com"
        }
      },
      "id": "AAMkADk0MGFkODE3LWEAAA="
    }
  ]
}
```

### <a name="synchronize-messages-in-the-same-folder-in-the-next-round"></a><span data-ttu-id="882a5-160">次のラウンドで同じフォルダー内のメッセージを同期する</span><span class="sxs-lookup"><span data-stu-id="882a5-160">Synchronize messages in the same folder in the next round</span></span>

<span data-ttu-id="882a5-p114">最後のランドの[最後の応答](#sample-third-request)からの `deltaLink` を使用すると、それ以降にそのフォルダーで (追加、削除、または更新によって) 変更されたこれらのメッセージのみを取得できます。次のラウンドの最初の要求は、同じ最大ページ サイズを維持することを前提とすると、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="882a5-p114">Using the `deltaLink` from the [last request](#sample-third-request) in the last round, you will be able to get only those messages that have changed (by being added, deleted, or updated) in that folder since then. Your first request in the next round will look like the following, assuming you prefer to keep the same maximum page size in the response:</span></span>

<!-- {
  "blockType": "ignored",
  "sampleKeys": ["AQMkADNkNAAAgEMAAAA"],
  "name": "get_messages_delta_next"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/mailfolders/AQMkADNkNAAAgEMAAAA/messages/delta?$deltatoken=GwcBoTmPuoGNlgXgF1nyUNMXY HTTP/1.1
Prefer: odata.maxpagesize=2
```

<span data-ttu-id="882a5-163">応答には `deltaLink` が含まれます。</span><span class="sxs-lookup"><span data-stu-id="882a5-163">The response contains a `deltaLink`.</span></span> <span data-ttu-id="882a5-164">これは、リモート メール フォルダー内のすべての変更が同期されていることを示します。</span><span class="sxs-lookup"><span data-stu-id="882a5-164">This indicates that all changes in the remote mail folder are now synchronized.</span></span> <span data-ttu-id="882a5-165">1 つのメッセージは削除され、その他のメッセージは変更されました。</span><span class="sxs-lookup"><span data-stu-id="882a5-165">One message was deleted and the other message was changed.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->

```json
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(message)",
  "@odata.deltaLink": "https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$deltatoken=GwcBoTmPuoGNlgXgF1nyUNMXY",
  "value": [
    {
      "@odata.type": "#microsoft.graph.message",
      "id": "AAMkADk0MGFkODE3LWE4MmYtNDRhOS0Dh_6qB-pB2Sa2pUum19a6YAAKnLuxoAAA=",
      "@removed": {
        "reason": "deleted"
      }
    },
    {
      "@odata.type": "#microsoft.graph.message",
      "@odata.etag": "W/\"CQAAABYAAAARn2vdzPFjSbaPPxzjlzOTAAASsKZz\"",
      "subject": "Holiday hours update",
      "isRead": "true",
      "sender": {
        "emailAddress": {
          "name": "Dana Swope",
          "address": "danas@contoso.onmicrosoft.com"
        }
      },
      "id": "AAMkADNkNAAASq35xAAA="
    }
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="882a5-166">関連項目</span><span class="sxs-lookup"><span data-stu-id="882a5-166">See also</span></span>

- [<span data-ttu-id="882a5-167">Microsoft Graph デルタ クエリ</span><span class="sxs-lookup"><span data-stu-id="882a5-167">Microsoft Graph delta query</span></span>](delta-query-overview.md)
- [<span data-ttu-id="882a5-168">カレンダー ビューのイベントへの増分の変更を取得する</span><span class="sxs-lookup"><span data-stu-id="882a5-168">Get incremental changes to events in a calendar view</span></span>](delta-query-events.md)
- [<span data-ttu-id="882a5-169">グループに対する増分の変更を取得する</span><span class="sxs-lookup"><span data-stu-id="882a5-169">Get incremental changes to groups</span></span>](delta-query-groups.md)
- [<span data-ttu-id="882a5-170">ユーザーへの増分の変更を取得する</span><span class="sxs-lookup"><span data-stu-id="882a5-170">Get incremental changes to users</span></span>](delta-query-users.md)
