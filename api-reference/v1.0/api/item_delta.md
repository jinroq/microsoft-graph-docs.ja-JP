# <a name="track-changes-for-a-drive"></a><span data-ttu-id="f1ebc-101">ドライブの変更履歴を記録する</span><span class="sxs-lookup"><span data-stu-id="f1ebc-101">Track changes for a Drive</span></span>

<span data-ttu-id="f1ebc-102">このメソッドでは、アプリがドライブおよびその子への変更履歴を時間の経過とともに記録できます。</span><span class="sxs-lookup"><span data-stu-id="f1ebc-102">This method allows your app to track changes to a drive and its children over time.</span></span>

<span data-ttu-id="f1ebc-p101">アプリはまず、パラメーターを指定せずに `delta` を呼び出します。サービスはドライブの階層の列挙を開始し、次に説明するように、アイテムのページと `@odata.nextLink` または `@odata.deltaLink` のいずれかを返します。`@odata.nextLink` が返されなくなるまで、または変更の空のセットが応答で返されるまで、アプリは `@odata.nextLink` を使って呼び出しを続けます。</span><span class="sxs-lookup"><span data-stu-id="f1ebc-p101">Your app begins by calling `delta` without any parameters. The service starts enumerating the drive's hierarchy, returning pages of items and either an `@odata.nextLink` or an `@odata.deltaLink`, as described below. Your app should continue calling with the `@odata.nextLink` until you no longer see an `@odata.nextLink` returned, or you see a response with an empty set of changes.</span></span>

<span data-ttu-id="f1ebc-p102">すべての変更を受信したら、それをローカルの状態に適用できます。今後の変更を確認するには、前回の応答の `@odata.deltaLink` を使ってもう一度 `delta` を呼び出します。</span><span class="sxs-lookup"><span data-stu-id="f1ebc-p102">After you have finished receiving all the changes, you may apply them to your local state. To check for changes in the future, call `delta` again with the `@odata.deltaLink` from the previous response.</span></span>

<span data-ttu-id="f1ebc-p103">削除されたアイテムは [`deleted` ファセット](../resources/deleted.md)付きで返されます。このプロパティ セットを持つアイテムは、ローカル状態から削除する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f1ebc-p103">Deleted items are returned with the [`deleted` facet](../resources/deleted.md). Items with this property set should be removed from your local state.</span></span> 

