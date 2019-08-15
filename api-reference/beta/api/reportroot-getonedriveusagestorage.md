---
title: 'reportRoot: getOneDriveUsageStorage'
description: OneDrive for Business で使用しているストレージの量の傾向を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 42af6eeccdd870e4781fe09ecc26ec910e17032e
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36411516"
---
# <a name="reportroot-getonedriveusagestorage"></a><span data-ttu-id="be3cb-103">reportRoot: getOneDriveUsageStorage</span><span class="sxs-lookup"><span data-stu-id="be3cb-103">reportRoot: getOneDriveUsageStorage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be3cb-104">OneDrive for Business で使用しているストレージの量の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="be3cb-104">Get the trend on the amount of storage you are using in OneDrive for Business.</span></span>

> <span data-ttu-id="be3cb-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: OneDrive for Business の使用状況](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="be3cb-105">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="be3cb-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="be3cb-106">Permissions</span></span>

<span data-ttu-id="be3cb-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="be3cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="be3cb-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="be3cb-109">Permission type</span></span>                        | <span data-ttu-id="be3cb-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="be3cb-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="be3cb-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="be3cb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="be3cb-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="be3cb-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="be3cb-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="be3cb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be3cb-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="be3cb-114">Not supported.</span></span>                           |
| <span data-ttu-id="be3cb-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="be3cb-115">Application</span></span>                            | <span data-ttu-id="be3cb-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="be3cb-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="be3cb-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="be3cb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageStorage(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="be3cb-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="be3cb-118">Function parameters</span></span>

<span data-ttu-id="be3cb-119">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="be3cb-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="be3cb-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="be3cb-120">Parameter</span></span> | <span data-ttu-id="be3cb-121">型</span><span class="sxs-lookup"><span data-stu-id="be3cb-121">Type</span></span>   | <span data-ttu-id="be3cb-122">説明</span><span class="sxs-lookup"><span data-stu-id="be3cb-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="be3cb-123">period</span><span class="sxs-lookup"><span data-stu-id="be3cb-123">period</span></span>    | <span data-ttu-id="be3cb-124">文字列</span><span class="sxs-lookup"><span data-stu-id="be3cb-124">string</span></span> | <span data-ttu-id="be3cb-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="be3cb-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="be3cb-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="be3cb-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="be3cb-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="be3cb-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="be3cb-128">必須。</span><span class="sxs-lookup"><span data-stu-id="be3cb-128">Required.</span></span> |

<span data-ttu-id="be3cb-129">このメソッドは、 `$format`応答をカスタマイズするための[OData クエリパラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="be3cb-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="be3cb-130">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="be3cb-130">The default output type is text/csv.</span></span> <span data-ttu-id="be3cb-131">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="be3cb-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="be3cb-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="be3cb-132">Request headers</span></span>

| <span data-ttu-id="be3cb-133">名前</span><span class="sxs-lookup"><span data-stu-id="be3cb-133">Name</span></span>          | <span data-ttu-id="be3cb-134">説明</span><span class="sxs-lookup"><span data-stu-id="be3cb-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="be3cb-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="be3cb-135">Authorization</span></span> | <span data-ttu-id="be3cb-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="be3cb-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="be3cb-138">応答</span><span class="sxs-lookup"><span data-stu-id="be3cb-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="be3cb-139">CSV</span><span class="sxs-lookup"><span data-stu-id="be3cb-139">CSV</span></span>

<span data-ttu-id="be3cb-140">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="be3cb-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="be3cb-141">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="be3cb-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="be3cb-142">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="be3cb-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="be3cb-143">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="be3cb-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="be3cb-144">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="be3cb-144">Report Refresh Date</span></span>
- <span data-ttu-id="be3cb-145">サイトの種類</span><span class="sxs-lookup"><span data-stu-id="be3cb-145">Site Type</span></span>
- <span data-ttu-id="be3cb-146">使用済みストレージ (バイト)</span><span class="sxs-lookup"><span data-stu-id="be3cb-146">Storage Used (Byte)</span></span>
- <span data-ttu-id="be3cb-147">レポート日付</span><span class="sxs-lookup"><span data-stu-id="be3cb-147">Report Date</span></span>
- <span data-ttu-id="be3cb-148">レポート期間</span><span class="sxs-lookup"><span data-stu-id="be3cb-148">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="be3cb-149">JSON</span><span class="sxs-lookup"><span data-stu-id="be3cb-149">JSON</span></span>

<span data-ttu-id="be3cb-150">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[site使い方 storage](../resources/siteusagestorage.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="be3cb-150">If successful, this method returns a `200 OK` response code and a **[siteUsageStorage](../resources/siteusagestorage.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be3cb-151">例</span><span class="sxs-lookup"><span data-stu-id="be3cb-151">Example</span></span>

### <a name="csv"></a><span data-ttu-id="be3cb-152">CSV</span><span class="sxs-lookup"><span data-stu-id="be3cb-152">CSV</span></span>

<span data-ttu-id="be3cb-153">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="be3cb-153">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="be3cb-154">要求</span><span class="sxs-lookup"><span data-stu-id="be3cb-154">Request</span></span>

<span data-ttu-id="be3cb-155">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="be3cb-155">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="be3cb-156">プロトコル</span><span class="sxs-lookup"><span data-stu-id="be3cb-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusagestorage_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageStorage(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="be3cb-157">C#</span><span class="sxs-lookup"><span data-stu-id="be3cb-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveusagestorage-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="be3cb-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="be3cb-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveusagestorage-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="be3cb-159">目的-C</span><span class="sxs-lookup"><span data-stu-id="be3cb-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveusagestorage-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="be3cb-160">応答</span><span class="sxs-lookup"><span data-stu-id="be3cb-160">Response</span></span>

<span data-ttu-id="be3cb-161">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="be3cb-161">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="be3cb-162">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="be3cb-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Storage Used (Byte),Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="be3cb-163">JSON</span><span class="sxs-lookup"><span data-stu-id="be3cb-163">JSON</span></span>

<span data-ttu-id="be3cb-164">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="be3cb-164">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="be3cb-165">要求</span><span class="sxs-lookup"><span data-stu-id="be3cb-165">Request</span></span>

<span data-ttu-id="be3cb-166">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="be3cb-166">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="be3cb-167">プロトコル</span><span class="sxs-lookup"><span data-stu-id="be3cb-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusagestorage_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageStorage(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="be3cb-168">C#</span><span class="sxs-lookup"><span data-stu-id="be3cb-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveusagestorage-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="be3cb-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="be3cb-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveusagestorage-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="be3cb-170">目的-C</span><span class="sxs-lookup"><span data-stu-id="be3cb-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveusagestorage-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="be3cb-171">応答</span><span class="sxs-lookup"><span data-stu-id="be3cb-171">Response</span></span>

<span data-ttu-id="be3cb-172">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="be3cb-172">The following is an example of the response.</span></span>

> <span data-ttu-id="be3cb-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="be3cb-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.siteUsageStorage"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 248

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.siteUsageStorage)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteType": "All", 
      "storageUsedInBytes": 132654293197, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
