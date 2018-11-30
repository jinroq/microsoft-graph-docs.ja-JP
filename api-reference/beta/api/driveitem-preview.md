---
title: 'driveItem: プレビュー'
description: このアクションを使用すると、一時的なプレビューをレンダリングするためにアイテムを短時間の埋め込み可能な Url を取得できます。
ms.openlocfilehash: 51432e53d6986e680dda8508ef0069c7713b3a9d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067932"
---
# <a name="driveitem-preview"></a><span data-ttu-id="8225a-103">driveItem: プレビュー</span><span class="sxs-lookup"><span data-stu-id="8225a-103">driveItem: preview</span></span>

> <span data-ttu-id="8225a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8225a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8225a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8225a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8225a-106">このアクションを使用すると、一時的なプレビューをレンダリングするためにアイテムを短時間の埋め込み可能な Url を取得できます。</span><span class="sxs-lookup"><span data-stu-id="8225a-106">This action allows you to obtain short-lived embeddable URLs for an item in order to render a temporary preview.</span></span>

<span data-ttu-id="8225a-107">有効期間の長い埋め込みリンクを取得する場合は、 [createLink][] API を使用してください。</span><span class="sxs-lookup"><span data-stu-id="8225a-107">If you want to obtain long-lived embeddable links, use the [createLink][] API instead.</span></span>

> <span data-ttu-id="8225a-108">**注:\*\*\*\*プレビュー**の動作は、現在 SharePoint およびビジネスのための OneDrive で使用可能なのみです。</span><span class="sxs-lookup"><span data-stu-id="8225a-108">**Note:** The **preview** action is currently only available on SharePoint and OneDrive for Business.</span></span>

[createLink]: driveitem-createlink.md

## <a name="permissions"></a><span data-ttu-id="8225a-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8225a-110">Permissions</span></span>

