# <a name="working-with-excel-in-microsoft-graph"></a><span data-ttu-id="ab09e-101">Microsoft Graph での Excel の操作</span><span class="sxs-lookup"><span data-stu-id="ab09e-101">Working with Excel in Microsoft Graph</span></span>

<span data-ttu-id="ab09e-p101">Microsoft Graph を使用すると、OneDrive、SharePoint、またはその他のサポートされているストレージ プラットフォームに格納されている Excel ブックを、Web アプリケーションやモバイル アプリケーションで読み取ったり変更したりすることができます。`Workbook` (つまり Excel ファイル) リソースには、リレーションシップを介するその他のすべての Excel リソースが含まれています。ファイルの場所を URL で指定すれば、[ドライブ API](drive.md) でブックにアクセスできます。例:</span><span class="sxs-lookup"><span data-stu-id="ab09e-p101">You can use Microsoft Graph to allow web and mobile applications to read and modify Excel workbooks stored in OneDrive, SharePoint, or other supported storage platforms. The `Workbook` (or Excel file) resource contains all the other Excel resources through relationships. You can access a workbook through the [Drive API](drive.md) by identifying the location of the file in the URL. For example:</span></span>

`https://graph.microsoft.com/{version}/me/drive/items/{id}/workbook/`  
`https://graph.microsoft.com/{version}/me/drive/root:/{item-path}:/workbook/`  

<span data-ttu-id="ab09e-p102">ブックに対して作成、読み取り、更新、削除 (CRUD) 操作を実行するための標準 REST API を使用して、一連の Excel オブジェクト (テーブル、範囲、またはグラフなど) にアクセスできます。たとえば、`GET https://graph.microsoft.com/{version}/me/drive/items/{id}/workbook/worksheets` では、</span><span class="sxs-lookup"><span data-stu-id="ab09e-p102">You can access a set of Excel objects (such as Table, Range, or Chart) by using standard REST APIs to perform  create, read, update, and delete (CRUD) operations on the workbook. For example, `GET https://graph.microsoft.com/{version}/me/drive/items/{id}/workbook/worksheets`</span></span>  
<span data-ttu-id="ab09e-108">ワークブックの一部であるワークシート オブジェクトのコレクションが返されます。</span><span class="sxs-lookup"><span data-stu-id="ab09e-108">returns a collection of worksheet objects that are part of the workbook.</span></span>    


<span data-ttu-id="ab09e-p103">**注:**Excel の REST API では、Office Open XML ファイル形式のブックのみをサポートしています。`.xls` 拡張子のブックはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ab09e-p103">**Note:** The Excel REST API supports only Office Open XML file formatted workbooks. The `.xls` extension workbooks are not supported.</span></span> 

## <a name="authorization-and-scopes"></a><span data-ttu-id="ab09e-111">承認とスコープ</span><span class="sxs-lookup"><span data-stu-id="ab09e-111">Authorization and scopes</span></span>

