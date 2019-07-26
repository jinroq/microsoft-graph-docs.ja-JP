---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: ドライブのコンテンツを同期する
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: fae431014e03b70e9d81d68977a4fa386b5447c7
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35891039"
---
# <a name="track-changes-for-a-drive"></a><span data-ttu-id="cfd71-102">ドライブの変更履歴を記録する</span><span class="sxs-lookup"><span data-stu-id="cfd71-102">Track changes for a Drive</span></span>

<span data-ttu-id="cfd71-103">このメソッドでは、アプリがドライブおよびその子への変更履歴を時間の経過とともに記録できます。</span><span class="sxs-lookup"><span data-stu-id="cfd71-103">This method allows your app to track changes to a drive and its children over time.</span></span>

<span data-ttu-id="cfd71-p101">アプリはまず、パラメーターを指定せずに `delta` を呼び出します。サービスはドライブの階層の列挙を開始し、次に説明するように、アイテムのページと `@odata.nextLink` または `@odata.deltaLink` のいずれかを返します。`@odata.nextLink` が返されなくなるまで、または変更の空のセットが応答で返されるまで、アプリは `@odata.nextLink` を使って呼び出しを続けます。</span><span class="sxs-lookup"><span data-stu-id="cfd71-p101">Your app begins by calling `delta` without any parameters. The service starts enumerating the drive's hierarchy, returning pages of items and either an `@odata.nextLink` or an `@odata.deltaLink`, as described below. Your app should continue calling with the `@odata.nextLink` until you no longer see an `@odata.nextLink` returned, or you see a response with an empty set of changes.</span></span>

<span data-ttu-id="cfd71-p102">すべての変更を受信したら、それをローカルの状態に適用できます。今後の変更を確認するには、前回の応答の `@odata.deltaLink` を使ってもう一度 `delta` を呼び出します。</span><span class="sxs-lookup"><span data-stu-id="cfd71-p102">After you have finished receiving all the changes, you may apply them to your local state. To check for changes in the future, call `delta` again with the `@odata.deltaLink` from the previous response.</span></span>

<span data-ttu-id="cfd71-p103">削除されたアイテムは [`deleted` ファセット](../resources/deleted.md)付きで返されます。このプロパティ セットを持つアイテムは、ローカル状態から削除する必要があります。</span><span class="sxs-lookup"><span data-stu-id="cfd71-p103">Deleted items are returned with the [`deleted` facet](../resources/deleted.md). Items with this property set should be removed from your local state.</span></span> 

<span data-ttu-id="cfd71-111">**注:** すべての変更を同期した後にフォルダーが空の場合にのみ、ローカルでそのフォルダーを削除する必要があります。</span><span class="sxs-lookup"><span data-stu-id="cfd71-111">**Note:** you should only delete a folder locally if it is empty after syncing all the changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="cfd71-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cfd71-112">Permissions</span></span>

