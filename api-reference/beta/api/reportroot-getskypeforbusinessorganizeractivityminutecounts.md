---
title: 'reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts'
description: 組織内のユーザーが開催、企画した電話会議セッションの長さ (分数) と種類に関する使用状況の傾向を取得します。 電話会議セッションの種類には、オーディオ/ビデオ、および Microsoft へのダイヤルインとダイヤルアウトがあります。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 035103416a1d106e49eada0066c4327e47d78730
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35265171"
---
# <a name="reportroot-getskypeforbusinessorganizeractivityminutecounts"></a><span data-ttu-id="3e4a7-104">reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="3e4a7-104">reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e4a7-105">組織内のユーザーが開催、企画した電話会議セッションの長さ (分数) と種類に関する使用状況の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="3e4a7-105">Get usage trends on the length in minutes and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="3e4a7-106">電話会議セッションの種類には、オーディオ/ビデオ、および Microsoft へのダイヤルインとダイヤルアウトがあります。</span><span class="sxs-lookup"><span data-stu-id="3e4a7-106">Types of conference sessions include audio/video, and dial-in and dial-out - Microsoft.</span></span>

> <span data-ttu-id="3e4a7-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Skype for Business 電話会議の開催者のアクティビティ](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3e4a7-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="permissions"></a><span data-ttu-id="3e4a7-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3e4a7-108">Permissions</span></span>

<span data-ttu-id="3e4a7-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3e4a7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3e4a7-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3e4a7-111">Permission type</span></span>                        | <span data-ttu-id="3e4a7-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3e4a7-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="3e4a7-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="3e4a7-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="3e4a7-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3e4a7-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="3e4a7-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3e4a7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e4a7-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3e4a7-116">Not supported.</span></span>                           |
| <span data-ttu-id="3e4a7-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3e4a7-117">Application</span></span>                            | <span data-ttu-id="3e4a7-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3e4a7-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="3e4a7-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3e4a7-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessOrganizerActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="3e4a7-120">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="3e4a7-120">Function parameters</span></span>

<span data-ttu-id="3e4a7-121">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="3e4a7-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="3e4a7-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="3e4a7-122">Parameter</span></span> | <span data-ttu-id="3e4a7-123">型</span><span class="sxs-lookup"><span data-stu-id="3e4a7-123">Type</span></span>   | <span data-ttu-id="3e4a7-124">説明</span><span class="sxs-lookup"><span data-stu-id="3e4a7-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="3e4a7-125">period</span><span class="sxs-lookup"><span data-stu-id="3e4a7-125">period</span></span>    | <span data-ttu-id="3e4a7-126">文字列</span><span class="sxs-lookup"><span data-stu-id="3e4a7-126">string</span></span> | <span data-ttu-id="3e4a7-127">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="3e4a7-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="3e4a7-128">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="3e4a7-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="3e4a7-129">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="3e4a7-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="3e4a7-130">必須。</span><span class="sxs-lookup"><span data-stu-id="3e4a7-130">Required.</span></span> |