<span data-ttu-id="ab09e-112">[Azure AD v.2 エンドポイント](https://developer.microsoft.com/en-us/graph/docs/authorization/converged_auth)を使用して Excel API を認証できます。</span><span class="sxs-lookup"><span data-stu-id="ab09e-112">You can use the [Azure AD v.2 endpoint](https://developer.microsoft.com/en-us/graph/docs/authorization/converged_auth) to authenticate Excel APIs.</span></span> <span data-ttu-id="ab09e-113">すべての API には、`Authorization: Bearer {access-token}` HTTP ヘッダーが必要です。</span><span class="sxs-lookup"><span data-stu-id="ab09e-113">All APIs require the `Authorization: Bearer {access-token}` HTTP header.</span></span>   
  
<span data-ttu-id="ab09e-114">Excel リソースを使用するには、以下のいずれかの[アクセス許可のスコープ](https://developer.microsoft.com/en-us/graph/docs/authorization/permission_scopes)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ab09e-114">One of the following [permission scopes](https://developer.microsoft.com/en-us/graph/docs/authorization/permission_scopes) is required to use the Excel resource:</span></span>

* <span data-ttu-id="ab09e-115">Files.Read (読み取りアクション用)</span><span class="sxs-lookup"><span data-stu-id="ab09e-115">Files.Read (for read actions)</span></span>
* <span data-ttu-id="ab09e-116">Files.ReadWrite (読み取りおよび書き込みアクション用)</span><span class="sxs-lookup"><span data-stu-id="ab09e-116">Files.ReadWrite (for read and write actions)</span></span>


## <a name="sessions-and-persistence"></a><span data-ttu-id="ab09e-117">セッションと永続化</span><span class="sxs-lookup"><span data-stu-id="ab09e-117">Sessions and persistence</span></span>

<span data-ttu-id="ab09e-118">次の 3 つのモードのいずれかで、Excel API を呼び出すことができます。</span><span class="sxs-lookup"><span data-stu-id="ab09e-118">Excel APIs can be called in one of three modes:</span></span> 

1. <span data-ttu-id="ab09e-119">永続セッション - ブックに加えられたすべての変更は永続化 (保存) されます。</span><span class="sxs-lookup"><span data-stu-id="ab09e-119">Persistent session - All changes made to the workbook are persisted (saved).</span></span> <span data-ttu-id="ab09e-120">これは、最も効率的でパフォーマンスの高い操作のモードです。</span><span class="sxs-lookup"><span data-stu-id="ab09e-120">This is the most efficient and performant mode of operation.</span></span> 
2. <span data-ttu-id="ab09e-p106">非永続セッション - API によって加えられた変更は元の場所に保存されません。代わりに、その特定の API セッション中に加えられた変更を反映するファイルの一時コピーが Excel のバックエンド サーバーに保持されます。Excel のセッションの有効期限が切れると、変更は失われます。分析を行ったり、計算の結果やグラフのイメージを取得したりする必要があるものの、ドキュメントの状態には影響を与えないアプリには、このモードが便利です。</span><span class="sxs-lookup"><span data-stu-id="ab09e-p106">Non-persistent session - Changes made by the API are not saved to the source location. Instead, the Excel backend server keeps a temporary copy of the file that reflects the changes made during that particular API session. When the Excel session expires, the changes are lost. This mode is useful for apps that need to do analysis or obtain the results of a calculation or a chart image, but not affect the document state.</span></span> 
3. <span data-ttu-id="ab09e-125">セッションレス - セッション情報を伴わずに API 呼び出しが行われます。</span><span class="sxs-lookup"><span data-stu-id="ab09e-125">Sessionless - The API call is made without session information.</span></span> <span data-ttu-id="ab09e-126">Excel サーバーは、操作を実行するたびにサーバーにあるブックのコピーを検索する必要があるので、これは Excel API を呼び出す上で効率的な方法とは言えません。</span><span class="sxs-lookup"><span data-stu-id="ab09e-126">Excel servers have to locate the server's copy of the workbook each time to perform the operation and hence this is not an efficient way for call Excel APIs.</span></span> <span data-ttu-id="ab09e-127">この方法は 1 回限りの要求を出すのには適しています。</span><span class="sxs-lookup"><span data-stu-id="ab09e-127">It is suitable for making one off requests.</span></span> 

<span data-ttu-id="ab09e-128">API でセッションを表すには、`workbook-session-id: {session-id}` ヘッダーを使用します。</span><span class="sxs-lookup"><span data-stu-id="ab09e-128">To represent the session in the API, use the `workbook-session-id: {session-id}` header.</span></span> 

><span data-ttu-id="ab09e-p108">**注:**セッション ヘッダーは Excel API が機能するために必要ではありません。しかし、パフォーマンスを向上させるためにセッション ヘッダーを使用することをお勧めします。セッション ヘッダーを使用しない場合は、API の呼び出し時に行われた変更がファイルに永続化_されます_。</span><span class="sxs-lookup"><span data-stu-id="ab09e-p108">**Note:** The session header is not required for an Excel API to work. However, we recommend that you use the session header to improve performance. If you don't use a session header, changes made during the API call _are_ persisted to the file.</span></span>  

### <a name="api-call-to-get-a-session"></a><span data-ttu-id="ab09e-132">セッションを取得するための API の呼び出し</span><span class="sxs-lookup"><span data-stu-id="ab09e-132">API call to get a session</span></span> 

#### <a name="request"></a><span data-ttu-id="ab09e-133">要求</span><span class="sxs-lookup"><span data-stu-id="ab09e-133">Request</span></span> 

<span data-ttu-id="ab09e-134">`persistchanges` 値を `true` または `false` に設定して JSON オブジェクトを渡します。</span><span class="sxs-lookup"><span data-stu-id="ab09e-134">Pass a JSON object by setting the `persistchanges` value to `true` or `false`.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/createSession
content-type: Application/Json 
authorization: Bearer {access-token}

{ "persistChanges": true }
```

<span data-ttu-id="ab09e-135">`persistChanges` の値が `false` に設定された場合に、非永続セッション ID が返されます。</span><span class="sxs-lookup"><span data-stu-id="ab09e-135">When the value of `persistChanges` is set to `false`, a non-persistent session id is returned.</span></span>  


#### <a name="response"></a><span data-ttu-id="ab09e-136">応答</span><span class="sxs-lookup"><span data-stu-id="ab09e-136">Response</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 201 Created
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#microsoft.graph.sessionInfo",
  "id": "{session-id}",
  "persistChanges": true
}
```

#### <a name="usage"></a><span data-ttu-id="ab09e-137">使用方法</span><span class="sxs-lookup"><span data-stu-id="ab09e-137">Usage</span></span> 

<span data-ttu-id="ab09e-138">以前の呼び出しから返されたセッション ID は、後続の API 要求のヘッダーとして渡されます</span><span class="sxs-lookup"><span data-stu-id="ab09e-138">The session ID returned from the previous call is passed as a header on subsequent API requests in</span></span>  
<span data-ttu-id="ab09e-139">`workbook-session-id` HTTP ヘッダー。</span><span class="sxs-lookup"><span data-stu-id="ab09e-139">`workbook-session-id` HTTP header.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

><span data-ttu-id="ab09e-140">注: セッション ID の有効期限が切れていた場合、そのセッションで `404` HTTP エラー コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="ab09e-140">Note: If the session id has expired, a `404` HTTP error code is returned on the session.</span></span> <span data-ttu-id="ab09e-141">このようなシナリオでは、新しいセッションを作成して続行できます。</span><span class="sxs-lookup"><span data-stu-id="ab09e-141">In such a scenarion, you can choose to create a new session and continue.</span></span> <span data-ttu-id="ab09e-142">または、定期的にセッションを更新して維持するという方法もあります。</span><span class="sxs-lookup"><span data-stu-id="ab09e-142">Another approach would be to refresh the session periodically to keep the session alive.</span></span> <span data-ttu-id="ab09e-143">通常、永続セッションの有効期限は、非アクティブ状態が約 7 分間経過した後に切れます。</span><span class="sxs-lookup"><span data-stu-id="ab09e-143">Typically the persistent session expires after about 7 minutes of inactivity.</span></span> <span data-ttu-id="ab09e-144">非永続セッションの有効期限は、非アクティブ状態が約 5 分間経過した後に切れます。</span><span class="sxs-lookup"><span data-stu-id="ab09e-144">Non persistent session expires after about 5 minutes of inactivity.</span></span> 

## <a name="common-excel-scenarios"></a><span data-ttu-id="ab09e-145">一般的な Excel のシナリオ</span><span class="sxs-lookup"><span data-stu-id="ab09e-145">Common Excel scenarios</span></span>

<span data-ttu-id="ab09e-146">このセクションでは、Excel オブジェクトで使用できる一般的な操作の例を示します。</span><span class="sxs-lookup"><span data-stu-id="ab09e-146">This section provides examples of the common operations you can use on Excel objects.</span></span>

### <a name="worksheet-operations"></a><span data-ttu-id="ab09e-147">ワークシート操作</span><span class="sxs-lookup"><span data-stu-id="ab09e-147">Worksheet operations</span></span>

#### <a name="list-worksheets-part-of-the-workbook"></a><span data-ttu-id="ab09e-148">ブックのワークシート部分の一覧表示</span><span class="sxs-lookup"><span data-stu-id="ab09e-148">List worksheets part of the workbook</span></span> 
<span data-ttu-id="ab09e-149">要求</span><span class="sxs-lookup"><span data-stu-id="ab09e-149">Request</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets
accept: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="ab09e-150">応答</span><span class="sxs-lookup"><span data-stu-id="ab09e-150">Response</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets",
  "value": [
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets(%27%7B00000000-0001-0000-0000-000000000000%7D%27)",
      "id": "{00000000-0001-0000-0000-000000000000}",
      "name": "Sheet1",
      "position": 0,
      "visibility": "Visible"
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets(%27%7B00000000-0001-0000-0100-000000000000%7D%27)",
      "id": "{00000000-0001-0000-0100-000000000000}",
      "name": "Sheet57664",
      "position": 1,
      "visibility": "Visible"
    }
  ]
}
```
#### <a name="add-a-new-worksheet"></a><span data-ttu-id="ab09e-151">新しいワークシートの追加</span><span class="sxs-lookup"><span data-stu-id="ab09e-151">Add a new worksheet</span></span> 
 
<!-- { "blockType": "ignored" } -->
```http
POST /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "name": "Sheet32243" }
```

<span data-ttu-id="ab09e-152">応答</span><span class="sxs-lookup"><span data-stu-id="ab09e-152">Response</span></span> 
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 201 Created
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets(%27%7B75A18F35-34AA-4F44-97CC-FDC3C05D9F40%7D%27)",
  "id": "{75A18F35-34AA-4F44-97CC-FDC3C05D9F40}",
  "name": "Sheet32243",
  "position": 5,
  "visibility": "Visible"
}
```

