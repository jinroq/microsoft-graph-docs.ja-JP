---
title: 'reportRoot: getMailboxUsageDetail'
description: メールボックスの使用状況に関する詳細を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 0fa58a26d37ea8ec772d9c7fccfd4bb61dead81b
ms.sourcegitcommit: 6fe086e6a9396a71a82179853547cb7b5e22d980
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/20/2019
ms.locfileid: "35805082"
---
# <a name="reportroot-getmailboxusagedetail"></a><span data-ttu-id="4b575-103">reportRoot: getMailboxUsageDetail</span><span class="sxs-lookup"><span data-stu-id="4b575-103">reportRoot: getMailboxUsageDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b575-104">メールボックスの使用状況に関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="4b575-104">Get details about mailbox usage.</span></span>

> <span data-ttu-id="4b575-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: メールボックスの使用状況](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4b575-105">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="4b575-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4b575-106">Permissions</span></span>

<span data-ttu-id="4b575-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4b575-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4b575-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4b575-109">Permission type</span></span>                        | <span data-ttu-id="4b575-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4b575-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="4b575-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="4b575-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4b575-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b575-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="4b575-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4b575-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b575-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4b575-114">Not supported.</span></span>                           |
| <span data-ttu-id="4b575-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4b575-115">Application</span></span>                            | <span data-ttu-id="4b575-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b575-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="4b575-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4b575-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageDetail(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="4b575-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="4b575-118">Function parameters</span></span>

<span data-ttu-id="4b575-119">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="4b575-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="4b575-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="4b575-120">Parameter</span></span> | <span data-ttu-id="4b575-121">型</span><span class="sxs-lookup"><span data-stu-id="4b575-121">Type</span></span>   | <span data-ttu-id="4b575-122">説明</span><span class="sxs-lookup"><span data-stu-id="4b575-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="4b575-123">period</span><span class="sxs-lookup"><span data-stu-id="4b575-123">period</span></span>    | <span data-ttu-id="4b575-124">文字列</span><span class="sxs-lookup"><span data-stu-id="4b575-124">string</span></span> | <span data-ttu-id="4b575-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="4b575-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="4b575-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="4b575-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="4b575-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="4b575-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="4b575-128">必須。</span><span class="sxs-lookup"><span data-stu-id="4b575-128">Required.</span></span> |

<span data-ttu-id="4b575-129">このメソッドは、応答をカスタマイズするための `$format`、`$top`、`$skipToken` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="4b575-129">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="4b575-130">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="4b575-130">The default output type is text/csv.</span></span> <span data-ttu-id="4b575-131">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="4b575-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4b575-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4b575-132">Request headers</span></span>

| <span data-ttu-id="4b575-133">名前</span><span class="sxs-lookup"><span data-stu-id="4b575-133">Name</span></span>          | <span data-ttu-id="4b575-134">説明</span><span class="sxs-lookup"><span data-stu-id="4b575-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="4b575-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b575-135">Authorization</span></span> | <span data-ttu-id="4b575-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4b575-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="4b575-138">応答</span><span class="sxs-lookup"><span data-stu-id="4b575-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="4b575-139">CSV</span><span class="sxs-lookup"><span data-stu-id="4b575-139">CSV</span></span>

<span data-ttu-id="4b575-140">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="4b575-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="4b575-141">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="4b575-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="4b575-142">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="4b575-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="4b575-143">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="4b575-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="4b575-144">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="4b575-144">Report Refresh Date</span></span>
- <span data-ttu-id="4b575-145">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="4b575-145">User Principal Name</span></span>
- <span data-ttu-id="4b575-146">表示名</span><span class="sxs-lookup"><span data-stu-id="4b575-146">Display Name</span></span>
- <span data-ttu-id="4b575-147">削除済み</span><span class="sxs-lookup"><span data-stu-id="4b575-147">Is Deleted</span></span>
- <span data-ttu-id="4b575-148">削除日</span><span class="sxs-lookup"><span data-stu-id="4b575-148">Deleted Date</span></span>
- <span data-ttu-id="4b575-149">作成日</span><span class="sxs-lookup"><span data-stu-id="4b575-149">Created Date</span></span>
- <span data-ttu-id="4b575-150">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="4b575-150">Last Activity Date</span></span>
- <span data-ttu-id="4b575-151">アイテム数</span><span class="sxs-lookup"><span data-stu-id="4b575-151">Item Count</span></span>
- <span data-ttu-id="4b575-152">使用済みストレージ (バイト)</span><span class="sxs-lookup"><span data-stu-id="4b575-152">Storage Used (Byte)</span></span>
- <span data-ttu-id="4b575-153">警告表示クォータ (バイト)</span><span class="sxs-lookup"><span data-stu-id="4b575-153">Issue Warning Quota (Byte)</span></span>
- <span data-ttu-id="4b575-154">送信禁止クォータ (バイト)</span><span class="sxs-lookup"><span data-stu-id="4b575-154">Prohibit Send Quota (Byte)</span></span>
- <span data-ttu-id="4b575-155">送受信禁止クォータ (バイト)</span><span class="sxs-lookup"><span data-stu-id="4b575-155">Prohibit Send/Receive Quota (Byte)</span></span>
- <span data-ttu-id="4b575-156">削除済みアイテムの数</span><span class="sxs-lookup"><span data-stu-id="4b575-156">Deleted Item Count</span></span>
- <span data-ttu-id="4b575-157">削除済みアイテムのサイズ (バイト)</span><span class="sxs-lookup"><span data-stu-id="4b575-157">Deleted Item Size (Byte)</span></span>
- <span data-ttu-id="4b575-158">レポート期間</span><span class="sxs-lookup"><span data-stu-id="4b575-158">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="4b575-159">JSON</span><span class="sxs-lookup"><span data-stu-id="4b575-159">JSON</span></span>

<span data-ttu-id="4b575-160">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[mailboxUsageDetail](../resources/mailboxusagedetail.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4b575-160">If successful, this method returns a `200 OK` response code and a **[mailboxUsageDetail](../resources/mailboxusagedetail.md)** object in the response body.</span></span>

<span data-ttu-id="4b575-161">この要求の既定のページサイズは200アイテムです。</span><span class="sxs-lookup"><span data-stu-id="4b575-161">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="4b575-162">例</span><span class="sxs-lookup"><span data-stu-id="4b575-162">Example</span></span>

### <a name="csv"></a><span data-ttu-id="4b575-163">CSV</span><span class="sxs-lookup"><span data-stu-id="4b575-163">CSV</span></span>

<span data-ttu-id="4b575-164">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4b575-164">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="4b575-165">要求</span><span class="sxs-lookup"><span data-stu-id="4b575-165">Request</span></span>

<span data-ttu-id="4b575-166">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4b575-166">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="4b575-167">プロトコル</span><span class="sxs-lookup"><span data-stu-id="4b575-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagedetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4b575-168">C#</span><span class="sxs-lookup"><span data-stu-id="4b575-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getmailboxusagedetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4b575-169">Javascript</span><span class="sxs-lookup"><span data-stu-id="4b575-169">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getmailboxusagedetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4b575-170">目的-C</span><span class="sxs-lookup"><span data-stu-id="4b575-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getmailboxusagedetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4b575-171">応答</span><span class="sxs-lookup"><span data-stu-id="4b575-171">Response</span></span>

<span data-ttu-id="4b575-172">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4b575-172">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="4b575-173">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="4b575-173">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Created Date,Last Activity Date,Item Count,Storage Used (Byte),Issue Warning Quota (Byte),Prohibit Send Quota (Byte),Prohibit Send/Receive Quota (Byte),Deleted Item Count,Deleted Item Size (Byte),Report Period
```

### <a name="json"></a><span data-ttu-id="4b575-174">JSON</span><span class="sxs-lookup"><span data-stu-id="4b575-174">JSON</span></span>

<span data-ttu-id="4b575-175">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="4b575-175">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="4b575-176">要求</span><span class="sxs-lookup"><span data-stu-id="4b575-176">Request</span></span>

<span data-ttu-id="4b575-177">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4b575-177">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="4b575-178">プロトコル</span><span class="sxs-lookup"><span data-stu-id="4b575-178">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagedetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4b575-179">C#</span><span class="sxs-lookup"><span data-stu-id="4b575-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getmailboxusagedetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4b575-180">Javascript</span><span class="sxs-lookup"><span data-stu-id="4b575-180">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getmailboxusagedetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4b575-181">目的-C</span><span class="sxs-lookup"><span data-stu-id="4b575-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getmailboxusagedetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4b575-182">応答</span><span class="sxs-lookup"><span data-stu-id="4b575-182">Response</span></span>

<span data-ttu-id="4b575-183">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4b575-183">The following is an example of the response.</span></span>

> <span data-ttu-id="4b575-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="4b575-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "deletedItemCount": 138481,
      "deletedItemSizeInBytes": 10414748704, 
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
