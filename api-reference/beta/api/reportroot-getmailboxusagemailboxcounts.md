---
title: 'reportRoot: getMailboxUsageMailboxCounts'
description: 組織内のユーザー メールボックスの合計数と、レポート期間中の各日にアクティブなメールボックス数を取得します。 メールボックスは、ユーザーが何らかの電子メールを送信するか、読んだ場合にアクティブとみなされます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 50d07440e09cdcaf404b24558dc30ae6b80bff2f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35978120"
---
# <a name="reportroot-getmailboxusagemailboxcounts"></a><span data-ttu-id="a4d09-104">reportRoot: getMailboxUsageMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="a4d09-104">reportRoot: getMailboxUsageMailboxCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4d09-105">組織内のユーザー メールボックスの合計数と、レポート期間中の各日にアクティブなメールボックス数を取得します。</span><span class="sxs-lookup"><span data-stu-id="a4d09-105">Get the total number of user mailboxes in your organization and how many are active each day of the reporting period.</span></span> <span data-ttu-id="a4d09-106">メールボックスは、ユーザーが何らかの電子メールを送信するか、読んだ場合にアクティブとみなされます。</span><span class="sxs-lookup"><span data-stu-id="a4d09-106">A mailbox is considered active if the user sent or read any email.</span></span>

> <span data-ttu-id="a4d09-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: メールボックスの使用状況](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a4d09-107">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="a4d09-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a4d09-108">Permissions</span></span>

<span data-ttu-id="a4d09-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a4d09-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a4d09-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a4d09-111">Permission type</span></span>                        | <span data-ttu-id="a4d09-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a4d09-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="a4d09-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="a4d09-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="a4d09-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a4d09-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="a4d09-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a4d09-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4d09-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a4d09-116">Not supported.</span></span>                           |
| <span data-ttu-id="a4d09-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a4d09-117">Application</span></span>                            | <span data-ttu-id="a4d09-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a4d09-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="a4d09-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a4d09-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageMailboxCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="a4d09-120">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="a4d09-120">Function parameters</span></span>

<span data-ttu-id="a4d09-121">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="a4d09-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="a4d09-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="a4d09-122">Parameter</span></span> | <span data-ttu-id="a4d09-123">型</span><span class="sxs-lookup"><span data-stu-id="a4d09-123">Type</span></span>   | <span data-ttu-id="a4d09-124">説明</span><span class="sxs-lookup"><span data-stu-id="a4d09-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="a4d09-125">period</span><span class="sxs-lookup"><span data-stu-id="a4d09-125">period</span></span>    | <span data-ttu-id="a4d09-126">文字列</span><span class="sxs-lookup"><span data-stu-id="a4d09-126">string</span></span> | <span data-ttu-id="a4d09-127">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="a4d09-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="a4d09-128">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="a4d09-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="a4d09-129">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="a4d09-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="a4d09-130">必須。</span><span class="sxs-lookup"><span data-stu-id="a4d09-130">Required.</span></span> |

