---
title: 'ドライブアイテム: プレビュー'
description: このアクションを使用すると、一時的なプレビューを表示するために、短時間に埋め込まれた、アイテムの Url を取得できます。
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
author: ''
ms.openlocfilehash: dc2feef9e80a04753efb6b371bffccf514f46233
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35956997"
---
# <a name="driveitem-preview"></a><span data-ttu-id="ad505-103">ドライブアイテム: プレビュー</span><span class="sxs-lookup"><span data-stu-id="ad505-103">driveItem: preview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad505-104">このアクションを使用すると、一時的なプレビューを表示するために、短時間に埋め込まれた、アイテムの Url を取得できます。</span><span class="sxs-lookup"><span data-stu-id="ad505-104">This action allows you to obtain short-lived embeddable URLs for an item in order to render a temporary preview.</span></span>

<span data-ttu-id="ad505-105">長時間の埋め込み可能なリンクを取得する場合は、代わりに[Createlink][] API を使用します。</span><span class="sxs-lookup"><span data-stu-id="ad505-105">If you want to obtain long-lived embeddable links, use the [createLink][] API instead.</span></span>

> <span data-ttu-id="ad505-106">**注:** 現在、**プレビュー**アクションは SharePoint および OneDrive for business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="ad505-106">**Note:** The **preview** action is currently only available on SharePoint and OneDrive for Business.</span></span>

[createLink]: driveitem-createlink.md

## <a name="permissions"></a><span data-ttu-id="ad505-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ad505-108">Permissions</span></span>

