# <a name="mailfolder-delta"></a><span data-ttu-id="82fd3-101">mailFolder: delta</span><span class="sxs-lookup"><span data-stu-id="82fd3-101">mailFolder: delta</span></span>

<span data-ttu-id="82fd3-102">ユーザーのメールボックスで追加または削除された一連のメール フォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="82fd3-102">Get a set of mail folders that have been added, deleted, or removed from the user's mailbox.</span></span>

<span data-ttu-id="82fd3-p101">メールボックス内のメール フォルダーに対する**デルタ**関数の呼び出しと GET 要求とは似ていますが、[状態トークン](../../../concepts/delta_query_overview.md)をこれらの呼び出しに適切に適用することにより、メール フォルダーの増分の変更をクエリできる点が異なります。これにより、ユーザーのメール フォルダーのローカル ストアの保守と同期を行う際に、そのメールボックスのメール フォルダーすべてを毎回サーバーからフェッチする必要がなくなります。</span><span class="sxs-lookup"><span data-stu-id="82fd3-p101">A **delta** function call for mail folders in a mailbox is similar to a GET request, except that by appropriately applying [state tokens](../../../concepts/delta_query_overview.md) in one or more of these calls, you can query for incremental changes in the mail folders. This allows you to maintain and synchronize a local store of a user's mail folders without having to fetch all the mail folders of that mailbox from the server every time.</span></span>

