---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 他の形式に変換する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 66a81e5b97d31bc3308409fdfc7bb72bb95eb854
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260180"
---
# <a name="download-a-file-in-another-format"></a><span data-ttu-id="50d7c-102">別の形式でファイルをダウンロードする</span><span class="sxs-lookup"><span data-stu-id="50d7c-102">Download a file in another format</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50d7c-103">この API を使用して、アイテムのコンテンツを特定の形式で取得します。</span><span class="sxs-lookup"><span data-stu-id="50d7c-103">Use this API to retrieve the contents of an item in a specific format.</span></span>
<span data-ttu-id="50d7c-104">すべてのファイルがすべての形式に変換できるわけではありません。</span><span class="sxs-lookup"><span data-stu-id="50d7c-104">Not all files can be converted into all formats.</span></span>

<span data-ttu-id="50d7c-105">アイテムを元の形式でダウンロードするには、「[アイテムのコンテンツをダウンロードする](driveitem-get-content.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="50d7c-105">To download the item in its original format, see [download an item's contents](driveitem-get-content.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50d7c-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="50d7c-106">Prerequisites</span></span>

<span data-ttu-id="50d7c-107">この API を呼び出すには、ユーザーがアプリケーションに対して、アプリが変換するファイルへの読み取りアクセス権を付与している必要があります。</span><span class="sxs-lookup"><span data-stu-id="50d7c-107">To call this API, the user must have granted the application read access to the file the app wishes to convert.</span></span>

## <a name="http-request"></a><span data-ttu-id="50d7c-108">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="50d7c-108">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drive/items/{item-id}/content?format={format}
GET /drive/root:/{path and filename}:/content?format={format}
```

## <a name="query-parameters"></a><span data-ttu-id="50d7c-109">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="50d7c-109">Query parameters</span></span>

| <span data-ttu-id="50d7c-110">パラメーター</span><span class="sxs-lookup"><span data-stu-id="50d7c-110">Parameter</span></span>      | <span data-ttu-id="50d7c-111">型</span><span class="sxs-lookup"><span data-stu-id="50d7c-111">Type</span></span>  | <span data-ttu-id="50d7c-112">説明</span><span class="sxs-lookup"><span data-stu-id="50d7c-112">Description</span></span>                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="50d7c-113">_format_</span><span class="sxs-lookup"><span data-stu-id="50d7c-113">_format_</span></span>  | <span data-ttu-id="50d7c-114">string</span><span class="sxs-lookup"><span data-stu-id="50d7c-114">string</span></span> | <span data-ttu-id="50d7c-115">アイテムのコンテンツをダウンロードする形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="50d7c-115">Specify the format the item's content should be downloaded as.</span></span> |


<span data-ttu-id="50d7c-116">**format** パラメーターには次の値を指定できます。</span><span class="sxs-lookup"><span data-stu-id="50d7c-116">The following values are valid for the **format** parameter:</span></span>

| <span data-ttu-id="50d7c-117">値</span><span class="sxs-lookup"><span data-stu-id="50d7c-117">Value</span></span> | <span data-ttu-id="50d7c-118">説明</span><span class="sxs-lookup"><span data-stu-id="50d7c-118">Description</span></span>                        | <span data-ttu-id="50d7c-119">サポートされているソースの拡張子</span><span class="sxs-lookup"><span data-stu-id="50d7c-119">Supported source extensions</span></span>
|:------|:-----------------------------------|---------------------------------
| <span data-ttu-id="50d7c-120">glb</span><span class="sxs-lookup"><span data-stu-id="50d7c-120">glb</span></span>   | <span data-ttu-id="50d7c-121">アイテムを GLB 形式に変換します。</span><span class="sxs-lookup"><span data-stu-id="50d7c-121">Converts the item into GLB format</span></span>  | <span data-ttu-id="50d7c-122">クール、fbx、obj、プライ、stl、3mf</span><span class="sxs-lookup"><span data-stu-id="50d7c-122">cool, fbx, obj, ply, stl, 3mf</span></span>
| <span data-ttu-id="50d7c-123">Html</span><span class="sxs-lookup"><span data-stu-id="50d7c-123">html</span></span>  | <span data-ttu-id="50d7c-124">アイテムを HTML 形式に変換します。</span><span class="sxs-lookup"><span data-stu-id="50d7c-124">Converts the item into HTML format</span></span> | <span data-ttu-id="50d7c-125">eml、md、msg</span><span class="sxs-lookup"><span data-stu-id="50d7c-125">eml, md, msg</span></span>
| <span data-ttu-id="50d7c-126">.jpg</span><span class="sxs-lookup"><span data-stu-id="50d7c-126">jpg</span></span>   | <span data-ttu-id="50d7c-127">項目を JPG 形式に変換します。</span><span class="sxs-lookup"><span data-stu-id="50d7c-127">Converts the item into JPG format</span></span>  | <span data-ttu-id="50d7c-128">3g2、3gp、3g2、3gpp、3mf、ai、arw、asf、avi、bas、bash、bat、bmp、c、cbl、cmd、クール、cpp、cr2、crw、cs、css、csv、dcm30、dcm、、.dic、dicm、dicom、dng、doc、.docx、dwg、eml、epi、.eps、epsf、epsi、epub、glb、h、および、heic、heic、htm、html、.ico、icon、java、jfif、jpeg、jpg、js、json、key、log、m2ts、m4a、m4v、markdown、md、mef、mov、movie、、mp4、mp4v、mrw、msg、mts、nef、nrw、ogg、obj、、、、pef、、、pict、、、php、pict、pl、プライ、png、.pot、potm、potx、pps、ppsx、ppsxm、ppt、pptm、.pptx、ps、ps1、psb、psd、py、raw、、rtf、rw1、rw2、sh、sketch、sql、sr2、、、、ts、txt、vb、webm、wma、wmv、xaml、xbm、xcf、xd、xml、xpm、yaml、yml</span><span class="sxs-lookup"><span data-stu-id="50d7c-128">3g2, 3gp, 3gp2, 3gpp, 3mf, ai, arw, asf, avi, bas, bash, bat, bmp, c, cbl, cmd, cool, cpp, cr2, crw, cs, css, csv, cur, dcm, dcm30, dic, dicm, dicom, dng, doc, docx, dwg, eml, epi, eps, epsf, epsi, epub, erf, fbx, fppx, gif, glb, h, hcp, heic, heif, htm, html, ico, icon, java, jfif, jpeg, jpg, js, json, key, log, m2ts, m4a, m4v, markdown, md, mef, mov, movie, mp3, mp4, mp4v, mrw, msg, mts, nef, nrw, numbers, obj, odp, odt, ogg, orf, pages, pano, pdf, pef, php, pict, pl, ply, png, pot, potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, ps, ps1, psb, psd, py, raw, rb, rtf, rw1, rw2, sh, sketch, sql, sr2, stl, tif, tiff, ts, txt, vb, webm, wma, wmv, xaml, xbm, xcf, xd, xml, xpm, yaml, yml</span></span>
| <span data-ttu-id="50d7c-129">pdf</span><span class="sxs-lookup"><span data-stu-id="50d7c-129">pdf</span></span>   | <span data-ttu-id="50d7c-130">アイテムを PDF 形式に変換します。</span><span class="sxs-lookup"><span data-stu-id="50d7c-130">Converts the item into PDF format</span></span>  | <span data-ttu-id="50d7c-131">doc、.docx、epub、eml、htm、html、md、msg、odp、ods、odt、pps、ppsx、ppt、.pptx、rtf、tif、tiff、xls、.xlsm、.xlsx</span><span class="sxs-lookup"><span data-stu-id="50d7c-131">doc, docx, epub, eml, htm, html, md, msg, odp, ods, odt, pps, ppsx, ppt, pptx, rtf, tif, tiff, xls, xlsm, xlsx</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="50d7c-132">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="50d7c-132">Optional request headers</span></span>

| <span data-ttu-id="50d7c-133">名前</span><span class="sxs-lookup"><span data-stu-id="50d7c-133">Name</span></span>            | <span data-ttu-id="50d7c-134">値</span><span class="sxs-lookup"><span data-stu-id="50d7c-134">Value</span></span>   | <span data-ttu-id="50d7c-135">説明</span><span class="sxs-lookup"><span data-stu-id="50d7c-135">Description</span></span>                                                                                                                                              |
|:----------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="50d7c-136">_if-none-match_</span><span class="sxs-lookup"><span data-stu-id="50d7c-136">_if-none-match_</span></span> | <span data-ttu-id="50d7c-137">String</span><span class="sxs-lookup"><span data-stu-id="50d7c-137">String</span></span>  | <span data-ttu-id="50d7c-138">この要求ヘッダーが含まれている場合、指定された eTag (または cTag) がファイルの現在のタグに一致すると、`HTTP 304 Not Modified` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="50d7c-138">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="example"></a><span data-ttu-id="50d7c-139">例</span><span class="sxs-lookup"><span data-stu-id="50d7c-139">Example</span></span>

<!-- { "blockType": "request", "name": "convert-item-content", "scopes": "files.read" } -->

```http
GET /drive/items/{item-id}/content?format={format}
```

## <a name="response"></a><span data-ttu-id="50d7c-140">応答</span><span class="sxs-lookup"><span data-stu-id="50d7c-140">Response</span></span>

<span data-ttu-id="50d7c-141">変換されたファイルの事前認証されたダウンロード URL にリダイレクトする、`302 Found` 応答を返します。</span><span class="sxs-lookup"><span data-stu-id="50d7c-141">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the converted file.</span></span>

<span data-ttu-id="50d7c-142">変換されたファイルをダウンロードするには、アプリが応答の `Location` ヘッダーに従う必要があります。</span><span class="sxs-lookup"><span data-stu-id="50d7c-142">To download the converted file, your app must follow the `Location` header in the response.</span></span>

<span data-ttu-id="50d7c-143">事前認証された URL は、短期間 (数分) のみ有効で、アクセスのために `Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="50d7c-143">Pre-authenticated URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to access.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="50d7c-144">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="50d7c-144">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="50d7c-145">C#</span><span class="sxs-lookup"><span data-stu-id="50d7c-145">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/convert-item-content-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="50d7c-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="50d7c-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/convert-item-content-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="50d7c-147">目的-C</span><span class="sxs-lookup"><span data-stu-id="50d7c-147">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/convert-item-content-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="error-responses"></a><span data-ttu-id="50d7c-148">エラー応答</span><span class="sxs-lookup"><span data-stu-id="50d7c-148">Error responses</span></span>

<span data-ttu-id="50d7c-149">エラーがどのように返されるかについては、「[エラー応答][error-response]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="50d7c-149">See [Error Responses][error-response] for more information about how errors are returned.</span></span>

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
    "Error: /api-reference/beta/api/driveitem-get-content-format.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/driveitem-get-content-format.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveitem-get-content-format.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
