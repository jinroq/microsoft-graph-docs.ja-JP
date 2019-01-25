---
title: 'driveItem: プレビュー'
description: このアクションを使用すると、一時的なプレビューをレンダリングするためにアイテムを短時間の埋め込み可能な Url を取得できます。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5a49a05e1e01616bc9bbbb713fd05805d9af3070
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508539"
---
# <a name="driveitem-preview"></a><span data-ttu-id="b01fc-103">driveItem: プレビュー</span><span class="sxs-lookup"><span data-stu-id="b01fc-103">driveItem: preview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b01fc-104">このアクションを使用すると、一時的なプレビューをレンダリングするためにアイテムを短時間の埋め込み可能な Url を取得できます。</span><span class="sxs-lookup"><span data-stu-id="b01fc-104">This action allows you to obtain short-lived embeddable URLs for an item in order to render a temporary preview.</span></span>

<span data-ttu-id="b01fc-105">有効期間の長い埋め込みリンクを取得する場合は、 [createLink][] API を使用してください。</span><span class="sxs-lookup"><span data-stu-id="b01fc-105">If you want to obtain long-lived embeddable links, use the [createLink][] API instead.</span></span>

> <span data-ttu-id="b01fc-106">**注:\*\*\*\*プレビュー**の動作は、現在 SharePoint およびビジネスのための OneDrive で使用可能なのみです。</span><span class="sxs-lookup"><span data-stu-id="b01fc-106">**Note:** The **preview** action is currently only available on SharePoint and OneDrive for Business.</span></span>

[createLink]: driveitem-createlink.md

## <a name="permissions"></a><span data-ttu-id="b01fc-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b01fc-108">Permissions</span></span>

