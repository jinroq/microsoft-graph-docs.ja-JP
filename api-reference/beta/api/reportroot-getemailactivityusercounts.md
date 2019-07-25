---
title: 'reportRoot: getEmailActivityUserCounts'
description: 送信、読み取り、受信などの電子メール アクティビティを実行しているそれぞれ別個のユーザーの数に関する傾向を把握することができます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 9a29131be4c2f8f1cc14c0d4b7138756a737a4c5
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35874044"
---
# <a name="reportroot-getemailactivityusercounts"></a><span data-ttu-id="23b8a-103">reportRoot: getEmailActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="23b8a-103">reportRoot: getEmailActivityUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23b8a-104">送信、読み取り、受信などの電子メール アクティビティを実行しているそれぞれ別個のユーザーの数に関する傾向を把握することができます。</span><span class="sxs-lookup"><span data-stu-id="23b8a-104">Enables you to understand trends on the number of unique users who are performing email activities like send, read, and receive.</span></span>

> <span data-ttu-id="23b8a-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: 電子メール アクティビティ](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="23b8a-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="permissions"></a><span data-ttu-id="23b8a-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="23b8a-106">Permissions</span></span>

<span data-ttu-id="23b8a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="23b8a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="23b8a-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="23b8a-109">Permission type</span></span>                        | <span data-ttu-id="23b8a-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="23b8a-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="23b8a-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="23b8a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="23b8a-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="23b8a-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="23b8a-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="23b8a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23b8a-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="23b8a-114">Not supported.</span></span>                           |
| <span data-ttu-id="23b8a-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="23b8a-115">Application</span></span>                            | <span data-ttu-id="23b8a-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="23b8a-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="23b8a-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="23b8a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="23b8a-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="23b8a-118">Function parameters</span></span>

<span data-ttu-id="23b8a-119">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="23b8a-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="23b8a-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="23b8a-120">Parameter</span></span> | <span data-ttu-id="23b8a-121">型</span><span class="sxs-lookup"><span data-stu-id="23b8a-121">Type</span></span>   | <span data-ttu-id="23b8a-122">説明</span><span class="sxs-lookup"><span data-stu-id="23b8a-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="23b8a-123">period</span><span class="sxs-lookup"><span data-stu-id="23b8a-123">period</span></span>    | <span data-ttu-id="23b8a-124">文字列</span><span class="sxs-lookup"><span data-stu-id="23b8a-124">string</span></span> | <span data-ttu-id="23b8a-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="23b8a-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="23b8a-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="23b8a-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="23b8a-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="23b8a-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="23b8a-128">必須。</span><span class="sxs-lookup"><span data-stu-id="23b8a-128">Required.</span></span> |

