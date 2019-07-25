---
title: 'reportRoot: getYammerDeviceUsageUserCounts'
description: デバイスの種類別に日次ユーザーの数を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 7982a1211e5dc714a76cdf188981e930952e6761
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871532"
---
# <a name="reportroot-getyammerdeviceusageusercounts"></a><span data-ttu-id="a4244-103">reportRoot: getYammerDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="a4244-103">reportRoot: getYammerDeviceUsageUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4244-104">デバイスの種類別に日次ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="a4244-104">Get the number of daily users by device type.</span></span>

> <span data-ttu-id="a4244-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer デバイスの使用状況](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a4244-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="a4244-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a4244-106">Permissions</span></span>

<span data-ttu-id="a4244-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a4244-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a4244-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a4244-109">Permission type</span></span>                        | <span data-ttu-id="a4244-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a4244-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="a4244-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="a4244-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a4244-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a4244-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="a4244-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a4244-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4244-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a4244-114">Not supported.</span></span>                           |
| <span data-ttu-id="a4244-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a4244-115">Application</span></span>                            | <span data-ttu-id="a4244-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a4244-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="a4244-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a4244-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="a4244-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="a4244-118">Function parameters</span></span>

<span data-ttu-id="a4244-119">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="a4244-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="a4244-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="a4244-120">Parameter</span></span> | <span data-ttu-id="a4244-121">型</span><span class="sxs-lookup"><span data-stu-id="a4244-121">Type</span></span>   | <span data-ttu-id="a4244-122">説明</span><span class="sxs-lookup"><span data-stu-id="a4244-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="a4244-123">period</span><span class="sxs-lookup"><span data-stu-id="a4244-123">period</span></span>    | <span data-ttu-id="a4244-124">文字列</span><span class="sxs-lookup"><span data-stu-id="a4244-124">string</span></span> | <span data-ttu-id="a4244-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="a4244-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="a4244-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="a4244-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="a4244-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="a4244-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="a4244-128">必須。</span><span class="sxs-lookup"><span data-stu-id="a4244-128">Required.</span></span> |

<span data-ttu-id="a4244-129">このメソッドは、 `$format`応答をカスタマイズするための[OData クエリパラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="a4244-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="a4244-130">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="a4244-130">The default output type is text/csv.</span></span> <span data-ttu-id="a4244-131">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="a4244-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a4244-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a4244-132">Request headers</span></span>

| <span data-ttu-id="a4244-133">名前</span><span class="sxs-lookup"><span data-stu-id="a4244-133">Name</span></span>          | <span data-ttu-id="a4244-134">説明</span><span class="sxs-lookup"><span data-stu-id="a4244-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="a4244-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4244-135">Authorization</span></span> | <span data-ttu-id="a4244-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a4244-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="a4244-138">応答</span><span class="sxs-lookup"><span data-stu-id="a4244-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="a4244-139">CSV</span><span class="sxs-lookup"><span data-stu-id="a4244-139">CSV</span></span>

<span data-ttu-id="a4244-140">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="a4244-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="a4244-141">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="a4244-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="a4244-142">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="a4244-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="a4244-143">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="a4244-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="a4244-144">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="a4244-144">Report Refresh Date</span></span>
- <span data-ttu-id="a4244-145">Web</span><span class="sxs-lookup"><span data-stu-id="a4244-145">Web</span></span>
- <span data-ttu-id="a4244-146">Windows スマートフォン</span><span class="sxs-lookup"><span data-stu-id="a4244-146">Windows Phone</span></span>
- <span data-ttu-id="a4244-147">Android スマートフォン</span><span class="sxs-lookup"><span data-stu-id="a4244-147">Android Phone</span></span>
- <span data-ttu-id="a4244-148">iPhone</span><span class="sxs-lookup"><span data-stu-id="a4244-148">iPhone</span></span>
- <span data-ttu-id="a4244-149">iPad</span><span class="sxs-lookup"><span data-stu-id="a4244-149">iPad</span></span>
- <span data-ttu-id="a4244-150">その他</span><span class="sxs-lookup"><span data-stu-id="a4244-150">Other</span></span>
- <span data-ttu-id="a4244-151">レポート日付</span><span class="sxs-lookup"><span data-stu-id="a4244-151">Report Date</span></span>
- <span data-ttu-id="a4244-152">レポート期間</span><span class="sxs-lookup"><span data-stu-id="a4244-152">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="a4244-153">JSON</span><span class="sxs-lookup"><span data-stu-id="a4244-153">JSON</span></span>

<span data-ttu-id="a4244-154">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[yammerDeviceUsageUserCounts](../resources/yammerdeviceusageusercounts.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a4244-154">If successful, this method returns a `200 OK` response code and a **[yammerDeviceUsageUserCounts](../resources/yammerdeviceusageusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4244-155">例</span><span class="sxs-lookup"><span data-stu-id="a4244-155">Example</span></span>

### <a name="csv"></a><span data-ttu-id="a4244-156">CSV</span><span class="sxs-lookup"><span data-stu-id="a4244-156">CSV</span></span>

<span data-ttu-id="a4244-157">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a4244-157">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="a4244-158">要求</span><span class="sxs-lookup"><span data-stu-id="a4244-158">Request</span></span>

<span data-ttu-id="a4244-159">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a4244-159">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a4244-160">プロトコル</span><span class="sxs-lookup"><span data-stu-id="a4244-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusageusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a4244-161">C#</span><span class="sxs-lookup"><span data-stu-id="a4244-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammerdeviceusageusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a4244-162">Javascript</span><span class="sxs-lookup"><span data-stu-id="a4244-162">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammerdeviceusageusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a4244-163">目的-C</span><span class="sxs-lookup"><span data-stu-id="a4244-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammerdeviceusageusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a4244-164">Java</span><span class="sxs-lookup"><span data-stu-id="a4244-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getyammerdeviceusageusercounts-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a4244-165">応答</span><span class="sxs-lookup"><span data-stu-id="a4244-165">Response</span></span>

<span data-ttu-id="a4244-166">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a4244-166">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="a4244-167">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="a4244-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iPhone,iPad,Other,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="a4244-168">JSON</span><span class="sxs-lookup"><span data-stu-id="a4244-168">JSON</span></span>

<span data-ttu-id="a4244-169">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="a4244-169">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="a4244-170">要求</span><span class="sxs-lookup"><span data-stu-id="a4244-170">Request</span></span>

<span data-ttu-id="a4244-171">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a4244-171">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a4244-172">プロトコル</span><span class="sxs-lookup"><span data-stu-id="a4244-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusageusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a4244-173">C#</span><span class="sxs-lookup"><span data-stu-id="a4244-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammerdeviceusageusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a4244-174">Javascript</span><span class="sxs-lookup"><span data-stu-id="a4244-174">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammerdeviceusageusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a4244-175">目的-C</span><span class="sxs-lookup"><span data-stu-id="a4244-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammerdeviceusageusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a4244-176">Java</span><span class="sxs-lookup"><span data-stu-id="a4244-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getyammerdeviceusageusercounts-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a4244-177">応答</span><span class="sxs-lookup"><span data-stu-id="a4244-177">Response</span></span>

<span data-ttu-id="a4244-178">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a4244-178">The following is an example of the response.</span></span>

> <span data-ttu-id="a4244-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="a4244-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerDeviceUsageUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 284

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerDeviceUsageUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "web": 63, 
      "windowsPhone": 1, 
      "androidPhone": 17, 
      "iPhone": 23, 
      "iPad": 1, 
      "other": 2, 
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
