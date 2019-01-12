---
title: 'driveItem: プレビュー'
description: このアクションを使用すると、一時的なプレビューをレンダリングするためにアイテムを短時間の埋め込み可能な Url を取得できます。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: ae5140bf6164aedd051f04c2c43c361f16517e7a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986076"
---
# <a name="driveitem-preview"></a><span data-ttu-id="d0dbf-103">driveItem: プレビュー</span><span class="sxs-lookup"><span data-stu-id="d0dbf-103">driveItem: preview</span></span>

<span data-ttu-id="d0dbf-104">このアクションを使用すると、一時的なプレビューをレンダリングするためにアイテムを短時間の埋め込み可能な Url を取得できます。</span><span class="sxs-lookup"><span data-stu-id="d0dbf-104">This action allows you to obtain short-lived embeddable URLs for an item in order to render a temporary preview.</span></span>

<span data-ttu-id="d0dbf-105">有効期間の長い埋め込みリンクを取得する場合は、 [createLink][] API を使用してください。</span><span class="sxs-lookup"><span data-stu-id="d0dbf-105">If you want to obtain long-lived embeddable links, use the [createLink][] API instead.</span></span>

> <span data-ttu-id="d0dbf-106">**注:\*\*\*\*プレビュー**の動作は、現在 SharePoint およびビジネスのための OneDrive で使用可能なのみです。</span><span class="sxs-lookup"><span data-stu-id="d0dbf-106">**Note:** The **preview** action is currently only available on SharePoint and OneDrive for Business.</span></span>

[createLink]: driveitem-createlink.md

## <a name="permissions"></a><span data-ttu-id="d0dbf-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d0dbf-108">Permissions</span></span>

