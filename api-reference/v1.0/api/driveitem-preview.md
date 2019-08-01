---
title: 'ドライブアイテム: プレビュー'
description: このアクションを使用すると、一時的なプレビューを表示するために、短時間に埋め込まれた、アイテムの Url を取得できます。
localization_priority: Normal
ms.prod: sharepoint
author: ''
doc_type: apiPageType
ms.openlocfilehash: 1de53b8183f4277c0241a08822ef539613b83a45
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36015342"
---
# <a name="driveitem-preview"></a><span data-ttu-id="ae450-103">ドライブアイテム: プレビュー</span><span class="sxs-lookup"><span data-stu-id="ae450-103">driveItem: preview</span></span>

<span data-ttu-id="ae450-104">このアクションを使用すると、一時的なプレビューを表示するために、短時間に埋め込まれた、アイテムの Url を取得できます。</span><span class="sxs-lookup"><span data-stu-id="ae450-104">This action allows you to obtain short-lived embeddable URLs for an item in order to render a temporary preview.</span></span>

<span data-ttu-id="ae450-105">長時間の埋め込み可能なリンクを取得する場合は、代わりに[Createlink][] API を使用します。</span><span class="sxs-lookup"><span data-stu-id="ae450-105">If you want to obtain long-lived embeddable links, use the [createLink][] API instead.</span></span>

> <span data-ttu-id="ae450-106">**注:** 現在、**プレビュー**アクションは SharePoint および OneDrive for business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="ae450-106">**Note:** The **preview** action is currently only available on SharePoint and OneDrive for Business.</span></span>

[createLink]: driveitem-createlink.md

## <a name="permissions"></a><span data-ttu-id="ae450-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ae450-108">Permissions</span></span>