#### <a name="get-a-new-worksheet"></a><span data-ttu-id="ab09e-153">新しいワークシートの取得</span><span class="sxs-lookup"><span data-stu-id="ab09e-153">Get a new worksheet</span></span> 

<span data-ttu-id="ab09e-154">名前に基づいてワークシートを取得します。</span><span class="sxs-lookup"><span data-stu-id="ab09e-154">Get a worksheet based on the name.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets/Sheet32243
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="ab09e-155">応答</span><span class="sxs-lookup"><span data-stu-id="ab09e-155">Response</span></span> 
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets(%27%7B75A18F35-34AA-4F44-97CC-FDC3C05D9F40%7D%27)",
  "id": "{75A18F35-34AA-4F44-97CC-FDC3C05D9F40}",
  "name": "Sheet32243",
  "position": 5,
  "visibility": "Visible"
}
```

<span data-ttu-id="ab09e-p110">** 注:ID を使用してワークシートを取得することもできます。ただし、現在、ID には `{` と '}' 文字が含まれているため、API を実行できるよう、URL エンコードする必要があります。例:`{75A18F35-34AA-4F44-97CC-FDC3C05D9F40}` という ID のワークシートを取得するためには、パスの ID を `/workbook/worksheets/%7B75A18F35-34AA-4F44-97CC-FDC3C05D9F40%7D` として URL エンコードします。</span><span class="sxs-lookup"><span data-stu-id="ab09e-p110">** Note: Worksheets can also be retrieved using the ID. However, currently the ID contains `{` and '}' characters, which needs to be URL encoded for the API to work. Example: In order to get a worksheet with ID of `{75A18F35-34AA-4F44-97CC-FDC3C05D9F40}`, URL encode the ID in the path as `/workbook/worksheets/%7B75A18F35-34AA-4F44-97CC-FDC3C05D9F40%7D`.</span></span> 

#### <a name="delete-a-worksheet"></a><span data-ttu-id="ab09e-159">ワークシートの削除</span><span class="sxs-lookup"><span data-stu-id="ab09e-159">Delete a worksheet</span></span>

<span data-ttu-id="ab09e-160">要求</span><span class="sxs-lookup"><span data-stu-id="ab09e-160">Request</span></span>
```
DELETE /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets('%7B75A18F35-34AA-4F44-97CC-FDC3C05D9F40%7D')
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="ab09e-161">応答</span><span class="sxs-lookup"><span data-stu-id="ab09e-161">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```


#### <a name="update-worksheet-properties"></a><span data-ttu-id="ab09e-162">ワークシート プロパティの更新</span><span class="sxs-lookup"><span data-stu-id="ab09e-162">Update worksheet properties</span></span>

<span data-ttu-id="ab09e-163">要求</span><span class="sxs-lookup"><span data-stu-id="ab09e-163">Request</span></span> 

```
PATCH /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets/SheetA
content-type: Application/Json 
accept: application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "name": "SheetA", "position": 3 }
```

<span data-ttu-id="ab09e-164">応答</span><span class="sxs-lookup"><span data-stu-id="ab09e-164">Response</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets(%27%7B00000000-0001-0000-0100-000000000000%7D%27)",
  "id": "{00000000-0001-0000-0100-000000000000}",
  "name": "SheetA",
  "position": 3,
  "visibility": "Visible"
}
```

### <a name="chart-operations"></a><span data-ttu-id="ab09e-165">グラフ操作</span><span class="sxs-lookup"><span data-stu-id="ab09e-165">Chart operations</span></span>

#### <a name="list-charts-that-are-part-of-the-worksheet"></a><span data-ttu-id="ab09e-166">ワークシートの一部になっているグラフを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="ab09e-166">List charts that are part of the worksheet</span></span> 

<span data-ttu-id="ab09e-167">要求</span><span class="sxs-lookup"><span data-stu-id="ab09e-167">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http 
GET /{version}/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts
accept: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id} 
```

<span data-ttu-id="ab09e-168">応答</span><span class="sxs-lookup"><span data-stu-id="ab09e-168">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL')/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts",
  "value": [
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL')/workbook/worksheets(%27%7B00000000-0001-0000-0000-000000000000%7D%27)/charts(%27%7B00000000-0008-0000-0100-000003000000%7D%27)",
      "height": 235.5,
      "id": "{00000000-0008-0000-0100-000003000000}",
      "left": 276.0,
      "name": "Chart 2",
      "top": 0.0,
      "width": 401.25
   }
  ]
}
```

<span data-ttu-id="ab09e-p111">** 注:ただし、ID には `{` と `}` 文字が含まれているため (例: `{00000000-0008-0000-0100-000003000000}`)、API を実行できるよう、URL エンコードする必要があります。例:グラフ オブジェクトを取得するためには、パスの ID を `/charts/%7B00000000-0008-0000-0100-000003000000%7D` として URL エンコードします。</span><span class="sxs-lookup"><span data-stu-id="ab09e-p111">** Note: Chart ID contains `{` and `}` characters (example: `{00000000-0008-0000-0100-000003000000}`), which needs to be URL encoded for the API to work. Example: In order to get a chart object, URL encode the ID in the path as `/charts/%7B00000000-0008-0000-0100-000003000000%7D`.</span></span> 

#### <a name="get-chart-image"></a><span data-ttu-id="ab09e-171">グラフの画像を取得する</span><span class="sxs-lookup"><span data-stu-id="ab09e-171">Get chart image</span></span>

<span data-ttu-id="ab09e-172">要求</span><span class="sxs-lookup"><span data-stu-id="ab09e-172">Request</span></span> 
<!-- { "blockType": "ignored" } -->
```http
GET /{version}/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts('%7B00000000-0008-0000-0100-000003000000%7D')/Image(width=0,height=0,fittingMode='fit')
authorization: Bearer {access-token} 
workbook-session-id: {session-id} 
```

