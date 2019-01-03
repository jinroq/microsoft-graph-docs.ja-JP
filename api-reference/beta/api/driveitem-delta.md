---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: ドライブのコンテンツを同期する
ms.openlocfilehash: 4ccaec230d5801f563f81e6a30584db9f7ed5714
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067957"
---
# <a name="track-changes-for-a-drive"></a><span data-ttu-id="e4a56-102">ドライブの変更履歴を記録する</span><span class="sxs-lookup"><span data-stu-id="e4a56-102">Track changes for a Drive</span></span>

> <span data-ttu-id="e4a56-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e4a56-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e4a56-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e4a56-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e4a56-105">このメソッドでは、アプリがドライブおよびその子への変更履歴を時間の経過とともに記録できます。</span><span class="sxs-lookup"><span data-stu-id="e4a56-105">This method allows your app to track changes to a drive and its children over time.</span></span>

<span data-ttu-id="e4a56-p102">アプリはまず、パラメーターを指定せずに `delta` を呼び出します。サービスはドライブの階層の列挙を開始し、次に説明するように、アイテムのページと `@odata.nextLink` または `@odata.deltaLink` のいずれかを返します。`@odata.nextLink` が返されなくなるまで、または変更の空のセットが応答で返されるまで、アプリは `@odata.nextLink` を使って呼び出しを続けます。</span><span class="sxs-lookup"><span data-stu-id="e4a56-p102">Your app begins by calling `delta` without any parameters. The service starts enumerating the drive's hierarchy, returning pages of items and either an `@odata.nextLink` or an `@odata.deltaLink`, as described below. Your app should continue calling with the `@odata.nextLink` until you no longer see an `@odata.nextLink` returned, or you see a response with an empty set of changes.</span></span>

<span data-ttu-id="e4a56-p103">すべての変更を受信したら、それをローカルの状態に適用できます。今後の変更を確認するには、前回の応答の `@odata.deltaLink` を使ってもう一度 `delta` を呼び出します。</span><span class="sxs-lookup"><span data-stu-id="e4a56-p103">After you have finished receiving all the changes, you may apply them to your local state. To check for changes in the future, call `delta` again with the `@odata.deltaLink` from the previous response.</span></span>

<span data-ttu-id="e4a56-p104">削除されたアイテムは [`deleted` ファセット](../resources/deleted.md)付きで返されます。このプロパティ セットを持つアイテムは、ローカル状態から削除する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e4a56-p104">Deleted items are returned with the [`deleted` facet](../resources/deleted.md). Items with this property set should be removed from your local state.</span></span> 

<span data-ttu-id="e4a56-113">**注:** すべての変更を同期した後にフォルダーが空の場合にのみ、ローカルでそのフォルダーを削除する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e4a56-113">**Note:** you should only delete a folder locally if it is empty after syncing all the changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="e4a56-114">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e4a56-114">Permissions</span></span>

