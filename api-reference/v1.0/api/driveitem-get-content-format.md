---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 他の形式に変換する
localization_priority: Priority
ms.prod: sharepoint
description: この API を使用して、アイテムのコンテンツを特定の形式で取得します。
doc_type: apiPageType
ms.openlocfilehash: c2757a64e15865e8278fd38dfed49916dd71d133
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36375080"
---
# <a name="download-a-file-in-another-format"></a><span data-ttu-id="c9079-103">別の形式でファイルをダウンロードする</span><span class="sxs-lookup"><span data-stu-id="c9079-103">Download a file in another format</span></span>

<span data-ttu-id="c9079-104">この API を使用して、アイテムのコンテンツを特定の形式で取得します。</span><span class="sxs-lookup"><span data-stu-id="c9079-104">Use this API to retrieve the contents of an item in a specific format.</span></span>
<span data-ttu-id="c9079-105">すべてのファイルがすべての形式に変換できるわけではありません。</span><span class="sxs-lookup"><span data-stu-id="c9079-105">Not all files can be converted into all formats.</span></span>

<span data-ttu-id="c9079-106">アイテムを元の形式でダウンロードするには、「[アイテムのコンテンツをダウンロードする](driveitem-get-content.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c9079-106">To download the item in its original format, see [download an item's contents](driveitem-get-content.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c9079-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="c9079-107">Prerequisites</span></span>

<span data-ttu-id="c9079-108">この API を呼び出すには、ユーザーがアプリケーションに対して、アプリが変換するファイルへの読み取りアクセス権を付与している必要があります。</span><span class="sxs-lookup"><span data-stu-id="c9079-108">To call this API, the user must have granted the application read access to the file the app wishes to convert.</span></span>

## <a name="http-request"></a><span data-ttu-id="c9079-109">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c9079-109">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drive/items/{item-id}/content?format={format}
GET /drive/root:/{path and filename}:/content?format={format}
```

## <a name="query-parameters"></a><span data-ttu-id="c9079-110">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c9079-110">Query parameters</span></span>

| <span data-ttu-id="c9079-111">パラメーター</span><span class="sxs-lookup"><span data-stu-id="c9079-111">Parameter</span></span>      | <span data-ttu-id="c9079-112">型</span><span class="sxs-lookup"><span data-stu-id="c9079-112">Type</span></span>  | <span data-ttu-id="c9079-113">説明</span><span class="sxs-lookup"><span data-stu-id="c9079-113">Description</span></span>                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="c9079-114">_format_</span><span class="sxs-lookup"><span data-stu-id="c9079-114">_format_</span></span>  | <span data-ttu-id="c9079-115">string</span><span class="sxs-lookup"><span data-stu-id="c9079-115">string</span></span> | <span data-ttu-id="c9079-116">アイテムのコンテンツをダウンロードする形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="c9079-116">Specify the format the item's content should be downloaded as.</span></span> |


### <a name="format-options"></a><span data-ttu-id="c9079-117">形式のオプション</span><span class="sxs-lookup"><span data-stu-id="c9079-117">Format options</span></span>

<span data-ttu-id="c9079-118">**format** パラメーターには次の値を指定できます。</span><span class="sxs-lookup"><span data-stu-id="c9079-118">The following values are valid for the **format** parameter:</span></span>

| <span data-ttu-id="c9079-119">形式の値</span><span class="sxs-lookup"><span data-stu-id="c9079-119">Format value</span></span> | <span data-ttu-id="c9079-120">説明</span><span class="sxs-lookup"><span data-stu-id="c9079-120">Description</span></span>                        | <span data-ttu-id="c9079-121">サポートされているソースの拡張子</span><span class="sxs-lookup"><span data-stu-id="c9079-121">Supported source extensions</span></span>
|:-------------|:-----------------------------------|----------------------------
| <span data-ttu-id="c9079-122">pdf</span><span class="sxs-lookup"><span data-stu-id="c9079-122">pdf</span></span>          | <span data-ttu-id="c9079-123">アイテムを PDF 形式に変換します。</span><span class="sxs-lookup"><span data-stu-id="c9079-123">Converts the item into PDF format.</span></span> | <span data-ttu-id="c9079-124">csv、doc、docx、odp、ods、odt、pot、potm、potx、pps、ppsx、ppsxm、ppt、pptm、pptx、rtf、xls、xlsx</span><span class="sxs-lookup"><span data-stu-id="c9079-124">csv, doc, docx, odp, ods, odt, pot, potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, rtf, xls, xlsx</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="c9079-125">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c9079-125">Optional request headers</span></span>

| <span data-ttu-id="c9079-126">名前</span><span class="sxs-lookup"><span data-stu-id="c9079-126">Name</span></span>            | <span data-ttu-id="c9079-127">値</span><span class="sxs-lookup"><span data-stu-id="c9079-127">Value</span></span>   | <span data-ttu-id="c9079-128">説明</span><span class="sxs-lookup"><span data-stu-id="c9079-128">Description</span></span>                                                                                                                                              |
|:----------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="c9079-129">_if-none-match_</span><span class="sxs-lookup"><span data-stu-id="c9079-129">_if-none-match_</span></span> | <span data-ttu-id="c9079-130">String</span><span class="sxs-lookup"><span data-stu-id="c9079-130">String</span></span>  | <span data-ttu-id="c9079-131">この要求ヘッダーが含まれている場合、指定された eTag (または cTag) がファイルの現在のタグに一致すると、`HTTP 304 Not Modified` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="c9079-131">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="example"></a><span data-ttu-id="c9079-132">例</span><span class="sxs-lookup"><span data-stu-id="c9079-132">Example</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c9079-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c9079-133">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "convert-item-content", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/content?format={format}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c9079-134">C#</span><span class="sxs-lookup"><span data-stu-id="c9079-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/convert-item-content-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c9079-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c9079-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/convert-item-content-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c9079-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c9079-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/convert-item-content-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c9079-137">Java</span><span class="sxs-lookup"><span data-stu-id="c9079-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/convert-item-content-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="c9079-138">応答</span><span class="sxs-lookup"><span data-stu-id="c9079-138">Response</span></span>

<span data-ttu-id="c9079-139">変換されたファイルの事前認証されたダウンロード URL にリダイレクトする、`302 Found` 応答を返します。</span><span class="sxs-lookup"><span data-stu-id="c9079-139">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the converted file.</span></span>

<span data-ttu-id="c9079-140">変換されたファイルをダウンロードするには、アプリが応答の `Location` ヘッダーに従う必要があります。</span><span class="sxs-lookup"><span data-stu-id="c9079-140">To download the converted file, your app must follow the `Location` header in the response.</span></span>

<span data-ttu-id="c9079-141">事前認証された URL は、短期間 (数分) のみ有効で、アクセスのために `Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="c9079-141">Pre-authenticated URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to access.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

### <a name="error-responses"></a><span data-ttu-id="c9079-142">エラー応答</span><span class="sxs-lookup"><span data-stu-id="c9079-142">Error responses</span></span>

<span data-ttu-id="c9079-143">エラーがどのように返されるかの詳細については、「[エラー応答][error-response]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c9079-143">See [Error Responses][error-response] for more information about how errors are returned.</span></span>

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