<span data-ttu-id="ab09e-173">応答</span><span class="sxs-lookup"><span data-stu-id="ab09e-173">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#Edm.String",
  "value": "{base-64-string}"
}
```

#### <a name="add-a-chart"></a><span data-ttu-id="ab09e-174">グラフの追加</span><span class="sxs-lookup"><span data-stu-id="ab09e-174">Add a chart</span></span>  

<span data-ttu-id="ab09e-175">要求</span><span class="sxs-lookup"><span data-stu-id="ab09e-175">Request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /{version}/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts/Add
content-type: Application/Json 
accept: application/Json 
authorization: Bearer {access-token} 

{ "type": "ColumnClustered", "sourcedata": "A1:C4", "seriesby": "Auto" }
```

<span data-ttu-id="ab09e-176">応答</span><span class="sxs-lookup"><span data-stu-id="ab09e-176">Response</span></span> 
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 201 Created
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#chart",
  "@odata.type": "#microsoft.graph.chart",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL')/workbook/worksheets(%27%7B00000000-0001-0000-0000-000000000000%7D%27)/charts(%27%7B2D421098-FA19-41F7-8528-EE7B00E4BB42%7D%27)",
  "height": 216.0,
  "id": "{2D421098-FA19-41F7-8528-EE7B00E4BB42}",
  "left": 0.0,
  "name": "Chart 2",
  "top": 0.0,
  "width": 360.0
}
```

#### <a name="update-a-chart"></a><span data-ttu-id="ab09e-177">グラフの更新</span><span class="sxs-lookup"><span data-stu-id="ab09e-177">Update a chart</span></span>

<!-- { "blockType": "ignored" } -->
```http 
PATCH /{version}/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts('%7B2D421098-FA19-41F7-8528-EE7B00E4BB42%7D')
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "height": 216.0, "left": 0, "name": "NewName", "top": 0, "width": 360.0 }

```
<span data-ttu-id="ab09e-178">応答</span><span class="sxs-lookup"><span data-stu-id="ab09e-178">Response</span></span> 

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL')/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL')/workbook/worksheets(%27%7B00000000-0001-0000-0000-000000000000%7D%27)/charts(%27%7B2D421098-FA19-41F7-8528-EE7B00E4BB42%7D%27)",
  "height": 216.0,
  "id": "{2D421098-FA19-41F7-8528-EE7B00E4BB42}",
  "left": 0.0,
  "name": "NewName",
  "top": 0.0,
  "width": 360.0
}
```

#### <a name="update-chart-source-data"></a><span data-ttu-id="ab09e-179">グラフのソース データの更新</span><span class="sxs-lookup"><span data-stu-id="ab09e-179">Update chart source data</span></span> 

<span data-ttu-id="ab09e-180">要求</span><span class="sxs-lookup"><span data-stu-id="ab09e-180">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /{version}/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts('%7B2D421098-FA19-41F7-8528-EE7B00E4BB42%7D')/setData
content-type: Application/Json 
accept: application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "sourceData": "A1:C4", "seriesBy": "Auto" }
```

<span data-ttu-id="ab09e-181">応答</span><span class="sxs-lookup"><span data-stu-id="ab09e-181">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```

### <a name="table-operations"></a><span data-ttu-id="ab09e-182">テーブルの操作</span><span class="sxs-lookup"><span data-stu-id="ab09e-182">Table operations</span></span> 

#### <a name="get-list-of-tables"></a><span data-ttu-id="ab09e-183">テーブル一覧の取得</span><span class="sxs-lookup"><span data-stu-id="ab09e-183">Get list of tables</span></span> 

<span data-ttu-id="ab09e-184">要求</span><span class="sxs-lookup"><span data-stu-id="ab09e-184">Request</span></span> 
<!-- { "blockType": "ignored" } -->
```http
GET /{version}/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/tables
accept: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="ab09e-185">応答</span><span class="sxs-lookup"><span data-stu-id="ab09e-185">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 
```

#### <a name="update-table"></a><span data-ttu-id="ab09e-186">テーブルの更新</span><span class="sxs-lookup"><span data-stu-id="ab09e-186">Update table</span></span>

<span data-ttu-id="ab09e-187">要求</span><span class="sxs-lookup"><span data-stu-id="ab09e-187">Request</span></span> 
<!-- { "blockType": "ignored" } -->
```http 
PATCH /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('2')
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "name": "NewTableName", "showHeaders": true, "showTotals": false, "style": "TableStyleMedium4" }
```

<span data-ttu-id="ab09e-188">応答</span><span class="sxs-lookup"><span data-stu-id="ab09e-188">Response</span></span> 
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%272%27)",
  "id": "2",
  "name": "NewTableName",
  "showHeaders": true,
  "showTotals": false,
  "style": "TableStyleMedium4"
}
```

#### <a name="get-list-of-table-rows"></a><span data-ttu-id="ab09e-189">テーブル行の一覧の取得</span><span class="sxs-lookup"><span data-stu-id="ab09e-189">Get list of table rows</span></span>
<span data-ttu-id="ab09e-190">要求</span><span class="sxs-lookup"><span data-stu-id="ab09e-190">Request</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('4')/Rows
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="ab09e-191">応答</span><span class="sxs-lookup"><span data-stu-id="ab09e-191">Response</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables('4')/rows",
  "value": [
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/rows/itemAt(0)",
      "index": 0,
      "values": [
        [
          42019,
          53,
          34
       ]
      ]
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/rows/itemAt(1)",
      "index": 1,
      "values": [
        [
          42020,
          45,
          39
        ]
      ]
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/rows/itemAt(2)",
      "index": 2,
      "values": [
        [
          42021,
          50,
          31
        ]
      ]
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/rows/itemAt(3)",
      "index": 3,
      "values": [
        [
          42022,
          43,
          39
        ]
      ]
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/rows/itemAt(4)",
      "index": 4,
      "values": [
        [
          42023,
          45,
          41
        ]
      ]
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/rows/itemAt(5)",
      "index": 5,
      "values": [
        [
          42024,
          52,
          40
        ]
      ]
    }
  ]
}
```

#### <a name="get-list-of-table-columns"></a><span data-ttu-id="ab09e-192">テーブル列の一覧の取得</span><span class="sxs-lookup"><span data-stu-id="ab09e-192">Get list of table columns</span></span>