<span data-ttu-id="b01fc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b01fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b01fc-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b01fc-111">Permission type</span></span>                        | <span data-ttu-id="b01fc-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b01fc-112">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="b01fc-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b01fc-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="b01fc-114">Files.Read、Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b01fc-114">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="b01fc-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b01fc-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b01fc-116">Files.Read、Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b01fc-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="b01fc-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b01fc-117">Application</span></span>                            | <span data-ttu-id="b01fc-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b01fc-118">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="b01fc-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b01fc-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/preview
POST /groups/{groupId}/drive/items/{itemId}/preview
POST /me/drive/items/{itemId}/preview
POST /sites/{siteId}/drive/items/{itemId}/preview
POST /users/{userId}/drive/items/{itemId}/preview
POST /shares/{shareId}/driveItem/preview
```

## <a name="request-body"></a><span data-ttu-id="b01fc-120">要求本文</span><span class="sxs-lookup"><span data-stu-id="b01fc-120">Request body</span></span>

<span data-ttu-id="b01fc-121">要求の本文では、アプリケーションが要求する埋め込み可能な URL のプロパティを定義します。</span><span class="sxs-lookup"><span data-stu-id="b01fc-121">The body of the request defines properties of the embeddable URL your application is requesting.</span></span>
<span data-ttu-id="b01fc-122">要求は、次のプロパティを含む JSON オブジェクトである必要があります。</span><span class="sxs-lookup"><span data-stu-id="b01fc-122">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="b01fc-123">名前</span><span class="sxs-lookup"><span data-stu-id="b01fc-123">Name</span></span>      |  <span data-ttu-id="b01fc-124">型</span><span class="sxs-lookup"><span data-stu-id="b01fc-124">Type</span></span>         | <span data-ttu-id="b01fc-125">説明</span><span class="sxs-lookup"><span data-stu-id="b01fc-125">Description</span></span>
|:------------|:--------------|:-----------------------------------------------
| <span data-ttu-id="b01fc-126">ビューアー</span><span class="sxs-lookup"><span data-stu-id="b01fc-126">viewer</span></span>      | <span data-ttu-id="b01fc-127">string</span><span class="sxs-lookup"><span data-stu-id="b01fc-127">string</span></span>        | <span data-ttu-id="b01fc-128">省略可能。</span><span class="sxs-lookup"><span data-stu-id="b01fc-128">Optional.</span></span> <span data-ttu-id="b01fc-129">使用するアプリケーションをプレビューします。</span><span class="sxs-lookup"><span data-stu-id="b01fc-129">Preview app to use.</span></span> <span data-ttu-id="b01fc-130">`onedrive` や `office` などになります。</span><span class="sxs-lookup"><span data-stu-id="b01fc-130">`onedrive` or `office`.</span></span> <span data-ttu-id="b01fc-131">Null の場合、適切なビューアーが自動的に選択されます。</span><span class="sxs-lookup"><span data-stu-id="b01fc-131">If null, a suitable viewer will be chosen automatically.</span></span>
| <span data-ttu-id="b01fc-132">クロムレス</span><span class="sxs-lookup"><span data-stu-id="b01fc-132">chromeless</span></span>  | <span data-ttu-id="b01fc-133">boolean</span><span class="sxs-lookup"><span data-stu-id="b01fc-133">boolean</span></span>       | <span data-ttu-id="b01fc-134">省略可能。</span><span class="sxs-lookup"><span data-stu-id="b01fc-134">Optional.</span></span> <span data-ttu-id="b01fc-135">場合`true`(既定値)、組み込みのビューのコントロールは含まれません。</span><span class="sxs-lookup"><span data-stu-id="b01fc-135">If `true` (default), the embedded view will not include any controls.</span></span>
| <span data-ttu-id="b01fc-136">AllowEdit</span><span class="sxs-lookup"><span data-stu-id="b01fc-136">allowEdit</span></span>   | <span data-ttu-id="b01fc-137">boolean</span><span class="sxs-lookup"><span data-stu-id="b01fc-137">boolean</span></span>       | <span data-ttu-id="b01fc-138">省略可能。</span><span class="sxs-lookup"><span data-stu-id="b01fc-138">Optional.</span></span> <span data-ttu-id="b01fc-139">場合`true`、埋め込まれた UI からファイルを編集することができます。</span><span class="sxs-lookup"><span data-stu-id="b01fc-139">If `true`, the file can be edited from the embedded UI.</span></span>
| <span data-ttu-id="b01fc-140">page</span><span class="sxs-lookup"><span data-stu-id="b01fc-140">page</span></span>        | <span data-ttu-id="b01fc-141">文字列と番号</span><span class="sxs-lookup"><span data-stu-id="b01fc-141">string/number</span></span> | <span data-ttu-id="b01fc-142">省略可能。</span><span class="sxs-lookup"><span data-stu-id="b01fc-142">Optional.</span></span> <span data-ttu-id="b01fc-143">該当する場合に、開始するドキュメントのページ数です。</span><span class="sxs-lookup"><span data-stu-id="b01fc-143">Page number of document to start at, if applicable.</span></span> <span data-ttu-id="b01fc-144">将来使用する場合は、ZIP などのファイルの種類を文字列として指定します。</span><span class="sxs-lookup"><span data-stu-id="b01fc-144">Specified as string for future use cases around file types such as ZIP.</span></span>
| <span data-ttu-id="b01fc-145">ズーム</span><span class="sxs-lookup"><span data-stu-id="b01fc-145">zoom</span></span>        | <span data-ttu-id="b01fc-146">number</span><span class="sxs-lookup"><span data-stu-id="b01fc-146">number</span></span>        | <span data-ttu-id="b01fc-147">省略可能。</span><span class="sxs-lookup"><span data-stu-id="b01fc-147">Optional.</span></span> <span data-ttu-id="b01fc-148">該当する場合に、開始するレベルを拡大します。</span><span class="sxs-lookup"><span data-stu-id="b01fc-148">Zoom level to start at, if applicable.</span></span>

## <a name="response"></a><span data-ttu-id="b01fc-149">応答</span><span class="sxs-lookup"><span data-stu-id="b01fc-149">Response</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

<span data-ttu-id="b01fc-150">応答は、次のプロパティを含む JSON オブジェクトになります。</span><span class="sxs-lookup"><span data-stu-id="b01fc-150">The response will be a JSON object containing the following properties:</span></span>

| <span data-ttu-id="b01fc-151">名前</span><span class="sxs-lookup"><span data-stu-id="b01fc-151">Name</span></span>           | <span data-ttu-id="b01fc-152">型</span><span class="sxs-lookup"><span data-stu-id="b01fc-152">Type</span></span>   | <span data-ttu-id="b01fc-153">説明</span><span class="sxs-lookup"><span data-stu-id="b01fc-153">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="b01fc-154">getUrl</span><span class="sxs-lookup"><span data-stu-id="b01fc-154">getUrl</span></span>         | <span data-ttu-id="b01fc-155">string</span><span class="sxs-lookup"><span data-stu-id="b01fc-155">string</span></span> | <span data-ttu-id="b01fc-156">HTTP の GET (iframe など) を使用して埋め込みの適切な URL</span><span class="sxs-lookup"><span data-stu-id="b01fc-156">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="b01fc-157">postUrl</span><span class="sxs-lookup"><span data-stu-id="b01fc-157">postUrl</span></span>        | <span data-ttu-id="b01fc-158">string</span><span class="sxs-lookup"><span data-stu-id="b01fc-158">string</span></span> | <span data-ttu-id="b01fc-159">HTTP POST を使用して埋め込みの適切な URL (フォーム ポスト、JS など)。</span><span class="sxs-lookup"><span data-stu-id="b01fc-159">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="b01fc-160">postParameters</span><span class="sxs-lookup"><span data-stu-id="b01fc-160">postParameters</span></span> | <span data-ttu-id="b01fc-161">string</span><span class="sxs-lookup"><span data-stu-id="b01fc-161">string</span></span> | <span data-ttu-id="b01fc-162">PostUrl を使用する場合は、POST のパラメーター</span><span class="sxs-lookup"><span data-stu-id="b01fc-162">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="b01fc-163">GetUrl、postUrl、またはその両方は、指定したオプションの埋め込みのサポートの現在の状態によって返される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="b01fc-163">Either getUrl, postUrl, or both might be returned depending on the current state of embed support for the specified options.</span></span>

<span data-ttu-id="b01fc-164">として書式設定された文字列は、postParameters`application/x-www-form-urlencoded`と postUrl のコンテンツの種類へのポストを実行し、それに応じて設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b01fc-164">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="b01fc-165">次に例を示します。</span><span class="sxs-lookup"><span data-stu-id="b01fc-165">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="viewers"></a><span data-ttu-id="b01fc-166">ビューアー</span><span class="sxs-lookup"><span data-stu-id="b01fc-166">Viewers</span></span>

<span data-ttu-id="b01fc-167">**ビューアー**パラメーターには、次の値を指定します。</span><span class="sxs-lookup"><span data-stu-id="b01fc-167">The following values are allowed for the **viewer** parameter.</span></span>

| <span data-ttu-id="b01fc-168">種類の値</span><span class="sxs-lookup"><span data-stu-id="b01fc-168">Type value</span></span> | <span data-ttu-id="b01fc-169">説明</span><span class="sxs-lookup"><span data-stu-id="b01fc-169">Description</span></span>
|:-----------|:----------------------------------------------------------------
| <span data-ttu-id="b01fc-170">Null
</span><span class="sxs-lookup"><span data-stu-id="b01fc-170">(null)</span></span>     | <span data-ttu-id="b01fc-171">ファイルを表示するための適切なアプリケーションを選択します。</span><span class="sxs-lookup"><span data-stu-id="b01fc-171">Chooses an appropriate app for rendering the file.</span></span> <span data-ttu-id="b01fc-172">使用するほとんどの場合、`onedrive`プレビューアーをファイルの種類によって異なる場合がありますが。</span><span class="sxs-lookup"><span data-stu-id="b01fc-172">In most cases this will use the `onedrive` previewer, but may vary by file type.</span></span>
| `onedrive` | <span data-ttu-id="b01fc-173">ファイルをレンダリングするのにには、OneDrive 対応のアプリケーションを使用します。</span><span class="sxs-lookup"><span data-stu-id="b01fc-173">Use the OneDrive previewer app to render the file.</span></span>
| `office`   | <span data-ttu-id="b01fc-174">WAC (Office オンライン) を使用して、ファイルをレンダリングします。</span><span class="sxs-lookup"><span data-stu-id="b01fc-174">Use the WAC (Office online) to render the file.</span></span> <span data-ttu-id="b01fc-175">Office ドキュメントに対してのみ有効です。</span><span class="sxs-lookup"><span data-stu-id="b01fc-175">Only valid for Office documents.</span></span>

### <a name="chrome-vs-chromeless"></a><span data-ttu-id="b01fc-176">クロムレスのクロム vs</span><span class="sxs-lookup"><span data-stu-id="b01fc-176">Chrome vs chromeless</span></span>

<span data-ttu-id="b01fc-177">場合`chromeless`が true の場合、プレビュー、ファイルの最小限のレンダリングになります。</span><span class="sxs-lookup"><span data-stu-id="b01fc-177">If `chromeless` is true, the preview will be a bare rendering of the file.</span></span>
<span data-ttu-id="b01fc-178">それ以外の場合、ドキュメント/ビューと対話するために表示されるその他のツールバーとボタンがある可能性があります。</span><span class="sxs-lookup"><span data-stu-id="b01fc-178">Otherwise, there may be additional toolbars/buttons displayed for interacting with the document/view.</span></span>

### <a name="viewedit"></a><span data-ttu-id="b01fc-179">表示/編集</span><span class="sxs-lookup"><span data-stu-id="b01fc-179">View/edit</span></span>

<span data-ttu-id="b01fc-180">場合`allowEdit`が true の場合、埋め込まれたプレビューをユーザーの操作によって、ドキュメントを変更できます。</span><span class="sxs-lookup"><span data-stu-id="b01fc-180">If `allowEdit` is true, the document can be modified by user interaction with the embedded preview.</span></span>
<span data-ttu-id="b01fc-181">この機能は、すべてのプレビューのアプリケーションまたはファイルの種類のできない場合があります。</span><span class="sxs-lookup"><span data-stu-id="b01fc-181">This capability may not be available for all preview apps or file types.</span></span>

### <a name="pagezoom"></a><span data-ttu-id="b01fc-182">ページ/ズーム</span><span class="sxs-lookup"><span data-stu-id="b01fc-182">Page/zoom</span></span>

<span data-ttu-id="b01fc-183">`page`と`zoom`オプションは、すべてのプレビュー アプリケーションを使用できない場合がありますが、プレビューのアプリケーションをサポートしている場合に適用されます。</span><span class="sxs-lookup"><span data-stu-id="b01fc-183">The `page` and `zoom` options might not be available for all preview apps, but will be applied if the preview app supports it.</span></span>
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-preview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