## <a name="permissions"></a><span data-ttu-id="82fd3-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="82fd3-105">Permissions</span></span>
<span data-ttu-id="82fd3-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="82fd3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="82fd3-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="82fd3-108">Permission type</span></span>      | <span data-ttu-id="82fd3-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="82fd3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="82fd3-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="82fd3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="82fd3-111">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="82fd3-111">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="82fd3-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="82fd3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82fd3-113">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="82fd3-113">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="82fd3-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="82fd3-114">Application</span></span> | <span data-ttu-id="82fd3-115">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="82fd3-115">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="82fd3-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="82fd3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/delta
GET /users/{id}/mailFolders/delta
```

## <a name="optional-query-parameters"></a><span data-ttu-id="82fd3-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="82fd3-117">Optional query parameters</span></span>

<span data-ttu-id="82fd3-p103">メール フォルダーの変更を追跡すると、1 つ以上の **デルタ**関数呼び出しのラウンドが発生します。任意のクエリ パラメーター (`$deltatoken` と `$skiptoken` 以外) を使用する場合は、最初の**デルタ**要求でこれを指定する必要があります。Microsoft Graph は、応答で提供される `nextLink` や `deltaLink` の URL のトークン部分に指定したパラメーターを自動的にエンコードします。必要なクエリ パラメーターを前もって指定しておくだけで済みます。それ以降の要求では、前の応答で `nextLink` や `deltaLink` の URL に必要なパラメーターが既にエンコードされ、含まれているため、この URL をコピーして適用するだけです。</span><span class="sxs-lookup"><span data-stu-id="82fd3-p103">Tracking changes in mail folders incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response. You only need to specify any desired query parameters once upfront. In subsequent requests, simply copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="82fd3-123">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="82fd3-123">Query parameter</span></span>      | <span data-ttu-id="82fd3-124">種類</span><span class="sxs-lookup"><span data-stu-id="82fd3-124">Type</span></span>   |<span data-ttu-id="82fd3-125">説明</span><span class="sxs-lookup"><span data-stu-id="82fd3-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="82fd3-126">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="82fd3-126">$deltatoken</span></span> | <span data-ttu-id="82fd3-127">文字列</span><span class="sxs-lookup"><span data-stu-id="82fd3-127">string</span></span> | <span data-ttu-id="82fd3-p104">同じメール フォルダー コレクションの前の**デルタ**関数呼び出しの `deltaLink` URL で[状態トークン](../../../concepts/delta_query_overview.md)が返され、その変更追跡のラウンドが完了したことを示します。このコレクションについて、このトークンを含む、`deltaLink` URL 全体を次の変更追跡のラウンドの最初の要求に保存し、適用します。</span><span class="sxs-lookup"><span data-stu-id="82fd3-p104">A [state token](../../../concepts/delta_query_overview.md) returned in the `deltaLink` URL of the previous **delta** function call for the same mail folder collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="82fd3-130">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="82fd3-130">$skiptoken</span></span> | <span data-ttu-id="82fd3-131">文字列</span><span class="sxs-lookup"><span data-stu-id="82fd3-131">string</span></span> | <span data-ttu-id="82fd3-132">前の**デルタ**関数呼び出しの `nextLink` URL で[状態トークン](../../../concepts/delta_query_overview.md)が返され、同じメール フォルダー コレクションに追跡すべき変更が他にもあることを示します。</span><span class="sxs-lookup"><span data-stu-id="82fd3-132">A [state token](../../../concepts/delta_query_overview.md) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same mail folder collection.</span></span> |

#### <a name="odata-query-parameters"></a><span data-ttu-id="82fd3-133">OData クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="82fd3-133">OData query parameters</span></span>

<span data-ttu-id="82fd3-p105">任意の GET リクエストと同様に `$select` クエリ パラメーターを使用して、最善のパフォーマンスを得るために必要なプロパティのみを指定することができます。_Id_ プロパティは常に返されます。</span><span class="sxs-lookup"><span data-stu-id="82fd3-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="82fd3-136">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="82fd3-136">Request headers</span></span>
| <span data-ttu-id="82fd3-137">名前</span><span class="sxs-lookup"><span data-stu-id="82fd3-137">Name</span></span>       | <span data-ttu-id="82fd3-138">型</span><span class="sxs-lookup"><span data-stu-id="82fd3-138">Type</span></span> | <span data-ttu-id="82fd3-139">説明</span><span class="sxs-lookup"><span data-stu-id="82fd3-139">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="82fd3-140">承認</span><span class="sxs-lookup"><span data-stu-id="82fd3-140">Authorization</span></span>  | <span data-ttu-id="82fd3-141">文字列</span><span class="sxs-lookup"><span data-stu-id="82fd3-141">string</span></span>  | <span data-ttu-id="82fd3-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="82fd3-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="82fd3-144">コンテンツ タイプ</span><span class="sxs-lookup"><span data-stu-id="82fd3-144">Content-Type</span></span>  | <span data-ttu-id="82fd3-145">文字列</span><span class="sxs-lookup"><span data-stu-id="82fd3-145">string</span></span>  | <span data-ttu-id="82fd3-p107">アプリケーションまたは json。必須。</span><span class="sxs-lookup"><span data-stu-id="82fd3-p107">application/json. Required.</span></span> |
| <span data-ttu-id="82fd3-148">優先</span><span class="sxs-lookup"><span data-stu-id="82fd3-148">Prefer</span></span> | <span data-ttu-id="82fd3-149">文字列</span><span class="sxs-lookup"><span data-stu-id="82fd3-149">string</span></span>  | <span data-ttu-id="82fd3-p108">odata.maxpagesize={x}.省略可能。</span><span class="sxs-lookup"><span data-stu-id="82fd3-p108">odata.maxpagesize={x}. Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="82fd3-152">応答</span><span class="sxs-lookup"><span data-stu-id="82fd3-152">Response</span></span>

<span data-ttu-id="82fd3-153">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [mailFolder](../resources/mailfolder.md) コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="82fd3-153">If successful, this method returns a `200 OK` response code and [mailFolder](../resources/mailfolder.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82fd3-154">例</span><span class="sxs-lookup"><span data-stu-id="82fd3-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="82fd3-155">要求</span><span class="sxs-lookup"><span data-stu-id="82fd3-155">Request</span></span>
<span data-ttu-id="82fd3-156">次の例に、**デルタ**関数呼び出しを 1 つ作成し、応答本文に含まれるメール フォルダーの最大数を 2 に制限する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="82fd3-156">The following example shows how to make a single **delta** function call, and limit the maximum number of mail folders in the response body to 2.</span></span>

<span data-ttu-id="82fd3-157">メールボックスのメール フォルダー内の変更を追跡するには、1 つ以上の**デルタ**関数呼び出しを作成し、適切な状態トークンを使用して、前回のデルタ クエリ以降になされた一連の増分の変更を取得します。</span><span class="sxs-lookup"><span data-stu-id="82fd3-157">To track changes in the mail folders of a mailbox, you would make one or more **delta** function calls, with appropriate state tokens, to get the set of incremental changes since the last delta query.</span></span> 

<span data-ttu-id="82fd3-p109">メール フォルダー内のメッセージ変更を追跡するために状態トークンを使用する方法を示す同様の例については、次をご覧ください。「[フォルダー内のメッセージへの増分の変更を取得する](../../../concepts/delta_query_messages.md)」。メール フォルダーの追跡とフォルダー内のメッセージの追跡の主な違いは、デルタ クエリ要求 URL と、**message** コレクションではなく **mailFolder** を返すクエリ応答にあります。</span><span class="sxs-lookup"><span data-stu-id="82fd3-p109">You can find a similar example that shows how to use the state tokens to track changes in the messages of a mail folder: [Get incremental changes to messages in a folder](../../../concepts/delta_query_messages.md). The main differences between tracking mail folders and tracking messages in a folder are in the delta query request URLs, and the query responses returning **mailFolder** rather than **message** collections.</span></span>

<!-- {
  "blockType": "request",
  "name": "mailfolder_delta"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/delta

Prefer: odata.maxpagesize=2
```

