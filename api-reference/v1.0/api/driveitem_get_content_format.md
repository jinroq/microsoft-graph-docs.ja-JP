---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 他の形式に変換する
ms.openlocfilehash: 46e8ed178384a81f232a753fe683f8e11efe8585
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/21/2018
ms.locfileid: "23269181"
---
# <a name="download-a-file-in-another-format"></a><span data-ttu-id="1c756-102">別の形式でファイルをダウンロードする</span><span class="sxs-lookup"><span data-stu-id="1c756-102">Download a file in another format</span></span>

<span data-ttu-id="1c756-103">この API を使用して、アイテムのコンテンツを特定の形式で取得します。</span><span class="sxs-lookup"><span data-stu-id="1c756-103">Use this API to retrieve the contents of an item in a specific format.</span></span>
<span data-ttu-id="1c756-104">すべてのファイルがすべての形式に変換できるわけではありません。</span><span class="sxs-lookup"><span data-stu-id="1c756-104">Not all files can be converted into all formats.</span></span>

<span data-ttu-id="1c756-105">アイテムを元の形式でダウンロードするには、[アイテムのコンテンツのダウンロードの説明](driveitem_get_content.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1c756-105">To download the item in it's original format, see [download an item's contents](driveitem_get_content.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1c756-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="1c756-106">Prerequisites</span></span>

<span data-ttu-id="1c756-107">この API を呼び出すには、ユーザーがアプリケーションに対して、アプリが変換するファイルへの読み取りアクセス権を付与している必要があります。</span><span class="sxs-lookup"><span data-stu-id="1c756-107">To call this API, the user must have granted the application read access to the file the app wishes to convert.</span></span>

## <a name="http-request"></a><span data-ttu-id="1c756-108">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1c756-108">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drive/items/{item-id}/content?format={format}
GET /drive/root:/{path and filename}:/content?format={format}
```

### <a name="optional-request-headers"></a><span data-ttu-id="1c756-109">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1c756-109">Optional request headers</span></span>

| <span data-ttu-id="1c756-110">名前</span><span class="sxs-lookup"><span data-stu-id="1c756-110">Name</span></span>            | <span data-ttu-id="1c756-111">値</span><span class="sxs-lookup"><span data-stu-id="1c756-111">Value</span></span>   | <span data-ttu-id="1c756-112">説明</span><span class="sxs-lookup"><span data-stu-id="1c756-112">Description</span></span>                                                                                                                                              |
|:----------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="1c756-113">_if-none-match_</span><span class="sxs-lookup"><span data-stu-id="1c756-113">_if-none-match_</span></span> | <span data-ttu-id="1c756-114">文字列</span><span class="sxs-lookup"><span data-stu-id="1c756-114">String</span></span>  | <span data-ttu-id="1c756-115">この要求ヘッダーが含まれている場合、指定された eTag (または cTag) がファイルの現在のタグに一致すると、`HTTP 304 Not Modified` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="1c756-115">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |


### <a name="query-string-parameters"></a><span data-ttu-id="1c756-116">クエリ文字列のパラメーター</span><span class="sxs-lookup"><span data-stu-id="1c756-116">Query string parameters</span></span>

| <span data-ttu-id="1c756-117">名前</span><span class="sxs-lookup"><span data-stu-id="1c756-117">Name</span></span>      | <span data-ttu-id="1c756-118">値</span><span class="sxs-lookup"><span data-stu-id="1c756-118">Value</span></span>  | <span data-ttu-id="1c756-119">説明</span><span class="sxs-lookup"><span data-stu-id="1c756-119">Description</span></span>                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="1c756-120">_format_</span><span class="sxs-lookup"><span data-stu-id="1c756-120">_format_</span></span>  | <span data-ttu-id="1c756-121">文字列</span><span class="sxs-lookup"><span data-stu-id="1c756-121">string</span></span> | <span data-ttu-id="1c756-122">アイテムのコンテンツをダウンロードする形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="1c756-122">Specify the format the item's content should be downloaded as.</span></span> |


#### <a name="format-options"></a><span data-ttu-id="1c756-123">形式のオプション</span><span class="sxs-lookup"><span data-stu-id="1c756-123">Format options</span></span>

<span data-ttu-id="1c756-124">**format** パラメーターには次の値を指定できます。</span><span class="sxs-lookup"><span data-stu-id="1c756-124">The following values are valid for the **convert** parameter:</span></span>

| <span data-ttu-id="1c756-125">形式の値</span><span class="sxs-lookup"><span data-stu-id="1c756-125">Format value</span></span> | <span data-ttu-id="1c756-126">説明</span><span class="sxs-lookup"><span data-stu-id="1c756-126">Description</span></span>                        | <span data-ttu-id="1c756-127">サポートされているソースの拡張子</span><span class="sxs-lookup"><span data-stu-id="1c756-127">Supported source extensions</span></span>
|:-------------|:-----------------------------------|----------------------------
| <span data-ttu-id="1c756-128">pdf</span><span class="sxs-lookup"><span data-stu-id="1c756-128">pdf</span></span>          | <span data-ttu-id="1c756-129">アイテムを PDF 形式に変換します。</span><span class="sxs-lookup"><span data-stu-id="1c756-129">Converts the item into PDF format.</span></span> | <span data-ttu-id="1c756-130">csv、doc、docx、odp、ods、odt、pot、potm、potx、pps、ppsx、ppsxm、ppt、pptm、pptx、rtf、xls、xlsx</span><span class="sxs-lookup"><span data-stu-id="1c756-130">csv, doc, docx, odp, ods, odt, pot, potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, rtf, xls, xlsx</span></span>

### <a name="example"></a><span data-ttu-id="1c756-131">例</span><span class="sxs-lookup"><span data-stu-id="1c756-131">Example</span></span>

<!-- { "blockType": "request", "name": "convert-item-content", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/content?format={format}
```

## <a name="response"></a><span data-ttu-id="1c756-132">応答</span><span class="sxs-lookup"><span data-stu-id="1c756-132">Response</span></span>

<span data-ttu-id="1c756-133">変換されたファイルの事前認証されたダウンロード URL にリダイレクトする、`302 Found` 応答を返します。</span><span class="sxs-lookup"><span data-stu-id="1c756-133">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the converted file.</span></span>

<span data-ttu-id="1c756-134">変換されたファイルをダウンロードするには、アプリが応答の `Location` ヘッダーに従う必要があります。</span><span class="sxs-lookup"><span data-stu-id="1c756-134">To download the converted file, your app must follow the `Location` header in the response.</span></span>

<span data-ttu-id="1c756-135">事前認証された URL は、短期間 (数分) のみ有効で、アクセスのために `Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="1c756-135">Pre-authenticated URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to access.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

### <a name="error-responses"></a><span data-ttu-id="1c756-136">エラー応答</span><span class="sxs-lookup"><span data-stu-id="1c756-136">Error responses</span></span>

<span data-ttu-id="1c756-137">エラーがどのように返されるかについては、「[エラー応答][error-response]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1c756-137">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: ../../../concepts/errors.md
[file-facet]: ../resources/file.md

<!-- {
  "type": "#page.annotation",
  "description": "Convert the contents of an item in OneDrive to a different format.",
  "keywords": "convert,pdf,convert to pdf",
  "section": "documentation",
  "tocPath": "Items/Download formats"
} -->