<span data-ttu-id="d0dbf-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d0dbf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d0dbf-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d0dbf-111">Permission type</span></span>                        | <span data-ttu-id="d0dbf-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d0dbf-112">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="d0dbf-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d0dbf-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="d0dbf-114">Files.Read、Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0dbf-114">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="d0dbf-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d0dbf-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0dbf-116">Files.Read、Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0dbf-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="d0dbf-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d0dbf-117">Application</span></span>                            | <span data-ttu-id="d0dbf-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d0dbf-118">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="d0dbf-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d0dbf-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/preview
POST /groups/{groupId}/drive/items/{itemId}/preview
POST /me/drive/items/{itemId}/preview
POST /sites/{siteId}/drive/items/{itemId}/preview
POST /users/{userId}/drive/items/{itemId}/preview
POST /shares/{shareId}/driveItem/preview
```

## <a name="request-body"></a><span data-ttu-id="d0dbf-120">要求本文</span><span class="sxs-lookup"><span data-stu-id="d0dbf-120">Request body</span></span>

<span data-ttu-id="d0dbf-121">要求の本文では、アプリケーションが要求する埋め込み可能な URL のプロパティを定義します。</span><span class="sxs-lookup"><span data-stu-id="d0dbf-121">The body of the request defines properties of the embeddable URL your application is requesting.</span></span>
<span data-ttu-id="d0dbf-122">要求は、次のプロパティを含む JSON オブジェクトである必要があります。</span><span class="sxs-lookup"><span data-stu-id="d0dbf-122">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="d0dbf-123">名前</span><span class="sxs-lookup"><span data-stu-id="d0dbf-123">Name</span></span>      |  <span data-ttu-id="d0dbf-124">種類</span><span class="sxs-lookup"><span data-stu-id="d0dbf-124">Type</span></span>         | <span data-ttu-id="d0dbf-125">説明</span><span class="sxs-lookup"><span data-stu-id="d0dbf-125">Description</span></span>
|:------------|:--------------|:-----------------------------------------------
| <span data-ttu-id="d0dbf-126">page</span><span class="sxs-lookup"><span data-stu-id="d0dbf-126">page</span></span>        | <span data-ttu-id="d0dbf-127">文字列と番号</span><span class="sxs-lookup"><span data-stu-id="d0dbf-127">string/number</span></span> | <span data-ttu-id="d0dbf-128">省略可能。</span><span class="sxs-lookup"><span data-stu-id="d0dbf-128">Optional.</span></span> <span data-ttu-id="d0dbf-129">該当する場合に、開始するドキュメントのページ数です。</span><span class="sxs-lookup"><span data-stu-id="d0dbf-129">Page number of document to start at, if applicable.</span></span> <span data-ttu-id="d0dbf-130">将来使用する場合は、ZIP などのファイルの種類を文字列として指定します。</span><span class="sxs-lookup"><span data-stu-id="d0dbf-130">Specified as string for future use cases around file types such as ZIP.</span></span>
| <span data-ttu-id="d0dbf-131">ズーム</span><span class="sxs-lookup"><span data-stu-id="d0dbf-131">zoom</span></span>        | <span data-ttu-id="d0dbf-132">number</span><span class="sxs-lookup"><span data-stu-id="d0dbf-132">number</span></span>        | <span data-ttu-id="d0dbf-133">省略可能。</span><span class="sxs-lookup"><span data-stu-id="d0dbf-133">Optional.</span></span> <span data-ttu-id="d0dbf-134">該当する場合に、開始するレベルを拡大します。</span><span class="sxs-lookup"><span data-stu-id="d0dbf-134">Zoom level to start at, if applicable.</span></span>

## <a name="response"></a><span data-ttu-id="d0dbf-135">応答</span><span class="sxs-lookup"><span data-stu-id="d0dbf-135">Response</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

<span data-ttu-id="d0dbf-136">応答は、次のプロパティを含む JSON オブジェクトになります。</span><span class="sxs-lookup"><span data-stu-id="d0dbf-136">The response will be a JSON object containing the following properties:</span></span>

| <span data-ttu-id="d0dbf-137">名前</span><span class="sxs-lookup"><span data-stu-id="d0dbf-137">Name</span></span>           | <span data-ttu-id="d0dbf-138">種類</span><span class="sxs-lookup"><span data-stu-id="d0dbf-138">Type</span></span>   | <span data-ttu-id="d0dbf-139">説明</span><span class="sxs-lookup"><span data-stu-id="d0dbf-139">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="d0dbf-140">getUrl</span><span class="sxs-lookup"><span data-stu-id="d0dbf-140">getUrl</span></span>         | <span data-ttu-id="d0dbf-141">文字列</span><span class="sxs-lookup"><span data-stu-id="d0dbf-141">string</span></span> | <span data-ttu-id="d0dbf-142">HTTP の GET (iframe など) を使用して埋め込みの適切な URL</span><span class="sxs-lookup"><span data-stu-id="d0dbf-142">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="d0dbf-143">postUrl</span><span class="sxs-lookup"><span data-stu-id="d0dbf-143">postUrl</span></span>        | <span data-ttu-id="d0dbf-144">文字列</span><span class="sxs-lookup"><span data-stu-id="d0dbf-144">string</span></span> | <span data-ttu-id="d0dbf-145">HTTP POST を使用して埋め込みの適切な URL (フォーム ポスト、JS など)。</span><span class="sxs-lookup"><span data-stu-id="d0dbf-145">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="d0dbf-146">postParameters</span><span class="sxs-lookup"><span data-stu-id="d0dbf-146">postParameters</span></span> | <span data-ttu-id="d0dbf-147">文字列</span><span class="sxs-lookup"><span data-stu-id="d0dbf-147">string</span></span> | <span data-ttu-id="d0dbf-148">PostUrl を使用する場合は、POST のパラメーター</span><span class="sxs-lookup"><span data-stu-id="d0dbf-148">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="d0dbf-149">GetUrl、postUrl、またはその両方は、指定したオプションの埋め込みのサポートの現在の状態によって返される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="d0dbf-149">Either getUrl, postUrl, or both might be returned depending on the current state of embed support for the specified options.</span></span>

<span data-ttu-id="d0dbf-150">として書式設定された文字列は、postParameters`application/x-www-form-urlencoded`と postUrl のコンテンツの種類へのポストを実行し、それに応じて設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d0dbf-150">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="d0dbf-151">例:</span><span class="sxs-lookup"><span data-stu-id="d0dbf-151">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="pagezoom"></a><span data-ttu-id="d0dbf-152">ページ/ズーム</span><span class="sxs-lookup"><span data-stu-id="d0dbf-152">Page/zoom</span></span>

<span data-ttu-id="d0dbf-153">'ページ' と '拡大' オプションは、すべてのプレビュー アプリケーションを使用できない場合がありますが、プレビュー アプリケーションでサポートされている場合に適用されます。</span><span class="sxs-lookup"><span data-stu-id="d0dbf-153">The 'page' and 'zoom' options may not be available for all preview apps, but will be applied if the preview app supports it.</span></span>
