---
author: JeremyKelley
description: この API を使用して、アイテムのコンテンツを特定の形式で取得します。
ms.date: 09/10/2017
title: 他の形式に変換する
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 47dc10a1292ab4b75f4bd5712b1d0deb9df1b44b
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36416801"
---
# <a name="download-a-file-in-another-format"></a><span data-ttu-id="60e23-103">別の形式でファイルをダウンロードする</span><span class="sxs-lookup"><span data-stu-id="60e23-103">Download a file in another format</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60e23-104">この API を使用して、アイテムのコンテンツを特定の形式で取得します。</span><span class="sxs-lookup"><span data-stu-id="60e23-104">Use this API to retrieve the contents of an item in a specific format.</span></span>
<span data-ttu-id="60e23-105">すべてのファイルがすべての形式に変換できるわけではありません。</span><span class="sxs-lookup"><span data-stu-id="60e23-105">Not all files can be converted into all formats.</span></span>

<span data-ttu-id="60e23-106">アイテムを元の形式でダウンロードするには、「[アイテムのコンテンツをダウンロードする](driveitem-get-content.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="60e23-106">To download the item in its original format, see [download an item's contents](driveitem-get-content.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="60e23-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="60e23-107">Prerequisites</span></span>

<span data-ttu-id="60e23-108">この API を呼び出すには、ユーザーがアプリケーションに対して、アプリが変換するファイルへの読み取りアクセス権を付与している必要があります。</span><span class="sxs-lookup"><span data-stu-id="60e23-108">To call this API, the user must have granted the application read access to the file the app wishes to convert.</span></span>

## <a name="http-request"></a><span data-ttu-id="60e23-109">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="60e23-109">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drive/items/{item-id}/content?format={format}
GET /drive/root:/{path and filename}:/content?format={format}
```

## <a name="query-parameters"></a><span data-ttu-id="60e23-110">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="60e23-110">Query parameters</span></span>

| <span data-ttu-id="60e23-111">パラメーター</span><span class="sxs-lookup"><span data-stu-id="60e23-111">Parameter</span></span>      | <span data-ttu-id="60e23-112">型</span><span class="sxs-lookup"><span data-stu-id="60e23-112">Type</span></span>  | <span data-ttu-id="60e23-113">説明</span><span class="sxs-lookup"><span data-stu-id="60e23-113">Description</span></span>                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="60e23-114">_format_</span><span class="sxs-lookup"><span data-stu-id="60e23-114">_format_</span></span>  | <span data-ttu-id="60e23-115">string</span><span class="sxs-lookup"><span data-stu-id="60e23-115">string</span></span> | <span data-ttu-id="60e23-116">アイテムのコンテンツをダウンロードする形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="60e23-116">Specify the format the item's content should be downloaded as.</span></span> |


<span data-ttu-id="60e23-117">**format** パラメーターには次の値を指定できます。</span><span class="sxs-lookup"><span data-stu-id="60e23-117">The following values are valid for the **format** parameter:</span></span>

| <span data-ttu-id="60e23-118">値</span><span class="sxs-lookup"><span data-stu-id="60e23-118">Value</span></span> | <span data-ttu-id="60e23-119">説明</span><span class="sxs-lookup"><span data-stu-id="60e23-119">Description</span></span>                        | <span data-ttu-id="60e23-120">サポートされているソースの拡張子</span><span class="sxs-lookup"><span data-stu-id="60e23-120">Supported source extensions</span></span>
|:------|:-----------------------------------|---------------------------------
| <span data-ttu-id="60e23-121">glb</span><span class="sxs-lookup"><span data-stu-id="60e23-121">glb</span></span>   | <span data-ttu-id="60e23-122">アイテムを GLB 形式に変換します。</span><span class="sxs-lookup"><span data-stu-id="60e23-122">Converts the item into GLB format</span></span>  | <span data-ttu-id="60e23-123">クール、fbx、obj、プライ、stl、3mf</span><span class="sxs-lookup"><span data-stu-id="60e23-123">cool, fbx, obj, ply, stl, 3mf</span></span>
| <span data-ttu-id="60e23-124">Html</span><span class="sxs-lookup"><span data-stu-id="60e23-124">html</span></span>  | <span data-ttu-id="60e23-125">アイテムを HTML 形式に変換します。</span><span class="sxs-lookup"><span data-stu-id="60e23-125">Converts the item into HTML format</span></span> | <span data-ttu-id="60e23-126">eml、md、msg</span><span class="sxs-lookup"><span data-stu-id="60e23-126">eml, md, msg</span></span>
| <span data-ttu-id="60e23-127">.jpg</span><span class="sxs-lookup"><span data-stu-id="60e23-127">jpg</span></span>   | <span data-ttu-id="60e23-128">項目を JPG 形式に変換します。</span><span class="sxs-lookup"><span data-stu-id="60e23-128">Converts the item into JPG format</span></span>  | <span data-ttu-id="60e23-129">3g2、3gp、3g2、3gpp、3mf、ai、arw、asf、avi、bas、bash、bat、bmp、c、cbl、cmd、クール、cpp、cr2、crw、cs、css、csv、dcm30、dcm、、.dic、dicm、dicom、dng、doc、.docx、dwg、eml、epi、.eps、epsf、epsi、epub、glb、h、および、heic、heic、htm、html、.ico、icon、java、jfif、jpeg、jpg、js、json、key、log、m2ts、m4a、m4v、markdown、md、mef、mov、movie、、mp4、mp4v、mrw、msg、mts、nef、nrw、ogg、obj、、、、pef、、、pict、、、php、pict、pl、プライ、png、.pot、potm、potx、pps、ppsx、ppsxm、ppt、pptm、.pptx、ps、ps1、psb、psd、py、raw、、rtf、rw1、rw2、sh、sketch、sql、sr2、、、、ts、txt、vb、webm、wma、wmv、xaml、xbm、xcf、xd、xml、xpm、yaml、yml</span><span class="sxs-lookup"><span data-stu-id="60e23-129">3g2, 3gp, 3gp2, 3gpp, 3mf, ai, arw, asf, avi, bas, bash, bat, bmp, c, cbl, cmd, cool, cpp, cr2, crw, cs, css, csv, cur, dcm, dcm30, dic, dicm, dicom, dng, doc, docx, dwg, eml, epi, eps, epsf, epsi, epub, erf, fbx, fppx, gif, glb, h, hcp, heic, heif, htm, html, ico, icon, java, jfif, jpeg, jpg, js, json, key, log, m2ts, m4a, m4v, markdown, md, mef, mov, movie, mp3, mp4, mp4v, mrw, msg, mts, nef, nrw, numbers, obj, odp, odt, ogg, orf, pages, pano, pdf, pef, php, pict, pl, ply, png, pot, potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, ps, ps1, psb, psd, py, raw, rb, rtf, rw1, rw2, sh, sketch, sql, sr2, stl, tif, tiff, ts, txt, vb, webm, wma, wmv, xaml, xbm, xcf, xd, xml, xpm, yaml, yml</span></span>
| <span data-ttu-id="60e23-130">pdf</span><span class="sxs-lookup"><span data-stu-id="60e23-130">pdf</span></span>   | <span data-ttu-id="60e23-131">アイテムを PDF 形式に変換します。</span><span class="sxs-lookup"><span data-stu-id="60e23-131">Converts the item into PDF format</span></span>  | <span data-ttu-id="60e23-132">doc、.docx、epub、eml、htm、html、md、msg、odp、ods、odt、pps、ppsx、ppt、.pptx、rtf、tif、tiff、xls、.xlsm、.xlsx</span><span class="sxs-lookup"><span data-stu-id="60e23-132">doc, docx, epub, eml, htm, html, md, msg, odp, ods, odt, pps, ppsx, ppt, pptx, rtf, tif, tiff, xls, xlsm, xlsx</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="60e23-133">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="60e23-133">Optional request headers</span></span>

| <span data-ttu-id="60e23-134">名前</span><span class="sxs-lookup"><span data-stu-id="60e23-134">Name</span></span>            | <span data-ttu-id="60e23-135">値</span><span class="sxs-lookup"><span data-stu-id="60e23-135">Value</span></span>   | <span data-ttu-id="60e23-136">説明</span><span class="sxs-lookup"><span data-stu-id="60e23-136">Description</span></span>                                                                                                                                              |
|:----------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="60e23-137">_if-none-match_</span><span class="sxs-lookup"><span data-stu-id="60e23-137">_if-none-match_</span></span> | <span data-ttu-id="60e23-138">String</span><span class="sxs-lookup"><span data-stu-id="60e23-138">String</span></span>  | <span data-ttu-id="60e23-139">この要求ヘッダーが含まれている場合、指定された eTag (または cTag) がファイルの現在のタグに一致すると、`HTTP 304 Not Modified` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="60e23-139">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="example"></a><span data-ttu-id="60e23-140">例</span><span class="sxs-lookup"><span data-stu-id="60e23-140">Example</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="60e23-141">プロトコル</span><span class="sxs-lookup"><span data-stu-id="60e23-141">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "convert-item-content", "scopes": "files.read" } -->

```http
GET /drive/items/{item-id}/content?format={format}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="60e23-142">C#</span><span class="sxs-lookup"><span data-stu-id="60e23-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/convert-item-content-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="60e23-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="60e23-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/convert-item-content-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="60e23-144">目的-C</span><span class="sxs-lookup"><span data-stu-id="60e23-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/convert-item-content-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="60e23-145">応答</span><span class="sxs-lookup"><span data-stu-id="60e23-145">Response</span></span>

<span data-ttu-id="60e23-146">変換されたファイルの事前認証されたダウンロード URL にリダイレクトする、`302 Found` 応答を返します。</span><span class="sxs-lookup"><span data-stu-id="60e23-146">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the converted file.</span></span>

<span data-ttu-id="60e23-147">変換されたファイルをダウンロードするには、アプリが応答の `Location` ヘッダーに従う必要があります。</span><span class="sxs-lookup"><span data-stu-id="60e23-147">To download the converted file, your app must follow the `Location` header in the response.</span></span>

<span data-ttu-id="60e23-148">事前認証された URL は、短期間 (数分) のみ有効で、アクセスのために `Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="60e23-148">Pre-authenticated URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to access.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

### <a name="error-responses"></a><span data-ttu-id="60e23-149">エラー応答</span><span class="sxs-lookup"><span data-stu-id="60e23-149">Error responses</span></span>

<span data-ttu-id="60e23-150">エラーがどのように返されるかについては、「[エラー応答][error-response]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="60e23-150">See [Error Responses][error-response] for more information about how errors are returned.</span></span>

[error-response]: /graph/errors
[file-facet]: ../resources/file.md

<!--
{
  "type": "#page.annotation",
  "description": "Convert the contents of an item in OneDrive to a different format.",
  "keywords": "convert,pdf,convert to pdf",
  "section": "documentation",
  "tocPath": "Items/Download formats",
  "suppressions": [
  ]
}
-->