<span data-ttu-id="f1ebc-110">**注:** すべての変更を同期した後にフォルダーが空の場合にのみ、ローカルでそのフォルダーを削除する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f1ebc-110">**Note:** you should only delete a folder locally if it is empty after syncing all the changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="f1ebc-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f1ebc-111">Permissions</span></span>
<span data-ttu-id="f1ebc-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f1ebc-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f1ebc-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f1ebc-114">Permission type</span></span>      | <span data-ttu-id="f1ebc-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f1ebc-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1ebc-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f1ebc-116">Delegated (work or school account)</span></span> | <span data-ttu-id="f1ebc-117">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1ebc-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="f1ebc-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f1ebc-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1ebc-119">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1ebc-119">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="f1ebc-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f1ebc-120">Application</span></span> | <span data-ttu-id="f1ebc-121">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1ebc-121">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1ebc-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f1ebc-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/delta
GET /drives/{drive-id}/root/delta
GET /groups/{group-id}/drive/root/delta
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f1ebc-123">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f1ebc-123">Optional query parameters</span></span>
<span data-ttu-id="f1ebc-124">このメソッドは、応答をカスタマイズするための `$select`、`$expand`、および `$top` [OData クエリ パラメーター](../../../concepts/query_parameters.md)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="f1ebc-124">This method supports the `$select` and `$top` [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-body"></a><span data-ttu-id="f1ebc-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="f1ebc-125">Request body</span></span>
<span data-ttu-id="f1ebc-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f1ebc-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1ebc-127">応答</span><span class="sxs-lookup"><span data-stu-id="f1ebc-127">Response</span></span>

<span data-ttu-id="f1ebc-128">成功した場合、このメソッドは応答本文で `200 OK` 応答コードと、[DriveItem](../resources/driveitem.md) リソースのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="f1ebc-128">If successful, this method returns a `200 OK` response code and a collection of [DriveItem](../resources/driveitem.md) resources in the response body.</span></span>

<span data-ttu-id="f1ebc-129">DriveItem のコレクションのほか、応答には次のプロパティのいずれかも含まれます。</span><span class="sxs-lookup"><span data-stu-id="f1ebc-129">In addition to the collection of DriveItems, the response will also include one of the following properties:</span></span>

| <span data-ttu-id="f1ebc-130">名前</span><span class="sxs-lookup"><span data-stu-id="f1ebc-130">Name</span></span>                 | <span data-ttu-id="f1ebc-131">値</span><span class="sxs-lookup"><span data-stu-id="f1ebc-131">Value</span></span>  | <span data-ttu-id="f1ebc-132">説明</span><span class="sxs-lookup"><span data-stu-id="f1ebc-132">Description</span></span>                                                                                                                                      |
|:---------------------|:-------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="f1ebc-133">**@odata.nextLink**</span><span class="sxs-lookup"><span data-stu-id="f1ebc-133">**@odata.nextLink**</span></span>  | <span data-ttu-id="f1ebc-134">url</span><span class="sxs-lookup"><span data-stu-id="f1ebc-134">url</span></span>    | <span data-ttu-id="f1ebc-135">現在のセットに追加の変更がある場合に、次の使用可能な変更ページを取得するための URL です。</span><span class="sxs-lookup"><span data-stu-id="f1ebc-135">A URL to retrieve the next available page of changes, if there are additional changes in the current set.</span></span>                                        |
| <span data-ttu-id="f1ebc-136">**@odata.deltaLink**</span><span class="sxs-lookup"><span data-stu-id="f1ebc-136">**@odata.deltaLink**</span></span> | <span data-ttu-id="f1ebc-137">url</span><span class="sxs-lookup"><span data-stu-id="f1ebc-137">url</span></span>    | <span data-ttu-id="f1ebc-p105">現在のすべての変更が返された後に、**@odata.nextLink** の代わりに返される URL です。今後の次の一連の変更を読み取るために使用されます。</span><span class="sxs-lookup"><span data-stu-id="f1ebc-p105">A URL returned instead of **@odata.nextLink** after all current changes have been returned. Used to read the next set of changes in the future.</span></span>  |

## <a name="example-initial-request"></a><span data-ttu-id="f1ebc-140">例 (最初の要求)</span><span class="sxs-lookup"><span data-stu-id="f1ebc-140">Example (Initial Request)</span></span>
<span data-ttu-id="f1ebc-141">ここでは、ローカルの状態を確立するために、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="f1ebc-141">Here is an example of how to call this API to establish your local state.</span></span>

##### <a name="request"></a><span data-ttu-id="f1ebc-142">要求</span><span class="sxs-lookup"><span data-stu-id="f1ebc-142">Request</span></span>
<span data-ttu-id="f1ebc-143">以下は最初の要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f1ebc-143">Here is an example of the initial request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_item_delta"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/delta
```

##### <a name="response"></a><span data-ttu-id="f1ebc-144">応答</span><span class="sxs-lookup"><span data-stu-id="f1ebc-144">Response</span></span>
<span data-ttu-id="f1ebc-145">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="f1ebc-145">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "0123456789abc",
            "name": "folder2",
            "folder": { }
        },
        {
            "id": "123010204abac",
            "name": "file.txt",
            "file": { }
        },
        {
            "id": "2353010204ddgg",
            "name": "file5.txt",
            "deleted": { }
        }
    ],
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/drive/delta(token=1230919asd190410jlka)"
}
```

<span data-ttu-id="f1ebc-p106">この応答には変更の最初のページが含まれており、**@odata.nextLink** プロパティは、現在のアイテムのセットで使用可能なアイテムがさらにあることを示しています。アプリは、アイテムのすべてのページが取得されるまで、**@odata.nextLink** の URL の値を要求し続ける必要があります。</span><span class="sxs-lookup"><span data-stu-id="f1ebc-p106">This response includes the first page of changes, and the **@odata.nextLink** property indicates that there are more items available in the current set of items. Your app should continue to request the URL value of **@odata.nextLink** until all pages of items have been retrieved.</span></span>

## <a name="example-last-page-in-a-set"></a><span data-ttu-id="f1ebc-148">例 (セットの最後のページ)</span><span class="sxs-lookup"><span data-stu-id="f1ebc-148">Example (Last page in a set)</span></span>
<span data-ttu-id="f1ebc-149">以下に、ローカルの状態を更新するためにこの API を呼び出す方法の例を示します。</span><span class="sxs-lookup"><span data-stu-id="f1ebc-149">Here is an example of how to call this API to update your local state.</span></span>

##### <a name="request"></a><span data-ttu-id="f1ebc-150">要求</span><span class="sxs-lookup"><span data-stu-id="f1ebc-150">Request</span></span>
<span data-ttu-id="f1ebc-151">以下は最初の要求後の要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f1ebc-151">Here is an example request after the initial request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_item_delta"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/delta(token='1230919asd190410jlka')
```

##### <a name="response"></a><span data-ttu-id="f1ebc-152">応答</span><span class="sxs-lookup"><span data-stu-id="f1ebc-152">Response</span></span>
<span data-ttu-id="f1ebc-153">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="f1ebc-153">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "0123456789abc",
            "name": "folder2",
            "folder": { },
            "deleted": { }
        },
        {
            "id": "123010204abac",
            "name": "file.txt",
            "file": { }
        }
    ],
    "@odata.deltaLink": "https://graph.microsoft.com/v1.0/me/drive/root/delta?(token='1230919asd190410jlka')"
}
```

<span data-ttu-id="f1ebc-154">この応答は、`folder2` という名前のアイテムが削除され、アイテム `file.txt` は最初の要求とローカルの状態を更新する今回の要求の間で追加または変更されたことを示しています。</span><span class="sxs-lookup"><span data-stu-id="f1ebc-154">This response indicates that the item named `folder2` was deleted and the item `file.txt` was either added or modified between the initial request and this request to update the local state.</span></span>

<span data-ttu-id="f1ebc-155">アイテムの最後のページには **@odata.deltaLink** プロパティが含まれます。このプロパティは現在のアイテム セット以降の変更を後で取得するために使用される URL を提供します。</span><span class="sxs-lookup"><span data-stu-id="f1ebc-155">The final page of items will include the **@odata.deltaLink** property, which provides the URL that can be used later to retrieve changes since the current set of items.</span></span>

## <a name="remarks"></a><span data-ttu-id="f1ebc-156">注釈</span><span class="sxs-lookup"><span data-stu-id="f1ebc-156">Remarks</span></span>

* <span data-ttu-id="f1ebc-p107">差分フィードは各変更を示すのではなく、各アイテムの最新の状態を示すものです。アイテムの名前が 2 回変更された場合、最新の名前で 1 回だけ表示されます。</span><span class="sxs-lookup"><span data-stu-id="f1ebc-p107">The delta feed shows the latest state for each item, not each change. If an item were renamed twice, it would only show up once, with its latest name.</span></span>
* <span data-ttu-id="f1ebc-p108">差分フィードには、さまざまな理由から同じアイテムが複数回表示される場合があります。その場合は最後に出現したものを使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f1ebc-p108">The same item may appear more than once in a delta feed, for various reasons. You should use the last occurrence you see.</span></span>
* <span data-ttu-id="f1ebc-p109">アイテムの `parentReference` プロパティには**パス**の値は含まれません。これは、フォルダー名を変更しても**デルタ**からそのフォルダーの子孫が返されることはないためです。**差分を使用する場合、アイテムは必ず ID で追跡する必要があります**。</span><span class="sxs-lookup"><span data-stu-id="f1ebc-p109">The `parentReference` property on items will not include a value for **path**. This occurs because renaming a folder does not result in any descendants of the folder being returned from **delta**. **When using delta you should always track items by id**.</span></span>

<span data-ttu-id="f1ebc-p110">指定したトークンの変更リストを、サービスが提供できない場合があります (長時間にわたって切断された後に、クライアントが古いトークンを再利用する場合や、サーバーの状態が変更され、新しいトークンが必要な場合など)。このような場合、サービスは次のエラー コードのいずれかを含むエラー応答で `HTTP 410 Gone` エラーを返し、また、新しい差分の列挙を最初から開始する新しい nextLink を含む `Location` ヘッダーを返します。完全な列挙処理が終了したら、返されたアイテムとローカルの状態を比較して、次の指示に従います。</span><span class="sxs-lookup"><span data-stu-id="f1ebc-p110">There may be cases when the service can't provide a list of changes for a given token (for example, if a client tries to reuse an old token after being disconnected for a long time, or if server state has changed and a new token is required). In these cases the service will return an `HTTP 410 Gone` error with an error response containing one of the error codes below, and a `Location` header containing a new nextLink that starts a fresh delta enumeration from scratch. After finishing the full enumeration, compare the returned items with your local state and follow these instructions.</span></span>

| <span data-ttu-id="f1ebc-167">エラーの種類</span><span class="sxs-lookup"><span data-stu-id="f1ebc-167">Error Type</span></span>                       | <span data-ttu-id="f1ebc-168">手順</span><span class="sxs-lookup"><span data-stu-id="f1ebc-168">Instructions</span></span>                                                                                                                                                                                                                    |
|:---------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `resyncChangesApplyDifferences`  | <span data-ttu-id="f1ebc-p111">最後に同期したときに、サービスがローカルの変更に対して最新の状態であったことが確実な場合、すべてのローカル アイテムをサーバーのバージョンと置き換えます (削除を含む)。サーバーが把握していないすべてのローカル変更をアップロードします。</span><span class="sxs-lookup"><span data-stu-id="f1ebc-p111">Replace any local items with the server's version (including deletes) if you're sure that the service was up to date with your local changes when you last sync'd. Upload any local changes that the server doesn't know about.</span></span> |
| `resyncChangesUploadDifferences` | <span data-ttu-id="f1ebc-171">サービスが返さないすべてのローカル アイテムをアップロードして、サーバーのバージョンと異なるすべてのファイルをアップロードします (どちらがより最新の状態であるかわからない場合は、両方のコピーを保持する)。</span><span class="sxs-lookup"><span data-stu-id="f1ebc-171">Upload any local items that the service did not return, and upload any files that differ from the server's version (keeping both copies if you're not sure which one is more up-to-date).</span></span>                                       |

