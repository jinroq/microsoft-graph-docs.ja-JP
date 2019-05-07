---
title: 'reportRoot: getSharePointSiteUsageFileCounts'
description: すべてのサイトのファイルの合計数と、アクティブ ファイルの数を取得します。 ファイル (ユーザーまたはシステム) は、一定期間中に保存、同期、変更、共有されるとアクティブとみなされます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: bdab1abcc25b0c11e7f89d49b02e792907cf65e7
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33639293"
---
# <a name="reportroot-getsharepointsiteusagefilecounts"></a><span data-ttu-id="726b4-104">reportRoot: getSharePointSiteUsageFileCounts</span><span class="sxs-lookup"><span data-stu-id="726b4-104">reportRoot: getSharePointSiteUsageFileCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="726b4-105">すべてのサイトのファイルの合計数と、アクティブ ファイルの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="726b4-105">Get the total number of files across all sites and the number of active files.</span></span> <span data-ttu-id="726b4-106">ファイル (ユーザーまたはシステム) は、一定期間中に保存、同期、変更、共有されるとアクティブとみなされます。</span><span class="sxs-lookup"><span data-stu-id="726b4-106">A file (user or system) is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span>

> <span data-ttu-id="726b4-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: SharePoint サイトの使用状況](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="726b4-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="726b4-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="726b4-108">Permissions</span></span>

<span data-ttu-id="726b4-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="726b4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="726b4-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="726b4-111">Permission type</span></span>                        | <span data-ttu-id="726b4-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="726b4-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="726b4-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="726b4-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="726b4-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="726b4-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="726b4-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="726b4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="726b4-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="726b4-116">Not supported.</span></span>                           |
| <span data-ttu-id="726b4-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="726b4-117">Application</span></span>                            | <span data-ttu-id="726b4-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="726b4-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="726b4-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="726b4-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="726b4-120">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="726b4-120">Function parameters</span></span>

<span data-ttu-id="726b4-121">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="726b4-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="726b4-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="726b4-122">Parameter</span></span> | <span data-ttu-id="726b4-123">型</span><span class="sxs-lookup"><span data-stu-id="726b4-123">Type</span></span>   | <span data-ttu-id="726b4-124">説明</span><span class="sxs-lookup"><span data-stu-id="726b4-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="726b4-125">period</span><span class="sxs-lookup"><span data-stu-id="726b4-125">period</span></span>    | <span data-ttu-id="726b4-126">文字列</span><span class="sxs-lookup"><span data-stu-id="726b4-126">string</span></span> | <span data-ttu-id="726b4-127">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="726b4-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="726b4-128">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="726b4-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="726b4-129">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="726b4-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="726b4-130">必須。</span><span class="sxs-lookup"><span data-stu-id="726b4-130">Required.</span></span> |

<span data-ttu-id="726b4-131">このメソッドは、 `$format`応答をカスタマイズするための[OData クエリパラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="726b4-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="726b4-132">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="726b4-132">The default output type is text/csv.</span></span> <span data-ttu-id="726b4-133">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="726b4-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="726b4-134">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="726b4-134">Request headers</span></span>

| <span data-ttu-id="726b4-135">名前</span><span class="sxs-lookup"><span data-stu-id="726b4-135">Name</span></span>          | <span data-ttu-id="726b4-136">説明</span><span class="sxs-lookup"><span data-stu-id="726b4-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="726b4-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="726b4-137">Authorization</span></span> | <span data-ttu-id="726b4-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="726b4-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="726b4-140">応答</span><span class="sxs-lookup"><span data-stu-id="726b4-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="726b4-141">CSV</span><span class="sxs-lookup"><span data-stu-id="726b4-141">CSV</span></span>

<span data-ttu-id="726b4-142">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="726b4-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="726b4-143">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="726b4-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="726b4-144">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="726b4-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="726b4-145">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="726b4-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="726b4-146">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="726b4-146">Report Refresh Date</span></span>
- <span data-ttu-id="726b4-147">サイトの種類</span><span class="sxs-lookup"><span data-stu-id="726b4-147">Site Type</span></span>
- <span data-ttu-id="726b4-148">合計</span><span class="sxs-lookup"><span data-stu-id="726b4-148">Total</span></span>
- <span data-ttu-id="726b4-149">アクティブ</span><span class="sxs-lookup"><span data-stu-id="726b4-149">Active</span></span>
- <span data-ttu-id="726b4-150">レポート日付</span><span class="sxs-lookup"><span data-stu-id="726b4-150">Report Date</span></span>
- <span data-ttu-id="726b4-151">レポート期間</span><span class="sxs-lookup"><span data-stu-id="726b4-151">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="726b4-152">JSON</span><span class="sxs-lookup"><span data-stu-id="726b4-152">JSON</span></span>

<span data-ttu-id="726b4-153">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[sharePointSiteUsageFileCounts](../resources/sharepointsiteusagefilecounts.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="726b4-153">If successful, this method returns a `200 OK` response code and a **[sharePointSiteUsageFileCounts](../resources/sharepointsiteusagefilecounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="726b4-154">例</span><span class="sxs-lookup"><span data-stu-id="726b4-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="726b4-155">CSV</span><span class="sxs-lookup"><span data-stu-id="726b4-155">CSV</span></span>

<span data-ttu-id="726b4-156">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="726b4-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="726b4-157">要求</span><span class="sxs-lookup"><span data-stu-id="726b4-157">Request</span></span>

<span data-ttu-id="726b4-158">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="726b4-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagefilecounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageFileCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="726b4-159">応答</span><span class="sxs-lookup"><span data-stu-id="726b4-159">Response</span></span>

<span data-ttu-id="726b4-160">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="726b4-160">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="726b4-161">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="726b4-161">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="726b4-162">Visual</span><span class="sxs-lookup"><span data-stu-id="726b4-162">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getsharepointsiteusagefilecounts_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="726b4-163">Java</span><span class="sxs-lookup"><span data-stu-id="726b4-163">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getsharepointsiteusagefilecounts_csv-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="726b4-164">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="726b4-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="726b4-165">JSON</span><span class="sxs-lookup"><span data-stu-id="726b4-165">JSON</span></span>

<span data-ttu-id="726b4-166">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="726b4-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="726b4-167">要求</span><span class="sxs-lookup"><span data-stu-id="726b4-167">Request</span></span>

<span data-ttu-id="726b4-168">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="726b4-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagefilecounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageFileCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="726b4-169">応答</span><span class="sxs-lookup"><span data-stu-id="726b4-169">Response</span></span>

<span data-ttu-id="726b4-170">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="726b4-170">The following is an example of the response.</span></span>

> <span data-ttu-id="726b4-p108">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="726b4-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointSiteUsageFileCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 255

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.sharePointSiteUsageFileCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteType": "All", 
      "total": 25687, 
      "active": 209, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="726b4-173">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="726b4-173">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="726b4-174">Visual</span><span class="sxs-lookup"><span data-stu-id="726b4-174">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getsharepointsiteusagefilecounts_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="726b4-175">Java</span><span class="sxs-lookup"><span data-stu-id="726b4-175">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getsharepointsiteusagefilecounts_json-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/reportroot-getsharepointsiteusagefilecounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getsharepointsiteusagefilecounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getsharepointsiteusagefilecounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getsharepointsiteusagefilecounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