##### <a name="response"></a><span data-ttu-id="82fd3-160">応答</span><span class="sxs-lookup"><span data-stu-id="82fd3-160">Response</span></span>

<span data-ttu-id="82fd3-161">要求が成功すると、応答には状態トークンが含まれます。これは、_skipToken_</span><span class="sxs-lookup"><span data-stu-id="82fd3-161">If the request is successful, the response would include a state token, which is either a _skipToken_</span></span>  
<span data-ttu-id="82fd3-p110">(_@odata.nextLink_ 応答ヘッダーに含まれる) か、_deltaToken_ (_@odata.deltaLink_ 応答ヘッダーに含まれる) のいずれかになります。前者はその回を続行する必要があることを示し、後者はその回のすべての変更の取得が完了したことを示します。</span><span class="sxs-lookup"><span data-stu-id="82fd3-p110">(in an _@odata.nextLink_ response header) or a _deltaToken_ (in an _@odata.deltaLink_ response header). Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="82fd3-164">以下の応答は、_@odata.nextLink_ 応答ヘッダーに含まれる _skipToken_ を示しています。</span><span class="sxs-lookup"><span data-stu-id="82fd3-164">The response below shows a _skipToken_ in an _@odata.nextLink_ response header.</span></span>

<span data-ttu-id="82fd3-p111">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="82fd3-p111">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

### <a name="see-also"></a><span data-ttu-id="82fd3-167">関連項目</span><span class="sxs-lookup"><span data-stu-id="82fd3-167">See also</span></span>

- [<span data-ttu-id="82fd3-168">デルタ クエリを使用して、Microsoft Graph データの変更を追跡する</span><span class="sxs-lookup"><span data-stu-id="82fd3-168">Use delta query to track changes in Microsoft Graph data</span></span>](../../../concepts/delta_query_overview.md)
- [<span data-ttu-id="82fd3-169">フォルダー内のメッセージへの増分の変更を取得する</span><span class="sxs-lookup"><span data-stu-id="82fd3-169">Get incremental changes to messages in a folder</span></span>](../../../concepts/delta_query_messages.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
