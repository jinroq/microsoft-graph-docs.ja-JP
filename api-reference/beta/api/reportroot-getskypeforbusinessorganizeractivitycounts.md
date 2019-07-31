---
title: 'reportRoot: getSkypeForBusinessOrganizerActivityCounts'
description: 組織内のユーザーが開催、企画した電話会議セッションの数と種類に関する使用状況の傾向を取得します。 会議セッションの種類には、IM、オーディオ/ビデオ、アプリケーション共有、Web、サード パーティへのダイヤルイン/ダイヤルアウト、Microsoft へのダイヤルイン/ダイヤルアウトなどがあります。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: f0a546d37813b98677edf1d77507f10b9234d383
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35988046"
---
# <a name="reportroot-getskypeforbusinessorganizeractivitycounts"></a><span data-ttu-id="6d7e7-104">reportRoot: getSkypeForBusinessOrganizerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="6d7e7-104">reportRoot: getSkypeForBusinessOrganizerActivityCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d7e7-105">組織内のユーザーが開催、企画した電話会議セッションの数と種類に関する使用状況の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="6d7e7-105">Get usage trends on the number and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="6d7e7-106">会議セッションの種類には、IM、オーディオ/ビデオ、アプリケーション共有、Web、サード パーティへのダイヤルイン/ダイヤルアウト、Microsoft へのダイヤルイン/ダイヤルアウトなどがあります。</span><span class="sxs-lookup"><span data-stu-id="6d7e7-106">Types of conference sessions include IM, audio/video, application sharing, web, dial-in/out - 3rd party, and Dial-in/out Microsoft.</span></span>

> <span data-ttu-id="6d7e7-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Skype for Business 電話会議の開催者のアクティビティ](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6d7e7-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="permissions"></a><span data-ttu-id="6d7e7-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6d7e7-108">Permissions</span></span>

<span data-ttu-id="6d7e7-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6d7e7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6d7e7-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6d7e7-111">Permission type</span></span>                        | <span data-ttu-id="6d7e7-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6d7e7-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="6d7e7-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="6d7e7-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="6d7e7-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6d7e7-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="6d7e7-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6d7e7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d7e7-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6d7e7-116">Not supported.</span></span>                           |
| <span data-ttu-id="6d7e7-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6d7e7-117">Application</span></span>                            | <span data-ttu-id="6d7e7-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6d7e7-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="6d7e7-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6d7e7-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessOrganizerActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="6d7e7-120">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="6d7e7-120">Function parameters</span></span>

<span data-ttu-id="6d7e7-121">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="6d7e7-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="6d7e7-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="6d7e7-122">Parameter</span></span> | <span data-ttu-id="6d7e7-123">型</span><span class="sxs-lookup"><span data-stu-id="6d7e7-123">Type</span></span>   | <span data-ttu-id="6d7e7-124">説明</span><span class="sxs-lookup"><span data-stu-id="6d7e7-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="6d7e7-125">period</span><span class="sxs-lookup"><span data-stu-id="6d7e7-125">period</span></span>    | <span data-ttu-id="6d7e7-126">文字列</span><span class="sxs-lookup"><span data-stu-id="6d7e7-126">string</span></span> | <span data-ttu-id="6d7e7-127">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="6d7e7-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="6d7e7-128">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="6d7e7-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="6d7e7-129">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="6d7e7-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="6d7e7-130">必須。</span><span class="sxs-lookup"><span data-stu-id="6d7e7-130">Required.</span></span> |

