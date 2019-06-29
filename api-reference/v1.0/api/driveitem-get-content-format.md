---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 他の形式に変換する
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: e0486012bbc9b4ba3fe019f69872dbdf8ab9724b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35279081"
---
# <a name="download-a-file-in-another-format"></a><span data-ttu-id="e12a8-102">別の形式でファイルをダウンロードする</span><span class="sxs-lookup"><span data-stu-id="e12a8-102">Download a file in another format</span></span>

<span data-ttu-id="e12a8-103">この API を使用して、アイテムのコンテンツを特定の形式で取得します。</span><span class="sxs-lookup"><span data-stu-id="e12a8-103">Use this API to retrieve the contents of an item in a specific format.</span></span>
<span data-ttu-id="e12a8-104">すべてのファイルがすべての形式に変換できるわけではありません。</span><span class="sxs-lookup"><span data-stu-id="e12a8-104">Not all files can be converted into all formats.</span></span>

<span data-ttu-id="e12a8-105">アイテムを元の形式でダウンロードするには、「[アイテムのコンテンツをダウンロードする](driveitem-get-content.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e12a8-105">To download the item in its original format, see [download an item's contents](driveitem-get-content.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e12a8-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="e12a8-106">Prerequisites</span></span>

<span data-ttu-id="e12a8-107">この API を呼び出すには、ユーザーがアプリケーションに対して、アプリが変換するファイルへの読み取りアクセス権を付与している必要があります。</span><span class="sxs-lookup"><span data-stu-id="e12a8-107">To call this API, the user must have granted the application read access to the file the app wishes to convert.</span></span>

## <a name="http-request"></a><span data-ttu-id="e12a8-108">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e12a8-108">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drive/items/{item-id}/content?format={format}
GET /drive/root:/{path and filename}:/content?format={format}
```

## <a name="query-parameters"></a><span data-ttu-id="e12a8-109">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e12a8-109">Query parameters</span></span>

| <span data-ttu-id="e12a8-110">パラメーター</span><span class="sxs-lookup"><span data-stu-id="e12a8-110">Parameter</span></span>      | <span data-ttu-id="e12a8-111">型</span><span class="sxs-lookup"><span data-stu-id="e12a8-111">Type</span></span>  | <span data-ttu-id="e12a8-112">説明</span><span class="sxs-lookup"><span data-stu-id="e12a8-112">Description</span></span>                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="e12a8-113">_format_</span><span class="sxs-lookup"><span data-stu-id="e12a8-113">_format_</span></span>  | <span data-ttu-id="e12a8-114">string</span><span class="sxs-lookup"><span data-stu-id="e12a8-114">string</span></span> | <span data-ttu-id="e12a8-115">アイテムのコンテンツをダウンロードする形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="e12a8-115">Specify the format the item's content should be downloaded as.</span></span> |


### <a name="format-options"></a><span data-ttu-id="e12a8-116">形式のオプション</span><span class="sxs-lookup"><span data-stu-id="e12a8-116">Format options</span></span>

<span data-ttu-id="e12a8-117">**format** パラメーターには次の値を指定できます。</span><span class="sxs-lookup"><span data-stu-id="e12a8-117">The following values are valid for the **format** parameter:</span></span>

| <span data-ttu-id="e12a8-118">形式の値</span><span class="sxs-lookup"><span data-stu-id="e12a8-118">Format value</span></span> | <span data-ttu-id="e12a8-119">説明</span><span class="sxs-lookup"><span data-stu-id="e12a8-119">Description</span></span>                        | <span data-ttu-id="e12a8-120">サポートされているソースの拡張子</span><span class="sxs-lookup"><span data-stu-id="e12a8-120">Supported source extensions</span></span>
|:-------------|:-----------------------------------|----------------------------
| <span data-ttu-id="e12a8-121">pdf</span><span class="sxs-lookup"><span data-stu-id="e12a8-121">pdf</span></span>          | <span data-ttu-id="e12a8-122">アイテムを PDF 形式に変換します。</span><span class="sxs-lookup"><span data-stu-id="e12a8-122">Converts the item into PDF format.</span></span> | <span data-ttu-id="e12a8-123">csv、doc、docx、odp、ods、odt、pot、potm、potx、pps、ppsx、ppsxm、ppt、pptm、pptx、rtf、xls、xlsx</span><span class="sxs-lookup"><span data-stu-id="e12a8-123">csv, doc, docx, odp, ods, odt, pot, potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, rtf, xls, xlsx</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="e12a8-124">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e12a8-124">Optional request headers</span></span>

| <span data-ttu-id="e12a8-125">名前</span><span class="sxs-lookup"><span data-stu-id="e12a8-125">Name</span></span>            | <span data-ttu-id="e12a8-126">値</span><span class="sxs-lookup"><span data-stu-id="e12a8-126">Value</span></span>   | <span data-ttu-id="e12a8-127">説明</span><span class="sxs-lookup"><span data-stu-id="e12a8-127">Description</span></span>                                                                                                                                              |
|:----------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="e12a8-128">_if-none-match_</span><span class="sxs-lookup"><span data-stu-id="e12a8-128">_if-none-match_</span></span> | <span data-ttu-id="e12a8-129">String</span><span class="sxs-lookup"><span data-stu-id="e12a8-129">String</span></span>  | <span data-ttu-id="e12a8-130">この要求ヘッダーが含まれている場合、指定された eTag (または cTag) がファイルの現在のタグに一致すると、`HTTP 304 Not Modified` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="e12a8-130">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="example"></a><span data-ttu-id="e12a8-131">例</span><span class="sxs-lookup"><span data-stu-id="e12a8-131">Example</span></span>

<!-- { "blockType": "request", "name": "convert-item-content", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/content?format={format}
```

## <a name="response"></a><span data-ttu-id="e12a8-132">応答</span><span class="sxs-lookup"><span data-stu-id="e12a8-132">Response</span></span>

<span data-ttu-id="e12a8-133">変換されたファイルの事前認証されたダウンロード URL にリダイレクトする、`302 Found` 応答を返します。</span><span class="sxs-lookup"><span data-stu-id="e12a8-133">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the converted file.</span></span>

<span data-ttu-id="e12a8-134">変換されたファイルをダウンロードするには、アプリが応答の `Location` ヘッダーに従う必要があります。</span><span class="sxs-lookup"><span data-stu-id="e12a8-134">To download the converted file, your app must follow the `Location` header in the response.</span></span>

<span data-ttu-id="e12a8-135">事前認証された URL は、短期間 (数分) のみ有効で、アクセスのために `Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="e12a8-135">Pre-authenticated URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to access.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e12a8-136">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="e12a8-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e12a8-137">C#</span><span class="sxs-lookup"><span data-stu-id="e12a8-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/convert-item-content-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e12a8-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="e12a8-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/convert-item-content-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e12a8-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e12a8-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/convert-item-content-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="error-responses"></a><span data-ttu-id="e12a8-140">エラー応答</span><span class="sxs-lookup"><span data-stu-id="e12a8-140">Error responses</span></span>

<span data-ttu-id="e12a8-141">エラーがどのように返されるかの詳細については、「[エラー応答][error-response]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e12a8-141">See [Error Responses][error-response] for more information about how errors are returned.</span></span>

[error-response]: /graph/errors
[file-facet]: ../resources/file.md

<!-- {
  "type": "#page.annotation",
  "description": "Convert the contents of an item in OneDrive to a different format.",
  "keywords": "convert,pdf,convert to pdf",
  "section": "documentation",
  "tocPath": "Items/Download formats",
  "suppressions": [
    "Error: /api-reference/v1.0/api/driveitem-get-content-format.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/driveitem-get-content-format.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/driveitem-get-content-format.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
