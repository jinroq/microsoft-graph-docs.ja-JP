---
title: 'reportRoot: getOneDriveUsageAccountCounts'
description: アクティブな OneDrive for Business サイトの数の傾向を取得します。 ユーザーがファイルを表示、変更、アップロード、ダウンロード、共有、同期したサイトはすべて、アクティブなサイトとみなされます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 79396cb1d5190b8f0e577513b53ec8ad58712467
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35446746"
---
# <a name="reportroot-getonedriveusageaccountcounts"></a><span data-ttu-id="aafab-104">reportRoot: getOneDriveUsageAccountCounts</span><span class="sxs-lookup"><span data-stu-id="aafab-104">reportRoot: getOneDriveUsageAccountCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aafab-105">アクティブな OneDrive for Business サイトの数の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="aafab-105">Get the trend in the number of active OneDrive for Business sites.</span></span> <span data-ttu-id="aafab-106">ユーザーがファイルを表示、変更、アップロード、ダウンロード、共有、同期したサイトはすべて、アクティブなサイトとみなされます。</span><span class="sxs-lookup"><span data-stu-id="aafab-106">Any site on which users viewed, modified, uploaded, downloaded, shared, or synced files is considered an active site.</span></span>

> <span data-ttu-id="aafab-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: OneDrive for Business の使用状況](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="aafab-107">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="aafab-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="aafab-108">Permissions</span></span>

<span data-ttu-id="aafab-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="aafab-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="aafab-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="aafab-111">Permission type</span></span>                        | <span data-ttu-id="aafab-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="aafab-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="aafab-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="aafab-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="aafab-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="aafab-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="aafab-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="aafab-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aafab-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aafab-116">Not supported.</span></span>                           |
| <span data-ttu-id="aafab-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="aafab-117">Application</span></span>                            | <span data-ttu-id="aafab-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="aafab-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="aafab-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="aafab-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageAccountCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="aafab-120">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="aafab-120">Function parameters</span></span>

<span data-ttu-id="aafab-121">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="aafab-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="aafab-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="aafab-122">Parameter</span></span> | <span data-ttu-id="aafab-123">型</span><span class="sxs-lookup"><span data-stu-id="aafab-123">Type</span></span>   | <span data-ttu-id="aafab-124">説明</span><span class="sxs-lookup"><span data-stu-id="aafab-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="aafab-125">period</span><span class="sxs-lookup"><span data-stu-id="aafab-125">period</span></span>    | <span data-ttu-id="aafab-126">文字列</span><span class="sxs-lookup"><span data-stu-id="aafab-126">string</span></span> | <span data-ttu-id="aafab-127">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="aafab-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="aafab-128">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="aafab-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="aafab-129">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="aafab-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="aafab-130">必須。</span><span class="sxs-lookup"><span data-stu-id="aafab-130">Required.</span></span> |

<span data-ttu-id="aafab-131">このメソッドは、 `$format`応答をカスタマイズするための[OData クエリパラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="aafab-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="aafab-132">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="aafab-132">The default output type is text/csv.</span></span> <span data-ttu-id="aafab-133">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="aafab-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aafab-134">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="aafab-134">Request headers</span></span>

| <span data-ttu-id="aafab-135">名前</span><span class="sxs-lookup"><span data-stu-id="aafab-135">Name</span></span>          | <span data-ttu-id="aafab-136">説明</span><span class="sxs-lookup"><span data-stu-id="aafab-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="aafab-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="aafab-137">Authorization</span></span> | <span data-ttu-id="aafab-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="aafab-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="aafab-140">応答</span><span class="sxs-lookup"><span data-stu-id="aafab-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="aafab-141">CSV</span><span class="sxs-lookup"><span data-stu-id="aafab-141">CSV</span></span>

<span data-ttu-id="aafab-142">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="aafab-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="aafab-143">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="aafab-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="aafab-144">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="aafab-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="aafab-145">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="aafab-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="aafab-146">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="aafab-146">Report Refresh Date</span></span>
- <span data-ttu-id="aafab-147">サイトの種類</span><span class="sxs-lookup"><span data-stu-id="aafab-147">Site Type</span></span>
- <span data-ttu-id="aafab-148">合計</span><span class="sxs-lookup"><span data-stu-id="aafab-148">Total</span></span>
- <span data-ttu-id="aafab-149">アクティブ</span><span class="sxs-lookup"><span data-stu-id="aafab-149">Active</span></span>
- <span data-ttu-id="aafab-150">レポート日付</span><span class="sxs-lookup"><span data-stu-id="aafab-150">Report Date</span></span>
- <span data-ttu-id="aafab-151">レポート期間</span><span class="sxs-lookup"><span data-stu-id="aafab-151">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="aafab-152">JSON</span><span class="sxs-lookup"><span data-stu-id="aafab-152">JSON</span></span>

<span data-ttu-id="aafab-153">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[Onedrive 使い方 account計数](../resources/onedriveusageaccountcounts.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="aafab-153">If successful, this method returns a `200 OK` response code and a **[oneDriveUsageAccountCounts](../resources/onedriveusageaccountcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aafab-154">例</span><span class="sxs-lookup"><span data-stu-id="aafab-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="aafab-155">CSV</span><span class="sxs-lookup"><span data-stu-id="aafab-155">CSV</span></span>

<span data-ttu-id="aafab-156">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="aafab-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="aafab-157">要求</span><span class="sxs-lookup"><span data-stu-id="aafab-157">Request</span></span>

<span data-ttu-id="aafab-158">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="aafab-158">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="aafab-159">プロトコル</span><span class="sxs-lookup"><span data-stu-id="aafab-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountcounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="aafab-160">C#</span><span class="sxs-lookup"><span data-stu-id="aafab-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveusageaccountcounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="aafab-161">Javascript</span><span class="sxs-lookup"><span data-stu-id="aafab-161">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveusageaccountcounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="aafab-162">目的-C</span><span class="sxs-lookup"><span data-stu-id="aafab-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveusageaccountcounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="aafab-163">応答</span><span class="sxs-lookup"><span data-stu-id="aafab-163">Response</span></span>

<span data-ttu-id="aafab-164">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="aafab-164">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="aafab-165">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="aafab-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Total,Active,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="aafab-166">JSON</span><span class="sxs-lookup"><span data-stu-id="aafab-166">JSON</span></span>

<span data-ttu-id="aafab-167">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="aafab-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="aafab-168">要求</span><span class="sxs-lookup"><span data-stu-id="aafab-168">Request</span></span>

<span data-ttu-id="aafab-169">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="aafab-169">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="aafab-170">プロトコル</span><span class="sxs-lookup"><span data-stu-id="aafab-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountcounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="aafab-171">C#</span><span class="sxs-lookup"><span data-stu-id="aafab-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveusageaccountcounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="aafab-172">Javascript</span><span class="sxs-lookup"><span data-stu-id="aafab-172">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveusageaccountcounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="aafab-173">目的-C</span><span class="sxs-lookup"><span data-stu-id="aafab-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveusageaccountcounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="aafab-174">応答</span><span class="sxs-lookup"><span data-stu-id="aafab-174">Response</span></span>

<span data-ttu-id="aafab-175">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="aafab-175">The following is an example of the response.</span></span>

> <span data-ttu-id="aafab-p108">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="aafab-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oneDriveUsageAccountCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 249

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.oneDriveUsageAccountCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteType": "All", 
      "total": 207, 
      "active": 89, 
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