<span data-ttu-id="8225a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8225a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8225a-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8225a-113">Permission type</span></span>                        | <span data-ttu-id="8225a-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8225a-114">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="8225a-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8225a-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="8225a-116">Files.Read、Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8225a-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="8225a-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8225a-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8225a-118">Files.Read、Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8225a-118">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="8225a-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8225a-119">Application</span></span>                            | <span data-ttu-id="8225a-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8225a-120">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="8225a-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8225a-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/preview
POST /groups/{groupId}/drive/items/{itemId}/preview
POST /me/drive/items/{itemId}/preview
POST /sites/{siteId}/drive/items/{itemId}/preview
POST /users/{userId}/drive/items/{itemId}/preview
POST /shares/{shareId}/driveItem/preview
```

## <a name="request-body"></a><span data-ttu-id="8225a-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="8225a-122">Request body</span></span>

<span data-ttu-id="8225a-123">要求の本文では、アプリケーションが要求する埋め込み可能な URL のプロパティを定義します。</span><span class="sxs-lookup"><span data-stu-id="8225a-123">The body of the request defines properties of the embeddable URL your application is requesting.</span></span>
<span data-ttu-id="8225a-124">要求は、次のプロパティを含む JSON オブジェクトである必要があります。</span><span class="sxs-lookup"><span data-stu-id="8225a-124">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="8225a-125">名前</span><span class="sxs-lookup"><span data-stu-id="8225a-125">Name</span></span>      |  <span data-ttu-id="8225a-126">型</span><span class="sxs-lookup"><span data-stu-id="8225a-126">Type</span></span>         | <span data-ttu-id="8225a-127">説明</span><span class="sxs-lookup"><span data-stu-id="8225a-127">Description</span></span>
|:------------|:--------------|:-----------------------------------------------
| <span data-ttu-id="8225a-128">ビューアー</span><span class="sxs-lookup"><span data-stu-id="8225a-128">viewer</span></span>      | <span data-ttu-id="8225a-129">文字列</span><span class="sxs-lookup"><span data-stu-id="8225a-129">string</span></span>        | <span data-ttu-id="8225a-130">省略可能。</span><span class="sxs-lookup"><span data-stu-id="8225a-130">Optional.</span></span> <span data-ttu-id="8225a-131">使用するアプリケーションをプレビューします。</span><span class="sxs-lookup"><span data-stu-id="8225a-131">Preview app to use.</span></span> <span data-ttu-id="8225a-132">`onedrive` や `office` などになります。</span><span class="sxs-lookup"><span data-stu-id="8225a-132">`onedrive` or `office`.</span></span> <span data-ttu-id="8225a-133">Null の場合、適切なビューアーが自動的に選択されます。</span><span class="sxs-lookup"><span data-stu-id="8225a-133">If null, a suitable viewer will be chosen automatically.</span></span>
| <span data-ttu-id="8225a-134">クロムレス</span><span class="sxs-lookup"><span data-stu-id="8225a-134">chromeless</span></span>  | <span data-ttu-id="8225a-135">ブール</span><span class="sxs-lookup"><span data-stu-id="8225a-135">boolean</span></span>       | <span data-ttu-id="8225a-136">省略可能。</span><span class="sxs-lookup"><span data-stu-id="8225a-136">Optional.</span></span> <span data-ttu-id="8225a-137">場合`true`(既定値)、組み込みのビューのコントロールは含まれません。</span><span class="sxs-lookup"><span data-stu-id="8225a-137">If `true` (default), the embedded view will not include any controls.</span></span>
| <span data-ttu-id="8225a-138">allowEdit</span><span class="sxs-lookup"><span data-stu-id="8225a-138">allowEdit</span></span>   | <span data-ttu-id="8225a-139">ブール</span><span class="sxs-lookup"><span data-stu-id="8225a-139">boolean</span></span>       | <span data-ttu-id="8225a-140">省略可能。</span><span class="sxs-lookup"><span data-stu-id="8225a-140">Optional.</span></span> <span data-ttu-id="8225a-141">場合`true`、埋め込まれた UI からファイルを編集することができます。</span><span class="sxs-lookup"><span data-stu-id="8225a-141">If `true`, the file can be edited from the embedded UI.</span></span>
| <span data-ttu-id="8225a-142">page</span><span class="sxs-lookup"><span data-stu-id="8225a-142">page</span></span>        | <span data-ttu-id="8225a-143">文字列と番号</span><span class="sxs-lookup"><span data-stu-id="8225a-143">string/number</span></span> | <span data-ttu-id="8225a-144">省略可能。</span><span class="sxs-lookup"><span data-stu-id="8225a-144">Optional.</span></span> <span data-ttu-id="8225a-145">該当する場合に、開始するドキュメントのページ数です。</span><span class="sxs-lookup"><span data-stu-id="8225a-145">Page number of document to start at, if applicable.</span></span> <span data-ttu-id="8225a-146">将来使用する場合は、ZIP などのファイルの種類を文字列として指定します。</span><span class="sxs-lookup"><span data-stu-id="8225a-146">Specified as string for future use cases around file types such as ZIP.</span></span>
| <span data-ttu-id="8225a-147">ズーム</span><span class="sxs-lookup"><span data-stu-id="8225a-147">zoom</span></span>        | <span data-ttu-id="8225a-148">数値</span><span class="sxs-lookup"><span data-stu-id="8225a-148">number</span></span>        | <span data-ttu-id="8225a-149">省略可能。</span><span class="sxs-lookup"><span data-stu-id="8225a-149">Optional.</span></span> <span data-ttu-id="8225a-150">該当する場合に、開始するレベルを拡大します。</span><span class="sxs-lookup"><span data-stu-id="8225a-150">Zoom level to start at, if applicable.</span></span>

## <a name="response"></a><span data-ttu-id="8225a-151">応答</span><span class="sxs-lookup"><span data-stu-id="8225a-151">Response</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

<span data-ttu-id="8225a-152">応答は、次のプロパティを含む JSON オブジェクトになります。</span><span class="sxs-lookup"><span data-stu-id="8225a-152">The response will be a JSON object containing the following properties:</span></span>

| <span data-ttu-id="8225a-153">名前</span><span class="sxs-lookup"><span data-stu-id="8225a-153">Name</span></span>           | <span data-ttu-id="8225a-154">型</span><span class="sxs-lookup"><span data-stu-id="8225a-154">Type</span></span>   | <span data-ttu-id="8225a-155">説明</span><span class="sxs-lookup"><span data-stu-id="8225a-155">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="8225a-156">getUrl</span><span class="sxs-lookup"><span data-stu-id="8225a-156">getUrl</span></span>         | <span data-ttu-id="8225a-157">文字列</span><span class="sxs-lookup"><span data-stu-id="8225a-157">string</span></span> | <span data-ttu-id="8225a-158">HTTP の GET (iframe など) を使用して埋め込みの適切な URL</span><span class="sxs-lookup"><span data-stu-id="8225a-158">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="8225a-159">postUrl</span><span class="sxs-lookup"><span data-stu-id="8225a-159">postUrl</span></span>        | <span data-ttu-id="8225a-160">文字列</span><span class="sxs-lookup"><span data-stu-id="8225a-160">string</span></span> | <span data-ttu-id="8225a-161">HTTP POST を使用して埋め込みの適切な URL (フォーム ポスト、JS など)。</span><span class="sxs-lookup"><span data-stu-id="8225a-161">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="8225a-162">postParameters</span><span class="sxs-lookup"><span data-stu-id="8225a-162">postParameters</span></span> | <span data-ttu-id="8225a-163">文字列</span><span class="sxs-lookup"><span data-stu-id="8225a-163">string</span></span> | <span data-ttu-id="8225a-164">PostUrl を使用する場合は、POST のパラメーター</span><span class="sxs-lookup"><span data-stu-id="8225a-164">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="8225a-165">GetUrl、postUrl、またはその両方は、指定したオプションの埋め込みのサポートの現在の状態によって返される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="8225a-165">Either getUrl, postUrl, or both might be returned depending on the current state of embed support for the specified options.</span></span>

<span data-ttu-id="8225a-166">として書式設定された文字列は、postParameters`application/x-www-form-urlencoded`と postUrl のコンテンツの種類へのポストを実行し、それに応じて設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="8225a-166">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="8225a-167">例:</span><span class="sxs-lookup"><span data-stu-id="8225a-167">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="viewers"></a><span data-ttu-id="8225a-168">ビューアー</span><span class="sxs-lookup"><span data-stu-id="8225a-168">Viewers</span></span>

<span data-ttu-id="8225a-169">**ビューアー**パラメーターには、次の値を指定します。</span><span class="sxs-lookup"><span data-stu-id="8225a-169">The following values are allowed for the **viewer** parameter.</span></span>

| <span data-ttu-id="8225a-170">種類の値</span><span class="sxs-lookup"><span data-stu-id="8225a-170">Type value</span></span> | <span data-ttu-id="8225a-171">説明</span><span class="sxs-lookup"><span data-stu-id="8225a-171">Description</span></span>
|:-----------|:----------------------------------------------------------------
| <span data-ttu-id="8225a-172">(null)</span><span class="sxs-lookup"><span data-stu-id="8225a-172">(null)</span></span>     | <span data-ttu-id="8225a-173">ファイルを表示するための適切なアプリケーションを選択します。</span><span class="sxs-lookup"><span data-stu-id="8225a-173">Chooses an appropriate app for rendering the file.</span></span> <span data-ttu-id="8225a-174">使用するほとんどの場合、`onedrive`プレビューアーをファイルの種類によって異なる場合がありますが。</span><span class="sxs-lookup"><span data-stu-id="8225a-174">In most cases this will use the `onedrive` previewer, but may vary by file type.</span></span>
| `onedrive` | <span data-ttu-id="8225a-175">ファイルをレンダリングするのにには、OneDrive 対応のアプリケーションを使用します。</span><span class="sxs-lookup"><span data-stu-id="8225a-175">Use the OneDrive previewer app to render the file.</span></span>
| `office`   | <span data-ttu-id="8225a-176">WAC (Office オンライン) を使用して、ファイルをレンダリングします。</span><span class="sxs-lookup"><span data-stu-id="8225a-176">Use the WAC (Office online) to render the file.</span></span> <span data-ttu-id="8225a-177">Office ドキュメントに対してのみ有効です。</span><span class="sxs-lookup"><span data-stu-id="8225a-177">Only valid for Office documents.</span></span>

### <a name="chrome-vs-chromeless"></a><span data-ttu-id="8225a-178">クロムレスのクロム vs</span><span class="sxs-lookup"><span data-stu-id="8225a-178">Chrome vs chromeless</span></span>

<span data-ttu-id="8225a-179">場合`chromeless`が true の場合、プレビュー、ファイルの最小限のレンダリングになります。</span><span class="sxs-lookup"><span data-stu-id="8225a-179">If `chromeless` is true, the preview will be a bare rendering of the file.</span></span>
<span data-ttu-id="8225a-180">それ以外の場合、ドキュメント/ビューと対話するために表示されるその他のツールバーとボタンがある可能性があります。</span><span class="sxs-lookup"><span data-stu-id="8225a-180">Otherwise, there may be additional toolbars/buttons displayed for interacting with the document/view.</span></span>

### <a name="viewedit"></a><span data-ttu-id="8225a-181">表示/編集</span><span class="sxs-lookup"><span data-stu-id="8225a-181">View/edit</span></span>

<span data-ttu-id="8225a-182">場合`allowEdit`が true の場合、埋め込まれたプレビューをユーザーの操作によって、ドキュメントを変更できます。</span><span class="sxs-lookup"><span data-stu-id="8225a-182">If `allowEdit` is true, the document can be modified by user interaction with the embedded preview.</span></span>
<span data-ttu-id="8225a-183">この機能は、すべてのプレビューのアプリケーションまたはファイルの種類のできない場合があります。</span><span class="sxs-lookup"><span data-stu-id="8225a-183">This capability may not be available for all preview apps or file types.</span></span>

### <a name="pagezoom"></a><span data-ttu-id="8225a-184">ページ/ズーム</span><span class="sxs-lookup"><span data-stu-id="8225a-184">Page/zoom</span></span>

<span data-ttu-id="8225a-185">`page`と`zoom`オプションは、すべてのプレビュー アプリケーションを使用できない場合がありますが、プレビューのアプリケーションをサポートしている場合に適用されます。</span><span class="sxs-lookup"><span data-stu-id="8225a-185">The `page` and `zoom` options might not be available for all preview apps, but will be applied if the preview app supports it.</span></span>
