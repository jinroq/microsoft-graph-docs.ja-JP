---
title: 'reportRoot: getSkypeForBusinessPeerToPeerActivityCounts'
description: 組織内で実施されたセッションの数と種類について、使用傾向を取得します。 セッションの種類には IM、オーディオ、ビデオ、アプリケーション共有、ファイル転送があります。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 7a208e909e3f155c7a5e35cccac2fc4aad914959
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359043"
---
# <a name="reportroot-getskypeforbusinesspeertopeeractivitycounts"></a><span data-ttu-id="fa08d-104">reportRoot: getSkypeForBusinessPeerToPeerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="fa08d-104">reportRoot: getSkypeForBusinessPeerToPeerActivityCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa08d-105">組織内で実施されたセッションの数と種類について、使用傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="fa08d-105">Get usage trends on the number and type of sessions held in your organization.</span></span> <span data-ttu-id="fa08d-106">セッションの種類には IM、オーディオ、ビデオ、アプリケーション共有、ファイル転送があります。</span><span class="sxs-lookup"><span data-stu-id="fa08d-106">Types of sessions include IM, audio, video, application sharing, and file transfer.</span></span>

> <span data-ttu-id="fa08d-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Skype for Business ピア ツー ピア アクティビティ](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fa08d-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="permissions"></a><span data-ttu-id="fa08d-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fa08d-108">Permissions</span></span>

<span data-ttu-id="fa08d-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fa08d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fa08d-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fa08d-111">Permission type</span></span>                        | <span data-ttu-id="fa08d-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fa08d-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="fa08d-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="fa08d-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="fa08d-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa08d-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="fa08d-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fa08d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa08d-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fa08d-116">Not supported.</span></span>                           |
| <span data-ttu-id="fa08d-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fa08d-117">Application</span></span>                            | <span data-ttu-id="fa08d-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa08d-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="fa08d-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fa08d-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessPeerToPeerActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="fa08d-120">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="fa08d-120">Function parameters</span></span>

<span data-ttu-id="fa08d-121">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="fa08d-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="fa08d-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="fa08d-122">Parameter</span></span> | <span data-ttu-id="fa08d-123">型</span><span class="sxs-lookup"><span data-stu-id="fa08d-123">Type</span></span>   | <span data-ttu-id="fa08d-124">説明</span><span class="sxs-lookup"><span data-stu-id="fa08d-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="fa08d-125">period</span><span class="sxs-lookup"><span data-stu-id="fa08d-125">period</span></span>    | <span data-ttu-id="fa08d-126">文字列</span><span class="sxs-lookup"><span data-stu-id="fa08d-126">string</span></span> | <span data-ttu-id="fa08d-127">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="fa08d-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="fa08d-128">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="fa08d-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="fa08d-129">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="fa08d-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="fa08d-130">必須。</span><span class="sxs-lookup"><span data-stu-id="fa08d-130">Required.</span></span> |