<span data-ttu-id="cfd71-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cfd71-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cfd71-115">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cfd71-115">Permission type</span></span>      | <span data-ttu-id="cfd71-116">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cfd71-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cfd71-117">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cfd71-117">Delegated (work or school account)</span></span> | <span data-ttu-id="cfd71-118">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfd71-118">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="cfd71-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cfd71-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cfd71-120">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfd71-120">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="cfd71-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cfd71-121">Application</span></span> | <span data-ttu-id="cfd71-122">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfd71-122">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cfd71-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cfd71-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/root/delta
GET /groups/{groupId}/drive/root/delta
GET /me/drive/root/delta
GET /sites/{siteId}/drive/root/delta
GET /users/{userId}/drive/root/delta
```

## <a name="function-parameters"></a><span data-ttu-id="cfd71-124">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="cfd71-124">Function parameters</span></span>

| <span data-ttu-id="cfd71-125">パラメーター</span><span class="sxs-lookup"><span data-stu-id="cfd71-125">Parameter</span></span>   | <span data-ttu-id="cfd71-126">型</span><span class="sxs-lookup"><span data-stu-id="cfd71-126">Type</span></span>  | <span data-ttu-id="cfd71-127">説明</span><span class="sxs-lookup"><span data-stu-id="cfd71-127">Description</span></span>                                                                                                                          |
|:-------|:-------|:-------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="cfd71-128">token</span><span class="sxs-lookup"><span data-stu-id="cfd71-128">token</span></span>  | <span data-ttu-id="cfd71-129">string</span><span class="sxs-lookup"><span data-stu-id="cfd71-129">string</span></span> | <span data-ttu-id="cfd71-130">省略可能。</span><span class="sxs-lookup"><span data-stu-id="cfd71-130">Optional.</span></span> <span data-ttu-id="cfd71-131">指定しない場合、階層の現在の状態を列挙します。</span><span class="sxs-lookup"><span data-stu-id="cfd71-131">If unspecified, enumerates the hierarchy's current state.</span></span> <span data-ttu-id="cfd71-132">`latest` の場合、最後のデルタ トークンを使用して、空の応答本文を返します。</span><span class="sxs-lookup"><span data-stu-id="cfd71-132">If `latest`, returns empty response with latest delta token.</span></span> <span data-ttu-id="cfd71-133">一つ前のデルタ トークンの場合は、そのトークン以降の新しい状態を返します。</span><span class="sxs-lookup"><span data-stu-id="cfd71-133">If a previous delta token, returns new state since that token.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="cfd71-134">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="cfd71-134">Optional query parameters</span></span>

<span data-ttu-id="cfd71-135">このメソッドは、応答をカスタマイズするための `$select`、`$expand`、`$top` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="cfd71-135">This method supports the `$select`, `$expand`, and `$top` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="cfd71-136">応答</span><span class="sxs-lookup"><span data-stu-id="cfd71-136">Response</span></span>

<span data-ttu-id="cfd71-137">成功した場合、このメソッドは応答本文で `200 OK` 応答コードと、[DriveItem](../resources/driveitem.md) リソースのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="cfd71-137">If successful, this method returns a `200 OK` response code and a collection of [DriveItem](../resources/driveitem.md) resources in the response body.</span></span>

<span data-ttu-id="cfd71-138">DriveItem のコレクションのほか、応答には次のプロパティのいずれかも含まれます。</span><span class="sxs-lookup"><span data-stu-id="cfd71-138">In addition to the collection of DriveItems, the response will also include one of the following properties:</span></span>

| <span data-ttu-id="cfd71-139">名前</span><span class="sxs-lookup"><span data-stu-id="cfd71-139">Name</span></span>                 | <span data-ttu-id="cfd71-140">値</span><span class="sxs-lookup"><span data-stu-id="cfd71-140">Value</span></span>  | <span data-ttu-id="cfd71-141">説明</span><span class="sxs-lookup"><span data-stu-id="cfd71-141">Description</span></span>                                                                                                                                      |
|:---------------------|:-------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="cfd71-142">**@odata.nextLink**</span><span class="sxs-lookup"><span data-stu-id="cfd71-142">**@odata.nextLink**</span></span>  | <span data-ttu-id="cfd71-143">url</span><span class="sxs-lookup"><span data-stu-id="cfd71-143">url</span></span>    | <span data-ttu-id="cfd71-144">現在のセットに追加の変更がある場合に、次の使用可能な変更ページを取得するための URL です。</span><span class="sxs-lookup"><span data-stu-id="cfd71-144">A URL to retrieve the next available page of changes, if there are additional changes in the current set.</span></span>                                        |
| <span data-ttu-id="cfd71-145">**@odata.deltaLink**</span><span class="sxs-lookup"><span data-stu-id="cfd71-145">**@odata.deltaLink**</span></span> | <span data-ttu-id="cfd71-146">url</span><span class="sxs-lookup"><span data-stu-id="cfd71-146">url</span></span>    | <span data-ttu-id="cfd71-p106">現在のすべての変更が返された後に、**@odata.nextLink** の代わりに返される URL です。今後の次の一連の変更を読み取るために使用されます。</span><span class="sxs-lookup"><span data-stu-id="cfd71-p106">A URL returned instead of **@odata.nextLink** after all current changes have been returned. Used to read the next set of changes in the future.</span></span>  |

## <a name="example-initial-request"></a><span data-ttu-id="cfd71-149">例 (最初の要求)</span><span class="sxs-lookup"><span data-stu-id="cfd71-149">Example (Initial Request)</span></span>

<span data-ttu-id="cfd71-150">ここでは、ローカルの状態を確立するために、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="cfd71-150">Here is an example of how to call this API to establish your local state.</span></span>

### <a name="request"></a><span data-ttu-id="cfd71-151">要求</span><span class="sxs-lookup"><span data-stu-id="cfd71-151">Request</span></span>

<span data-ttu-id="cfd71-152">以下は最初の要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cfd71-152">Here is an example of the initial request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="cfd71-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="cfd71-153">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get_item_delta_first", "tags": "service.graph" } -->

```http
GET https://graph.microsoft.com/v1.0/me/drive/root/delta
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cfd71-154">C#</span><span class="sxs-lookup"><span data-stu-id="cfd71-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-item-delta-first-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cfd71-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="cfd71-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-item-delta-first-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cfd71-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cfd71-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-item-delta-first-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="cfd71-157">Java</span><span class="sxs-lookup"><span data-stu-id="cfd71-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-item-delta-first-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cfd71-158">応答</span><span class="sxs-lookup"><span data-stu-id="cfd71-158">Response</span></span>