<span data-ttu-id="e4a56-p105">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e4a56-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4a56-117">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e4a56-117">Permission type</span></span>      | <span data-ttu-id="e4a56-118">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e4a56-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e4a56-119">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e4a56-119">Delegated (work or school account)</span></span> | <span data-ttu-id="e4a56-120">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4a56-120">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="e4a56-121">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e4a56-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4a56-122">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4a56-122">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="e4a56-123">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e4a56-123">Application</span></span> | <span data-ttu-id="e4a56-124">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4a56-124">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e4a56-125">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e4a56-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/root/delta
GET /groups/{groupId}/drive/root/delta
GET /me/drive/root/delta
GET /sites/{siteId}/drive/root/delta
GET /users/{userId}/drive/root/delta
```

## <a name="function-parameters"></a><span data-ttu-id="e4a56-126">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="e4a56-126">Function parameters</span></span>

| <span data-ttu-id="e4a56-127">名前</span><span class="sxs-lookup"><span data-stu-id="e4a56-127">Name</span></span>   | <span data-ttu-id="e4a56-128">値</span><span class="sxs-lookup"><span data-stu-id="e4a56-128">Value</span></span>  | <span data-ttu-id="e4a56-129">説明</span><span class="sxs-lookup"><span data-stu-id="e4a56-129">Description</span></span>                                                                                                                          |
|:-------|:-------|:-------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="e4a56-130">token</span><span class="sxs-lookup"><span data-stu-id="e4a56-130">token</span></span>  | <span data-ttu-id="e4a56-131">文字列</span><span class="sxs-lookup"><span data-stu-id="e4a56-131">string</span></span> | <span data-ttu-id="e4a56-132">省略可能。</span><span class="sxs-lookup"><span data-stu-id="e4a56-132">Optional.</span></span> <span data-ttu-id="e4a56-133">オプションを指定しない場合は、階層の現在の状態を列挙します。</span><span class="sxs-lookup"><span data-stu-id="e4a56-133">If unspecified, enumerates the hierarchy's current state.</span></span> <span data-ttu-id="e4a56-134">場合`latest`、最新のデルタ ・ トークンを使用して応答を空にするを返します。</span><span class="sxs-lookup"><span data-stu-id="e4a56-134">If `latest`, returns empty response with latest delta token.</span></span> <span data-ttu-id="e4a56-135">場合、以前のデルタ ・ トークンは、そのトークンから新しい状態を返します。</span><span class="sxs-lookup"><span data-stu-id="e4a56-135">If a previous delta token, returns new state since that token.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="e4a56-136">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e4a56-136">Optional query parameters</span></span>

<span data-ttu-id="e4a56-137">このメソッドは、応答をカスタマイズするための `$select`、`$expand`、`$top` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e4a56-137">This method supports the `$select`, `$expand`, and `$top` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="e4a56-138">応答</span><span class="sxs-lookup"><span data-stu-id="e4a56-138">Response</span></span>

<span data-ttu-id="e4a56-139">成功した場合、このメソッドは応答本文で `200 OK` 応答コードと、[DriveItem](../resources/driveitem.md) リソースのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="e4a56-139">If successful, this method returns a `200 OK` response code and a collection of [DriveItem](../resources/driveitem.md) resources in the response body.</span></span>

<span data-ttu-id="e4a56-140">DriveItem のコレクションのほか、応答には次のプロパティのいずれかも含まれます。</span><span class="sxs-lookup"><span data-stu-id="e4a56-140">In addition to the collection of DriveItems, the response will also include one of the following properties:</span></span>

| <span data-ttu-id="e4a56-141">名前</span><span class="sxs-lookup"><span data-stu-id="e4a56-141">Name</span></span>                 | <span data-ttu-id="e4a56-142">値</span><span class="sxs-lookup"><span data-stu-id="e4a56-142">Value</span></span>  | <span data-ttu-id="e4a56-143">説明</span><span class="sxs-lookup"><span data-stu-id="e4a56-143">Description</span></span>                                                                                                                                      |
|:---------------------|:-------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="e4a56-144">**@odata.nextLink**</span><span class="sxs-lookup"><span data-stu-id="e4a56-144">**@odata.nextLink**</span></span>  | <span data-ttu-id="e4a56-145">url</span><span class="sxs-lookup"><span data-stu-id="e4a56-145">url</span></span>    | <span data-ttu-id="e4a56-146">現在のセットに追加の変更がある場合に、次の使用可能な変更ページを取得するための URL です。</span><span class="sxs-lookup"><span data-stu-id="e4a56-146">A URL to retrieve the next available page of changes, if there are additional changes in the current set.</span></span>                                        |
| <span data-ttu-id="e4a56-147">**@odata.deltaLink**</span><span class="sxs-lookup"><span data-stu-id="e4a56-147">**@odata.deltaLink**</span></span> | <span data-ttu-id="e4a56-148">url</span><span class="sxs-lookup"><span data-stu-id="e4a56-148">url</span></span>    | <span data-ttu-id="e4a56-p107">現在のすべての変更が返された後に、**@odata.nextLink** の代わりに返される URL です。今後の次の一連の変更を読み取るために使用されます。</span><span class="sxs-lookup"><span data-stu-id="e4a56-p107">A URL returned instead of **@odata.nextLink** after all current changes have been returned. Used to read the next set of changes in the future.</span></span>  |

## <a name="example-initial-request"></a><span data-ttu-id="e4a56-151">例 (最初の要求)</span><span class="sxs-lookup"><span data-stu-id="e4a56-151">Example (Initial Request)</span></span>

<span data-ttu-id="e4a56-152">ここでは、ローカルの状態を確立するために、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="e4a56-152">Here is an example of how to call this API to establish your local state.</span></span>

### <a name="request"></a><span data-ttu-id="e4a56-153">要求</span><span class="sxs-lookup"><span data-stu-id="e4a56-153">Request</span></span>

<span data-ttu-id="e4a56-154">以下は最初の要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e4a56-154">Here is an example of the initial request.</span></span>

<!-- { "blockType": "request", "name": "get_item_delta_first" } -->

```http
GET https://graph.microsoft.com/v1.0/me/drive/root/delta
```

### <a name="response"></a><span data-ttu-id="e4a56-155">応答</span><span class="sxs-lookup"><span data-stu-id="e4a56-155">Response</span></span>

<span data-ttu-id="e4a56-156">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="e4a56-156">Here is an example of the response.</span></span>

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

<span data-ttu-id="e4a56-p108">この応答には変更の最初のページが含まれており、**@odata.nextLink** プロパティは、現在のアイテムのセットで使用可能なアイテムがさらにあることを示しています。アプリは、アイテムのすべてのページが取得されるまで、**@odata.nextLink** の URL の値を要求し続ける必要があります。</span><span class="sxs-lookup"><span data-stu-id="e4a56-p108">This response includes the first page of changes, and the **@odata.nextLink** property indicates that there are more items available in the current set of items. Your app should continue to request the URL value of **@odata.nextLink** until all pages of items have been retrieved.</span></span>

## <a name="example-last-page-in-a-set"></a><span data-ttu-id="e4a56-159">例 (セットの最後のページ)</span><span class="sxs-lookup"><span data-stu-id="e4a56-159">Example (Last page in a set)</span></span>

<span data-ttu-id="e4a56-160">以下に、ローカルの状態を更新するためにこの API を呼び出す方法の例を示します。</span><span class="sxs-lookup"><span data-stu-id="e4a56-160">Here is an example of how to call this API to update your local state.</span></span>

### <a name="request"></a><span data-ttu-id="e4a56-161">要求</span><span class="sxs-lookup"><span data-stu-id="e4a56-161">Request</span></span>

<span data-ttu-id="e4a56-162">以下は最初の要求後の要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e4a56-162">Here is an example request after the initial request.</span></span>

<!-- { "blockType": "request", "name": "get_item_delta_last" }-->

```http
GET https://graph.microsoft.com/v1.0/me/drive/root/delta(token='1230919asd190410jlka')
```

### <a name="response"></a><span data-ttu-id="e4a56-163">応答</span><span class="sxs-lookup"><span data-stu-id="e4a56-163">Response</span></span>

<span data-ttu-id="e4a56-164">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="e4a56-164">Here is an example of the response.</span></span>

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

<span data-ttu-id="e4a56-165">この応答は、`folder2` という名前のアイテムが削除され、アイテム `file.txt` は最初の要求とローカルの状態を更新する今回の要求の間で追加または変更されたことを示しています。</span><span class="sxs-lookup"><span data-stu-id="e4a56-165">This response indicates that the item named `folder2` was deleted and the item `file.txt` was either added or modified between the initial request and this request to update the local state.</span></span>

<span data-ttu-id="e4a56-166">アイテムの最後のページには **@odata.deltaLink** プロパティが含まれます。このプロパティは現在のアイテム セット以降の変更を後で取得するために使用される URL を提供します。</span><span class="sxs-lookup"><span data-stu-id="e4a56-166">The final page of items will include the **@odata.deltaLink** property, which provides the URL that can be used later to retrieve changes since the current set of items.</span></span>

<span data-ttu-id="e4a56-p109">指定したトークンの変更リストを、サービスが提供できない場合があります (長時間にわたって切断された後に、クライアントが古いトークンを再利用する場合や、サーバーの状態が変更され、新しいトークンが必要な場合など)。このような場合、サービスは次のエラー コードのいずれかを含むエラー応答で `HTTP 410 Gone` エラーを返し、また、新しい差分の列挙を最初から開始する新しい nextLink を含む `Location` ヘッダーを返します。完全な列挙処理が終了したら、返されたアイテムとローカルの状態を比較して、次の指示に従います。</span><span class="sxs-lookup"><span data-stu-id="e4a56-p109">There may be cases when the service can't provide a list of changes for a given token (for example, if a client tries to reuse an old token after being disconnected for a long time, or if server state has changed and a new token is required). In these cases the service will return an `HTTP 410 Gone` error with an error response containing one of the error codes below, and a `Location` header containing a new nextLink that starts a fresh delta enumeration from scratch. After finishing the full enumeration, compare the returned items with your local state and follow these instructions.</span></span>

| <span data-ttu-id="e4a56-170">エラーの種類</span><span class="sxs-lookup"><span data-stu-id="e4a56-170">Error Type</span></span>                       | <span data-ttu-id="e4a56-171">手順</span><span class="sxs-lookup"><span data-stu-id="e4a56-171">Instructions</span></span>                                                                                                                                                                                                                    |
|:---------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `resyncChangesApplyDifferences`  | <span data-ttu-id="e4a56-p110">最後に同期したときに、サービスがローカルの変更に対して最新の状態であったことが確実な場合、すべてのローカル アイテムをサーバーのバージョンと置き換えます (削除を含む)。サーバーが把握していないすべてのローカル変更をアップロードします。</span><span class="sxs-lookup"><span data-stu-id="e4a56-p110">Replace any local items with the server's version (including deletes) if you're sure that the service was up to date with your local changes when you last sync'd. Upload any local changes that the server doesn't know about.</span></span> |
| `resyncChangesUploadDifferences` | <span data-ttu-id="e4a56-174">サービスが返さないすべてのローカル アイテムをアップロードして、サーバーのバージョンと異なるすべてのファイルをアップロードします (どちらがより最新の状態であるかわからない場合は、両方のコピーを保持する)。</span><span class="sxs-lookup"><span data-stu-id="e4a56-174">Upload any local items that the service did not return, and upload any files that differ from the server's version (keeping both copies if you're not sure which one is more up-to-date).</span></span>                                       |

## <a name="retrieving-the-current-deltalink"></a><span data-ttu-id="e4a56-175">現在の deltaLink を取得する</span><span class="sxs-lookup"><span data-stu-id="e4a56-175">Retrieving the current deltaLink</span></span>

<span data-ttu-id="e4a56-176">シナリオによっては、ドライブにすでにあるすべてのアイテムを最初に列挙する代わりに、現在の deltaLink 値を要求すると便利な場合があります。</span><span class="sxs-lookup"><span data-stu-id="e4a56-176">In some scenarios, it may be useful to request the current deltaLink value without first enumerating all of the items in the drive already.</span></span>

<span data-ttu-id="e4a56-177">これは、アプリで変更についてのみ知る必要があり、既存のアイテムは知る必要がない場合に役立ちます。</span><span class="sxs-lookup"><span data-stu-id="e4a56-177">This can be useful if your app only wants to know about changes, and doesn't need to know about existing items.</span></span>
<span data-ttu-id="e4a56-178">最新の deltaLink を取得するには、クエリ文字列パラメーター `?token=latest` を指定して `delta` を呼び出します。</span><span class="sxs-lookup"><span data-stu-id="e4a56-178">To retrieve the latest deltaLink, call `delta` with a query string parameter `?token=latest`.</span></span>

<span data-ttu-id="e4a56-179">**注: フォルダーまたはドライブ内のアイテムの完全なローカル表現を維持しようとしている場合は、最初の列挙に `delta` を使用する必要があります。その他の方法 (フォルダーの `children` コレクションをページングするなど) は、列挙時に書き込みが発生した場合に、すべてのアイテムを 1 つ残らず返す保証がありません。`delta` の使用は、必要とするデータのすべてを読み取ったことを保証する唯一の方法です。**</span><span class="sxs-lookup"><span data-stu-id="e4a56-179">**Note: If you are trying to maintain a full local representation of the items in a folder or a drive, you must use `delta` for the initial enumeration. Other approaches, such as paging through the `children` collection of a folder, are not guaranteed to return every single item if any writes take place during the enumeration. Using `delta` is the only way to guarantee that you've read all of the data you need to.**</span></span>

### <a name="request"></a><span data-ttu-id="e4a56-180">要求</span><span class="sxs-lookup"><span data-stu-id="e4a56-180">Request</span></span>

<!-- { "blockType": "request", "name": "get-delta-latest", "scope": "files.read", "target": "action" } -->

```http
GET /me/drive/root/delta?token=latest
```

### <a name="response"></a><span data-ttu-id="e4a56-181">応答</span><span class="sxs-lookup"><span data-stu-id="e4a56-181">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItem)" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [ ],
    "@odata.deltaLink": "https://graph.microsoft.com/v1.0/me/drive/root/delta?token=1230919asd190410jlka"
}
```

