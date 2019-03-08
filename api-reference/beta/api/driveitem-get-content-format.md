---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 他の形式に変換する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: c3761525d0acbd5613a71519d9ebd56ab8475f03
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481826"
---
# <a name="download-a-file-in-another-format"></a><span data-ttu-id="efbad-102">別の形式でファイルをダウンロードする</span><span class="sxs-lookup"><span data-stu-id="efbad-102">Download a file in another format</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="efbad-103">この API を使用して、アイテムのコンテンツを特定の形式で取得します。</span><span class="sxs-lookup"><span data-stu-id="efbad-103">Use this API to retrieve the contents of an item in a specific format.</span></span>
<span data-ttu-id="efbad-104">すべてのファイルがすべての形式に変換できるわけではありません。</span><span class="sxs-lookup"><span data-stu-id="efbad-104">Not all files can be converted into all formats.</span></span>

<span data-ttu-id="efbad-105">アイテムを元の形式でダウンロードするには、「[アイテムのコンテンツをダウンロード](driveitem-get-content.md)する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="efbad-105">To download the item in its original format, see [download an item's contents](driveitem-get-content.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="efbad-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="efbad-106">Prerequisites</span></span>

<span data-ttu-id="efbad-107">この API を呼び出すには、ユーザーがアプリケーションに対して、アプリが変換するファイルへの読み取りアクセス権を付与している必要があります。</span><span class="sxs-lookup"><span data-stu-id="efbad-107">To call this API, the user must have granted the application read access to the file the app wishes to convert.</span></span>

## <a name="http-request"></a><span data-ttu-id="efbad-108">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="efbad-108">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drive/items/{item-id}/content?format={format}
GET /drive/root:/{path and filename}:/content?format={format}
```

## <a name="query-parameters"></a><span data-ttu-id="efbad-109">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="efbad-109">Query parameters</span></span>

| <span data-ttu-id="efbad-110">パラメーター</span><span class="sxs-lookup"><span data-stu-id="efbad-110">Parameter</span></span>      | <span data-ttu-id="efbad-111">型</span><span class="sxs-lookup"><span data-stu-id="efbad-111">Type</span></span>  | <span data-ttu-id="efbad-112">説明</span><span class="sxs-lookup"><span data-stu-id="efbad-112">Description</span></span>                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="efbad-113">_format_</span><span class="sxs-lookup"><span data-stu-id="efbad-113">_format_</span></span>  | <span data-ttu-id="efbad-114">string</span><span class="sxs-lookup"><span data-stu-id="efbad-114">string</span></span> | <span data-ttu-id="efbad-115">アイテムのコンテンツをダウンロードする形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="efbad-115">Specify the format the item's content should be downloaded as.</span></span> |


<span data-ttu-id="efbad-116">**format**パラメーターには、次の値が有効です。</span><span class="sxs-lookup"><span data-stu-id="efbad-116">The following values are valid for the **format** parameter:</span></span>

| <span data-ttu-id="efbad-117">値</span><span class="sxs-lookup"><span data-stu-id="efbad-117">Value</span></span> | <span data-ttu-id="efbad-118">説明</span><span class="sxs-lookup"><span data-stu-id="efbad-118">Description</span></span>                        | <span data-ttu-id="efbad-119">サポートされているソースの拡張子</span><span class="sxs-lookup"><span data-stu-id="efbad-119">Supported source extensions</span></span>
|:------|:-----------------------------------|---------------------------------
| <span data-ttu-id="efbad-120">glb</span><span class="sxs-lookup"><span data-stu-id="efbad-120">glb</span></span>   | <span data-ttu-id="efbad-121">アイテムを GLB 形式に変換します。</span><span class="sxs-lookup"><span data-stu-id="efbad-121">Converts the item into GLB format</span></span>  | <span data-ttu-id="efbad-122">クール、fbx、obj、プライ、stl、3mf</span><span class="sxs-lookup"><span data-stu-id="efbad-122">cool, fbx, obj, ply, stl, 3mf</span></span>
| <span data-ttu-id="efbad-123">Html</span><span class="sxs-lookup"><span data-stu-id="efbad-123">html</span></span>  | <span data-ttu-id="efbad-124">アイテムを HTML 形式に変換します。</span><span class="sxs-lookup"><span data-stu-id="efbad-124">Converts the item into HTML format</span></span> | <span data-ttu-id="efbad-125">eml、md、msg</span><span class="sxs-lookup"><span data-stu-id="efbad-125">eml, md, msg</span></span>
| <span data-ttu-id="efbad-126">.jpg</span><span class="sxs-lookup"><span data-stu-id="efbad-126">jpg</span></span>   | <span data-ttu-id="efbad-127">項目を JPG 形式に変換します。</span><span class="sxs-lookup"><span data-stu-id="efbad-127">Converts the item into JPG format</span></span>  | <span data-ttu-id="efbad-128">3g2、3gp、3g2、3gpp、3mf、ai、arw、asf、avi、bas、bash、bat、bmp、c、cbl、cmd、クール、cpp、cr2、crw、cs、css、csv、dcm30、dcm、、.dic、dicm、dicom、dng、doc、.docx、dwg、eml、epi、.eps、epsf、epsi、epub、glb、h、および、heic、heic、htm、html、.ico、icon、java、jfif、jpeg、jpg、js、json、key、log、m2ts、m4a、m4v、markdown、md、mef、mov、movie、、mp4、mp4v、mrw、msg、mts、nef、nrw、ogg、obj、、、、pef、、、pict、、、php、pict、pl、プライ、png、.pot、potm、potx、pps、ppsx、ppsxm、ppt、pptm、.pptx、ps、ps1、psb、psd、py、raw、、rtf、rw1、rw2、sh、sketch、sql、sr2、、、、ts、txt、vb、webm、wma、wmv、xaml、xbm、xcf、xd、xml、xpm、yaml、yml</span><span class="sxs-lookup"><span data-stu-id="efbad-128">3g2, 3gp, 3gp2, 3gpp, 3mf, ai, arw, asf, avi, bas, bash, bat, bmp, c, cbl, cmd, cool, cpp, cr2, crw, cs, css, csv, cur, dcm, dcm30, dic, dicm, dicom, dng, doc, docx, dwg, eml, epi, eps, epsf, epsi, epub, erf, fbx, fppx, gif, glb, h, hcp, heic, heif, htm, html, ico, icon, java, jfif, jpeg, jpg, js, json, key, log, m2ts, m4a, m4v, markdown, md, mef, mov, movie, mp3, mp4, mp4v, mrw, msg, mts, nef, nrw, numbers, obj, odp, odt, ogg, orf, pages, pano, pdf, pef, php, pict, pl, ply, png, pot, potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, ps, ps1, psb, psd, py, raw, rb, rtf, rw1, rw2, sh, sketch, sql, sr2, stl, tif, tiff, ts, txt, vb, webm, wma, wmv, xaml, xbm, xcf, xd, xml, xpm, yaml, yml</span></span>
| <span data-ttu-id="efbad-129">文書</span><span class="sxs-lookup"><span data-stu-id="efbad-129">pdf</span></span>   | <span data-ttu-id="efbad-130">アイテムを PDF 形式に変換します。</span><span class="sxs-lookup"><span data-stu-id="efbad-130">Converts the item into PDF format</span></span>  | <span data-ttu-id="efbad-131">doc、.docx、epub、eml、htm、html、md、msg、odp、ods、odt、pps、ppsx、ppt、.pptx、rtf、tif、tiff、xls、.xlsm、.xlsx</span><span class="sxs-lookup"><span data-stu-id="efbad-131">doc, docx, epub, eml, htm, html, md, msg, odp, ods, odt, pps, ppsx, ppt, pptx, rtf, tif, tiff, xls, xlsm, xlsx</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="efbad-132">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="efbad-132">Optional request headers</span></span>

| <span data-ttu-id="efbad-133">名前</span><span class="sxs-lookup"><span data-stu-id="efbad-133">Name</span></span>            | <span data-ttu-id="efbad-134">値</span><span class="sxs-lookup"><span data-stu-id="efbad-134">Value</span></span>   | <span data-ttu-id="efbad-135">説明</span><span class="sxs-lookup"><span data-stu-id="efbad-135">Description</span></span>                                                                                                                                              |
|:----------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="efbad-136">_if-none-match_</span><span class="sxs-lookup"><span data-stu-id="efbad-136">_if-none-match_</span></span> | <span data-ttu-id="efbad-137">String</span><span class="sxs-lookup"><span data-stu-id="efbad-137">String</span></span>  | <span data-ttu-id="efbad-138">この要求ヘッダーが含まれている場合、指定された eTag (または cTag) がファイルの現在のタグに一致すると、`HTTP 304 Not Modified` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="efbad-138">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="example"></a><span data-ttu-id="efbad-139">例</span><span class="sxs-lookup"><span data-stu-id="efbad-139">Example</span></span>

<!-- { "blockType": "request", "name": "convert-item-content", "scopes": "files.read" } -->

```http
GET /drive/items/{item-id}/content?format={format}
```

## <a name="response"></a><span data-ttu-id="efbad-140">応答</span><span class="sxs-lookup"><span data-stu-id="efbad-140">Response</span></span>

<span data-ttu-id="efbad-141">変換されたファイルの事前認証されたダウンロード URL にリダイレクトする、`302 Found` 応答を返します。</span><span class="sxs-lookup"><span data-stu-id="efbad-141">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the converted file.</span></span>

<span data-ttu-id="efbad-142">変換されたファイルをダウンロードするには、アプリが応答の `Location` ヘッダーに従う必要があります。</span><span class="sxs-lookup"><span data-stu-id="efbad-142">To download the converted file, your app must follow the `Location` header in the response.</span></span>

<span data-ttu-id="efbad-143">事前認証された URL は、短期間 (数分) のみ有効で、アクセスのために `Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="efbad-143">Pre-authenticated URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to access.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

### <a name="error-responses"></a><span data-ttu-id="efbad-144">エラー応答</span><span class="sxs-lookup"><span data-stu-id="efbad-144">Error responses</span></span>

<span data-ttu-id="efbad-145">エラーがどのように返されるかについては、「[エラー応答][error-response]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="efbad-145">See [Error Responses][error-response] for more information about how errors are returned.</span></span>

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
    "Error: /api-reference/beta/api/driveitem-get-content-format.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
