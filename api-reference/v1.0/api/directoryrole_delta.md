# <a name="directoryrole-delta"></a><span data-ttu-id="ba721-101">directoryRole: デルタ</span><span class="sxs-lookup"><span data-stu-id="ba721-101">directoryRole: delta</span></span>

<span data-ttu-id="ba721-102">Get を新しく作成するには、更新、または全体のリソースのコレクションのすべての読み取りを実行することがなくディレクトリの役割を削除します。</span><span class="sxs-lookup"><span data-stu-id="ba721-102">Get newly created, updated, or deleted directory roles without having to perform a full read of the entire resource collection.</span></span> <span data-ttu-id="ba721-103">詳細については、[デルタのクエリを使用する](../../../concepts/delta_query_overview.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ba721-103">See [Using Delta Query](../../../concepts/delta_query_overview.md) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="ba721-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ba721-104">Permissions</span></span>

<span data-ttu-id="ba721-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ba721-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="ba721-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ba721-107">Permission type</span></span>      | <span data-ttu-id="ba721-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ba721-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ba721-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ba721-109">Delegated (work or school account)</span></span> | <span data-ttu-id="ba721-110">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ba721-110">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ba721-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ba721-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba721-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ba721-112">Not supported.</span></span>    |
|<span data-ttu-id="ba721-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ba721-113">Application</span></span> | <span data-ttu-id="ba721-114">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba721-114">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba721-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ba721-115">HTTP request</span></span>

<span data-ttu-id="ba721-116">変更の追跡を開始するには、 [directoryRole](../resources/directoryrole.md)リソースで**デルタ**関数を含む要求を行います。</span><span class="sxs-lookup"><span data-stu-id="ba721-116">To begin tracking changes, you make a request including the **delta** function on the [directoryRole](../resources/directoryrole.md) resource.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/delta
```

## <a name="query-parameters"></a><span data-ttu-id="ba721-117">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ba721-117">Query parameters</span></span>

<span data-ttu-id="ba721-118">変更を追跡する一連の 1 つまたは複数の**delta**関数の呼び出しが発生します。</span><span class="sxs-lookup"><span data-stu-id="ba721-118">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="ba721-119">任意のクエリ パラメーターを使用する場合 (以外の`$deltatoken`と`$skiptoken`)、**デルタ**の初期要求で指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ba721-119">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="ba721-120">Microsoft Graph が自動的に任意指定のパラメーターをエンコードのトークンの部分に、`nextLink`または`deltaLink`の応答で提供される URL です。</span><span class="sxs-lookup"><span data-stu-id="ba721-120">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="ba721-121">必要なクエリ パラメーターを前もって 1 回指定しておくだけで済みます。</span><span class="sxs-lookup"><span data-stu-id="ba721-121">You only need to specify any desired query parameters once upfront.</span></span> <span data-ttu-id="ba721-122">その後の要求では、前の応答で得られた `nextLink` や `deltaLink` の URL をコピーして適用します。エンコード済みの必要なパラメーターがこの URL に既に含まれているためです。</span><span class="sxs-lookup"><span data-stu-id="ba721-122">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="ba721-123">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ba721-123">Query parameter</span></span>      | <span data-ttu-id="ba721-124">種類</span><span class="sxs-lookup"><span data-stu-id="ba721-124">Type</span></span>   |<span data-ttu-id="ba721-125">説明</span><span class="sxs-lookup"><span data-stu-id="ba721-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ba721-126">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="ba721-126">$deltatoken</span></span> | <span data-ttu-id="ba721-127">文字列</span><span class="sxs-lookup"><span data-stu-id="ba721-127">string</span></span> | <span data-ttu-id="ba721-128">返される[トークンの状態](../../../concepts/delta_query_overview.md)、`deltaLink`の変更の追跡には、そのラウンドの完了を示す前の**デルタ**関数呼び出し、同じリソースを収集するための URL です。</span><span class="sxs-lookup"><span data-stu-id="ba721-128">A [state token](../../../concepts/delta_query_overview.md) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="ba721-129">保存し、全体を適用する`deltaLink`コレクションの変更履歴の次のラウンドの最初の要求にこのトークンを含む URL です。</span><span class="sxs-lookup"><span data-stu-id="ba721-129">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="ba721-130">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="ba721-130">$skiptoken</span></span> | <span data-ttu-id="ba721-131">文字列</span><span class="sxs-lookup"><span data-stu-id="ba721-131">string</span></span> | <span data-ttu-id="ba721-132">返される[トークンの状態](../../../concepts/delta_query_overview.md)、`nextLink`で同じリソースのコレクションを追跡するにさらに変更が加えられたことを示す前の**デルタ**関数の呼び出しの URL です。</span><span class="sxs-lookup"><span data-stu-id="ba721-132">A [state token](../../../concepts/delta_query_overview.md) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same resource collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="ba721-133">OData クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ba721-133">OData query parameters</span></span>

<span data-ttu-id="ba721-134">このメソッドは、応答をカスタマイズするため、OData クエリ パラメーターをサポートします。</span><span class="sxs-lookup"><span data-stu-id="ba721-134">This method supports OData query parameters to help customize the response.</span></span>

- <span data-ttu-id="ba721-p105">任意の GET リクエストと同様に `$select` クエリ パラメーターを使用して、最善のパフォーマンスを得るために必要なプロパティのみを指定することができます。_Id_ プロパティは常に返されます。</span><span class="sxs-lookup"><span data-stu-id="ba721-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span>

- <span data-ttu-id="ba721-137">サポートが制限されて`$filter`。</span><span class="sxs-lookup"><span data-stu-id="ba721-137">There is limited support for `$filter`:</span></span>

  - <span data-ttu-id="ba721-138">サポートされる唯一の`$filter`の id で特定のリソースに対する変更を追跡するための式が:`$filter=id+eq+{value}`または`$filter=id+eq+{value1}+or+id+eq+{value2}`。</span><span class="sxs-lookup"><span data-stu-id="ba721-138">The only supported `$filter` expression is for tracking changes for specific resources, by their id:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="ba721-139">URL の最大長を指定することができます id の数が制限されます。</span><span class="sxs-lookup"><span data-stu-id="ba721-139">The number of ids you can specify is limited by the maximum URL length.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ba721-140">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ba721-140">Request headers</span></span>

| <span data-ttu-id="ba721-141">名前</span><span class="sxs-lookup"><span data-stu-id="ba721-141">Name</span></span>       | <span data-ttu-id="ba721-142">説明</span><span class="sxs-lookup"><span data-stu-id="ba721-142">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ba721-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba721-143">Authorization</span></span>  | <span data-ttu-id="ba721-144">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="ba721-144">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="ba721-145">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ba721-145">Content-Type</span></span>  | <span data-ttu-id="ba721-146">application/json</span><span class="sxs-lookup"><span data-stu-id="ba721-146">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ba721-147">要求本文</span><span class="sxs-lookup"><span data-stu-id="ba721-147">Request body</span></span>

<span data-ttu-id="ba721-148">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ba721-148">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="ba721-149">応答</span><span class="sxs-lookup"><span data-stu-id="ba721-149">Response</span></span>

<span data-ttu-id="ba721-150">かどうかは成功すると、このメソッドを返します`200 OK`、応答の本体で応答コードと[directoryRole](../resources/directoryrole.md)コレクションのオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="ba721-150">If successful, this method returns `200 OK` response code and [directoryRole](../resources/directoryrole.md) collection object in the response body.</span></span> <span data-ttu-id="ba721-151">応答にも含まれています、`nextLink`の URL、または`deltaLink`URL です。</span><span class="sxs-lookup"><span data-stu-id="ba721-151">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="ba721-152">場合、`nextLink`の URL が返されますが、セッション内で取得するデータのページを追加します。</span><span class="sxs-lookup"><span data-stu-id="ba721-152">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="ba721-153">アプリケーションの継続を使用して要求を作成する、`nextLink`までの URL を`deltaLink`URL が応答に含まれています。</span><span class="sxs-lookup"><span data-stu-id="ba721-153">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>

- <span data-ttu-id="ba721-154">場合、`deltaLink`の URL が返される、返されるリソースの既存の状態に関する多くのデータはありません。</span><span class="sxs-lookup"><span data-stu-id="ba721-154">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="ba721-155">保存`deltaLink`の URL、将来的に、リソースへの変更の詳細については、次の**デルタ ・** 呼び出しに適用するとします。</span><span class="sxs-lookup"><span data-stu-id="ba721-155">Save `deltaLink` URL and apply it in the next **delta** call to learn about changes to the resource in the future.</span></span>

### <a name="example"></a><span data-ttu-id="ba721-156">例</span><span class="sxs-lookup"><span data-stu-id="ba721-156">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ba721-157">要求</span><span class="sxs-lookup"><span data-stu-id="ba721-157">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryRole_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/directoryRoles/delta
```

##### <a name="response"></a><span data-ttu-id="ba721-158">応答</span><span class="sxs-lookup"><span data-stu-id="ba721-158">Response</span></span>

<span data-ttu-id="ba721-p110">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ba721-p110">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- { 
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole",
  "isCollection": true 
} --> 
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#directoryRoles",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/directoryRoles/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
      {
      "description": "description-value",
      "displayName": "displayName-value",
      "roleTemplateId": "roleTemplateId-value",
      "id": "id-value"
    }
  ]
}
```

### <a name="see-also"></a><span data-ttu-id="ba721-161">関連項目</span><span class="sxs-lookup"><span data-stu-id="ba721-161">See also</span></span>

- <span data-ttu-id="ba721-162">詳細については[Microsoft のグラフのデータの変更を追跡するためにデルタのクエリを使用します。](../../../concepts/delta_query_overview.md)</span><span class="sxs-lookup"><span data-stu-id="ba721-162">[Use delta query to track changes in Microsoft Graph data](../../../concepts/delta_query_overview.md) for more details</span></span>
- <span data-ttu-id="ba721-163">要求の例については、「[ユーザーに対する増分の変更の取得](../../../concepts/delta_query_users.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="ba721-163">[Get incremental changes for users](../../../concepts/delta_query_users.md) for an example requests.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryRole: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->