## <a name="remarks"></a><span data-ttu-id="e4a56-182">注釈</span><span class="sxs-lookup"><span data-stu-id="e4a56-182">Remarks</span></span>

* <span data-ttu-id="e4a56-p112">差分フィードは各変更を示すのではなく、各アイテムの最新の状態を示すものです。アイテムの名前が 2 回変更された場合、最新の名前で 1 回だけ表示されます。</span><span class="sxs-lookup"><span data-stu-id="e4a56-p112">The delta feed shows the latest state for each item, not each change. If an item were renamed twice, it would only show up once, with its latest name.</span></span>
* <span data-ttu-id="e4a56-p113">差分フィードには、さまざまな理由から同じアイテムが複数回表示される場合があります。その場合は最後に出現したものを使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e4a56-p113">The same item may appear more than once in a delta feed, for various reasons. You should use the last occurrence you see.</span></span>
* <span data-ttu-id="e4a56-p114">アイテムの `parentReference` プロパティには**パス**の値は含まれません。これは、フォルダー名を変更しても**デルタ**からそのフォルダーの子孫が返されることはないためです。**差分を使用する場合、アイテムは必ず ID で追跡する必要があります**。</span><span class="sxs-lookup"><span data-stu-id="e4a56-p114">The `parentReference` property on items will not include a value for **path**. This occurs because renaming a folder does not result in any descendants of the folder being returned from **delta**. **When using delta you should always track items by id**.</span></span>
* <span data-ttu-id="e4a56-190">OneDrive for Business および SharePoint では、`delta` は `root` フォルダーでのみサポートされ、ドライブ内の他のフォルダーではサポートされません。</span><span class="sxs-lookup"><span data-stu-id="e4a56-190">In OneDrive for Business and SharePoint, `delta` is only supported on the `root` folder, not on other folders within a drive.</span></span>

* <span data-ttu-id="e4a56-191">Delta は DriveItem の次のプロパティを返しません。</span><span class="sxs-lookup"><span data-stu-id="e4a56-191">Delta will not return the following DriveItem properties:</span></span>

* <span data-ttu-id="e4a56-192">**cTag**</span><span class="sxs-lookup"><span data-stu-id="e4a56-192">**cTag**</span></span>
* <span data-ttu-id="e4a56-193">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="e4a56-193">**lastModifiedBy**</span></span>
* <span data-ttu-id="e4a56-194">**size**</span><span class="sxs-lookup"><span data-stu-id="e4a56-194">**size**</span></span>

## <a name="error-responses"></a><span data-ttu-id="e4a56-195">エラー応答</span><span class="sxs-lookup"><span data-stu-id="e4a56-195">Error responses</span></span>

<span data-ttu-id="e4a56-196">前述した再同期エラーの詳細に加えて、エラーがどのように返されるかについては、「[エラー応答][error-response]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e4a56-196">In addition to the resync errors detailed above, see [Error Responses][error-response] for details about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Sync changes from the service to your client state.",
  "keywords": "sync,delta,changes,$delta",
  "section": "documentation",
  "tocPath": "Items/Sync changes"
} -->