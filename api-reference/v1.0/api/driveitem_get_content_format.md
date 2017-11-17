---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: "他の形式に変換する"
ms.openlocfilehash: 3031500beaec2d765075abfd925a6333f50368f9
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="download-a-file-in-another-format"></a><span data-ttu-id="3d415-102">別の形式でファイルをダウンロードする</span><span class="sxs-lookup"><span data-stu-id="3d415-102">Download a file in another format</span></span>

<span data-ttu-id="3d415-103">この API を使用して、アイテムのコンテンツを特定の形式で取得します。</span><span class="sxs-lookup"><span data-stu-id="3d415-103">Use this API to retrieve the contents of an item in a specific format.</span></span>
<span data-ttu-id="3d415-104">すべてのファイルがすべての形式に変換できるわけではありません。</span><span class="sxs-lookup"><span data-stu-id="3d415-104">Not all files can be converted into all formats.</span></span>

<span data-ttu-id="3d415-105">アイテムを元の形式でダウンロードするには、[アイテムのコンテンツのダウンロードの説明](driveitem_get_content.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3d415-105">To download the item in it's original format, see [download an item's contents](driveitem_get_content.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3d415-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="3d415-106">Prerequisites</span></span>

<span data-ttu-id="3d415-107">この API を呼び出すには、ユーザーがアプリケーションに対して、アプリが変換するファイルへの読み取りアクセス権を付与している必要があります。</span><span class="sxs-lookup"><span data-stu-id="3d415-107">To call this API, the user must have granted the application read access to the file the app wishes to convert.</span></span>

## <a name="http-request"></a><span data-ttu-id="3d415-108">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3d415-108">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drive/items/{item-id}/content?format={format}
GET /drive/root:/{path and filename}:/content?format={format}
```

### <a name="optional-request-headers"></a><span data-ttu-id="3d415-109">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3d415-109">Optional request headers</span></span>

| <span data-ttu-id="3d415-110">名前</span><span class="sxs-lookup"><span data-stu-id="3d415-110">Name</span></span>            | <span data-ttu-id="3d415-111">値</span><span class="sxs-lookup"><span data-stu-id="3d415-111">Value</span></span>   | <span data-ttu-id="3d415-112">説明</span><span class="sxs-lookup"><span data-stu-id="3d415-112">Description</span></span>                                                                                                                                              |
|:----------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="3d415-113">_if-none-match_</span><span class="sxs-lookup"><span data-stu-id="3d415-113">_if-none-match_</span></span> | <span data-ttu-id="3d415-114">String</span><span class="sxs-lookup"><span data-stu-id="3d415-114">String</span></span>  | <span data-ttu-id="3d415-115">この要求ヘッダーが含まれている場合、指定された eTag (または cTag) がファイルの現在のタグに一致すると、`HTTP 304 Not Modified` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="3d415-115">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |


### <a name="query-string-parameters"></a><span data-ttu-id="3d415-116">クエリ文字列のパラメーター</span><span class="sxs-lookup"><span data-stu-id="3d415-116">Query string parameters</span></span>

| <span data-ttu-id="3d415-117">名前</span><span class="sxs-lookup"><span data-stu-id="3d415-117">Name</span></span>      | <span data-ttu-id="3d415-118">値</span><span class="sxs-lookup"><span data-stu-id="3d415-118">Value</span></span>  | <span data-ttu-id="3d415-119">説明</span><span class="sxs-lookup"><span data-stu-id="3d415-119">Description</span></span>                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="3d415-120">_format_</span><span class="sxs-lookup"><span data-stu-id="3d415-120">_format_</span></span>  | <span data-ttu-id="3d415-121">string</span><span class="sxs-lookup"><span data-stu-id="3d415-121">string</span></span> | <span data-ttu-id="3d415-122">アイテムのコンテンツをダウンロードする形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="3d415-122">Specify the format the item's content should be downloaded as.</span></span> |


<span data-ttu-id="3d415-123">**convert** パラメーターには次の値を指定できます。</span><span class="sxs-lookup"><span data-stu-id="3d415-123">The following values are valid for the **convert** parameter:</span></span>

| <span data-ttu-id="3d415-124">値</span><span class="sxs-lookup"><span data-stu-id="3d415-124">Value</span></span>   | <span data-ttu-id="3d415-125">説明</span><span class="sxs-lookup"><span data-stu-id="3d415-125">Description</span></span>                        | <span data-ttu-id="3d415-126">サポートされているソースの拡張子</span><span class="sxs-lookup"><span data-stu-id="3d415-126">Supported source extensions</span></span> |
|:--------|:-----------------------------------|-----------------------------|
| <span data-ttu-id="3d415-127">**pdf**</span><span class="sxs-lookup"><span data-stu-id="3d415-127">**pdf**</span></span> | <span data-ttu-id="3d415-128">アイテムを PDF 形式に変換します。</span><span class="sxs-lookup"><span data-stu-id="3d415-128">Converts the item into PDF format.</span></span> | <span data-ttu-id="3d415-129">csv、doc、docx、odp、ods、odt、pot、potm、potx、pps、ppsx、ppsxm、ppt、pptm、pptx、rtf、xls、xlsx</span><span class="sxs-lookup"><span data-stu-id="3d415-129">csv, doc, docx, odp, ods, odt, pot, potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, rtf, xls, xlsx</span></span> | 

### <a name="example"></a><span data-ttu-id="3d415-130">例</span><span class="sxs-lookup"><span data-stu-id="3d415-130">Example</span></span>

<!-- { "blockType": "request", "name": "convert-item-content", "scopes": "files.read" } -->

```http
GET /drive/items/{item-id}/content?format={format}
```

## <a name="response"></a><span data-ttu-id="3d415-131">応答</span><span class="sxs-lookup"><span data-stu-id="3d415-131">Response</span></span>

<span data-ttu-id="3d415-132">変換されたファイルの事前認証されたダウンロード URL にリダイレクトする、`302 Found` 応答を返します。</span><span class="sxs-lookup"><span data-stu-id="3d415-132">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the converted file.</span></span>

<span data-ttu-id="3d415-133">変換されたファイルをダウンロードするには、アプリが応答の `Location` ヘッダーに従う必要があります。</span><span class="sxs-lookup"><span data-stu-id="3d415-133">To download the converted file, your app must follow the `Location` header in the response.</span></span>

<span data-ttu-id="3d415-134">事前認証された URL は、短期間 (数分) のみ有効で、アクセスのために `Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="3d415-134">Pre-authenticated URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to access.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

### <a name="error-responses"></a><span data-ttu-id="3d415-135">エラー応答</span><span class="sxs-lookup"><span data-stu-id="3d415-135">Error responses</span></span>

<span data-ttu-id="3d415-136">エラーがどのように返されるかについては、「[エラー応答][error-response]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3d415-136">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: ../../../concepts/errors.md
[file-facet]: ../resources/file.md

<!-- {
  "type": "#page.annotation",
  "description": "Convert the contents of an item in OneDrive to a different format.",
  "keywords": "convert,pdf,convert to pdf",
  "section": "documentation",
  "tocPath": "Items/Download formats"
} -->