<span data-ttu-id="a4d09-131">このメソッドは、 `$format`応答をカスタマイズするための[OData クエリパラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="a4d09-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="a4d09-132">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="a4d09-132">The default output type is text/csv.</span></span> <span data-ttu-id="a4d09-133">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="a4d09-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a4d09-134">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a4d09-134">Request headers</span></span>

| <span data-ttu-id="a4d09-135">名前</span><span class="sxs-lookup"><span data-stu-id="a4d09-135">Name</span></span>          | <span data-ttu-id="a4d09-136">説明</span><span class="sxs-lookup"><span data-stu-id="a4d09-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="a4d09-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4d09-137">Authorization</span></span> | <span data-ttu-id="a4d09-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a4d09-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="a4d09-140">応答</span><span class="sxs-lookup"><span data-stu-id="a4d09-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="a4d09-141">CSV</span><span class="sxs-lookup"><span data-stu-id="a4d09-141">CSV</span></span>

<span data-ttu-id="a4d09-142">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="a4d09-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="a4d09-143">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="a4d09-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="a4d09-144">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="a4d09-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="a4d09-145">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="a4d09-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="a4d09-146">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="a4d09-146">Report Refresh Date</span></span>
- <span data-ttu-id="a4d09-147">合計</span><span class="sxs-lookup"><span data-stu-id="a4d09-147">Total</span></span>
- <span data-ttu-id="a4d09-148">アクティブ</span><span class="sxs-lookup"><span data-stu-id="a4d09-148">Active</span></span>
- <span data-ttu-id="a4d09-149">レポート日付</span><span class="sxs-lookup"><span data-stu-id="a4d09-149">Report Date</span></span>
- <span data-ttu-id="a4d09-150">レポート期間</span><span class="sxs-lookup"><span data-stu-id="a4d09-150">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="a4d09-151">JSON</span><span class="sxs-lookup"><span data-stu-id="a4d09-151">JSON</span></span>

<span data-ttu-id="a4d09-152">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[mailboxUsageMailboxCounts](../resources/mailboxusagemailboxcounts.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a4d09-152">If successful, this method returns a `200 OK` response code and a **[mailboxUsageMailboxCounts](../resources/mailboxusagemailboxcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4d09-153">例</span><span class="sxs-lookup"><span data-stu-id="a4d09-153">Example</span></span>

### <a name="csv"></a><span data-ttu-id="a4d09-154">CSV</span><span class="sxs-lookup"><span data-stu-id="a4d09-154">CSV</span></span>

<span data-ttu-id="a4d09-155">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a4d09-155">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="a4d09-156">要求</span><span class="sxs-lookup"><span data-stu-id="a4d09-156">Request</span></span>

<span data-ttu-id="a4d09-157">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a4d09-157">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a4d09-158">プロトコル</span><span class="sxs-lookup"><span data-stu-id="a4d09-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagemailboxcounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageMailboxCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a4d09-159">C#</span><span class="sxs-lookup"><span data-stu-id="a4d09-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getmailboxusagemailboxcounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a4d09-160">Javascript</span><span class="sxs-lookup"><span data-stu-id="a4d09-160">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getmailboxusagemailboxcounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a4d09-161">目的-C</span><span class="sxs-lookup"><span data-stu-id="a4d09-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getmailboxusagemailboxcounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a4d09-162">Java</span><span class="sxs-lookup"><span data-stu-id="a4d09-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getmailboxusagemailboxcounts-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a4d09-163">応答</span><span class="sxs-lookup"><span data-stu-id="a4d09-163">Response</span></span>

<span data-ttu-id="a4d09-164">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a4d09-164">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="a4d09-165">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="a4d09-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Total,Active,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="a4d09-166">JSON</span><span class="sxs-lookup"><span data-stu-id="a4d09-166">JSON</span></span>

<span data-ttu-id="a4d09-167">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="a4d09-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="a4d09-168">要求</span><span class="sxs-lookup"><span data-stu-id="a4d09-168">Request</span></span>

<span data-ttu-id="a4d09-169">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a4d09-169">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a4d09-170">プロトコル</span><span class="sxs-lookup"><span data-stu-id="a4d09-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagemailboxcounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageMailboxCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a4d09-171">C#</span><span class="sxs-lookup"><span data-stu-id="a4d09-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getmailboxusagemailboxcounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a4d09-172">Javascript</span><span class="sxs-lookup"><span data-stu-id="a4d09-172">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getmailboxusagemailboxcounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a4d09-173">目的-C</span><span class="sxs-lookup"><span data-stu-id="a4d09-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getmailboxusagemailboxcounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a4d09-174">Java</span><span class="sxs-lookup"><span data-stu-id="a4d09-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getmailboxusagemailboxcounts-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a4d09-175">応答</span><span class="sxs-lookup"><span data-stu-id="a4d09-175">Response</span></span>

<span data-ttu-id="a4d09-176">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a4d09-176">The following is an example of the response.</span></span>

> <span data-ttu-id="a4d09-p108">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="a4d09-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxUsageMailboxCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 232

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.mailboxUsageMailboxCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "total": 202, 
      "active": 198, 
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