<span data-ttu-id="6d7e7-131">このメソッドは、 `$format`応答をカスタマイズするための[OData クエリパラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="6d7e7-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="6d7e7-132">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="6d7e7-132">The default output type is text/csv.</span></span> <span data-ttu-id="6d7e7-133">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="6d7e7-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6d7e7-134">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6d7e7-134">Request headers</span></span>

| <span data-ttu-id="6d7e7-135">名前</span><span class="sxs-lookup"><span data-stu-id="6d7e7-135">Name</span></span>          | <span data-ttu-id="6d7e7-136">説明</span><span class="sxs-lookup"><span data-stu-id="6d7e7-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="6d7e7-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d7e7-137">Authorization</span></span> | <span data-ttu-id="6d7e7-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6d7e7-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="6d7e7-140">応答</span><span class="sxs-lookup"><span data-stu-id="6d7e7-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="6d7e7-141">CSV</span><span class="sxs-lookup"><span data-stu-id="6d7e7-141">CSV</span></span>

<span data-ttu-id="6d7e7-142">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="6d7e7-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="6d7e7-143">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="6d7e7-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="6d7e7-144">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="6d7e7-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="6d7e7-145">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="6d7e7-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="6d7e7-146">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="6d7e7-146">Report Refresh Date</span></span>
- <span data-ttu-id="6d7e7-147">レポート日付</span><span class="sxs-lookup"><span data-stu-id="6d7e7-147">Report Date</span></span>
- <span data-ttu-id="6d7e7-148">レポート期間</span><span class="sxs-lookup"><span data-stu-id="6d7e7-148">Report Period</span></span>
- <span data-ttu-id="6d7e7-149">IM</span><span class="sxs-lookup"><span data-stu-id="6d7e7-149">IM</span></span>
- <span data-ttu-id="6d7e7-150">オーディオ/ビデオ</span><span class="sxs-lookup"><span data-stu-id="6d7e7-150">Audio/Video</span></span>
- <span data-ttu-id="6d7e7-151">アプリ共有</span><span class="sxs-lookup"><span data-stu-id="6d7e7-151">App Sharing</span></span>
- <span data-ttu-id="6d7e7-152">Web</span><span class="sxs-lookup"><span data-stu-id="6d7e7-152">Web</span></span>
- <span data-ttu-id="6d7e7-153">サード パーティのダイヤルイン/アウト</span><span class="sxs-lookup"><span data-stu-id="6d7e7-153">Dial-in/out 3rd Party</span></span>
- <span data-ttu-id="6d7e7-154">Microsoft へのダイヤルイン/アウト</span><span class="sxs-lookup"><span data-stu-id="6d7e7-154">Dial-in/out Microsoft</span></span>

### <a name="json"></a><span data-ttu-id="6d7e7-155">JSON</span><span class="sxs-lookup"><span data-stu-id="6d7e7-155">JSON</span></span>

<span data-ttu-id="6d7e7-156">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[Skypeforbusinessオーガナイザー eractivity計数](../resources/skypeforbusinessorganizeractivitycounts.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6d7e7-156">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessOrganizerActivityCounts](../resources/skypeforbusinessorganizeractivitycounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d7e7-157">例</span><span class="sxs-lookup"><span data-stu-id="6d7e7-157">Example</span></span>

### <a name="csv"></a><span data-ttu-id="6d7e7-158">CSV</span><span class="sxs-lookup"><span data-stu-id="6d7e7-158">CSV</span></span>

<span data-ttu-id="6d7e7-159">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6d7e7-159">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="6d7e7-160">要求</span><span class="sxs-lookup"><span data-stu-id="6d7e7-160">Request</span></span>

<span data-ttu-id="6d7e7-161">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6d7e7-161">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6d7e7-162">プロトコル</span><span class="sxs-lookup"><span data-stu-id="6d7e7-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessorganizeractivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessOrganizerActivityCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6d7e7-163">C#</span><span class="sxs-lookup"><span data-stu-id="6d7e7-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessorganizeractivitycounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6d7e7-164">Javascript</span><span class="sxs-lookup"><span data-stu-id="6d7e7-164">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessorganizeractivitycounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6d7e7-165">目的-C</span><span class="sxs-lookup"><span data-stu-id="6d7e7-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessorganizeractivitycounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6d7e7-166">Java</span><span class="sxs-lookup"><span data-stu-id="6d7e7-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessorganizeractivitycounts-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6d7e7-167">応答</span><span class="sxs-lookup"><span data-stu-id="6d7e7-167">Response</span></span>

<span data-ttu-id="6d7e7-168">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6d7e7-168">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="6d7e7-169">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="6d7e7-169">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio/Video,App Sharing,Web,Dial-in/out 3rd Party,Dial-in/out Microsoft
```

### <a name="json"></a><span data-ttu-id="6d7e7-170">JSON</span><span class="sxs-lookup"><span data-stu-id="6d7e7-170">JSON</span></span>

<span data-ttu-id="6d7e7-171">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="6d7e7-171">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="6d7e7-172">要求</span><span class="sxs-lookup"><span data-stu-id="6d7e7-172">Request</span></span>

<span data-ttu-id="6d7e7-173">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6d7e7-173">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6d7e7-174">プロトコル</span><span class="sxs-lookup"><span data-stu-id="6d7e7-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessorganizeractivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessOrganizerActivityCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6d7e7-175">C#</span><span class="sxs-lookup"><span data-stu-id="6d7e7-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessorganizeractivitycounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6d7e7-176">Javascript</span><span class="sxs-lookup"><span data-stu-id="6d7e7-176">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessorganizeractivitycounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6d7e7-177">目的-C</span><span class="sxs-lookup"><span data-stu-id="6d7e7-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessorganizeractivitycounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6d7e7-178">Java</span><span class="sxs-lookup"><span data-stu-id="6d7e7-178">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessorganizeractivitycounts-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6d7e7-179">応答</span><span class="sxs-lookup"><span data-stu-id="6d7e7-179">Response</span></span>

<span data-ttu-id="6d7e7-180">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6d7e7-180">The following is an example of the response.</span></span>

> <span data-ttu-id="6d7e7-p108">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="6d7e7-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessOrganizerActivityCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 315

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessOrganizerActivityCounts)", 
  "value": [
    {
      "im": 20, 
      "audioVideo": 43, 
      "appSharing": 20, 
      "web": 6, 
      "dialInOut3rdParty": 0, 
      "dialInOutMicrosoft": 48, 
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