<span data-ttu-id="cfd71-159">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="cfd71-159">Here is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItem)", "truncated": true, "scope": "file.read" } -->

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

<span data-ttu-id="cfd71-p107">この応答には変更の最初のページが含まれており、**@odata.nextLink** プロパティは、現在のアイテムのセットで使用可能なアイテムがさらにあることを示しています。アプリは、アイテムのすべてのページが取得されるまで、**@odata.nextLink** の URL の値を要求し続ける必要があります。</span><span class="sxs-lookup"><span data-stu-id="cfd71-p107">This response includes the first page of changes, and the **@odata.nextLink** property indicates that there are more items available in the current set of items. Your app should continue to request the URL value of **@odata.nextLink** until all pages of items have been retrieved.</span></span>

## <a name="example-last-page-in-a-set"></a><span data-ttu-id="cfd71-162">例 (セットの最後のページ)</span><span class="sxs-lookup"><span data-stu-id="cfd71-162">Example (Last page in a set)</span></span>

<span data-ttu-id="cfd71-163">以下に、ローカルの状態を更新するためにこの API を呼び出す方法の例を示します。</span><span class="sxs-lookup"><span data-stu-id="cfd71-163">Here is an example of how to call this API to update your local state.</span></span>

### <a name="request"></a><span data-ttu-id="cfd71-164">要求</span><span class="sxs-lookup"><span data-stu-id="cfd71-164">Request</span></span>

<span data-ttu-id="cfd71-165">以下は最初の要求後の要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cfd71-165">Here is an example request after the initial request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="cfd71-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="cfd71-166">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-item-delta-last", "tags": "service.graph" }-->

