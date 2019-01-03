---
title: 'reportRoot: getEmailActivityUserDetail'
description: ユーザーが実行した電子メール アクティビティに関する詳細を取得します。
ms.openlocfilehash: a7469a46f7063ade9d7b0fb241b548ca0c2a7e83
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070731"
---
# <a name="reportroot-getemailactivityuserdetail"></a><span data-ttu-id="b972f-103">reportRoot: getEmailActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="b972f-103">reportRoot: getEmailActivityUserDetail</span></span>

> <span data-ttu-id="b972f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b972f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b972f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b972f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b972f-106">ユーザーが実行した電子メール アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="b972f-106">Get details about email activity users have performed.</span></span>

> <span data-ttu-id="b972f-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: 電子メール アクティビティ](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b972f-107">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="permissions"></a><span data-ttu-id="b972f-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b972f-108">Permissions</span></span>

<span data-ttu-id="b972f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b972f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b972f-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b972f-111">Permission type</span></span>                        | <span data-ttu-id="b972f-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b972f-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b972f-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="b972f-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="b972f-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b972f-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b972f-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b972f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b972f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b972f-116">Not supported.</span></span>                           |
| <span data-ttu-id="b972f-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b972f-117">Application</span></span>                            | <span data-ttu-id="b972f-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b972f-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="b972f-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b972f-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailActivityUserDetail(period='{period_value}')
GET /reports/getEmailActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="b972f-120">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="b972f-120">Function parameters</span></span>

<span data-ttu-id="b972f-121">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="b972f-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="b972f-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="b972f-122">Parameter</span></span> | <span data-ttu-id="b972f-123">型</span><span class="sxs-lookup"><span data-stu-id="b972f-123">Type</span></span>   | <span data-ttu-id="b972f-124">説明</span><span class="sxs-lookup"><span data-stu-id="b972f-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b972f-125">period</span><span class="sxs-lookup"><span data-stu-id="b972f-125">period</span></span>    | <span data-ttu-id="b972f-126">文字列</span><span class="sxs-lookup"><span data-stu-id="b972f-126">string</span></span> | <span data-ttu-id="b972f-127">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="b972f-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b972f-128">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="b972f-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b972f-129">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="b972f-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="b972f-130">date</span><span class="sxs-lookup"><span data-stu-id="b972f-130">date</span></span>      | <span data-ttu-id="b972f-131">日付</span><span class="sxs-lookup"><span data-stu-id="b972f-131">Date</span></span>   | <span data-ttu-id="b972f-132">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="b972f-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="b972f-133">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="b972f-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="b972f-134">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="b972f-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="b972f-135">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b972f-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="b972f-136">このメソッドは、応答をカスタマイズするための `$format`、`$top`、`$skipToken` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="b972f-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="b972f-137">既定の出力の種類は、テキストまたは csv です。</span><span class="sxs-lookup"><span data-stu-id="b972f-137">The default output type is text/csv.</span></span> <span data-ttu-id="b972f-138">ただし、出力の種類を指定する場合は、設定をテキストまたは csv またはアプリケーションまたは json OData $format クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="b972f-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b972f-139">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b972f-139">Request headers</span></span>

| <span data-ttu-id="b972f-140">名前</span><span class="sxs-lookup"><span data-stu-id="b972f-140">Name</span></span>          | <span data-ttu-id="b972f-141">説明</span><span class="sxs-lookup"><span data-stu-id="b972f-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="b972f-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="b972f-142">Authorization</span></span> | <span data-ttu-id="b972f-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b972f-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="b972f-145">応答</span><span class="sxs-lookup"><span data-stu-id="b972f-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="b972f-146">CSV</span><span class="sxs-lookup"><span data-stu-id="b972f-146">CSV</span></span>