<span data-ttu-id="f1ebc-p112">OneDrive for Business および SharePoint では、`delta` は `root` フォルダーでのみサポートされ、他のフォルダーではサポートされません。また、DriveItem の次のプロパティも返しません。</span><span class="sxs-lookup"><span data-stu-id="f1ebc-p112">In OneDrive for Business and SharePoint, `delta` is only supported on the `root` folder, not on other folders. It also will not return the following DriveItem properties:</span></span>

* <span data-ttu-id="f1ebc-174">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="f1ebc-174">**createdBy**</span></span>
* <span data-ttu-id="f1ebc-175">**cTag**</span><span class="sxs-lookup"><span data-stu-id="f1ebc-175">**cTag**</span></span>
* <span data-ttu-id="f1ebc-176">**eTag**</span><span class="sxs-lookup"><span data-stu-id="f1ebc-176">**eTag**</span></span>
* <span data-ttu-id="f1ebc-177">**fileSystemInfo**</span><span class="sxs-lookup"><span data-stu-id="f1ebc-177">**fileSystemInfo**</span></span>
* <span data-ttu-id="f1ebc-178">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="f1ebc-178">**lastModifiedBy**</span></span>
* <span data-ttu-id="f1ebc-179">**parentReference**</span><span class="sxs-lookup"><span data-stu-id="f1ebc-179">**parentReference**</span></span>
* <span data-ttu-id="f1ebc-180">**size**</span><span class="sxs-lookup"><span data-stu-id="f1ebc-180">**size**</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "Get item delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
