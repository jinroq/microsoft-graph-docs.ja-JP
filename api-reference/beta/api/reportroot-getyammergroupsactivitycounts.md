---
title: 'reportRoot: getYammerGroupsActivityCounts'
description: グループ内で投稿、読み取り、および「いいね!」を付けた Yammer メッセージの数を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 5c57553d7619fa9202f1f02f15054d2c950752af
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33639090"
---
# <a name="reportroot-getyammergroupsactivitycounts"></a><span data-ttu-id="444a3-103">reportRoot: getYammerGroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="444a3-103">reportRoot: getYammerGroupsActivityCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="444a3-104">グループ内で投稿、読み取り、および「いいね!」を付けた Yammer メッセージの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="444a3-104">Get the number of Yammer messages posted, read, and liked in groups.</span></span>

> <span data-ttu-id="444a3-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer グループ アクティビティ](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="444a3-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="permissions"></a><span data-ttu-id="444a3-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="444a3-106">Permissions</span></span>

<span data-ttu-id="444a3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="444a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="444a3-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="444a3-109">Permission type</span></span>                        | <span data-ttu-id="444a3-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="444a3-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="444a3-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="444a3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="444a3-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="444a3-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="444a3-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="444a3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="444a3-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="444a3-114">Not supported.</span></span>                           |
| <span data-ttu-id="444a3-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="444a3-115">Application</span></span>                            | <span data-ttu-id="444a3-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="444a3-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="444a3-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="444a3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="444a3-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="444a3-118">Function parameters</span></span>

<span data-ttu-id="444a3-119">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="444a3-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="444a3-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="444a3-120">Parameter</span></span> | <span data-ttu-id="444a3-121">型</span><span class="sxs-lookup"><span data-stu-id="444a3-121">Type</span></span>   | <span data-ttu-id="444a3-122">説明</span><span class="sxs-lookup"><span data-stu-id="444a3-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="444a3-123">period</span><span class="sxs-lookup"><span data-stu-id="444a3-123">period</span></span>    | <span data-ttu-id="444a3-124">文字列</span><span class="sxs-lookup"><span data-stu-id="444a3-124">string</span></span> | <span data-ttu-id="444a3-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="444a3-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="444a3-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="444a3-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="444a3-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="444a3-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="444a3-128">必須。</span><span class="sxs-lookup"><span data-stu-id="444a3-128">Required.</span></span> |

<span data-ttu-id="444a3-129">このメソッドは、 `$format`応答をカスタマイズするための[OData クエリパラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="444a3-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="444a3-130">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="444a3-130">The default output type is text/csv.</span></span> <span data-ttu-id="444a3-131">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="444a3-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="444a3-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="444a3-132">Request headers</span></span>

| <span data-ttu-id="444a3-133">名前</span><span class="sxs-lookup"><span data-stu-id="444a3-133">Name</span></span>          | <span data-ttu-id="444a3-134">説明</span><span class="sxs-lookup"><span data-stu-id="444a3-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="444a3-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="444a3-135">Authorization</span></span> | <span data-ttu-id="444a3-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="444a3-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="444a3-138">応答</span><span class="sxs-lookup"><span data-stu-id="444a3-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="444a3-139">CSV</span><span class="sxs-lookup"><span data-stu-id="444a3-139">CSV</span></span>

<span data-ttu-id="444a3-140">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="444a3-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="444a3-141">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="444a3-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="444a3-142">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="444a3-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="444a3-143">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="444a3-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="444a3-144">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="444a3-144">Report Refresh Date</span></span>
- <span data-ttu-id="444a3-145">いいね!</span><span class="sxs-lookup"><span data-stu-id="444a3-145">Liked</span></span>
- <span data-ttu-id="444a3-146">投稿</span><span class="sxs-lookup"><span data-stu-id="444a3-146">Posted</span></span>
- <span data-ttu-id="444a3-147">読み取り</span><span class="sxs-lookup"><span data-stu-id="444a3-147">Read</span></span>
- <span data-ttu-id="444a3-148">レポート日付</span><span class="sxs-lookup"><span data-stu-id="444a3-148">Report Date</span></span>
- <span data-ttu-id="444a3-149">レポート期間</span><span class="sxs-lookup"><span data-stu-id="444a3-149">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="444a3-150">JSON</span><span class="sxs-lookup"><span data-stu-id="444a3-150">JSON</span></span>

<span data-ttu-id="444a3-151">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[yammerGroupsActivityCounts](../resources/yammergroupsactivitycounts.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="444a3-151">If successful, this method returns a `200 OK` response code and a **[yammerGroupsActivityCounts](../resources/yammergroupsactivitycounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="444a3-152">例</span><span class="sxs-lookup"><span data-stu-id="444a3-152">Example</span></span>

### <a name="csv"></a><span data-ttu-id="444a3-153">CSV</span><span class="sxs-lookup"><span data-stu-id="444a3-153">CSV</span></span>

<span data-ttu-id="444a3-154">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="444a3-154">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="444a3-155">要求</span><span class="sxs-lookup"><span data-stu-id="444a3-155">Request</span></span>

<span data-ttu-id="444a3-156">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="444a3-156">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="444a3-157">応答</span><span class="sxs-lookup"><span data-stu-id="444a3-157">Response</span></span>

<span data-ttu-id="444a3-158">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="444a3-158">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="444a3-159">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="444a3-159">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="444a3-160">Visual</span><span class="sxs-lookup"><span data-stu-id="444a3-160">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getyammergroupsactivitycounts_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="444a3-161">Java</span><span class="sxs-lookup"><span data-stu-id="444a3-161">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getyammergroupsactivitycounts_csv-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="444a3-162">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="444a3-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Liked,Posted,Read,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="444a3-163">JSON</span><span class="sxs-lookup"><span data-stu-id="444a3-163">JSON</span></span>

<span data-ttu-id="444a3-164">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="444a3-164">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="444a3-165">要求</span><span class="sxs-lookup"><span data-stu-id="444a3-165">Request</span></span>

<span data-ttu-id="444a3-166">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="444a3-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="444a3-167">応答</span><span class="sxs-lookup"><span data-stu-id="444a3-167">Response</span></span>

<span data-ttu-id="444a3-168">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="444a3-168">The following is an example of the response.</span></span>

> <span data-ttu-id="444a3-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="444a3-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerGroupsActivityCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 241

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerGroupsActivityCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "liked": 13, 
      "posted": 50, 
      "read": 69, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="444a3-171">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="444a3-171">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="444a3-172">Visual</span><span class="sxs-lookup"><span data-stu-id="444a3-172">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getyammergroupsactivitycounts_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="444a3-173">Java</span><span class="sxs-lookup"><span data-stu-id="444a3-173">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getyammergroupsactivitycounts_json-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/reportroot-getyammergroupsactivitycounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getyammergroupsactivitycounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getyammergroupsactivitycounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getyammergroupsactivitycounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