```http
GET https://graph.microsoft.com/v1.0/me/drive/root/delta(token='1230919asd190410jlka')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cfd71-167">C#</span><span class="sxs-lookup"><span data-stu-id="cfd71-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-item-delta-last-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cfd71-168">Javascript</span><span class="sxs-lookup"><span data-stu-id="cfd71-168">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-item-delta-last-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cfd71-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cfd71-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-item-delta-last-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="cfd71-170">Java</span><span class="sxs-lookup"><span data-stu-id="cfd71-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-item-delta-last-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cfd71-171">応答</span><span class="sxs-lookup"><span data-stu-id="cfd71-171">Response</span></span>

<span data-ttu-id="cfd71-172">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="cfd71-172">Here is an example of the response.</span></span>

<!-- { "blockType": "response", "truncated": true, "@odata.type": "Collection(microsoft.graph.driveItem)", "scope": "file.read" } -->

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

<span data-ttu-id="cfd71-173">この応答は、`folder2` という名前のアイテムが削除され、アイテム `file.txt` は最初の要求とローカルの状態を更新する今回の要求の間で追加または変更されたことを示しています。</span><span class="sxs-lookup"><span data-stu-id="cfd71-173">This response indicates that the item named `folder2` was deleted and the item `file.txt` was either added or modified between the initial request and this request to update the local state.</span></span>

<span data-ttu-id="cfd71-174">アイテムの最後のページには **@odata.deltaLink** プロパティが含まれます。このプロパティは現在のアイテム セット以降の変更を後で取得するために使用される URL を提供します。</span><span class="sxs-lookup"><span data-stu-id="cfd71-174">The final page of items will include the **@odata.deltaLink** property, which provides the URL that can be used later to retrieve changes since the current set of items.</span></span>

<span data-ttu-id="cfd71-p108">指定したトークンの変更リストを、サービスが提供できない場合があります (長時間にわたって切断された後に、クライアントが古いトークンを再利用する場合や、サーバーの状態が変更され、新しいトークンが必要な場合など)。このような場合、サービスは次のエラー コードのいずれかを含むエラー応答で `HTTP 410 Gone` エラーを返し、また、新しい差分の列挙を最初から開始する新しい nextLink を含む `Location` ヘッダーを返します。完全な列挙処理が終了したら、返されたアイテムとローカルの状態を比較して、次の指示に従います。</span><span class="sxs-lookup"><span data-stu-id="cfd71-p108">There may be cases when the service can't provide a list of changes for a given token (for example, if a client tries to reuse an old token after being disconnected for a long time, or if server state has changed and a new token is required). In these cases the service will return an `HTTP 410 Gone` error with an error response containing one of the error codes below, and a `Location` header containing a new nextLink that starts a fresh delta enumeration from scratch. After finishing the full enumeration, compare the returned items with your local state and follow these instructions.</span></span>

| <span data-ttu-id="cfd71-178">エラーの種類</span><span class="sxs-lookup"><span data-stu-id="cfd71-178">Error Type</span></span>                       | <span data-ttu-id="cfd71-179">手順</span><span class="sxs-lookup"><span data-stu-id="cfd71-179">Instructions</span></span>                                                                                                                                                                                                                    |
|:---------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `resyncChangesApplyDifferences`  | <span data-ttu-id="cfd71-p109">最後に同期したときに、サービスがローカルの変更に対して最新の状態であったことが確実な場合、すべてのローカル アイテムをサーバーのバージョンと置き換えます (削除を含む)。サーバーが把握していないすべてのローカル変更をアップロードします。</span><span class="sxs-lookup"><span data-stu-id="cfd71-p109">Replace any local items with the server's version (including deletes) if you're sure that the service was up to date with your local changes when you last sync'd. Upload any local changes that the server doesn't know about.</span></span> |
| `resyncChangesUploadDifferences` | <span data-ttu-id="cfd71-182">サービスが返さないすべてのローカル アイテムをアップロードして、サーバーのバージョンと異なるすべてのファイルをアップロードします (どちらがより最新の状態であるかわからない場合は、両方のコピーを保持する)。</span><span class="sxs-lookup"><span data-stu-id="cfd71-182">Upload any local items that the service did not return, and upload any files that differ from the server's version (keeping both copies if you're not sure which one is more up-to-date).</span></span>                                       |

## <a name="retrieving-the-current-deltalink"></a><span data-ttu-id="cfd71-183">現在の deltaLink を取得する</span><span class="sxs-lookup"><span data-stu-id="cfd71-183">Retrieving the current deltaLink</span></span>

<span data-ttu-id="cfd71-184">シナリオによっては、ドライブにすでにあるすべてのアイテムを最初に列挙する代わりに、現在の deltaLink 値を要求すると便利な場合があります。</span><span class="sxs-lookup"><span data-stu-id="cfd71-184">In some scenarios, it may be useful to request the current deltaLink value without first enumerating all of the items in the drive already.</span></span>

<span data-ttu-id="cfd71-185">これは、アプリで変更についてのみ知る必要があり、既存のアイテムは知る必要がない場合に役立ちます。</span><span class="sxs-lookup"><span data-stu-id="cfd71-185">This can be useful if your app only wants to know about changes, and doesn't need to know about existing items.</span></span>
<span data-ttu-id="cfd71-186">最新の deltaLink を取得するには、クエリ文字列パラメーター `?token=latest` を指定して `delta` を呼び出します。</span><span class="sxs-lookup"><span data-stu-id="cfd71-186">To retrieve the latest deltaLink, call `delta` with a query string parameter `?token=latest`.</span></span>

<span data-ttu-id="cfd71-187">**注: フォルダーまたはドライブ内のアイテムの完全なローカル表現を維持しようとしている場合は、最初の列挙に `delta` を使用する必要があります。その他の方法 (フォルダーの `children` コレクションをページングするなど) は、列挙時に書き込みが発生した場合に、すべてのアイテムを 1 つ残らず返す保証がありません。`delta` の使用は、必要とするデータのすべてを読み取ったことを保証する唯一の方法です。**</span><span class="sxs-lookup"><span data-stu-id="cfd71-187">**Note: If you are trying to maintain a full local representation of the items in a folder or a drive, you must use `delta` for the initial enumeration. Other approaches, such as paging through the `children` collection of a folder, are not guaranteed to return every single item if any writes take place during the enumeration. Using `delta` is the only way to guarantee that you've read all of the data you need to.**</span></span>

### <a name="request"></a><span data-ttu-id="cfd71-188">要求</span><span class="sxs-lookup"><span data-stu-id="cfd71-188">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="cfd71-189">HTTP</span><span class="sxs-lookup"><span data-stu-id="cfd71-189">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-delta-latest", "scopes": "files.read", "tags": "service.graph", "target": "action" } -->

```http
GET /me/drive/root/delta?token=latest
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cfd71-190">C#</span><span class="sxs-lookup"><span data-stu-id="cfd71-190">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-delta-latest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cfd71-191">Javascript</span><span class="sxs-lookup"><span data-stu-id="cfd71-191">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-delta-latest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cfd71-192">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cfd71-192">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-delta-latest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="cfd71-193">Java</span><span class="sxs-lookup"><span data-stu-id="cfd71-193">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-delta-latest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cfd71-194">応答</span><span class="sxs-lookup"><span data-stu-id="cfd71-194">Response</span></span>

