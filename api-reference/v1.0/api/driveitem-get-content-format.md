---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 他の形式に変換する
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 2470f3f8176b7b7b5b79757f6f0feb54eae6c3a8
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35445437"
---
# <a name="download-a-file-in-another-format"></a><span data-ttu-id="107d1-102">別の形式でファイルをダウンロードする</span><span class="sxs-lookup"><span data-stu-id="107d1-102">Download a file in another format</span></span>

<span data-ttu-id="107d1-103">この API を使用して、アイテムのコンテンツを特定の形式で取得します。</span><span class="sxs-lookup"><span data-stu-id="107d1-103">Use this API to retrieve the contents of an item in a specific format.</span></span>
<span data-ttu-id="107d1-104">すべてのファイルがすべての形式に変換できるわけではありません。</span><span class="sxs-lookup"><span data-stu-id="107d1-104">Not all files can be converted into all formats.</span></span>

<span data-ttu-id="107d1-105">アイテムを元の形式でダウンロードするには、「[アイテムのコンテンツをダウンロードする](driveitem-get-content.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="107d1-105">To download the item in its original format, see [download an item's contents](driveitem-get-content.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="107d1-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="107d1-106">Prerequisites</span></span>

<span data-ttu-id="107d1-107">この API を呼び出すには、ユーザーがアプリケーションに対して、アプリが変換するファイルへの読み取りアクセス権を付与している必要があります。</span><span class="sxs-lookup"><span data-stu-id="107d1-107">To call this API, the user must have granted the application read access to the file the app wishes to convert.</span></span>

## <a name="http-request"></a><span data-ttu-id="107d1-108">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="107d1-108">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drive/items/{item-id}/content?format={format}
GET /drive/root:/{path and filename}:/content?format={format}
```

## <a name="query-parameters"></a><span data-ttu-id="107d1-109">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="107d1-109">Query parameters</span></span>

| <span data-ttu-id="107d1-110">パラメーター</span><span class="sxs-lookup"><span data-stu-id="107d1-110">Parameter</span></span>      | <span data-ttu-id="107d1-111">型</span><span class="sxs-lookup"><span data-stu-id="107d1-111">Type</span></span>  | <span data-ttu-id="107d1-112">説明</span><span class="sxs-lookup"><span data-stu-id="107d1-112">Description</span></span>                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="107d1-113">_format_</span><span class="sxs-lookup"><span data-stu-id="107d1-113">_format_</span></span>  | <span data-ttu-id="107d1-114">string</span><span class="sxs-lookup"><span data-stu-id="107d1-114">string</span></span> | <span data-ttu-id="107d1-115">アイテムのコンテンツをダウンロードする形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="107d1-115">Specify the format the item's content should be downloaded as.</span></span> |


### <a name="format-options"></a><span data-ttu-id="107d1-116">形式のオプション</span><span class="sxs-lookup"><span data-stu-id="107d1-116">Format options</span></span>

<span data-ttu-id="107d1-117">**format** パラメーターには次の値を指定できます。</span><span class="sxs-lookup"><span data-stu-id="107d1-117">The following values are valid for the **format** parameter:</span></span>

| <span data-ttu-id="107d1-118">形式の値</span><span class="sxs-lookup"><span data-stu-id="107d1-118">Format value</span></span> | <span data-ttu-id="107d1-119">説明</span><span class="sxs-lookup"><span data-stu-id="107d1-119">Description</span></span>                        | <span data-ttu-id="107d1-120">サポートされているソースの拡張子</span><span class="sxs-lookup"><span data-stu-id="107d1-120">Supported source extensions</span></span>
|:-------------|:-----------------------------------|----------------------------
| <span data-ttu-id="107d1-121">pdf</span><span class="sxs-lookup"><span data-stu-id="107d1-121">pdf</span></span>          | <span data-ttu-id="107d1-122">アイテムを PDF 形式に変換します。</span><span class="sxs-lookup"><span data-stu-id="107d1-122">Converts the item into PDF format.</span></span> | <span data-ttu-id="107d1-123">csv、doc、docx、odp、ods、odt、pot、potm、potx、pps、ppsx、ppsxm、ppt、pptm、pptx、rtf、xls、xlsx</span><span class="sxs-lookup"><span data-stu-id="107d1-123">csv, doc, docx, odp, ods, odt, pot, potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, rtf, xls, xlsx</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="107d1-124">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="107d1-124">Optional request headers</span></span>

| <span data-ttu-id="107d1-125">名前</span><span class="sxs-lookup"><span data-stu-id="107d1-125">Name</span></span>            | <span data-ttu-id="107d1-126">値</span><span class="sxs-lookup"><span data-stu-id="107d1-126">Value</span></span>   | <span data-ttu-id="107d1-127">説明</span><span class="sxs-lookup"><span data-stu-id="107d1-127">Description</span></span>                                                                                                                                              |
|:----------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="107d1-128">_if-none-match_</span><span class="sxs-lookup"><span data-stu-id="107d1-128">_if-none-match_</span></span> | <span data-ttu-id="107d1-129">String</span><span class="sxs-lookup"><span data-stu-id="107d1-129">String</span></span>  | <span data-ttu-id="107d1-130">この要求ヘッダーが含まれている場合、指定された eTag (または cTag) がファイルの現在のタグに一致すると、`HTTP 304 Not Modified` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="107d1-130">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="example"></a><span data-ttu-id="107d1-131">例</span><span class="sxs-lookup"><span data-stu-id="107d1-131">Example</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="107d1-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="107d1-132">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "convert-item-content", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/content?format={format}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="107d1-133">C#</span><span class="sxs-lookup"><span data-stu-id="107d1-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/convert-item-content-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="107d1-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="107d1-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/convert-item-content-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="107d1-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="107d1-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/convert-item-content-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="107d1-136">応答</span><span class="sxs-lookup"><span data-stu-id="107d1-136">Response</span></span>

<span data-ttu-id="107d1-137">変換されたファイルの事前認証されたダウンロード URL にリダイレクトする、`302 Found` 応答を返します。</span><span class="sxs-lookup"><span data-stu-id="107d1-137">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the converted file.</span></span>

<span data-ttu-id="107d1-138">変換されたファイルをダウンロードするには、アプリが応答の `Location` ヘッダーに従う必要があります。</span><span class="sxs-lookup"><span data-stu-id="107d1-138">To download the converted file, your app must follow the `Location` header in the response.</span></span>

<span data-ttu-id="107d1-139">事前認証された URL は、短期間 (数分) のみ有効で、アクセスのために `Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="107d1-139">Pre-authenticated URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to access.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

### <a name="error-responses"></a><span data-ttu-id="107d1-140">エラー応答</span><span class="sxs-lookup"><span data-stu-id="107d1-140">Error responses</span></span>

<span data-ttu-id="107d1-141">エラーがどのように返されるかの詳細については、「[エラー応答][error-response]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="107d1-141">See [Error Responses][error-response] for more information about how errors are returned.</span></span>

[error-response]: /graph/errors
[file-facet]: ../resources/file.md

<!-- {
  "type": "#page.annotation",
  "description": "Convert the contents of an item in OneDrive to a different format.",
  "keywords": "convert,pdf,convert to pdf",
  "section": "documentation",
  "tocPath": "Items/Download formats",
  "suppressions": [
  ]
} -->
