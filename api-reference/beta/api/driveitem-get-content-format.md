---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 他の形式に変換する
ms.openlocfilehash: 70558e7c0497c71f620481ff67b7d07cc255cd95
ms.sourcegitcommit: 12c6e82f1417022540e534ebadbd0e8d7fb5abde
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/08/2018
ms.locfileid: "27209720"
---
# <a name="download-a-file-in-another-format"></a><span data-ttu-id="ff5e8-102">別の形式でファイルをダウンロードする</span><span class="sxs-lookup"><span data-stu-id="ff5e8-102">Download a file in another format</span></span>

> <span data-ttu-id="ff5e8-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ff5e8-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ff5e8-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ff5e8-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ff5e8-105">この API を使用して、アイテムのコンテンツを特定の形式で取得します。</span><span class="sxs-lookup"><span data-stu-id="ff5e8-105">Use this API to retrieve the contents of an item in a specific format.</span></span>
<span data-ttu-id="ff5e8-106">すべてのファイルがすべての形式に変換できるわけではありません。</span><span class="sxs-lookup"><span data-stu-id="ff5e8-106">Not all files can be converted into all formats.</span></span>

<span data-ttu-id="ff5e8-107">元の形式でアイテムをダウンロードするには、[アイテムの内容をダウンロードする](driveitem-get-content.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ff5e8-107">To download the item in its original format, see [download an item's contents](driveitem-get-content.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ff5e8-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="ff5e8-108">Prerequisites</span></span>

<span data-ttu-id="ff5e8-109">この API を呼び出すには、ユーザーがアプリケーションに対して、アプリが変換するファイルへの読み取りアクセス権を付与している必要があります。</span><span class="sxs-lookup"><span data-stu-id="ff5e8-109">To call this API, the user must have granted the application read access to the file the app wishes to convert.</span></span>

## <a name="http-request"></a><span data-ttu-id="ff5e8-110">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ff5e8-110">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drive/items/{item-id}/content?format={format}
GET /drive/root:/{path and filename}:/content?format={format}
```

## <a name="query-parameters"></a><span data-ttu-id="ff5e8-111">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ff5e8-111">Query parameters</span></span>

| <span data-ttu-id="ff5e8-112">パラメーター</span><span class="sxs-lookup"><span data-stu-id="ff5e8-112">Parameter</span></span>      | <span data-ttu-id="ff5e8-113">Type</span><span class="sxs-lookup"><span data-stu-id="ff5e8-113">Type</span></span>  | <span data-ttu-id="ff5e8-114">説明</span><span class="sxs-lookup"><span data-stu-id="ff5e8-114">Description</span></span>                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="ff5e8-115">_format_</span><span class="sxs-lookup"><span data-stu-id="ff5e8-115">_format_</span></span>  | <span data-ttu-id="ff5e8-116">文字列</span><span class="sxs-lookup"><span data-stu-id="ff5e8-116">string</span></span> | <span data-ttu-id="ff5e8-117">アイテムのコンテンツをダウンロードする形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="ff5e8-117">Specify the format the item's content should be downloaded as.</span></span> |


<span data-ttu-id="ff5e8-118">次の値は、 **format**パラメーターに有効です。</span><span class="sxs-lookup"><span data-stu-id="ff5e8-118">The following values are valid for the **format** parameter:</span></span>

| <span data-ttu-id="ff5e8-119">値</span><span class="sxs-lookup"><span data-stu-id="ff5e8-119">Value</span></span> | <span data-ttu-id="ff5e8-120">説明</span><span class="sxs-lookup"><span data-stu-id="ff5e8-120">Description</span></span>                        | <span data-ttu-id="ff5e8-121">サポートされているソースの拡張子</span><span class="sxs-lookup"><span data-stu-id="ff5e8-121">Supported source extensions</span></span>
|:------|:-----------------------------------|---------------------------------
| <span data-ttu-id="ff5e8-122">glb</span><span class="sxs-lookup"><span data-stu-id="ff5e8-122">glb</span></span>   | <span data-ttu-id="ff5e8-123">GLB の形式にアイテムを変換します。</span><span class="sxs-lookup"><span data-stu-id="ff5e8-123">Converts the item into GLB format</span></span>  | <span data-ttu-id="ff5e8-124">クール、fbx、obj、プライ、stl、3mf</span><span class="sxs-lookup"><span data-stu-id="ff5e8-124">cool, fbx, obj, ply, stl, 3mf</span></span>
| <span data-ttu-id="ff5e8-125">html</span><span class="sxs-lookup"><span data-stu-id="ff5e8-125">html</span></span>  | <span data-ttu-id="ff5e8-126">項目を HTML 形式に変換します。</span><span class="sxs-lookup"><span data-stu-id="ff5e8-126">Converts the item into HTML format</span></span> | <span data-ttu-id="ff5e8-127">eml, md, メッセージ</span><span class="sxs-lookup"><span data-stu-id="ff5e8-127">eml, md, msg</span></span>
| <span data-ttu-id="ff5e8-128">jpg</span><span class="sxs-lookup"><span data-stu-id="ff5e8-128">jpg</span></span>   | <span data-ttu-id="ff5e8-129">アイテムを JPG 形式に変換します。</span><span class="sxs-lookup"><span data-stu-id="ff5e8-129">Converts the item into JPG format</span></span>  | <span data-ttu-id="ff5e8-130">3 g 2、3 gp、3gp2、3 gpp、3mf、ai、arw、asf、avi、bas、bash、bat、bmp、c、cbl、cmd、冷却、cpp、cr2、crw、cs、css、csv、cur、dcm、dcm30、dic、dicm、dicom、dng、doc、docx、dwg、eml、epi、eps、epsf、epsi、epub 形式、erf、fbx、fppx、gif、glb、h、hcp、heic、heif、htm、html、ico、アイコン、java、欠落、jpeg、jpg、js、json、キー、ログ、m2ts、m4a、m4v、値下げ、md、mef、mov、ビデオ、mp3、mp4、mp4v、mrw、msg、mts、nef、nrw、番号、obj、odp、密接に関連、ogg、orf、ページ、pano、pdf、pef、php、pict、pl、プライ、png、ポット、potm、potx、pps、ppsx、ppsxm、ppt、pptm、pptx、ps、ps1、psb、psd、py、生の、rb、rtf 形式、rw1、rw2、sh では、スケッチ、sql、sr2、stl、tif、tiff、ts、txt、vb、webm、wma、wmv、xaml、xbm、xcf、xd、xml、xpm、yaml、yml</span><span class="sxs-lookup"><span data-stu-id="ff5e8-130">3g2, 3gp, 3gp2, 3gpp, 3mf, ai, arw, asf, avi, bas, bash, bat, bmp, c, cbl, cmd, cool, cpp, cr2, crw, cs, css, csv, cur, dcm, dcm30, dic, dicm, dicom, dng, doc, docx, dwg, eml, epi, eps, epsf, epsi, epub, erf, fbx, fppx, gif, glb, h, hcp, heic, heif, htm, html, ico, icon, java, jfif, jpeg, jpg, js, json, key, log, m2ts, m4a, m4v, markdown, md, mef, mov, movie, mp3, mp4, mp4v, mrw, msg, mts, nef, nrw, numbers, obj, odp, odt, ogg, orf, pages, pano, pdf, pef, php, pict, pl, ply, png, pot, potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, ps, ps1, psb, psd, py, raw, rb, rtf, rw1, rw2, sh, sketch, sql, sr2, stl, tif, tiff, ts, txt, vb, webm, wma, wmv, xaml, xbm, xcf, xd, xml, xpm, yaml, yml</span></span>
| <span data-ttu-id="ff5e8-131">pdf</span><span class="sxs-lookup"><span data-stu-id="ff5e8-131">pdf</span></span>   | <span data-ttu-id="ff5e8-132">項目を PDF 形式に変換します。</span><span class="sxs-lookup"><span data-stu-id="ff5e8-132">Converts the item into PDF format</span></span>  | <span data-ttu-id="ff5e8-133">doc、docx、epub 形式、eml、htm、html、md、メッセージ、odp、ods、密接に関連、pps、ppsx、ppt、pptx、rtf 形式、tif、tiff、xls、xlsm、xlsx</span><span class="sxs-lookup"><span data-stu-id="ff5e8-133">doc, docx, epub, eml, htm, html, md, msg, odp, ods, odt, pps, ppsx, ppt, pptx, rtf, tif, tiff, xls, xlsm, xlsx</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="ff5e8-134">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ff5e8-134">Optional request headers</span></span>

| <span data-ttu-id="ff5e8-135">名前</span><span class="sxs-lookup"><span data-stu-id="ff5e8-135">Name</span></span>            | <span data-ttu-id="ff5e8-136">値</span><span class="sxs-lookup"><span data-stu-id="ff5e8-136">Value</span></span>   | <span data-ttu-id="ff5e8-137">説明</span><span class="sxs-lookup"><span data-stu-id="ff5e8-137">Description</span></span>                                                                                                                                              |
|:----------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="ff5e8-138">_if-none-match_</span><span class="sxs-lookup"><span data-stu-id="ff5e8-138">_if-none-match_</span></span> | <span data-ttu-id="ff5e8-139">String</span><span class="sxs-lookup"><span data-stu-id="ff5e8-139">String</span></span>  | <span data-ttu-id="ff5e8-140">この要求ヘッダーが含まれている場合、指定された eTag (または cTag) がファイルの現在のタグに一致すると、`HTTP 304 Not Modified` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="ff5e8-140">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="example"></a><span data-ttu-id="ff5e8-141">例</span><span class="sxs-lookup"><span data-stu-id="ff5e8-141">Example</span></span>

<!-- { "blockType": "request", "name": "convert-item-content", "scopes": "files.read" } -->

```http
GET /drive/items/{item-id}/content?format={format}
```

## <a name="response"></a><span data-ttu-id="ff5e8-142">応答</span><span class="sxs-lookup"><span data-stu-id="ff5e8-142">Response</span></span>

<span data-ttu-id="ff5e8-143">変換されたファイルの事前認証されたダウンロード URL にリダイレクトする、`302 Found` 応答を返します。</span><span class="sxs-lookup"><span data-stu-id="ff5e8-143">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the converted file.</span></span>

<span data-ttu-id="ff5e8-144">変換されたファイルをダウンロードするには、アプリが応答の `Location` ヘッダーに従う必要があります。</span><span class="sxs-lookup"><span data-stu-id="ff5e8-144">To download the converted file, your app must follow the `Location` header in the response.</span></span>

<span data-ttu-id="ff5e8-145">事前認証された URL は、短期間 (数分) のみ有効で、アクセスのために `Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="ff5e8-145">Pre-authenticated URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to access.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

### <a name="error-responses"></a><span data-ttu-id="ff5e8-146">エラー応答</span><span class="sxs-lookup"><span data-stu-id="ff5e8-146">Error responses</span></span>

<span data-ttu-id="ff5e8-147">エラーがどのように返されるかについては、「[エラー応答][error-response]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ff5e8-147">See [Error Responses][error-response] for more information about how errors are returned.</span></span>

[error-response]: /graph/errors
[file-facet]: ../resources/file.md

<!-- {
  "type": "#page.annotation",
  "description": "Convert the contents of an item in OneDrive to a different format.",
  "keywords": "convert,pdf,convert to pdf",
  "section": "documentation",
  "tocPath": "Items/Download formats"
} -->