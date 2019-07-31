---
title: 'reportRoot: getSharePointSiteUsageStorage'
description: レポート期間中に割り当てられ、消費したストレージの傾向を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: f0c46abc8f77e7129941083f1a6a3cd533b1ab16
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35988077"
---
# <a name="reportroot-getsharepointsiteusagestorage"></a><span data-ttu-id="79525-103">reportRoot: getSharePointSiteUsageStorage</span><span class="sxs-lookup"><span data-stu-id="79525-103">reportRoot: getSharePointSiteUsageStorage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79525-104">レポート期間中に割り当てられ、消費したストレージの傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="79525-104">Get the trend of storage allocated and consumed during the reporting period.</span></span>

> <span data-ttu-id="79525-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: SharePoint サイトの使用状況](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="79525-105">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="79525-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="79525-106">Permissions</span></span>

<span data-ttu-id="79525-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="79525-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="79525-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="79525-109">Permission type</span></span>                        | <span data-ttu-id="79525-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="79525-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="79525-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="79525-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="79525-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="79525-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="79525-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="79525-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79525-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79525-114">Not supported.</span></span>                           |
| <span data-ttu-id="79525-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="79525-115">Application</span></span>                            | <span data-ttu-id="79525-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="79525-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="79525-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="79525-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageStorage(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="79525-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="79525-118">Function parameters</span></span>

<span data-ttu-id="79525-119">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="79525-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="79525-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="79525-120">Parameter</span></span> | <span data-ttu-id="79525-121">型</span><span class="sxs-lookup"><span data-stu-id="79525-121">Type</span></span>   | <span data-ttu-id="79525-122">説明</span><span class="sxs-lookup"><span data-stu-id="79525-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="79525-123">period</span><span class="sxs-lookup"><span data-stu-id="79525-123">period</span></span>    | <span data-ttu-id="79525-124">文字列</span><span class="sxs-lookup"><span data-stu-id="79525-124">string</span></span> | <span data-ttu-id="79525-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="79525-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="79525-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="79525-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="79525-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="79525-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="79525-128">必須。</span><span class="sxs-lookup"><span data-stu-id="79525-128">Required.</span></span> |

<span data-ttu-id="79525-129">このメソッドは、 `$format`応答をカスタマイズするための[OData クエリパラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="79525-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="79525-130">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="79525-130">The default output type is text/csv.</span></span> <span data-ttu-id="79525-131">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="79525-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="79525-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="79525-132">Request headers</span></span>

| <span data-ttu-id="79525-133">名前</span><span class="sxs-lookup"><span data-stu-id="79525-133">Name</span></span>          | <span data-ttu-id="79525-134">説明</span><span class="sxs-lookup"><span data-stu-id="79525-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="79525-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="79525-135">Authorization</span></span> | <span data-ttu-id="79525-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="79525-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="79525-138">応答</span><span class="sxs-lookup"><span data-stu-id="79525-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="79525-139">CSV</span><span class="sxs-lookup"><span data-stu-id="79525-139">CSV</span></span>

<span data-ttu-id="79525-140">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="79525-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="79525-141">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="79525-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="79525-142">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="79525-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="79525-143">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="79525-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="79525-144">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="79525-144">Report Refresh Date</span></span>
- <span data-ttu-id="79525-145">サイトの種類</span><span class="sxs-lookup"><span data-stu-id="79525-145">Site Type</span></span>
- <span data-ttu-id="79525-146">使用済みストレージ (バイト)</span><span class="sxs-lookup"><span data-stu-id="79525-146">Storage Used (Byte)</span></span>
- <span data-ttu-id="79525-147">レポート日付</span><span class="sxs-lookup"><span data-stu-id="79525-147">Report Date</span></span>
- <span data-ttu-id="79525-148">レポート期間</span><span class="sxs-lookup"><span data-stu-id="79525-148">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="79525-149">JSON</span><span class="sxs-lookup"><span data-stu-id="79525-149">JSON</span></span>

<span data-ttu-id="79525-150">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[site使い方 storage](../resources/siteusagestorage.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="79525-150">If successful, this method returns a `200 OK` response code and a **[siteUsageStorage](../resources/siteusagestorage.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79525-151">例</span><span class="sxs-lookup"><span data-stu-id="79525-151">Example</span></span>

### <a name="csv"></a><span data-ttu-id="79525-152">CSV</span><span class="sxs-lookup"><span data-stu-id="79525-152">CSV</span></span>

<span data-ttu-id="79525-153">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="79525-153">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="79525-154">要求</span><span class="sxs-lookup"><span data-stu-id="79525-154">Request</span></span>

<span data-ttu-id="79525-155">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="79525-155">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="79525-156">プロトコル</span><span class="sxs-lookup"><span data-stu-id="79525-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagestorage_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageStorage(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="79525-157">C#</span><span class="sxs-lookup"><span data-stu-id="79525-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointsiteusagestorage-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="79525-158">Javascript</span><span class="sxs-lookup"><span data-stu-id="79525-158">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointsiteusagestorage-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="79525-159">目的-C</span><span class="sxs-lookup"><span data-stu-id="79525-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointsiteusagestorage-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="79525-160">Java</span><span class="sxs-lookup"><span data-stu-id="79525-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getsharepointsiteusagestorage-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="79525-161">応答</span><span class="sxs-lookup"><span data-stu-id="79525-161">Response</span></span>

<span data-ttu-id="79525-162">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="79525-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="79525-163">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="79525-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="79525-164">JSON</span><span class="sxs-lookup"><span data-stu-id="79525-164">JSON</span></span>

<span data-ttu-id="79525-165">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="79525-165">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="79525-166">要求</span><span class="sxs-lookup"><span data-stu-id="79525-166">Request</span></span>

<span data-ttu-id="79525-167">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="79525-167">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="79525-168">プロトコル</span><span class="sxs-lookup"><span data-stu-id="79525-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagestorage_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageStorage(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="79525-169">C#</span><span class="sxs-lookup"><span data-stu-id="79525-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointsiteusagestorage-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="79525-170">Javascript</span><span class="sxs-lookup"><span data-stu-id="79525-170">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointsiteusagestorage-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="79525-171">目的-C</span><span class="sxs-lookup"><span data-stu-id="79525-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointsiteusagestorage-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="79525-172">Java</span><span class="sxs-lookup"><span data-stu-id="79525-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getsharepointsiteusagestorage-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="79525-173">応答</span><span class="sxs-lookup"><span data-stu-id="79525-173">Response</span></span>

<span data-ttu-id="79525-174">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="79525-174">The following is an example of the response.</span></span>

> <span data-ttu-id="79525-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="79525-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "storageUsedInBytes": 171835798971, 
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
