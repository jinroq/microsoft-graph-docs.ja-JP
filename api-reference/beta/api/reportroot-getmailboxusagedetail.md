---
title: 'reportRoot: getMailboxUsageDetail'
description: メールボックスの使用状況に関する詳細を取得します。
ms.openlocfilehash: 317d258a51250992c47b20675bb2cb580ce408dd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066480"
---
# <a name="reportroot-getmailboxusagedetail"></a><span data-ttu-id="fb577-103">reportRoot: getMailboxUsageDetail</span><span class="sxs-lookup"><span data-stu-id="fb577-103">reportRoot: getMailboxUsageDetail</span></span>

> <span data-ttu-id="fb577-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fb577-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fb577-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fb577-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fb577-106">メールボックスの使用状況に関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="fb577-106">Get details about mailbox usage.</span></span>

> <span data-ttu-id="fb577-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: メールボックスの使用状況](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fb577-107">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="fb577-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fb577-108">Permissions</span></span>

<span data-ttu-id="fb577-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fb577-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fb577-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fb577-111">Permission type</span></span>                        | <span data-ttu-id="fb577-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fb577-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="fb577-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="fb577-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="fb577-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fb577-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="fb577-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fb577-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb577-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fb577-116">Not supported.</span></span>                           |
| <span data-ttu-id="fb577-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fb577-117">Application</span></span>                            | <span data-ttu-id="fb577-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fb577-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="fb577-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fb577-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageDetail(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="fb577-120">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="fb577-120">Function parameters</span></span>

<span data-ttu-id="fb577-121">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="fb577-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="fb577-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="fb577-122">Parameter</span></span> | <span data-ttu-id="fb577-123">型</span><span class="sxs-lookup"><span data-stu-id="fb577-123">Type</span></span>   | <span data-ttu-id="fb577-124">説明</span><span class="sxs-lookup"><span data-stu-id="fb577-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="fb577-125">period</span><span class="sxs-lookup"><span data-stu-id="fb577-125">period</span></span>    | <span data-ttu-id="fb577-126">文字列</span><span class="sxs-lookup"><span data-stu-id="fb577-126">string</span></span> | <span data-ttu-id="fb577-127">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="fb577-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="fb577-128">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="fb577-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="fb577-129">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="fb577-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="fb577-130">必須。</span><span class="sxs-lookup"><span data-stu-id="fb577-130">Required.</span></span> |

<span data-ttu-id="fb577-131">このメソッドは、応答をカスタマイズするための `$format`、`$top`、`$skipToken` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="fb577-131">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="fb577-132">既定の出力の種類は、テキストまたは csv です。</span><span class="sxs-lookup"><span data-stu-id="fb577-132">The default output type is text/csv.</span></span> <span data-ttu-id="fb577-133">ただし、出力の種類を指定する場合は、設定をテキストまたは csv またはアプリケーションまたは json OData $format クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="fb577-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fb577-134">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fb577-134">Request headers</span></span>

| <span data-ttu-id="fb577-135">名前</span><span class="sxs-lookup"><span data-stu-id="fb577-135">Name</span></span>          | <span data-ttu-id="fb577-136">説明</span><span class="sxs-lookup"><span data-stu-id="fb577-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="fb577-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb577-137">Authorization</span></span> | <span data-ttu-id="fb577-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="fb577-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="fb577-140">応答</span><span class="sxs-lookup"><span data-stu-id="fb577-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="fb577-141">CSV</span><span class="sxs-lookup"><span data-stu-id="fb577-141">CSV</span></span>

<span data-ttu-id="fb577-142">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="fb577-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="fb577-143">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="fb577-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="fb577-144">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="fb577-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="fb577-145">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="fb577-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="fb577-146">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="fb577-146">Report Refresh Date</span></span>
- <span data-ttu-id="fb577-147">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="fb577-147">User Principal Name</span></span>
- <span data-ttu-id="fb577-148">表示名</span><span class="sxs-lookup"><span data-stu-id="fb577-148">Display Name</span></span>
- <span data-ttu-id="fb577-149">削除済み</span><span class="sxs-lookup"><span data-stu-id="fb577-149">Is Deleted</span></span>
- <span data-ttu-id="fb577-150">削除日</span><span class="sxs-lookup"><span data-stu-id="fb577-150">Deleted Date</span></span>
- <span data-ttu-id="fb577-151">作成日</span><span class="sxs-lookup"><span data-stu-id="fb577-151">Created Date</span></span>
- <span data-ttu-id="fb577-152">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="fb577-152">Last Activity Date</span></span>
- <span data-ttu-id="fb577-153">アイテム数</span><span class="sxs-lookup"><span data-stu-id="fb577-153">Item Count</span></span>
- <span data-ttu-id="fb577-154">使用済みストレージ (バイト)</span><span class="sxs-lookup"><span data-stu-id="fb577-154">Storage Used (Byte)</span></span>
- <span data-ttu-id="fb577-155">警告表示クォータ (バイト)</span><span class="sxs-lookup"><span data-stu-id="fb577-155">Issue Warning Quota (Byte)</span></span>
- <span data-ttu-id="fb577-156">送信禁止クォータ (バイト)</span><span class="sxs-lookup"><span data-stu-id="fb577-156">Prohibit Send Quota (Byte)</span></span>
- <span data-ttu-id="fb577-157">送受信禁止クォータ (バイト)</span><span class="sxs-lookup"><span data-stu-id="fb577-157">Prohibit Send/Receive Quota (Byte)</span></span>
- <span data-ttu-id="fb577-158">レポート期間</span><span class="sxs-lookup"><span data-stu-id="fb577-158">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="fb577-159">JSON</span><span class="sxs-lookup"><span data-stu-id="fb577-159">JSON</span></span>

<span data-ttu-id="fb577-160">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に**[mailboxUsageDetail](../resources/mailboxusagedetail.md)** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="fb577-160">If successful, this method returns a `200 OK` response code and a **[mailboxUsageDetail](../resources/mailboxusagedetail.md)** object in the response body.</span></span>

<span data-ttu-id="fb577-161">この要求の既定のページ サイズは、アイテムは 200 個です。</span><span class="sxs-lookup"><span data-stu-id="fb577-161">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="fb577-162">使用例</span><span class="sxs-lookup"><span data-stu-id="fb577-162">Example</span></span>

### <a name="csv"></a><span data-ttu-id="fb577-163">CSV</span><span class="sxs-lookup"><span data-stu-id="fb577-163">CSV</span></span>

<span data-ttu-id="fb577-164">次に、CSV を出力する例を示します。</span><span class="sxs-lookup"><span data-stu-id="fb577-164">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="fb577-165">要求</span><span class="sxs-lookup"><span data-stu-id="fb577-165">Request</span></span>

<span data-ttu-id="fb577-166">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fb577-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagedetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="fb577-167">応答</span><span class="sxs-lookup"><span data-stu-id="fb577-167">Response</span></span>

<span data-ttu-id="fb577-168">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fb577-168">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="fb577-169">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="fb577-169">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="fb577-170">JSON</span><span class="sxs-lookup"><span data-stu-id="fb577-170">JSON</span></span>

<span data-ttu-id="fb577-171">次に、JSON を取得する例を示します。</span><span class="sxs-lookup"><span data-stu-id="fb577-171">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="fb577-172">要求</span><span class="sxs-lookup"><span data-stu-id="fb577-172">Request</span></span>

<span data-ttu-id="fb577-173">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fb577-173">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagedetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="fb577-174">応答</span><span class="sxs-lookup"><span data-stu-id="fb577-174">Response</span></span>

<span data-ttu-id="fb577-175">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fb577-175">The following is an example of the response.</span></span>

> <span data-ttu-id="fb577-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="fb577-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