<!-- { "blockType": "response", "isEmpty": true, "@odata.type": "Collection(microsoft.graph.driveItem)" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [ ],
    "@odata.deltaLink": "https://graph.microsoft.com/v1.0/me/drive/root/delta?token=1230919asd190410jlka"
}
```

## <a name="remarks"></a><span data-ttu-id="cfd71-195">備考</span><span class="sxs-lookup"><span data-stu-id="cfd71-195">Remarks</span></span>

* <span data-ttu-id="cfd71-p111">差分フィードは各変更を示すのではなく、各アイテムの最新の状態を示すものです。アイテムの名前が 2 回変更された場合、最新の名前で 1 回だけ表示されます。</span><span class="sxs-lookup"><span data-stu-id="cfd71-p111">The delta feed shows the latest state for each item, not each change. If an item were renamed twice, it would only show up once, with its latest name.</span></span>
* <span data-ttu-id="cfd71-p112">差分フィードには、さまざまな理由から同じアイテムが複数回表示される場合があります。その場合は最後に出現したものを使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="cfd71-p112">The same item may appear more than once in a delta feed, for various reasons. You should use the last occurrence you see.</span></span>
* <span data-ttu-id="cfd71-p113">アイテムの `parentReference` プロパティには**パス**の値は含まれません。これは、フォルダー名を変更しても**デルタ**からそのフォルダーの子孫が返されることはないためです。**差分を使用する場合、アイテムは必ず ID で追跡する必要があります**。</span><span class="sxs-lookup"><span data-stu-id="cfd71-p113">The `parentReference` property on items will not include a value for **path**. This occurs because renaming a folder does not result in any descendants of the folder being returned from **delta**. **When using delta you should always track items by id**.</span></span>
* <span data-ttu-id="cfd71-203">OneDrive for Business および SharePoint では、`delta` は `root` フォルダーでのみサポートされ、ドライブ内の他のフォルダーではサポートされません。</span><span class="sxs-lookup"><span data-stu-id="cfd71-203">In OneDrive for Business and SharePoint, `delta` is only supported on the `root` folder, not on other folders within a drive.</span></span>

* <span data-ttu-id="cfd71-204">デルタ クエリは、次の表に示す通り、操作とサービスの種類によって、一部の DriveItem プロパティを返しません。</span><span class="sxs-lookup"><span data-stu-id="cfd71-204">Delta query will not return some DriveItem properties, depending on the operation and service type, as shown in the following tables.</span></span>

    <span data-ttu-id="cfd71-205">**OneDrive for Business**</span><span class="sxs-lookup"><span data-stu-id="cfd71-205">**OneDrive for Business**</span></span>
    
    | <span data-ttu-id="cfd71-206">操作の種類</span><span class="sxs-lookup"><span data-stu-id="cfd71-206">Operation type</span></span> | <span data-ttu-id="cfd71-207">デルタ クエリに省略されるプロパティ</span><span class="sxs-lookup"><span data-stu-id="cfd71-207">Properties omitted by delta query</span></span> |
    |---------|----------|
    | <span data-ttu-id="cfd71-208">作成/変更</span><span class="sxs-lookup"><span data-stu-id="cfd71-208">Create/Modify</span></span> | <span data-ttu-id="cfd71-209">`ctag`, `lastModifiedBy`</span><span class="sxs-lookup"><span data-stu-id="cfd71-209"></span></span> |
    | <span data-ttu-id="cfd71-210">削除</span><span class="sxs-lookup"><span data-stu-id="cfd71-210">Delete</span></span> | <span data-ttu-id="cfd71-211">`ctag`, `lastModifiedBy`, `name`</span><span class="sxs-lookup"><span data-stu-id="cfd71-211"></span></span> |


    <span data-ttu-id="cfd71-212">**OneDrive (コンシューマー向け)**</span><span class="sxs-lookup"><span data-stu-id="cfd71-212">**OneDrive (consumer)**</span></span>
    
    | <span data-ttu-id="cfd71-213">操作の種類</span><span class="sxs-lookup"><span data-stu-id="cfd71-213">Operation type</span></span> | <span data-ttu-id="cfd71-214">デルタ クエリに省略されるプロパティ</span><span class="sxs-lookup"><span data-stu-id="cfd71-214">Properties omitted by delta query</span></span> |
    |---------|----------|
    | <span data-ttu-id="cfd71-215">作成/変更</span><span class="sxs-lookup"><span data-stu-id="cfd71-215">Create/Modify</span></span> | <span data-ttu-id="cfd71-216">該当なし</span><span class="sxs-lookup"><span data-stu-id="cfd71-216">n/a</span></span> |
    | <span data-ttu-id="cfd71-217">削除</span><span class="sxs-lookup"><span data-stu-id="cfd71-217">Delete</span></span> | <span data-ttu-id="cfd71-218">`ctag`, `size`</span><span class="sxs-lookup"><span data-stu-id="cfd71-218"></span></span> |

## <a name="error-responses"></a><span data-ttu-id="cfd71-219">エラー応答</span><span class="sxs-lookup"><span data-stu-id="cfd71-219">Error responses</span></span>

<span data-ttu-id="cfd71-220">前述した再同期エラーの詳細に加えて、エラーがどのように返されるかについては、「[エラー応答][error-response]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cfd71-220">In addition to the resync errors detailed above, see [Error Responses][error-response] for details about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Sync changes from the service to your client state.",
  "keywords": "sync,delta,changes,$delta",
  "section": "documentation",
  "tocPath": "Items/Sync changes",
  "suppressions": [
  ]
} -->