<span data-ttu-id="23b8a-129">このメソッドは、 `$format`応答をカスタマイズするための[OData クエリパラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="23b8a-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="23b8a-130">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="23b8a-130">The default output type is text/csv.</span></span> <span data-ttu-id="23b8a-131">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="23b8a-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="23b8a-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="23b8a-132">Request headers</span></span>

| <span data-ttu-id="23b8a-133">名前</span><span class="sxs-lookup"><span data-stu-id="23b8a-133">Name</span></span>          | <span data-ttu-id="23b8a-134">説明</span><span class="sxs-lookup"><span data-stu-id="23b8a-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="23b8a-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="23b8a-135">Authorization</span></span> | <span data-ttu-id="23b8a-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="23b8a-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="23b8a-138">応答</span><span class="sxs-lookup"><span data-stu-id="23b8a-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="23b8a-139">CSV</span><span class="sxs-lookup"><span data-stu-id="23b8a-139">CSV</span></span>

<span data-ttu-id="23b8a-140">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="23b8a-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="23b8a-141">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="23b8a-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="23b8a-142">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="23b8a-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="23b8a-143">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="23b8a-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="23b8a-144">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="23b8a-144">Report Refresh Date</span></span>
- <span data-ttu-id="23b8a-145">送信</span><span class="sxs-lookup"><span data-stu-id="23b8a-145">Send</span></span>
- <span data-ttu-id="23b8a-146">受信</span><span class="sxs-lookup"><span data-stu-id="23b8a-146">Receive</span></span>
- <span data-ttu-id="23b8a-147">読み取り</span><span class="sxs-lookup"><span data-stu-id="23b8a-147">Read</span></span>
- <span data-ttu-id="23b8a-148">レポート日付</span><span class="sxs-lookup"><span data-stu-id="23b8a-148">Report Date</span></span>
- <span data-ttu-id="23b8a-149">レポート期間</span><span class="sxs-lookup"><span data-stu-id="23b8a-149">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="23b8a-150">JSON</span><span class="sxs-lookup"><span data-stu-id="23b8a-150">JSON</span></span>

<span data-ttu-id="23b8a-151">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[emailactivitysummary](../resources/emailactivitysummary.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="23b8a-151">If successful, this method returns a `200 OK` response code and an **[emailActivitySummary](../resources/emailactivitysummary.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23b8a-152">例</span><span class="sxs-lookup"><span data-stu-id="23b8a-152">Example</span></span>

### <a name="csv"></a><span data-ttu-id="23b8a-153">CSV</span><span class="sxs-lookup"><span data-stu-id="23b8a-153">CSV</span></span>

<span data-ttu-id="23b8a-154">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="23b8a-154">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="23b8a-155">要求</span><span class="sxs-lookup"><span data-stu-id="23b8a-155">Request</span></span>

<span data-ttu-id="23b8a-156">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="23b8a-156">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="23b8a-157">プロトコル</span><span class="sxs-lookup"><span data-stu-id="23b8a-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getemailactivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailActivityUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="23b8a-158">C#</span><span class="sxs-lookup"><span data-stu-id="23b8a-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailactivityusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="23b8a-159">Javascript</span><span class="sxs-lookup"><span data-stu-id="23b8a-159">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailactivityusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="23b8a-160">目的-C</span><span class="sxs-lookup"><span data-stu-id="23b8a-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailactivityusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="23b8a-161">Java</span><span class="sxs-lookup"><span data-stu-id="23b8a-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getemailactivityusercounts-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="23b8a-162">応答</span><span class="sxs-lookup"><span data-stu-id="23b8a-162">Response</span></span>

<span data-ttu-id="23b8a-163">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="23b8a-163">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="23b8a-164">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="23b8a-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="23b8a-165">JSON</span><span class="sxs-lookup"><span data-stu-id="23b8a-165">JSON</span></span>

<span data-ttu-id="23b8a-166">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="23b8a-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="23b8a-167">要求</span><span class="sxs-lookup"><span data-stu-id="23b8a-167">Request</span></span>

<span data-ttu-id="23b8a-168">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="23b8a-168">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="23b8a-169">プロトコル</span><span class="sxs-lookup"><span data-stu-id="23b8a-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getemailactivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailActivityUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="23b8a-170">C#</span><span class="sxs-lookup"><span data-stu-id="23b8a-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailactivityusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="23b8a-171">Javascript</span><span class="sxs-lookup"><span data-stu-id="23b8a-171">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailactivityusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="23b8a-172">目的-C</span><span class="sxs-lookup"><span data-stu-id="23b8a-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailactivityusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="23b8a-173">Java</span><span class="sxs-lookup"><span data-stu-id="23b8a-173">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getemailactivityusercounts-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="23b8a-174">応答</span><span class="sxs-lookup"><span data-stu-id="23b8a-174">Response</span></span>

<span data-ttu-id="23b8a-175">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="23b8a-175">The following is an example of the response.</span></span>

> <span data-ttu-id="23b8a-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="23b8a-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailActivitySummary"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 237

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailActivitySummary)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "send": 69, 
      "receive": 197, 
      "read": 158, 
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