<span data-ttu-id="ab09e-193">要求</span><span class="sxs-lookup"><span data-stu-id="ab09e-193">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('4')/Columns
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="ab09e-194">応答</span><span class="sxs-lookup"><span data-stu-id="ab09e-194">Response</span></span> 

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK 
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables('4')/columns",
  "value": [
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/columns(%271%27)",
      "id": "1",
      "index": 0,
      "name": "Date",
      "values": [
        [
          "Date"
        ],
        [
          42019
       ],
        [
          42020
        ],
        [
          42021
        ],
        [
          42022
        ],
        [
          42023
        ],
        [
          42024
        ]
      ]
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/columns(%272%27)",
      "id": "2",
      "index": 1,
      "name": "High (F)",
      "values": [
        [
          "High (F)"
        ],
        [
          53
        ],
        [
          45
        ],
        [
          50
        ],
        [
          43
        ],
        [
          45
        ],
        [
          52
        ]
      ]
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/columns(%273%27)",
      "id": "3",
      "index": 2,
      "name": "Low (F)",
      "values": [
        [
          "Low (F)"
        ],
        [
          34
        ],
        [
          39
        ],
        [
          31
        ],
        [
          39
        ],
        [
          41
        ],
        [
          40
        ]
      ]
    }
  ]
}
```


#### <a name="add-a-table-row"></a><span data-ttu-id="ab09e-195">テーブル行の追加</span><span class="sxs-lookup"><span data-stu-id="ab09e-195">Add a table row</span></span>

<span data-ttu-id="ab09e-196">要求</span><span class="sxs-lookup"><span data-stu-id="ab09e-196">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('4')/Rows
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "values": [ [ "Jan-15-2016", "49", "37" ] ], "index": null }
```

<span data-ttu-id="ab09e-197">応答</span><span class="sxs-lookup"><span data-stu-id="ab09e-197">Response</span></span> 
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 201 Created
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables('4')/rows/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/rows(null)",
  "index": 6,
  "values": [
    [
      "Jan-15-2016",
      49,
      37
    ]
  ]
}
```

#### <a name="add-a-table-column"></a><span data-ttu-id="ab09e-198">テーブル列の追加</span><span class="sxs-lookup"><span data-stu-id="ab09e-198">Add a table column</span></span> 

<span data-ttu-id="ab09e-199">要求</span><span class="sxs-lookup"><span data-stu-id="ab09e-199">Request</span></span> 
<!-- { "blockType": "ignored" } -->
```http 
POST /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('2')/Columns
content-type: Application/Json 
accept: application/Json 


{ "values": [ [ "Status" ], [ "Open" ], [ "Closed" ] ], "index": 2 }
```

<span data-ttu-id="ab09e-200">応答</span><span class="sxs-lookup"><span data-stu-id="ab09e-200">Response</span></span> 

<!-- { "blockType": "ignored" } -->
```http 
HTTP code: 201 Created
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables('2')/columns/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%272%27)/columns(%274%27)",
  "id": "4",
  "index": 2,
  "name": "Status",
  "values": [
    [
      "Status"
    ],
    [
      "Open"
    ],
    [
      "Closed"
    ]
  ]
}
```

#### <a name="delete-table-row"></a><span data-ttu-id="ab09e-201">テーブル行の削除</span><span class="sxs-lookup"><span data-stu-id="ab09e-201">Delete table row</span></span>

<span data-ttu-id="ab09e-202">要求</span><span class="sxs-lookup"><span data-stu-id="ab09e-202">Request</span></span> 
<!-- { "blockType": "ignored" } -->
```http  
DELETE /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('4')/Rows/$/ItemAt(index=6)
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="ab09e-203">応答</span><span class="sxs-lookup"><span data-stu-id="ab09e-203">Response</span></span> 
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```

#### <a name="delete-table-column"></a><span data-ttu-id="ab09e-204">テーブル列の削除</span><span class="sxs-lookup"><span data-stu-id="ab09e-204">Delete table column</span></span> 
<span data-ttu-id="ab09e-205">要求</span><span class="sxs-lookup"><span data-stu-id="ab09e-205">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('4')/Columns('3')
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="ab09e-206">応答</span><span class="sxs-lookup"><span data-stu-id="ab09e-206">Response</span></span> 
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```

#### <a name="convert-table-to-range"></a><span data-ttu-id="ab09e-207">テーブルを範囲に変換する</span><span class="sxs-lookup"><span data-stu-id="ab09e-207">Convert table to range</span></span> 
<span data-ttu-id="ab09e-208">要求</span><span class="sxs-lookup"><span data-stu-id="ab09e-208">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('1')/convertToRange
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="ab09e-209">応答</span><span class="sxs-lookup"><span data-stu-id="ab09e-209">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK 
content-type: application/json;odata.metadata 
```

#### <a name="table-sort"></a><span data-ttu-id="ab09e-210">テーブルの並べ替え</span><span class="sxs-lookup"><span data-stu-id="ab09e-210">Table sort</span></span>
<span data-ttu-id="ab09e-211">要求</span><span class="sxs-lookup"><span data-stu-id="ab09e-211">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets('Sheet15799')/tables('table2')/sort/apply
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{
"fields" : [
  { "key": 0,
   "ascending": true
  }
]
}
```


<span data-ttu-id="ab09e-212">応答</span><span class="sxs-lookup"><span data-stu-id="ab09e-212">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```

#### <a name="table-filter"></a><span data-ttu-id="ab09e-213">テーブル フィルター</span><span class="sxs-lookup"><span data-stu-id="ab09e-213">Table filter</span></span>
<span data-ttu-id="ab09e-214">要求</span><span class="sxs-lookup"><span data-stu-id="ab09e-214">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets('Sheet15799')/tables('table2')/columns(id='2')/filter/apply
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{
"criteria" : 
  { "filterOn": "custom",
   "criterion1": ">15",
   "operator": "and",
   "criterion2": "<50"
   
  }
}
```

<span data-ttu-id="ab09e-215">応答</span><span class="sxs-lookup"><span data-stu-id="ab09e-215">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```


#### <a name="clear-filter"></a><span data-ttu-id="ab09e-216">フィルターのクリア</span><span class="sxs-lookup"><span data-stu-id="ab09e-216">Clear filter</span></span>
<span data-ttu-id="ab09e-217">要求</span><span class="sxs-lookup"><span data-stu-id="ab09e-217">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets('Sheet15799')/tables('table2')/columns(id='2')/filter/clear
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="ab09e-218">応答</span><span class="sxs-lookup"><span data-stu-id="ab09e-218">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```

### <a name="range-operations"></a><span data-ttu-id="ab09e-219">範囲の操作</span><span class="sxs-lookup"><span data-stu-id="ab09e-219">Range operations</span></span>

#### <a name="get-range"></a><span data-ttu-id="ab09e-220">範囲の取得</span><span class="sxs-lookup"><span data-stu-id="ab09e-220">Get Range</span></span> 

