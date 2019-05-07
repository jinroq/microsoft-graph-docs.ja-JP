---
title: 'reportRoot: getYammerDeviceUsageUserCounts'
description: デバイスの種類別に日次ユーザーの数を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: aa5b73442c276c188ced793a45d8f60494b6f744
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33639055"
---
# <a name="reportroot-getyammerdeviceusageusercounts"></a><span data-ttu-id="8c315-103">reportRoot: getYammerDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="8c315-103">reportRoot: getYammerDeviceUsageUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c315-104">デバイスの種類別に日次ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="8c315-104">Get the number of daily users by device type.</span></span>

> <span data-ttu-id="8c315-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer デバイスの使用状況](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8c315-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="8c315-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8c315-106">Permissions</span></span>

<span data-ttu-id="8c315-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8c315-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8c315-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8c315-109">Permission type</span></span>                        | <span data-ttu-id="8c315-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8c315-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="8c315-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="8c315-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8c315-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8c315-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="8c315-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8c315-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c315-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8c315-114">Not supported.</span></span>                           |
| <span data-ttu-id="8c315-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8c315-115">Application</span></span>                            | <span data-ttu-id="8c315-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8c315-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="8c315-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8c315-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="8c315-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="8c315-118">Function parameters</span></span>

<span data-ttu-id="8c315-119">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="8c315-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="8c315-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="8c315-120">Parameter</span></span> | <span data-ttu-id="8c315-121">型</span><span class="sxs-lookup"><span data-stu-id="8c315-121">Type</span></span>   | <span data-ttu-id="8c315-122">説明</span><span class="sxs-lookup"><span data-stu-id="8c315-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="8c315-123">period</span><span class="sxs-lookup"><span data-stu-id="8c315-123">period</span></span>    | <span data-ttu-id="8c315-124">文字列</span><span class="sxs-lookup"><span data-stu-id="8c315-124">string</span></span> | <span data-ttu-id="8c315-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="8c315-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="8c315-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="8c315-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="8c315-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="8c315-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="8c315-128">必須。</span><span class="sxs-lookup"><span data-stu-id="8c315-128">Required.</span></span> |

<span data-ttu-id="8c315-129">このメソッドは、 `$format`応答をカスタマイズするための[OData クエリパラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="8c315-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="8c315-130">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="8c315-130">The default output type is text/csv.</span></span> <span data-ttu-id="8c315-131">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="8c315-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8c315-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8c315-132">Request headers</span></span>

| <span data-ttu-id="8c315-133">名前</span><span class="sxs-lookup"><span data-stu-id="8c315-133">Name</span></span>          | <span data-ttu-id="8c315-134">説明</span><span class="sxs-lookup"><span data-stu-id="8c315-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="8c315-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c315-135">Authorization</span></span> | <span data-ttu-id="8c315-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8c315-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="8c315-138">応答</span><span class="sxs-lookup"><span data-stu-id="8c315-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="8c315-139">CSV</span><span class="sxs-lookup"><span data-stu-id="8c315-139">CSV</span></span>

<span data-ttu-id="8c315-140">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="8c315-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="8c315-141">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="8c315-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="8c315-142">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="8c315-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="8c315-143">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="8c315-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="8c315-144">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="8c315-144">Report Refresh Date</span></span>
- <span data-ttu-id="8c315-145">Web</span><span class="sxs-lookup"><span data-stu-id="8c315-145">Web</span></span>
- <span data-ttu-id="8c315-146">Windows スマートフォン</span><span class="sxs-lookup"><span data-stu-id="8c315-146">Windows Phone</span></span>
- <span data-ttu-id="8c315-147">Android スマートフォン</span><span class="sxs-lookup"><span data-stu-id="8c315-147">Android Phone</span></span>
- <span data-ttu-id="8c315-148">iPhone</span><span class="sxs-lookup"><span data-stu-id="8c315-148">iPhone</span></span>
- <span data-ttu-id="8c315-149">iPad</span><span class="sxs-lookup"><span data-stu-id="8c315-149">iPad</span></span>
- <span data-ttu-id="8c315-150">その他</span><span class="sxs-lookup"><span data-stu-id="8c315-150">Other</span></span>
- <span data-ttu-id="8c315-151">レポート日付</span><span class="sxs-lookup"><span data-stu-id="8c315-151">Report Date</span></span>
- <span data-ttu-id="8c315-152">レポート期間</span><span class="sxs-lookup"><span data-stu-id="8c315-152">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="8c315-153">JSON</span><span class="sxs-lookup"><span data-stu-id="8c315-153">JSON</span></span>

<span data-ttu-id="8c315-154">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[yammerDeviceUsageUserCounts](../resources/yammerdeviceusageusercounts.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8c315-154">If successful, this method returns a `200 OK` response code and a **[yammerDeviceUsageUserCounts](../resources/yammerdeviceusageusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c315-155">例</span><span class="sxs-lookup"><span data-stu-id="8c315-155">Example</span></span>

### <a name="csv"></a><span data-ttu-id="8c315-156">CSV</span><span class="sxs-lookup"><span data-stu-id="8c315-156">CSV</span></span>

<span data-ttu-id="8c315-157">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8c315-157">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="8c315-158">要求</span><span class="sxs-lookup"><span data-stu-id="8c315-158">Request</span></span>

<span data-ttu-id="8c315-159">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8c315-159">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusageusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="8c315-160">応答</span><span class="sxs-lookup"><span data-stu-id="8c315-160">Response</span></span>

<span data-ttu-id="8c315-161">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8c315-161">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="8c315-162">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="8c315-162">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8c315-163">Visual</span><span class="sxs-lookup"><span data-stu-id="8c315-163">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getyammerdeviceusageusercounts_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8c315-164">Java</span><span class="sxs-lookup"><span data-stu-id="8c315-164">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getyammerdeviceusageusercounts_csv-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="8c315-165">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="8c315-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="8c315-166">JSON</span><span class="sxs-lookup"><span data-stu-id="8c315-166">JSON</span></span>

<span data-ttu-id="8c315-167">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="8c315-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="8c315-168">要求</span><span class="sxs-lookup"><span data-stu-id="8c315-168">Request</span></span>

<span data-ttu-id="8c315-169">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8c315-169">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusageusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="8c315-170">応答</span><span class="sxs-lookup"><span data-stu-id="8c315-170">Response</span></span>

<span data-ttu-id="8c315-171">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8c315-171">The following is an example of the response.</span></span>

> <span data-ttu-id="8c315-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="8c315-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="8c315-174">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="8c315-174">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8c315-175">Visual</span><span class="sxs-lookup"><span data-stu-id="8c315-175">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getyammerdeviceusageusercounts_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8c315-176">Java</span><span class="sxs-lookup"><span data-stu-id="8c315-176">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getyammerdeviceusageusercounts_json-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getyammerdeviceusageusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getyammerdeviceusageusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getyammerdeviceusageusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getyammerdeviceusageusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