<span data-ttu-id="ad505-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ad505-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ad505-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ad505-111">Permission type</span></span>                        | <span data-ttu-id="ad505-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ad505-112">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="ad505-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ad505-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="ad505-114">ファイル。読み取り、ファイルの読み取り/書き込み。すべてのファイル。</span><span class="sxs-lookup"><span data-stu-id="ad505-114">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="ad505-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ad505-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad505-116">ファイル。読み取り、ファイルの読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="ad505-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="ad505-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ad505-117">Application</span></span>                            | <span data-ttu-id="ad505-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ad505-118">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="ad505-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ad505-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/preview
POST /groups/{groupId}/drive/items/{itemId}/preview
POST /me/drive/items/{itemId}/preview
POST /sites/{siteId}/drive/items/{itemId}/preview
POST /users/{userId}/drive/items/{itemId}/preview
POST /shares/{shareId}/driveItem/preview
```

## <a name="request-body"></a><span data-ttu-id="ad505-120">要求本文</span><span class="sxs-lookup"><span data-stu-id="ad505-120">Request body</span></span>

<span data-ttu-id="ad505-121">要求の本文は、アプリケーションが要求している埋め込み可能な URL のプロパティを定義します。</span><span class="sxs-lookup"><span data-stu-id="ad505-121">The body of the request defines properties of the embeddable URL your application is requesting.</span></span>
<span data-ttu-id="ad505-122">要求は、次のプロパティを含む JSON オブジェクトである必要があります。</span><span class="sxs-lookup"><span data-stu-id="ad505-122">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="ad505-123">名前</span><span class="sxs-lookup"><span data-stu-id="ad505-123">Name</span></span>      |  <span data-ttu-id="ad505-124">型</span><span class="sxs-lookup"><span data-stu-id="ad505-124">Type</span></span>         | <span data-ttu-id="ad505-125">説明</span><span class="sxs-lookup"><span data-stu-id="ad505-125">Description</span></span>
|:------------|:--------------|:-----------------------------------------------
| <span data-ttu-id="ad505-126">ビューアー</span><span class="sxs-lookup"><span data-stu-id="ad505-126">viewer</span></span>      | <span data-ttu-id="ad505-127">string</span><span class="sxs-lookup"><span data-stu-id="ad505-127">string</span></span>        | <span data-ttu-id="ad505-128">省略可能。</span><span class="sxs-lookup"><span data-stu-id="ad505-128">Optional.</span></span> <span data-ttu-id="ad505-129">使用するプレビューアプリ。</span><span class="sxs-lookup"><span data-stu-id="ad505-129">Preview app to use.</span></span> <span data-ttu-id="ad505-130">`onedrive` または `office`。</span><span class="sxs-lookup"><span data-stu-id="ad505-130">`onedrive` or `office`.</span></span> <span data-ttu-id="ad505-131">Null の場合は、適切なビューアーが自動的に選択されます。</span><span class="sxs-lookup"><span data-stu-id="ad505-131">If null, a suitable viewer will be chosen automatically.</span></span>
| <span data-ttu-id="ad505-132">chromeless</span><span class="sxs-lookup"><span data-stu-id="ad505-132">chromeless</span></span>  | <span data-ttu-id="ad505-133">ブール値</span><span class="sxs-lookup"><span data-stu-id="ad505-133">boolean</span></span>       | <span data-ttu-id="ad505-134">省略可能。</span><span class="sxs-lookup"><span data-stu-id="ad505-134">Optional.</span></span> <span data-ttu-id="ad505-135">If `true` (既定値) の場合、埋め込まれたビューにコントロールは含まれません。</span><span class="sxs-lookup"><span data-stu-id="ad505-135">If `true` (default), the embedded view will not include any controls.</span></span>
| <span data-ttu-id="ad505-136">allowEdit</span><span class="sxs-lookup"><span data-stu-id="ad505-136">allowEdit</span></span>   | <span data-ttu-id="ad505-137">ブール値</span><span class="sxs-lookup"><span data-stu-id="ad505-137">boolean</span></span>       | <span data-ttu-id="ad505-138">省略可能。</span><span class="sxs-lookup"><span data-stu-id="ad505-138">Optional.</span></span> <span data-ttu-id="ad505-139">の`true`場合は、埋め込み UI からファイルを編集できます。</span><span class="sxs-lookup"><span data-stu-id="ad505-139">If `true`, the file can be edited from the embedded UI.</span></span>
| <span data-ttu-id="ad505-140">page</span><span class="sxs-lookup"><span data-stu-id="ad505-140">page</span></span>        | <span data-ttu-id="ad505-141">文字列または数値</span><span class="sxs-lookup"><span data-stu-id="ad505-141">string/number</span></span> | <span data-ttu-id="ad505-142">省略可能。</span><span class="sxs-lookup"><span data-stu-id="ad505-142">Optional.</span></span> <span data-ttu-id="ad505-143">開始するドキュメントのページ番号 (該当する場合)。</span><span class="sxs-lookup"><span data-stu-id="ad505-143">Page number of document to start at, if applicable.</span></span> <span data-ttu-id="ad505-144">ZIP などのファイルの種類に関する今後のユースケースの文字列として指定されます。</span><span class="sxs-lookup"><span data-stu-id="ad505-144">Specified as string for future use cases around file types such as ZIP.</span></span>
| <span data-ttu-id="ad505-145">ズーム</span><span class="sxs-lookup"><span data-stu-id="ad505-145">zoom</span></span>        | <span data-ttu-id="ad505-146">number</span><span class="sxs-lookup"><span data-stu-id="ad505-146">number</span></span>        | <span data-ttu-id="ad505-147">省略可能。</span><span class="sxs-lookup"><span data-stu-id="ad505-147">Optional.</span></span> <span data-ttu-id="ad505-148">必要に応じて、開始するズームレベルを表示します。</span><span class="sxs-lookup"><span data-stu-id="ad505-148">Zoom level to start at, if applicable.</span></span>

## <a name="response"></a><span data-ttu-id="ad505-149">応答</span><span class="sxs-lookup"><span data-stu-id="ad505-149">Response</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

<span data-ttu-id="ad505-150">応答は、次のプロパティを含む JSON オブジェクトになります。</span><span class="sxs-lookup"><span data-stu-id="ad505-150">The response will be a JSON object containing the following properties:</span></span>

| <span data-ttu-id="ad505-151">名前</span><span class="sxs-lookup"><span data-stu-id="ad505-151">Name</span></span>           | <span data-ttu-id="ad505-152">型</span><span class="sxs-lookup"><span data-stu-id="ad505-152">Type</span></span>   | <span data-ttu-id="ad505-153">説明</span><span class="sxs-lookup"><span data-stu-id="ad505-153">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="ad505-154">getUrl</span><span class="sxs-lookup"><span data-stu-id="ad505-154">getUrl</span></span>         | <span data-ttu-id="ad505-155">string</span><span class="sxs-lookup"><span data-stu-id="ad505-155">string</span></span> | <span data-ttu-id="ad505-156">HTTP GET (iframes など) を使用した埋め込みに適した URL</span><span class="sxs-lookup"><span data-stu-id="ad505-156">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="ad505-157">postUrl</span><span class="sxs-lookup"><span data-stu-id="ad505-157">postUrl</span></span>        | <span data-ttu-id="ad505-158">string</span><span class="sxs-lookup"><span data-stu-id="ad505-158">string</span></span> | <span data-ttu-id="ad505-159">HTTP POST (form post、JS など) を使用した埋め込みに適した URL</span><span class="sxs-lookup"><span data-stu-id="ad505-159">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="ad505-160">postParameters</span><span class="sxs-lookup"><span data-stu-id="ad505-160">postParameters</span></span> | <span data-ttu-id="ad505-161">string</span><span class="sxs-lookup"><span data-stu-id="ad505-161">string</span></span> | <span data-ttu-id="ad505-162">PostUrl を使用する場合に含める POST パラメーター</span><span class="sxs-lookup"><span data-stu-id="ad505-162">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="ad505-163">指定したオプションの embed サポートの現在の状態に応じて、getUrl、postUrl、または both のどちらかが返される場合があります。</span><span class="sxs-lookup"><span data-stu-id="ad505-163">Either getUrl, postUrl, or both might be returned depending on the current state of embed support for the specified options.</span></span>

<span data-ttu-id="ad505-164">postParameters はとして`application/x-www-form-urlencoded`書式設定された文字列です。 postparameters への投稿を実行する場合は、コンテンツタイプを適宜設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ad505-164">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="ad505-165">次に例を示します。</span><span class="sxs-lookup"><span data-stu-id="ad505-165">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="viewers"></a><span data-ttu-id="ad505-166">表示者</span><span class="sxs-lookup"><span data-stu-id="ad505-166">Viewers</span></span>

<span data-ttu-id="ad505-167">**Viewer**パラメーターには次の値を使用できます。</span><span class="sxs-lookup"><span data-stu-id="ad505-167">The following values are allowed for the **viewer** parameter.</span></span>

| <span data-ttu-id="ad505-168">種類の値</span><span class="sxs-lookup"><span data-stu-id="ad505-168">Type value</span></span> | <span data-ttu-id="ad505-169">説明</span><span class="sxs-lookup"><span data-stu-id="ad505-169">Description</span></span>
|:-----------|:----------------------------------------------------------------
| <span data-ttu-id="ad505-170">null</span><span class="sxs-lookup"><span data-stu-id="ad505-170">(null)</span></span>     | <span data-ttu-id="ad505-171">ファイルをレンダリングするための適切なアプリを選択します。</span><span class="sxs-lookup"><span data-stu-id="ad505-171">Chooses an appropriate app for rendering the file.</span></span> <span data-ttu-id="ad505-172">ほとんどの場合、これは`onedrive`プレビューアーを使用しますが、ファイルの種類によって異なる場合があります。</span><span class="sxs-lookup"><span data-stu-id="ad505-172">In most cases this will use the `onedrive` previewer, but may vary by file type.</span></span>
| `onedrive` | <span data-ttu-id="ad505-173">OneDrive プレビューアーアプリを使用して、ファイルをレンダリングします。</span><span class="sxs-lookup"><span data-stu-id="ad505-173">Use the OneDrive previewer app to render the file.</span></span>
| `office`   | <span data-ttu-id="ad505-174">Web 版の Office を使用して、ファイルを表示します。</span><span class="sxs-lookup"><span data-stu-id="ad505-174">Use the web version of Office to render the file.</span></span> <span data-ttu-id="ad505-175">Office ドキュメントに対してのみ有効です。</span><span class="sxs-lookup"><span data-stu-id="ad505-175">Only valid for Office documents.</span></span>

### <a name="chrome-vs-chromeless"></a><span data-ttu-id="ad505-176">クロム vs chromeless</span><span class="sxs-lookup"><span data-stu-id="ad505-176">Chrome vs chromeless</span></span>

<span data-ttu-id="ad505-177">が`chromeless` true の場合、プレビューはファイルのベア・レンダリングとなります。</span><span class="sxs-lookup"><span data-stu-id="ad505-177">If `chromeless` is true, the preview will be a bare rendering of the file.</span></span>
<span data-ttu-id="ad505-178">それ以外の場合は、ドキュメント/ビューと対話するためのツールバー/ボタンが追加されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="ad505-178">Otherwise, there may be additional toolbars/buttons displayed for interacting with the document/view.</span></span>

### <a name="viewedit"></a><span data-ttu-id="ad505-179">表示/編集</span><span class="sxs-lookup"><span data-stu-id="ad505-179">View/edit</span></span>

<span data-ttu-id="ad505-180">が`allowEdit` true の場合、ドキュメントは、埋め込みプレビューでユーザーが操作することで変更できます。</span><span class="sxs-lookup"><span data-stu-id="ad505-180">If `allowEdit` is true, the document can be modified by user interaction with the embedded preview.</span></span>
<span data-ttu-id="ad505-181">この機能は、プレビューアプリやファイルの種類によっては使用できない場合があります。</span><span class="sxs-lookup"><span data-stu-id="ad505-181">This capability may not be available for all preview apps or file types.</span></span>

### <a name="pagezoom"></a><span data-ttu-id="ad505-182">ページ/ズーム</span><span class="sxs-lookup"><span data-stu-id="ad505-182">Page/zoom</span></span>

<span data-ttu-id="ad505-183">および`page` `zoom`オプションは、すべてのプレビューアプリで使用できるわけではありませんが、プレビューアプリがサポートしている場合は適用されます。</span><span class="sxs-lookup"><span data-stu-id="ad505-183">The `page` and `zoom` options might not be available for all preview apps, but will be applied if the preview app supports it.</span></span>