<span data-ttu-id="ab09e-221">要求</span><span class="sxs-lookup"><span data-stu-id="ab09e-221">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/worksheets('test')/range(address='A1:B2')
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="ab09e-222">応答</span><span class="sxs-lookup"><span data-stu-id="ab09e-222">Response</span></span> 

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#range",
  "@odata.type": "#microsoft.graph.range",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/worksheets(%27%7B00000000-0001-0000-0300-000000000000%7D%27)/range(address=%27A1:B2%27)",
  "address": "test!A1:B2",
  "addressLocal": "test!A1:B2",
  "cellCount": 4,
  "columnCount": 2,
  "columnHidden": false,
  "columnIndex": 0,
  "formulas": [
    [
      "",
      ""
    ],
    [
      "",
      ""
    ]
  ],
  "formulasLocal": [
    [
      "",
      ""
    ],
    [
      "",
      ""
    ]
  ],
  "formulasR1C1": [
    [
      "",
      ""
    ],
    [
      "",
      ""
    ]
  ],
  "hidden": false,
  "numberFormat": [
    [
      "General",
      "General"
    ],
    [
      "General",
      "General"
    ]
  ],
  "rowCount": 2,
  "rowHidden": false,
  "rowIndex": 0,
  "text": [
    [
      "",
      ""
    ],
    [
      "",
      ""
    ]
  ],
  "values": [
    [
      "",
      ""
    ],
    [
      "",
      ""
    ]
  ],
  "valueTypes": [
    [
      "Empty",
      "Empty"
    ],
    [
      "Empty",
      "Empty"
    ]
  ]
}
```

#### <a name="range-update"></a><span data-ttu-id="ab09e-223">範囲の更新</span><span class="sxs-lookup"><span data-stu-id="ab09e-223">Range update</span></span> 

<!-- { "blockType": "ignored" } -->
```http
PATCH /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/worksheets('test')/range(address='test!A1:B2')
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "values": [ [ "Test", "Value" ], [ "For", "Update" ] ] }
```

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#range",
  "@odata.type": "#microsoft.graph.range",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/worksheets(%27%7B00000000-0001-0000-0300-000000000000%7D%27)/range(address=%27test!A1:B2%27)",
  "address": "test!A1:B2",
  "addressLocal": "test!A1:B2",
  "cellCount": 4,
  "columnCount": 2,
  "columnHidden": false,
  "columnIndex": 0,
  "formulas": [
    [
      "Test",
      "Value"
    ],
    [
      "For",
      "Update"
    ]
  ],
  "formulasLocal": [
    [
      "Test",
      "Value"
    ],
    [
      "For",
      "Update"
    ]
  ],
  "formulasR1C1": [
    [
      "Test",
      "Value"
    ],
    [
      "For",
      "Update"
    ]
  ],
  "hidden": false,
  "numberFormat": [
    [
      "General",
      "General"
    ],
    [
      "General",
      "General"
    ]
  ],
  "rowCount": 2,
  "rowHidden": false,
  "rowIndex": 0,
  "text": [
    [
      "Test",
      "Value"
    ],
    [
      "For",
      "Update"
    ]
  ],
  "values": [
    [
      "Test",
      "Value"
    ],
    [
      "For",
      "Update"
    ]
  ],
  "valueTypes": [
    [
      "String",
      "String"
    ],
    [
      "String",
      "String"
    ]
  ]
}
```

#### <a name="range-sort"></a><span data-ttu-id="ab09e-224">範囲の並べ替え</span><span class="sxs-lookup"><span data-stu-id="ab09e-224">Range sort</span></span>
<span data-ttu-id="ab09e-225">要求</span><span class="sxs-lookup"><span data-stu-id="ab09e-225">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets('Sheet15799')/usedRange/sort/apply
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{
"fields" : [
  { "key": 0,
   "ascending": true
  }
]
}
```

<span data-ttu-id="ab09e-226">応答</span><span class="sxs-lookup"><span data-stu-id="ab09e-226">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```


### <a name="named-items"></a><span data-ttu-id="ab09e-227">名前付きアイテム</span><span class="sxs-lookup"><span data-stu-id="ab09e-227">Named items</span></span>
<span data-ttu-id="ab09e-228">要求</span><span class="sxs-lookup"><span data-stu-id="ab09e-228">Request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/names
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="ab09e-229">応答</span><span class="sxs-lookup"><span data-stu-id="ab09e-229">Response</span></span> 

<!-- { "blockType": "ignored" } -->
```http 
HTTP code: 200 OK
content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/names",
  "value": [
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/names(%27data%27)",
      "name": "data",
      "type": "Range",
      "value": "Range!$A$1:$D$3",
      "visible": true
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/names(%27myrange%27)",
      "name": "myrange",
      "type": "Range",
      "value": "Range!$E$1:$F$7",
      "visible": true
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/names(%27range1%27)",
      "name": "range1",
      "type": "Range",
      "value": "Range!$I$1:$M$11",
      "visible": true
    }
  ]
}
```

### <a name="work-with-nulls"></a><span data-ttu-id="ab09e-230">Null の操作</span><span class="sxs-lookup"><span data-stu-id="ab09e-230">Work with nulls</span></span>

#### <a name="null-input-in-2-d-array"></a><span data-ttu-id="ab09e-231">2 次元配列での null の入力</span><span class="sxs-lookup"><span data-stu-id="ab09e-231">null input in 2-D array</span></span>

<span data-ttu-id="ab09e-p112">範囲およびテーブル リソースでは、2 次元配列内の (値、番号書式、数式に対する) `null` の入力は無視されます。値や値の番号書式または数式のグリッドに `null` の入力を送信する場合、指定の対象 (セル) に対しては更新が行われません。</span><span class="sxs-lookup"><span data-stu-id="ab09e-p112">`null` input inside a two-dimensional array (for values, number-format, formula) is ignored in the Range and Table resources. No update will take place to the intended target (cell) when `null` input is sent in values or number-format or formula grid of values.</span></span>

<span data-ttu-id="ab09e-234">たとえば、範囲の特定の部分 (セルの番号書式など) のみを更新し、範囲のその他の部分では既存の番号書式を保持する場合は、必要な部分で番号書式を設定し、他のセルに対しては `null` を送信します。</span><span class="sxs-lookup"><span data-stu-id="ab09e-234">For example, to only update specific parts of the Range, such as a cell's Number Format, and to retain the existing number-format on other parts of the Range, set the Number Format where needed and send `null` for the other cells.</span></span>

<span data-ttu-id="ab09e-235">次の設定要求では、範囲内のある部分の番号書式のみを設定し、残りの部分では (null 値を渡すことで) 既存の番号書式を保持します。</span><span class="sxs-lookup"><span data-stu-id="ab09e-235">In the following set request, only some parts of the Range Number Format are set while the existing Number Format on the remaining part is retained (by passing nulls).</span></span>

