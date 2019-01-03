---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 他の形式に変換する
ms.openlocfilehash: d5fbeeb28e2c0d2bf23652f451f87d12b1a06435
ms.sourcegitcommit: 12c6e82f1417022540e534ebadbd0e8d7fb5abde
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/08/2018
ms.locfileid: "27209706"
---
# <a name="download-a-file-in-another-format"></a><span data-ttu-id="5501d-102">別の形式でファイルをダウンロードする</span><span class="sxs-lookup"><span data-stu-id="5501d-102">Download a file in another format</span></span>

<span data-ttu-id="5501d-103">この API を使用して、アイテムのコンテンツを特定の形式で取得します。</span><span class="sxs-lookup"><span data-stu-id="5501d-103">Use this API to retrieve the contents of an item in a specific format.</span></span>
<span data-ttu-id="5501d-104">すべてのファイルがすべての形式に変換できるわけではありません。</span><span class="sxs-lookup"><span data-stu-id="5501d-104">Not all files can be converted into all formats.</span></span>

<span data-ttu-id="5501d-105">元の形式でアイテムをダウンロードするには、[アイテムの内容をダウンロードする](driveitem-get-content.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5501d-105">To download the item in its original format, see [download an item's contents](driveitem-get-content.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5501d-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="5501d-106">Prerequisites</span></span>

<span data-ttu-id="5501d-107">この API を呼び出すには、ユーザーがアプリケーションに対して、アプリが変換するファイルへの読み取りアクセス権を付与している必要があります。</span><span class="sxs-lookup"><span data-stu-id="5501d-107">To call this API, the user must have granted the application read access to the file the app wishes to convert.</span></span>

## <a name="http-request"></a><span data-ttu-id="5501d-108">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5501d-108">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drive/items/{item-id}/content?format={format}
GET /drive/root:/{path and filename}:/content?format={format}
```

## <a name="query-parameters"></a><span data-ttu-id="5501d-109">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="5501d-109">Query parameters</span></span>

| <span data-ttu-id="5501d-110">パラメーター</span><span class="sxs-lookup"><span data-stu-id="5501d-110">Parameter</span></span>      | <span data-ttu-id="5501d-111">Type</span><span class="sxs-lookup"><span data-stu-id="5501d-111">Type</span></span>  | <span data-ttu-id="5501d-112">説明</span><span class="sxs-lookup"><span data-stu-id="5501d-112">Description</span></span>                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="5501d-113">_format_</span><span class="sxs-lookup"><span data-stu-id="5501d-113">_format_</span></span>  | <span data-ttu-id="5501d-114">文字列</span><span class="sxs-lookup"><span data-stu-id="5501d-114">string</span></span> | <span data-ttu-id="5501d-115">アイテムのコンテンツをダウンロードする形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="5501d-115">Specify the format the item's content should be downloaded as.</span></span> |


### <a name="format-options"></a><span data-ttu-id="5501d-116">書式のオプション</span><span class="sxs-lookup"><span data-stu-id="5501d-116">Format options</span></span>

<span data-ttu-id="5501d-117">次の値は、 **format**パラメーターに有効です。</span><span class="sxs-lookup"><span data-stu-id="5501d-117">The following values are valid for the **format** parameter:</span></span>

| <span data-ttu-id="5501d-118">形式の値</span><span class="sxs-lookup"><span data-stu-id="5501d-118">Format value</span></span> | <span data-ttu-id="5501d-119">説明</span><span class="sxs-lookup"><span data-stu-id="5501d-119">Description</span></span>                        | <span data-ttu-id="5501d-120">サポートされているソースの拡張子</span><span class="sxs-lookup"><span data-stu-id="5501d-120">Supported source extensions</span></span>
|:-------------|:-----------------------------------|----------------------------
| <span data-ttu-id="5501d-121">pdf</span><span class="sxs-lookup"><span data-stu-id="5501d-121">pdf</span></span>          | <span data-ttu-id="5501d-122">アイテムを PDF 形式に変換します。</span><span class="sxs-lookup"><span data-stu-id="5501d-122">Converts the item into PDF format.</span></span> | <span data-ttu-id="5501d-123">csv、doc、docx、odp、ods、odt、pot、potm、potx、pps、ppsx、ppsxm、ppt、pptm、pptx、rtf、xls、xlsx</span><span class="sxs-lookup"><span data-stu-id="5501d-123">csv, doc, docx, odp, ods, odt, pot, potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, rtf, xls, xlsx</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="5501d-124">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5501d-124">Optional request headers</span></span>

| <span data-ttu-id="5501d-125">名前</span><span class="sxs-lookup"><span data-stu-id="5501d-125">Name</span></span>            | <span data-ttu-id="5501d-126">値</span><span class="sxs-lookup"><span data-stu-id="5501d-126">Value</span></span>   | <span data-ttu-id="5501d-127">説明</span><span class="sxs-lookup"><span data-stu-id="5501d-127">Description</span></span>                                                                                                                                              |
|:----------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="5501d-128">_if-none-match_</span><span class="sxs-lookup"><span data-stu-id="5501d-128">_if-none-match_</span></span> | <span data-ttu-id="5501d-129">String</span><span class="sxs-lookup"><span data-stu-id="5501d-129">String</span></span>  | <span data-ttu-id="5501d-130">この要求ヘッダーが含まれている場合、指定された eTag (または cTag) がファイルの現在のタグに一致すると、`HTTP 304 Not Modified` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="5501d-130">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="example"></a><span data-ttu-id="5501d-131">例</span><span class="sxs-lookup"><span data-stu-id="5501d-131">Example</span></span>

<!-- { "blockType": "request", "name": "convert-item-content", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/content?format={format}
```

## <a name="response"></a><span data-ttu-id="5501d-132">応答</span><span class="sxs-lookup"><span data-stu-id="5501d-132">Response</span></span>

<span data-ttu-id="5501d-133">変換されたファイルの事前認証されたダウンロード URL にリダイレクトする、`302 Found` 応答を返します。</span><span class="sxs-lookup"><span data-stu-id="5501d-133">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the converted file.</span></span>

<span data-ttu-id="5501d-134">変換されたファイルをダウンロードするには、アプリが応答の `Location` ヘッダーに従う必要があります。</span><span class="sxs-lookup"><span data-stu-id="5501d-134">To download the converted file, your app must follow the `Location` header in the response.</span></span>

<span data-ttu-id="5501d-135">事前認証された URL は、短期間 (数分) のみ有効で、アクセスのために `Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="5501d-135">Pre-authenticated URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to access.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

### <a name="error-responses"></a><span data-ttu-id="5501d-136">エラー応答</span><span class="sxs-lookup"><span data-stu-id="5501d-136">Error responses</span></span>

<span data-ttu-id="5501d-137">エラーがどのように返されるかについては、「[エラー応答][error-response]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5501d-137">See [Error Responses][error-response] for more information about how errors are returned.</span></span>

[error-response]: /graph/errors
[file-facet]: ../resources/file.md

<!-- {
  "type": "#page.annotation",
  "description": "Convert the contents of an item in OneDrive to a different format.",
  "keywords": "convert,pdf,convert to pdf",
  "section": "documentation",
  "tocPath": "Items/Download formats"
} -->