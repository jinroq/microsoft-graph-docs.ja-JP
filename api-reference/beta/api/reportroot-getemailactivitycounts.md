---
title: 'reportRoot: getEmailActivityCounts'
description: 組織内の電子メール アクティビティ (送信、読み取り、受信の数) の傾向を把握できます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: b3a669b557300170dc15a122d356f0f7da93d6d2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35978162"
---
# <a name="reportroot-getemailactivitycounts"></a><span data-ttu-id="4c23b-103">reportRoot: getEmailActivityCounts</span><span class="sxs-lookup"><span data-stu-id="4c23b-103">reportRoot: getEmailActivityCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c23b-104">組織内の電子メール アクティビティ (送信、読み取り、受信の数) の傾向を把握できます。</span><span class="sxs-lookup"><span data-stu-id="4c23b-104">Enables you to understand the trends of email activity (like how many were sent, read, and received) in your organization.</span></span>

> <span data-ttu-id="4c23b-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: 電子メール アクティビティ](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4c23b-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="permissions"></a><span data-ttu-id="4c23b-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4c23b-106">Permissions</span></span>

<span data-ttu-id="4c23b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4c23b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4c23b-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4c23b-109">Permission type</span></span>                        | <span data-ttu-id="4c23b-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4c23b-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="4c23b-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="4c23b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4c23b-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4c23b-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="4c23b-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4c23b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c23b-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4c23b-114">Not supported.</span></span>                           |
| <span data-ttu-id="4c23b-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4c23b-115">Application</span></span>                            | <span data-ttu-id="4c23b-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4c23b-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="4c23b-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4c23b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="4c23b-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="4c23b-118">Function parameters</span></span>

<span data-ttu-id="4c23b-119">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="4c23b-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="4c23b-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="4c23b-120">Parameter</span></span> | <span data-ttu-id="4c23b-121">型</span><span class="sxs-lookup"><span data-stu-id="4c23b-121">Type</span></span>   | <span data-ttu-id="4c23b-122">説明</span><span class="sxs-lookup"><span data-stu-id="4c23b-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="4c23b-123">period</span><span class="sxs-lookup"><span data-stu-id="4c23b-123">period</span></span>    | <span data-ttu-id="4c23b-124">文字列</span><span class="sxs-lookup"><span data-stu-id="4c23b-124">string</span></span> | <span data-ttu-id="4c23b-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="4c23b-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="4c23b-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="4c23b-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="4c23b-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="4c23b-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="4c23b-128">必須。</span><span class="sxs-lookup"><span data-stu-id="4c23b-128">Required.</span></span> |

<span data-ttu-id="4c23b-129">このメソッドは、 `$format`応答をカスタマイズするための[OData クエリパラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="4c23b-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="4c23b-130">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="4c23b-130">The default output type is text/csv.</span></span> <span data-ttu-id="4c23b-131">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="4c23b-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4c23b-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4c23b-132">Request headers</span></span>

| <span data-ttu-id="4c23b-133">名前</span><span class="sxs-lookup"><span data-stu-id="4c23b-133">Name</span></span>          | <span data-ttu-id="4c23b-134">説明</span><span class="sxs-lookup"><span data-stu-id="4c23b-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="4c23b-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c23b-135">Authorization</span></span> | <span data-ttu-id="4c23b-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4c23b-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="4c23b-138">応答</span><span class="sxs-lookup"><span data-stu-id="4c23b-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="4c23b-139">CSV</span><span class="sxs-lookup"><span data-stu-id="4c23b-139">CSV</span></span>

<span data-ttu-id="4c23b-140">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="4c23b-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="4c23b-141">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="4c23b-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="4c23b-142">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="4c23b-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="4c23b-143">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="4c23b-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="4c23b-144">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="4c23b-144">Report Refresh Date</span></span>
- <span data-ttu-id="4c23b-145">送信</span><span class="sxs-lookup"><span data-stu-id="4c23b-145">Send</span></span>
- <span data-ttu-id="4c23b-146">受信</span><span class="sxs-lookup"><span data-stu-id="4c23b-146">Receive</span></span>
- <span data-ttu-id="4c23b-147">読み取り</span><span class="sxs-lookup"><span data-stu-id="4c23b-147">Read</span></span>
- <span data-ttu-id="4c23b-148">レポート日付</span><span class="sxs-lookup"><span data-stu-id="4c23b-148">Report Date</span></span>
- <span data-ttu-id="4c23b-149">レポート期間</span><span class="sxs-lookup"><span data-stu-id="4c23b-149">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="4c23b-150">JSON</span><span class="sxs-lookup"><span data-stu-id="4c23b-150">JSON</span></span>

<span data-ttu-id="4c23b-151">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[emailactivitysummary](../resources/emailactivitysummary.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4c23b-151">If successful, this method returns a `200 OK` response code and an **[emailActivitySummary](../resources/emailactivitysummary.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c23b-152">例</span><span class="sxs-lookup"><span data-stu-id="4c23b-152">Example</span></span>

### <a name="csv"></a><span data-ttu-id="4c23b-153">CSV</span><span class="sxs-lookup"><span data-stu-id="4c23b-153">CSV</span></span>

<span data-ttu-id="4c23b-154">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4c23b-154">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="4c23b-155">要求</span><span class="sxs-lookup"><span data-stu-id="4c23b-155">Request</span></span>

<span data-ttu-id="4c23b-156">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4c23b-156">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="4c23b-157">プロトコル</span><span class="sxs-lookup"><span data-stu-id="4c23b-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getemailactivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailActivityCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4c23b-158">C#</span><span class="sxs-lookup"><span data-stu-id="4c23b-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailactivitycounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4c23b-159">Javascript</span><span class="sxs-lookup"><span data-stu-id="4c23b-159">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailactivitycounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4c23b-160">目的-C</span><span class="sxs-lookup"><span data-stu-id="4c23b-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailactivitycounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4c23b-161">Java</span><span class="sxs-lookup"><span data-stu-id="4c23b-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getemailactivitycounts-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4c23b-162">応答</span><span class="sxs-lookup"><span data-stu-id="4c23b-162">Response</span></span>

<span data-ttu-id="4c23b-163">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4c23b-163">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="4c23b-164">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="4c23b-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Send,Receive,Read,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="4c23b-165">JSON</span><span class="sxs-lookup"><span data-stu-id="4c23b-165">JSON</span></span>

<span data-ttu-id="4c23b-166">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="4c23b-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="4c23b-167">要求</span><span class="sxs-lookup"><span data-stu-id="4c23b-167">Request</span></span>

<span data-ttu-id="4c23b-168">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4c23b-168">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="4c23b-169">プロトコル</span><span class="sxs-lookup"><span data-stu-id="4c23b-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getemailactivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailActivityCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4c23b-170">C#</span><span class="sxs-lookup"><span data-stu-id="4c23b-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailactivitycounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4c23b-171">Javascript</span><span class="sxs-lookup"><span data-stu-id="4c23b-171">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailactivitycounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4c23b-172">目的-C</span><span class="sxs-lookup"><span data-stu-id="4c23b-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailactivitycounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4c23b-173">Java</span><span class="sxs-lookup"><span data-stu-id="4c23b-173">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getemailactivitycounts-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4c23b-174">応答</span><span class="sxs-lookup"><span data-stu-id="4c23b-174">Response</span></span>

<span data-ttu-id="4c23b-175">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4c23b-175">The following is an example of the response.</span></span>

> <span data-ttu-id="4c23b-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="4c23b-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailActivitySummary"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 242

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailActivitySummary)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "send": 504, 
      "receive": 76506, 
      "read": 12161, 
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