<span data-ttu-id="3e4a7-131">このメソッドは、 `$format`応答をカスタマイズするための[OData クエリパラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="3e4a7-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="3e4a7-132">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="3e4a7-132">The default output type is text/csv.</span></span> <span data-ttu-id="3e4a7-133">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="3e4a7-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3e4a7-134">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3e4a7-134">Request headers</span></span>

| <span data-ttu-id="3e4a7-135">名前</span><span class="sxs-lookup"><span data-stu-id="3e4a7-135">Name</span></span>          | <span data-ttu-id="3e4a7-136">説明</span><span class="sxs-lookup"><span data-stu-id="3e4a7-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="3e4a7-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e4a7-137">Authorization</span></span> | <span data-ttu-id="3e4a7-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3e4a7-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="3e4a7-140">応答</span><span class="sxs-lookup"><span data-stu-id="3e4a7-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="3e4a7-141">CSV</span><span class="sxs-lookup"><span data-stu-id="3e4a7-141">CSV</span></span>

<span data-ttu-id="3e4a7-142">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="3e4a7-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="3e4a7-143">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="3e4a7-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="3e4a7-144">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="3e4a7-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="3e4a7-145">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="3e4a7-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="3e4a7-146">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="3e4a7-146">Report Refresh Date</span></span>
- <span data-ttu-id="3e4a7-147">レポート日付</span><span class="sxs-lookup"><span data-stu-id="3e4a7-147">Report Date</span></span>
- <span data-ttu-id="3e4a7-148">レポート期間</span><span class="sxs-lookup"><span data-stu-id="3e4a7-148">Report Period</span></span>
- <span data-ttu-id="3e4a7-149">オーディオ/ビデオ</span><span class="sxs-lookup"><span data-stu-id="3e4a7-149">Audio/Video</span></span>
- <span data-ttu-id="3e4a7-150">Microsoft へのダイヤルイン</span><span class="sxs-lookup"><span data-stu-id="3e4a7-150">Dial-in Microsoft</span></span>
- <span data-ttu-id="3e4a7-151">Microsoft からダイヤルアウト</span><span class="sxs-lookup"><span data-stu-id="3e4a7-151">Dial-out Microsoft</span></span>

### <a name="json"></a><span data-ttu-id="3e4a7-152">JSON</span><span class="sxs-lookup"><span data-stu-id="3e4a7-152">JSON</span></span>

<span data-ttu-id="3e4a7-153">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[skypeForBusinessOrganizerActivityMinuteCounts](../resources/skypeforbusinessorganizeractivityminutecounts.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3e4a7-153">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessOrganizerActivityMinuteCounts](../resources/skypeforbusinessorganizeractivityminutecounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e4a7-154">例</span><span class="sxs-lookup"><span data-stu-id="3e4a7-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="3e4a7-155">CSV</span><span class="sxs-lookup"><span data-stu-id="3e4a7-155">CSV</span></span>

<span data-ttu-id="3e4a7-156">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3e4a7-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="3e4a7-157">要求</span><span class="sxs-lookup"><span data-stu-id="3e4a7-157">Request</span></span>

<span data-ttu-id="3e4a7-158">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3e4a7-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessorganizeractivityminutecounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessOrganizerActivityMinuteCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="3e4a7-159">応答</span><span class="sxs-lookup"><span data-stu-id="3e4a7-159">Response</span></span>

<span data-ttu-id="3e4a7-160">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3e4a7-160">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="3e4a7-161">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="3e4a7-161">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3e4a7-162">C#</span><span class="sxs-lookup"><span data-stu-id="3e4a7-162">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessorganizeractivityminutecounts_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3e4a7-163">Javascript</span><span class="sxs-lookup"><span data-stu-id="3e4a7-163">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessorganizeractivityminutecounts_csv-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3e4a7-164">目的-C</span><span class="sxs-lookup"><span data-stu-id="3e4a7-164">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessorganizeractivityminutecounts_csv-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="3e4a7-165">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="3e4a7-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Audio/Video,Dial-in Microsoft,Dial-out Microsoft
```

### <a name="json"></a><span data-ttu-id="3e4a7-166">JSON</span><span class="sxs-lookup"><span data-stu-id="3e4a7-166">JSON</span></span>

<span data-ttu-id="3e4a7-167">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="3e4a7-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="3e4a7-168">要求</span><span class="sxs-lookup"><span data-stu-id="3e4a7-168">Request</span></span>

<span data-ttu-id="3e4a7-169">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3e4a7-169">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessorganizeractivityminutecounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessOrganizerActivityMinuteCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="3e4a7-170">応答</span><span class="sxs-lookup"><span data-stu-id="3e4a7-170">Response</span></span>

<span data-ttu-id="3e4a7-171">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3e4a7-171">The following is an example of the response.</span></span>

> <span data-ttu-id="3e4a7-p108">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="3e4a7-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessOrganizerActivityMinuteCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 288

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessOrganizerActivityMinuteCounts)", 
  "value": [
    {
      "audioVideo": 1912, 
      "dialInMicrosoft": 108, 
      "dialOutMicrosoft": 0, 
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="3e4a7-174">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="3e4a7-174">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3e4a7-175">C#</span><span class="sxs-lookup"><span data-stu-id="3e4a7-175">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessorganizeractivityminutecounts_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3e4a7-176">Javascript</span><span class="sxs-lookup"><span data-stu-id="3e4a7-176">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessorganizeractivityminutecounts_json-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3e4a7-177">目的-C</span><span class="sxs-lookup"><span data-stu-id="3e4a7-177">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessorganizeractivityminutecounts_json-Objective-C-snippets.md)]
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
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessorganizeractivityminutecounts.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessorganizeractivityminutecounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessorganizeractivityminutecounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessorganizeractivityminutecounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessorganizeractivityminutecounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
