---
title: 'reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts'
description: 組織内のユーザーが開催、企画した電話会議セッションの長さ (分数) と種類に関する使用状況の傾向を取得します。 電話会議セッションの種類には、オーディオ/ビデオ、および Microsoft へのダイヤルインとダイヤルアウトがあります。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 302340f7bdb939bcdb2b11c80f03fac4ad05099e
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36411285"
---
# <a name="reportroot-getskypeforbusinessorganizeractivityminutecounts"></a><span data-ttu-id="00509-104">reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="00509-104">reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00509-105">組織内のユーザーが開催、企画した電話会議セッションの長さ (分数) と種類に関する使用状況の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="00509-105">Get usage trends on the length in minutes and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="00509-106">電話会議セッションの種類には、オーディオ/ビデオ、および Microsoft へのダイヤルインとダイヤルアウトがあります。</span><span class="sxs-lookup"><span data-stu-id="00509-106">Types of conference sessions include audio/video, and dial-in and dial-out - Microsoft.</span></span>

> <span data-ttu-id="00509-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Skype for Business 電話会議の開催者のアクティビティ](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="00509-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="permissions"></a><span data-ttu-id="00509-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="00509-108">Permissions</span></span>

<span data-ttu-id="00509-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="00509-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="00509-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="00509-111">Permission type</span></span>                        | <span data-ttu-id="00509-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="00509-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="00509-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="00509-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="00509-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="00509-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="00509-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="00509-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00509-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="00509-116">Not supported.</span></span>                           |
| <span data-ttu-id="00509-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="00509-117">Application</span></span>                            | <span data-ttu-id="00509-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="00509-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="00509-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="00509-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessOrganizerActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="00509-120">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="00509-120">Function parameters</span></span>

<span data-ttu-id="00509-121">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="00509-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="00509-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="00509-122">Parameter</span></span> | <span data-ttu-id="00509-123">型</span><span class="sxs-lookup"><span data-stu-id="00509-123">Type</span></span>   | <span data-ttu-id="00509-124">説明</span><span class="sxs-lookup"><span data-stu-id="00509-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="00509-125">period</span><span class="sxs-lookup"><span data-stu-id="00509-125">period</span></span>    | <span data-ttu-id="00509-126">文字列</span><span class="sxs-lookup"><span data-stu-id="00509-126">string</span></span> | <span data-ttu-id="00509-127">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="00509-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="00509-128">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="00509-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="00509-129">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="00509-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="00509-130">必須。</span><span class="sxs-lookup"><span data-stu-id="00509-130">Required.</span></span> |

<span data-ttu-id="00509-131">このメソッドは、 `$format`応答をカスタマイズするための[OData クエリパラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="00509-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="00509-132">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="00509-132">The default output type is text/csv.</span></span> <span data-ttu-id="00509-133">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="00509-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="00509-134">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="00509-134">Request headers</span></span>

| <span data-ttu-id="00509-135">名前</span><span class="sxs-lookup"><span data-stu-id="00509-135">Name</span></span>          | <span data-ttu-id="00509-136">説明</span><span class="sxs-lookup"><span data-stu-id="00509-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="00509-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="00509-137">Authorization</span></span> | <span data-ttu-id="00509-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="00509-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="00509-140">応答</span><span class="sxs-lookup"><span data-stu-id="00509-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="00509-141">CSV</span><span class="sxs-lookup"><span data-stu-id="00509-141">CSV</span></span>

<span data-ttu-id="00509-142">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="00509-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="00509-143">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="00509-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="00509-144">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="00509-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="00509-145">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="00509-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="00509-146">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="00509-146">Report Refresh Date</span></span>
- <span data-ttu-id="00509-147">レポート日付</span><span class="sxs-lookup"><span data-stu-id="00509-147">Report Date</span></span>
- <span data-ttu-id="00509-148">レポート期間</span><span class="sxs-lookup"><span data-stu-id="00509-148">Report Period</span></span>
- <span data-ttu-id="00509-149">オーディオ/ビデオ</span><span class="sxs-lookup"><span data-stu-id="00509-149">Audio/Video</span></span>
- <span data-ttu-id="00509-150">Microsoft へのダイヤルイン</span><span class="sxs-lookup"><span data-stu-id="00509-150">Dial-in Microsoft</span></span>
- <span data-ttu-id="00509-151">Microsoft からダイヤルアウト</span><span class="sxs-lookup"><span data-stu-id="00509-151">Dial-out Microsoft</span></span>

### <a name="json"></a><span data-ttu-id="00509-152">JSON</span><span class="sxs-lookup"><span data-stu-id="00509-152">JSON</span></span>

<span data-ttu-id="00509-153">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[skypeForBusinessOrganizerActivityMinuteCounts](../resources/skypeforbusinessorganizeractivityminutecounts.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="00509-153">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessOrganizerActivityMinuteCounts](../resources/skypeforbusinessorganizeractivityminutecounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00509-154">例</span><span class="sxs-lookup"><span data-stu-id="00509-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="00509-155">CSV</span><span class="sxs-lookup"><span data-stu-id="00509-155">CSV</span></span>

<span data-ttu-id="00509-156">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="00509-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="00509-157">要求</span><span class="sxs-lookup"><span data-stu-id="00509-157">Request</span></span>

<span data-ttu-id="00509-158">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="00509-158">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="00509-159">プロトコル</span><span class="sxs-lookup"><span data-stu-id="00509-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessorganizeractivityminutecounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessOrganizerActivityMinuteCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="00509-160">C#</span><span class="sxs-lookup"><span data-stu-id="00509-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessorganizeractivityminutecounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="00509-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="00509-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessorganizeractivityminutecounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="00509-162">目的-C</span><span class="sxs-lookup"><span data-stu-id="00509-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessorganizeractivityminutecounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="00509-163">応答</span><span class="sxs-lookup"><span data-stu-id="00509-163">Response</span></span>

<span data-ttu-id="00509-164">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="00509-164">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="00509-165">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="00509-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="00509-166">JSON</span><span class="sxs-lookup"><span data-stu-id="00509-166">JSON</span></span>

<span data-ttu-id="00509-167">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="00509-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="00509-168">要求</span><span class="sxs-lookup"><span data-stu-id="00509-168">Request</span></span>

<span data-ttu-id="00509-169">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="00509-169">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="00509-170">プロトコル</span><span class="sxs-lookup"><span data-stu-id="00509-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessorganizeractivityminutecounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessOrganizerActivityMinuteCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="00509-171">C#</span><span class="sxs-lookup"><span data-stu-id="00509-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessorganizeractivityminutecounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="00509-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="00509-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessorganizeractivityminutecounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="00509-173">目的-C</span><span class="sxs-lookup"><span data-stu-id="00509-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessorganizeractivityminutecounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="00509-174">応答</span><span class="sxs-lookup"><span data-stu-id="00509-174">Response</span></span>

<span data-ttu-id="00509-175">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="00509-175">The following is an example of the response.</span></span>

> <span data-ttu-id="00509-p108">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="00509-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