```json
{
  "values" : [["Eurasia", "29.96", "0.25", "15-Feb" ]],
  "numberFormat" : [[null, null, null, "m/d/yyyy;@"]]
}
```

#### <a name="null-input-for-a-property"></a><span data-ttu-id="ab09e-236">プロパティに対する null の入力</span><span class="sxs-lookup"><span data-stu-id="ab09e-236">null input for a property</span></span>

<span data-ttu-id="ab09e-p113">`null` を、プロパティ全体に対する単独の入力として指定することはできません。たとえば、値全体を null に設定したり無視したりすることはできないため、以下は無効になります。</span><span class="sxs-lookup"><span data-stu-id="ab09e-p113">`null` is not a valid single input for the entire property. For example, the following is not valid because the entire values cannot be set to null or ignored.</span></span>

```json
{
"values":  null
}

```

<span data-ttu-id="ab09e-239">null は有効なカラー値ではないため、以下も無効になります。</span><span class="sxs-lookup"><span data-stu-id="ab09e-239">The following is not valid either as null is not a valid color value.</span></span>

```json
{
"color" :  null
}
```

#### <a name="null-response"></a><span data-ttu-id="ab09e-240">null 応答</span><span class="sxs-lookup"><span data-stu-id="ab09e-240">Null-Response</span></span>

<span data-ttu-id="ab09e-241">均一でない値で構成された書式設定プロパティを表現すると、null 値が応答で返されます。</span><span class="sxs-lookup"><span data-stu-id="ab09e-241">Representation of formatting properties that consists of non-uniform values results in the return of a null value in the response.</span></span>

<span data-ttu-id="ab09e-p114">たとえば、範囲は 1 つ以上のセルで構成できます。指定した範囲に含まれる個々のセルの書式設定値が均一でない場合、その範囲のレベルの表示形式は定義されません。</span><span class="sxs-lookup"><span data-stu-id="ab09e-p114">For example, a Range can consist of one or more cells. In cases where the individual cells contained in the Range specified don't have uniform formatting values, the range level representation will be undefined.</span></span>

```json
{
  "size: : null,
  "color" : null
}
```


### <a name="blank-input-and-output"></a><span data-ttu-id="ab09e-244">空の入力と出力</span><span class="sxs-lookup"><span data-stu-id="ab09e-244">Blank input and output</span></span>

<span data-ttu-id="ab09e-p115">更新要求にある空の値は、それぞれのプロパティをクリアまたはリセットする命令として扱われます。空の値は、間にスペースを入れない 2 つの二重引用符によって表されます。`""`</span><span class="sxs-lookup"><span data-stu-id="ab09e-p115">Blank values in update requests are treated as an instruction to clear or reset the respective property. A blank value is represented by two double quotation marks with no space in-between: `""`</span></span>

<span data-ttu-id="ab09e-247">例:</span><span class="sxs-lookup"><span data-stu-id="ab09e-247">Examples:</span></span>

* <span data-ttu-id="ab09e-248">`values` の場合は、範囲の値がクリアされます。これは、アプリケーションの内容をクリアするのと同じです。</span><span class="sxs-lookup"><span data-stu-id="ab09e-248">For `values`, the range value is cleared out. This is the same as clearing the contents in the application.</span></span>

* <span data-ttu-id="ab09e-249">`numberFormat` の場合は、番号書式が `General` に設定されます。</span><span class="sxs-lookup"><span data-stu-id="ab09e-249">For `numberFormat`, the number format is set to `General`.</span></span>

* <span data-ttu-id="ab09e-250">`formula` および `formulaLocale` の場合は、数式の値がクリアされます。</span><span class="sxs-lookup"><span data-stu-id="ab09e-250">For `formula` and `formulaLocale`, the formula values are cleared.</span></span>


<span data-ttu-id="ab09e-p116">読み取り操作では、セルの内容が空白の場合に空白の値を受け取ることが予想されます。セルにデータや値が含まれていない場合、API は空の値を返します。空の値は、間にスペースを入れない 2 つの二重引用符によって表されます。`""`</span><span class="sxs-lookup"><span data-stu-id="ab09e-p116">For read operations, expect to receive blank values if the contents of the cells are blanks. If the cell contains no data or value, the API returns a blank value. Blank value is represented by two double quotation marks with no space in-between: `""`</span></span>

```json
{
  "values" : [["", "some", "data", "in", "other", "cells", ""]]
}
```

```json
{
  "formula" : [["", "", "=Rand()"]]
}
```


### <a name="unbounded-range"></a><span data-ttu-id="ab09e-254">無制限の範囲</span><span class="sxs-lookup"><span data-stu-id="ab09e-254">Unbounded Range</span></span>

#### <a name="read"></a><span data-ttu-id="ab09e-255">読み取り</span><span class="sxs-lookup"><span data-stu-id="ab09e-255">Read</span></span>

<span data-ttu-id="ab09e-256">無制限の範囲のアドレスは、列識別子のみがあって行識別子が未指定であるか、あるいは行識別子のみがあって列識別子が未指定です。たとえば、次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="ab09e-256">Unbounded Range address contains only column or row identifiers and unspecified row identifier or column identifiers (respectively), such as:</span></span>

* <span data-ttu-id="ab09e-257">`C:C`、`A:F`、`A:XFD` (行が未指定)</span><span class="sxs-lookup"><span data-stu-id="ab09e-257">`C:C`, `A:F`, `A:XFD` (contains unspecified rows)</span></span>
* <span data-ttu-id="ab09e-258">`2:2`、`1:4`、`1:1048546` (列が未指定)</span><span class="sxs-lookup"><span data-stu-id="ab09e-258">`2:2`, `1:4`, `1:1048546` (contains unspecified columns)</span></span>

<span data-ttu-id="ab09e-p117">API が無制限の範囲を取得する要求を行う場合 (`getRange('C:C')`)、返される応答では、`values`、`text`、`numberFormat`、または `formula` などのセル レベルのプロパティに `null` が含まれます。`address`、または `cellCount` などのその他の範囲プロパティは、無制限の範囲を反映します。</span><span class="sxs-lookup"><span data-stu-id="ab09e-p117">When the API makes a request to retrieve an unbounded Range (`getRange('C:C')`), the response returned contains `null` for cell-level properties such as `values`, `text`, `numberFormat`, or `formula`. Other Range properties such as `address` or `cellCount` will reflect the unbounded range.</span></span>

#### <a name="write"></a><span data-ttu-id="ab09e-261">書き込み</span><span class="sxs-lookup"><span data-stu-id="ab09e-261">Write</span></span>