<span data-ttu-id="fa08d-131">このメソッドは、 `$format`応答をカスタマイズするための[OData クエリパラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="fa08d-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="fa08d-132">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="fa08d-132">The default output type is text/csv.</span></span> <span data-ttu-id="fa08d-133">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="fa08d-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fa08d-134">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fa08d-134">Request headers</span></span>

| <span data-ttu-id="fa08d-135">名前</span><span class="sxs-lookup"><span data-stu-id="fa08d-135">Name</span></span>          | <span data-ttu-id="fa08d-136">説明</span><span class="sxs-lookup"><span data-stu-id="fa08d-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="fa08d-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa08d-137">Authorization</span></span> | <span data-ttu-id="fa08d-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="fa08d-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="fa08d-140">応答</span><span class="sxs-lookup"><span data-stu-id="fa08d-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="fa08d-141">CSV</span><span class="sxs-lookup"><span data-stu-id="fa08d-141">CSV</span></span>

<span data-ttu-id="fa08d-142">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="fa08d-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="fa08d-143">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="fa08d-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="fa08d-144">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="fa08d-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="fa08d-145">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="fa08d-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="fa08d-146">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="fa08d-146">Report Refresh Date</span></span>
- <span data-ttu-id="fa08d-147">レポート日付</span><span class="sxs-lookup"><span data-stu-id="fa08d-147">Report Date</span></span>
- <span data-ttu-id="fa08d-148">レポート期間</span><span class="sxs-lookup"><span data-stu-id="fa08d-148">Report Period</span></span>
- <span data-ttu-id="fa08d-149">IM</span><span class="sxs-lookup"><span data-stu-id="fa08d-149">IM</span></span>
- <span data-ttu-id="fa08d-150">オーディオ</span><span class="sxs-lookup"><span data-stu-id="fa08d-150">Audio</span></span>
- <span data-ttu-id="fa08d-151">ビデオ</span><span class="sxs-lookup"><span data-stu-id="fa08d-151">Video</span></span>
- <span data-ttu-id="fa08d-152">アプリ共有</span><span class="sxs-lookup"><span data-stu-id="fa08d-152">App Sharing</span></span>
- <span data-ttu-id="fa08d-153">ファイル転送</span><span class="sxs-lookup"><span data-stu-id="fa08d-153">File Transfer</span></span>

### <a name="json"></a><span data-ttu-id="fa08d-154">JSON</span><span class="sxs-lookup"><span data-stu-id="fa08d-154">JSON</span></span>

<span data-ttu-id="fa08d-155">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[skypeForBusinessPeerToPeerActivityCounts](../resources/skypeforbusinesspeertopeeractivitycounts.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="fa08d-155">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessPeerToPeerActivityCounts](../resources/skypeforbusinesspeertopeeractivitycounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa08d-156">例</span><span class="sxs-lookup"><span data-stu-id="fa08d-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="fa08d-157">CSV</span><span class="sxs-lookup"><span data-stu-id="fa08d-157">CSV</span></span>

<span data-ttu-id="fa08d-158">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fa08d-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="fa08d-159">要求</span><span class="sxs-lookup"><span data-stu-id="fa08d-159">Request</span></span>

<span data-ttu-id="fa08d-160">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fa08d-160">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="fa08d-161">プロトコル</span><span class="sxs-lookup"><span data-stu-id="fa08d-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinesspeertopeeractivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fa08d-162">C#</span><span class="sxs-lookup"><span data-stu-id="fa08d-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinesspeertopeeractivitycounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fa08d-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fa08d-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinesspeertopeeractivitycounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fa08d-164">目的-C</span><span class="sxs-lookup"><span data-stu-id="fa08d-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinesspeertopeeractivitycounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="fa08d-165">Java</span><span class="sxs-lookup"><span data-stu-id="fa08d-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinesspeertopeeractivitycounts-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fa08d-166">応答</span><span class="sxs-lookup"><span data-stu-id="fa08d-166">Response</span></span>

<span data-ttu-id="fa08d-167">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fa08d-167">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="fa08d-168">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="fa08d-168">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio,Video,App Sharing,File Transfer
```

### <a name="json"></a><span data-ttu-id="fa08d-169">JSON</span><span class="sxs-lookup"><span data-stu-id="fa08d-169">JSON</span></span>

<span data-ttu-id="fa08d-170">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="fa08d-170">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="fa08d-171">要求</span><span class="sxs-lookup"><span data-stu-id="fa08d-171">Request</span></span>

<span data-ttu-id="fa08d-172">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fa08d-172">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="fa08d-173">プロトコル</span><span class="sxs-lookup"><span data-stu-id="fa08d-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinesspeertopeeractivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fa08d-174">C#</span><span class="sxs-lookup"><span data-stu-id="fa08d-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinesspeertopeeractivitycounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fa08d-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fa08d-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinesspeertopeeractivitycounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fa08d-176">目的-C</span><span class="sxs-lookup"><span data-stu-id="fa08d-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinesspeertopeeractivitycounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="fa08d-177">Java</span><span class="sxs-lookup"><span data-stu-id="fa08d-177">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinesspeertopeeractivitycounts-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fa08d-178">応答</span><span class="sxs-lookup"><span data-stu-id="fa08d-178">Response</span></span>

<span data-ttu-id="fa08d-179">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fa08d-179">The following is an example of the response.</span></span>

> <span data-ttu-id="fa08d-p108">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="fa08d-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 288

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessPeerToPeerActivityCounts)", 
  "value": [
    {
      "im": 1177, 
      "audio": 107, 
      "video": 7, 
      "appSharing": 74, 
      "fileTransfer": 24, 
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