<span data-ttu-id="ae450-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ae450-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ae450-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ae450-111">Permission type</span></span>                        | <span data-ttu-id="ae450-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ae450-112">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="ae450-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ae450-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="ae450-114">ファイル。読み取り、ファイルの読み取り/書き込み。すべてのファイル。</span><span class="sxs-lookup"><span data-stu-id="ae450-114">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="ae450-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ae450-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae450-116">ファイル。読み取り、ファイルの読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="ae450-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="ae450-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ae450-117">Application</span></span>                            | <span data-ttu-id="ae450-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae450-118">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="ae450-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ae450-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/preview
POST /groups/{groupId}/drive/items/{itemId}/preview
POST /me/drive/items/{itemId}/preview
POST /sites/{siteId}/drive/items/{itemId}/preview
POST /users/{userId}/drive/items/{itemId}/preview
POST /shares/{shareId}/driveItem/preview
```

## <a name="request-body"></a><span data-ttu-id="ae450-120">要求本文</span><span class="sxs-lookup"><span data-stu-id="ae450-120">Request body</span></span>

<span data-ttu-id="ae450-121">要求の本文は、アプリケーションが要求している埋め込み可能な URL のプロパティを定義します。</span><span class="sxs-lookup"><span data-stu-id="ae450-121">The body of the request defines properties of the embeddable URL your application is requesting.</span></span>
<span data-ttu-id="ae450-122">要求は、次のプロパティを含む JSON オブジェクトである必要があります。</span><span class="sxs-lookup"><span data-stu-id="ae450-122">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="ae450-123">名前</span><span class="sxs-lookup"><span data-stu-id="ae450-123">Name</span></span>      |  <span data-ttu-id="ae450-124">型</span><span class="sxs-lookup"><span data-stu-id="ae450-124">Type</span></span>         | <span data-ttu-id="ae450-125">説明</span><span class="sxs-lookup"><span data-stu-id="ae450-125">Description</span></span>
|:------------|:--------------|:-----------------------------------------------
| <span data-ttu-id="ae450-126">page</span><span class="sxs-lookup"><span data-stu-id="ae450-126">page</span></span>        | <span data-ttu-id="ae450-127">文字列または数値</span><span class="sxs-lookup"><span data-stu-id="ae450-127">string/number</span></span> | <span data-ttu-id="ae450-128">省略可能。</span><span class="sxs-lookup"><span data-stu-id="ae450-128">Optional.</span></span> <span data-ttu-id="ae450-129">開始するドキュメントのページ番号 (該当する場合)。</span><span class="sxs-lookup"><span data-stu-id="ae450-129">Page number of document to start at, if applicable.</span></span> <span data-ttu-id="ae450-130">ZIP などのファイルの種類に関する今後のユースケースの文字列として指定されます。</span><span class="sxs-lookup"><span data-stu-id="ae450-130">Specified as string for future use cases around file types such as ZIP.</span></span>
| <span data-ttu-id="ae450-131">ズーム</span><span class="sxs-lookup"><span data-stu-id="ae450-131">zoom</span></span>        | <span data-ttu-id="ae450-132">number</span><span class="sxs-lookup"><span data-stu-id="ae450-132">number</span></span>        | <span data-ttu-id="ae450-133">省略可能。</span><span class="sxs-lookup"><span data-stu-id="ae450-133">Optional.</span></span> <span data-ttu-id="ae450-134">必要に応じて、開始するズームレベルを表示します。</span><span class="sxs-lookup"><span data-stu-id="ae450-134">Zoom level to start at, if applicable.</span></span>

## <a name="response"></a><span data-ttu-id="ae450-135">応答</span><span class="sxs-lookup"><span data-stu-id="ae450-135">Response</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

<span data-ttu-id="ae450-136">応答は、次のプロパティを含む JSON オブジェクトになります。</span><span class="sxs-lookup"><span data-stu-id="ae450-136">The response will be a JSON object containing the following properties:</span></span>

| <span data-ttu-id="ae450-137">名前</span><span class="sxs-lookup"><span data-stu-id="ae450-137">Name</span></span>           | <span data-ttu-id="ae450-138">型</span><span class="sxs-lookup"><span data-stu-id="ae450-138">Type</span></span>   | <span data-ttu-id="ae450-139">説明</span><span class="sxs-lookup"><span data-stu-id="ae450-139">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="ae450-140">getUrl</span><span class="sxs-lookup"><span data-stu-id="ae450-140">getUrl</span></span>         | <span data-ttu-id="ae450-141">string</span><span class="sxs-lookup"><span data-stu-id="ae450-141">string</span></span> | <span data-ttu-id="ae450-142">HTTP GET (iframes など) を使用した埋め込みに適した URL</span><span class="sxs-lookup"><span data-stu-id="ae450-142">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="ae450-143">postUrl</span><span class="sxs-lookup"><span data-stu-id="ae450-143">postUrl</span></span>        | <span data-ttu-id="ae450-144">string</span><span class="sxs-lookup"><span data-stu-id="ae450-144">string</span></span> | <span data-ttu-id="ae450-145">HTTP POST (form post、JS など) を使用した埋め込みに適した URL</span><span class="sxs-lookup"><span data-stu-id="ae450-145">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="ae450-146">postParameters</span><span class="sxs-lookup"><span data-stu-id="ae450-146">postParameters</span></span> | <span data-ttu-id="ae450-147">string</span><span class="sxs-lookup"><span data-stu-id="ae450-147">string</span></span> | <span data-ttu-id="ae450-148">PostUrl を使用する場合に含める POST パラメーター</span><span class="sxs-lookup"><span data-stu-id="ae450-148">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="ae450-149">指定したオプションの embed サポートの現在の状態に応じて、getUrl、postUrl、または both のどちらかが返される場合があります。</span><span class="sxs-lookup"><span data-stu-id="ae450-149">Either getUrl, postUrl, or both might be returned depending on the current state of embed support for the specified options.</span></span>

<span data-ttu-id="ae450-150">postParameters はとして`application/x-www-form-urlencoded`書式設定された文字列です。 postparameters への投稿を実行する場合は、コンテンツタイプを適宜設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ae450-150">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="ae450-151">次に例を示します。</span><span class="sxs-lookup"><span data-stu-id="ae450-151">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="pagezoom"></a><span data-ttu-id="ae450-152">ページ/ズーム</span><span class="sxs-lookup"><span data-stu-id="ae450-152">Page/zoom</span></span>

<span data-ttu-id="ae450-153">[ページ] と [ズーム] オプションは、すべてのプレビューアプリで使用できるわけではありませんが、プレビューアプリがサポートしている場合は適用されます。</span><span class="sxs-lookup"><span data-stu-id="ae450-153">The 'page' and 'zoom' options may not be available for all preview apps, but will be applied if the preview app supports it.</span></span>