<span data-ttu-id="b972f-147">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="b972f-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b972f-148">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="b972f-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b972f-149">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="b972f-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b972f-150">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="b972f-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b972f-151">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="b972f-151">Report Refresh Date</span></span>
- <span data-ttu-id="b972f-152">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="b972f-152">User Principal Name</span></span>
- <span data-ttu-id="b972f-153">表示名</span><span class="sxs-lookup"><span data-stu-id="b972f-153">Display Name</span></span>
- <span data-ttu-id="b972f-154">削除済み</span><span class="sxs-lookup"><span data-stu-id="b972f-154">Is Deleted</span></span>
- <span data-ttu-id="b972f-155">削除日</span><span class="sxs-lookup"><span data-stu-id="b972f-155">Deleted Date</span></span>
- <span data-ttu-id="b972f-156">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="b972f-156">Last Activity Date</span></span>
- <span data-ttu-id="b972f-157">送信数</span><span class="sxs-lookup"><span data-stu-id="b972f-157">Send Count</span></span>
- <span data-ttu-id="b972f-158">受信数</span><span class="sxs-lookup"><span data-stu-id="b972f-158">Receive Count</span></span>
- <span data-ttu-id="b972f-159">読み取り数</span><span class="sxs-lookup"><span data-stu-id="b972f-159">Read Count</span></span>
- <span data-ttu-id="b972f-160">割り当て済み製品</span><span class="sxs-lookup"><span data-stu-id="b972f-160">Assigned Products</span></span>
- <span data-ttu-id="b972f-161">レポート期間</span><span class="sxs-lookup"><span data-stu-id="b972f-161">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="b972f-162">JSON</span><span class="sxs-lookup"><span data-stu-id="b972f-162">JSON</span></span>

<span data-ttu-id="b972f-163">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の**[emailActivityUserDetail](../resources/emailactivityuserdetail.md)** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="b972f-163">If successful, this method returns a `200 OK` response code and an **[emailActivityUserDetail](../resources/emailactivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="b972f-164">この要求の既定のページ サイズは、アイテムは 200 個です。</span><span class="sxs-lookup"><span data-stu-id="b972f-164">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="b972f-165">使用例</span><span class="sxs-lookup"><span data-stu-id="b972f-165">Example</span></span>

### <a name="csv"></a><span data-ttu-id="b972f-166">CSV</span><span class="sxs-lookup"><span data-stu-id="b972f-166">CSV</span></span>

<span data-ttu-id="b972f-167">次に、CSV を出力する例を示します。</span><span class="sxs-lookup"><span data-stu-id="b972f-167">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="b972f-168">要求</span><span class="sxs-lookup"><span data-stu-id="b972f-168">Request</span></span>

<span data-ttu-id="b972f-169">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b972f-169">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailactivityuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailActivityUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="b972f-170">応答</span><span class="sxs-lookup"><span data-stu-id="b972f-170">Response</span></span>

<span data-ttu-id="b972f-171">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b972f-171">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="b972f-172">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="b972f-172">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Last Activity Date,Send Count,Receive Count,Read Count,Assigned Products,Report Period
```

### <a name="json"></a><span data-ttu-id="b972f-173">JSON</span><span class="sxs-lookup"><span data-stu-id="b972f-173">JSON</span></span>

<span data-ttu-id="b972f-174">次に、JSON を取得する例を示します。</span><span class="sxs-lookup"><span data-stu-id="b972f-174">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="b972f-175">要求</span><span class="sxs-lookup"><span data-stu-id="b972f-175">Request</span></span>

<span data-ttu-id="b972f-176">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b972f-176">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailactivityuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailActivityUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="b972f-177">応答</span><span class="sxs-lookup"><span data-stu-id="b972f-177">Response</span></span>

<span data-ttu-id="b972f-178">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b972f-178">The following is an example of the response.</span></span>

> <span data-ttu-id="b972f-p108">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="b972f-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailActivityUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 424

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailActivityUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "displayName": "displayName-value", 
      "isDeleted": false, 
      "deletedDate": null, 
      "lastActivityDate": "2017-09-01", 
      "sendCount": 86, 
      "receiveCount": 3198, 
      "readCount": 388, 
      "assignedProducts": [
        "OFFICE 365 ENTERPRISE E5"
      ], 
      "reportPeriod": "7"
    }
  ]
}
```