<span data-ttu-id="ab09e-262">無制限のセル範囲にセル レベルのプロパティ (values、numberFormat など) を設定することは、入力要求が長すぎて処理できない可能性があるため、**許可されていません**。</span><span class="sxs-lookup"><span data-stu-id="ab09e-262">Setting cell level properties (such as values, numberFormat, etc.) on unbounded Range is **not allowed** because the input request might be too large to handle.</span></span>

<span data-ttu-id="ab09e-263">たとえば、要求された範囲が無制限であるため、次の更新要求は無効です。</span><span class="sxs-lookup"><span data-stu-id="ab09e-263">For example, the following is not a valid update request because the requested range is unbounded.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets('Sheet1')/range(address="A:B")

{
  "values" : "Due Date"
}
```

<span data-ttu-id="ab09e-264">このような範囲に対して更新操作を実行しようとすると、API はエラーを返します。</span><span class="sxs-lookup"><span data-stu-id="ab09e-264">When an update operation is attempted on such a Range, the API will return an error.</span></span>


### <a name="large-range"></a><span data-ttu-id="ab09e-265">広い範囲</span><span class="sxs-lookup"><span data-stu-id="ab09e-265">Large Range</span></span>

<span data-ttu-id="ab09e-p118">広い範囲とは、1 つの API の呼び出しに対してサイズが大きすぎる範囲を意味します。範囲に含まれる、セル数、値、番号書式、数式などの多くの要因によって、応答のサイズが大きくなりすぎて API での操作に適さなくなることがあります。API は、要求されたデータを返したり、それに書き込んだりしようと最善を尽くします。しかし、大きなサイズが関係していると、リソース使用率が大きくなるために、API エラー状態になることがあります。</span><span class="sxs-lookup"><span data-stu-id="ab09e-p118">Large Range implies a Range of a size that is too large for a single API call. Many factors such as number of cells, values, numberFormat, and formulas contained in the range can make the response so large that it becomes unsuitable for API interaction. The API makes a best attempt to return or write to the requested data. However, the large size involved might result in an API error condition because of the large resource utilization.</span></span>

<span data-ttu-id="ab09e-270">これを回避するには、広い範囲の読み取りや書き込みは、よりサイズの小さい複数の範囲に分けて実行することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="ab09e-270">To avoid this, we recommend that you read or write for large Range in multiple smaller range sizes.</span></span>


### <a name="single-input-copy"></a><span data-ttu-id="ab09e-271">単一の入力のコピー</span><span class="sxs-lookup"><span data-stu-id="ab09e-271">Single input copy</span></span>

<span data-ttu-id="ab09e-p119">同じ値または番号書式での範囲の更新や、範囲全体への同じ数式の適用をサポートするため、set API では以下の方法が用いられています。Excel では、この動作は、Ctrl+Enter モードで範囲に値や数式を入力することに似ています。</span><span class="sxs-lookup"><span data-stu-id="ab09e-p119">To support updating a range with the same values or number-format or applying same formula across a range, the following convention is used in the set API. In Excel, this behavior is similar to inputting values or formulas to a range in the CTRL+Enter mode.</span></span>

<span data-ttu-id="ab09e-274">API は *1 つのセル値*を探し、対象の範囲ディメンションが入力の範囲ディメンションと一致しない場合は、CTRL+Enter モードで範囲全体を、要求で指定された値または数式で更新します。</span><span class="sxs-lookup"><span data-stu-id="ab09e-274">The API will look for a *single cell value* and, if the target range dimension doesn't match the input range dimension, it will apply the update to the entire range in the CTRL+Enter model with the value or formula provided in the request.</span></span>

#### <a name="examples"></a><span data-ttu-id="ab09e-275">例</span><span class="sxs-lookup"><span data-stu-id="ab09e-275">Examples</span></span>

<span data-ttu-id="ab09e-p120">次の要求では、"Sample text" というテキストで選択範囲が更新されます。範囲に 200 個のセルがある一方、指定された入力には 1 つのセルの値のみがあることにご注意ください。</span><span class="sxs-lookup"><span data-stu-id="ab09e-p120">The following request updates the selected range with the text of "Sample text". Note that Range has 200 cells, whereas the provided input only has 1 cell value.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets('Sheet1')/range(address="A1:B00")

{
  "values" : "Sample text"
}
```

### <a name="workbook-functions"></a><span data-ttu-id="ab09e-278">ブックの関数</span><span class="sxs-lookup"><span data-stu-id="ab09e-278">Workbook functions</span></span> 
<span data-ttu-id="ab09e-279">/Functions リソースに含まれている関数のコレクションを介して、ブックの関数にアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="ab09e-279">You can access the workbook functions through a collection of functions included in the /Functions resource.</span></span> 

<!-- LG: Where is the Functions resource? We should link to this.
-->
##### <a name="request"></a><span data-ttu-id="ab09e-280">要求</span><span class="sxs-lookup"><span data-stu-id="ab09e-280">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
https://graph.microsoft.com/v1.0/me/drive/root:/book1.xlsx:/workbook/functions/pmt
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{
    "rate": 4.5,
    "nper": 12,
    "pv": -1250
}
```


##### <a name="response"></a><span data-ttu-id="ab09e-281">応答</span><span class="sxs-lookup"><span data-stu-id="ab09e-281">Response</span></span> 

<!-- { "blockType": "ignored" } -->
```http 
HTTP code: 200 OK
content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#workbookFunctionResult",
    "@odata.type": "#microsoft.graph.workbookFunctionResult",
    "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/root/workbook/functions/pmt()",
    "error": null,
    "value": 5625.00000734125
}
```

## <a name="error-information"></a><span data-ttu-id="ab09e-282">エラー情報</span><span class="sxs-lookup"><span data-stu-id="ab09e-282">Error information</span></span> 

<span data-ttu-id="ab09e-p121">HTTP エラー コードとエラー オブジェクトで、エラーが返されます。エラー `code` と `message` は、エラーの原因を説明します。</span><span class="sxs-lookup"><span data-stu-id="ab09e-p121">Errors are returned with an HTTP error code and an error object. An error `code` and `message` explain the reason for the error.</span></span>
 
<span data-ttu-id="ab09e-285">次に例を示します。</span><span class="sxs-lookup"><span data-stu-id="ab09e-285">The following is an example.</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 400 Bad Request
Content-Type: application/json

{
  "error": {
    "code": "ItemAlreadyExists",
    "message": "A resource with the same name or identifier already exists.",
    "innerError": {
      "request-id": "214ca7ea-9ea4-442e-9c67-71fdda0a559c",
      "date": "2016-07-28T03:56:09"
    }
  }
}
```

