---
title: 'reportRoot: getMailboxUsageDetail'
description: メールボックスの使用状況に関する詳細を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 1fdd5346fa95453b4f2504382e5f20206bea0fb1
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35447034"
---
# <a name="reportroot-getmailboxusagedetail"></a><span data-ttu-id="8ac71-103">reportRoot: getMailboxUsageDetail</span><span class="sxs-lookup"><span data-stu-id="8ac71-103">reportRoot: getMailboxUsageDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ac71-104">メールボックスの使用状況に関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="8ac71-104">Get details about mailbox usage.</span></span>

> <span data-ttu-id="8ac71-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: メールボックスの使用状況](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8ac71-105">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="8ac71-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8ac71-106">Permissions</span></span>

<span data-ttu-id="8ac71-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8ac71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8ac71-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8ac71-109">Permission type</span></span>                        | <span data-ttu-id="8ac71-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8ac71-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="8ac71-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="8ac71-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8ac71-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8ac71-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="8ac71-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8ac71-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ac71-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8ac71-114">Not supported.</span></span>                           |
| <span data-ttu-id="8ac71-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8ac71-115">Application</span></span>                            | <span data-ttu-id="8ac71-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8ac71-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="8ac71-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8ac71-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageDetail(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="8ac71-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="8ac71-118">Function parameters</span></span>

<span data-ttu-id="8ac71-119">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="8ac71-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="8ac71-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="8ac71-120">Parameter</span></span> | <span data-ttu-id="8ac71-121">型</span><span class="sxs-lookup"><span data-stu-id="8ac71-121">Type</span></span>   | <span data-ttu-id="8ac71-122">説明</span><span class="sxs-lookup"><span data-stu-id="8ac71-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="8ac71-123">period</span><span class="sxs-lookup"><span data-stu-id="8ac71-123">period</span></span>    | <span data-ttu-id="8ac71-124">文字列</span><span class="sxs-lookup"><span data-stu-id="8ac71-124">string</span></span> | <span data-ttu-id="8ac71-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="8ac71-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="8ac71-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="8ac71-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="8ac71-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="8ac71-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="8ac71-128">必須。</span><span class="sxs-lookup"><span data-stu-id="8ac71-128">Required.</span></span> |

<span data-ttu-id="8ac71-129">このメソッドは、応答をカスタマイズするための `$format`、`$top`、`$skipToken` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="8ac71-129">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="8ac71-130">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="8ac71-130">The default output type is text/csv.</span></span> <span data-ttu-id="8ac71-131">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="8ac71-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8ac71-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8ac71-132">Request headers</span></span>

| <span data-ttu-id="8ac71-133">名前</span><span class="sxs-lookup"><span data-stu-id="8ac71-133">Name</span></span>          | <span data-ttu-id="8ac71-134">説明</span><span class="sxs-lookup"><span data-stu-id="8ac71-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="8ac71-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ac71-135">Authorization</span></span> | <span data-ttu-id="8ac71-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8ac71-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="8ac71-138">応答</span><span class="sxs-lookup"><span data-stu-id="8ac71-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="8ac71-139">CSV</span><span class="sxs-lookup"><span data-stu-id="8ac71-139">CSV</span></span>

<span data-ttu-id="8ac71-140">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="8ac71-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="8ac71-141">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="8ac71-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="8ac71-142">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="8ac71-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="8ac71-143">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="8ac71-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="8ac71-144">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="8ac71-144">Report Refresh Date</span></span>
- <span data-ttu-id="8ac71-145">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="8ac71-145">User Principal Name</span></span>
- <span data-ttu-id="8ac71-146">表示名</span><span class="sxs-lookup"><span data-stu-id="8ac71-146">Display Name</span></span>
- <span data-ttu-id="8ac71-147">削除済み</span><span class="sxs-lookup"><span data-stu-id="8ac71-147">Is Deleted</span></span>
- <span data-ttu-id="8ac71-148">削除日</span><span class="sxs-lookup"><span data-stu-id="8ac71-148">Deleted Date</span></span>
- <span data-ttu-id="8ac71-149">作成日</span><span class="sxs-lookup"><span data-stu-id="8ac71-149">Created Date</span></span>
- <span data-ttu-id="8ac71-150">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="8ac71-150">Last Activity Date</span></span>
- <span data-ttu-id="8ac71-151">アイテム数</span><span class="sxs-lookup"><span data-stu-id="8ac71-151">Item Count</span></span>
- <span data-ttu-id="8ac71-152">使用済みストレージ (バイト)</span><span class="sxs-lookup"><span data-stu-id="8ac71-152">Storage Used (Byte)</span></span>
- <span data-ttu-id="8ac71-153">警告表示クォータ (バイト)</span><span class="sxs-lookup"><span data-stu-id="8ac71-153">Issue Warning Quota (Byte)</span></span>
- <span data-ttu-id="8ac71-154">送信禁止クォータ (バイト)</span><span class="sxs-lookup"><span data-stu-id="8ac71-154">Prohibit Send Quota (Byte)</span></span>
- <span data-ttu-id="8ac71-155">送受信禁止クォータ (バイト)</span><span class="sxs-lookup"><span data-stu-id="8ac71-155">Prohibit Send/Receive Quota (Byte)</span></span>
- <span data-ttu-id="8ac71-156">レポート期間</span><span class="sxs-lookup"><span data-stu-id="8ac71-156">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="8ac71-157">JSON</span><span class="sxs-lookup"><span data-stu-id="8ac71-157">JSON</span></span>

<span data-ttu-id="8ac71-158">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[mailboxUsageDetail](../resources/mailboxusagedetail.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8ac71-158">If successful, this method returns a `200 OK` response code and a **[mailboxUsageDetail](../resources/mailboxusagedetail.md)** object in the response body.</span></span>

<span data-ttu-id="8ac71-159">この要求の既定のページサイズは200アイテムです。</span><span class="sxs-lookup"><span data-stu-id="8ac71-159">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="8ac71-160">例</span><span class="sxs-lookup"><span data-stu-id="8ac71-160">Example</span></span>

### <a name="csv"></a><span data-ttu-id="8ac71-161">CSV</span><span class="sxs-lookup"><span data-stu-id="8ac71-161">CSV</span></span>

<span data-ttu-id="8ac71-162">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8ac71-162">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="8ac71-163">要求</span><span class="sxs-lookup"><span data-stu-id="8ac71-163">Request</span></span>

<span data-ttu-id="8ac71-164">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8ac71-164">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8ac71-165">プロトコル</span><span class="sxs-lookup"><span data-stu-id="8ac71-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagedetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8ac71-166">C#</span><span class="sxs-lookup"><span data-stu-id="8ac71-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getmailboxusagedetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8ac71-167">Javascript</span><span class="sxs-lookup"><span data-stu-id="8ac71-167">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getmailboxusagedetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8ac71-168">目的-C</span><span class="sxs-lookup"><span data-stu-id="8ac71-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getmailboxusagedetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8ac71-169">応答</span><span class="sxs-lookup"><span data-stu-id="8ac71-169">Response</span></span>

<span data-ttu-id="8ac71-170">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8ac71-170">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="8ac71-171">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="8ac71-171">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Created Date,Last Activity Date,Item Count,Storage Used (Byte),Issue Warning Quota (Byte),Prohibit Send Quota (Byte),Prohibit Send/Receive Quota (Byte),Report Period
```

### <a name="json"></a><span data-ttu-id="8ac71-172">JSON</span><span class="sxs-lookup"><span data-stu-id="8ac71-172">JSON</span></span>

<span data-ttu-id="8ac71-173">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="8ac71-173">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="8ac71-174">要求</span><span class="sxs-lookup"><span data-stu-id="8ac71-174">Request</span></span>

<span data-ttu-id="8ac71-175">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8ac71-175">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8ac71-176">プロトコル</span><span class="sxs-lookup"><span data-stu-id="8ac71-176">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagedetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8ac71-177">C#</span><span class="sxs-lookup"><span data-stu-id="8ac71-177">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getmailboxusagedetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8ac71-178">Javascript</span><span class="sxs-lookup"><span data-stu-id="8ac71-178">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getmailboxusagedetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8ac71-179">目的-C</span><span class="sxs-lookup"><span data-stu-id="8ac71-179">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getmailboxusagedetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8ac71-180">応答</span><span class="sxs-lookup"><span data-stu-id="8ac71-180">Response</span></span>

<span data-ttu-id="8ac71-181">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8ac71-181">The following is an example of the response.</span></span>

> <span data-ttu-id="8ac71-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="8ac71-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxUsageDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 526

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.mailboxUsageDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "displayName": "displayName-value", 
      "isDeleted": false, 
      "deletedDate": null, 
      "createdDate": "2016-03-30", 
      "lastActivityDate": "2017-09-01", 
      "itemCount": 138481, 
      "storageUsedInBytes": 10414748704, 
      "issueWarningQuotaInBytes": 10522698752, 
      "prohibitSendQuotaInBytes": 10630040576, 
      "prohibitSendReceiveQuotaInBytes": 10737418240, 
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
