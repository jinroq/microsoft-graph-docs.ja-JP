---
title: 'reportRoot: getYammerActivityUserDetail'
description: ユーザー別の Yammer アクティビティに関する詳細を取得します。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: a08447c8926c4448052285b22b36d5bd1bd0c2e4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523499"
---
# <a name="reportroot-getyammeractivityuserdetail"></a><span data-ttu-id="53374-103">reportRoot: getYammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="53374-103">reportRoot: getYammerActivityUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53374-104">ユーザー別の Yammer アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="53374-104">Get details about Yammer activity by user.</span></span>

> <span data-ttu-id="53374-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer アクティビティ](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="53374-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="permissions"></a><span data-ttu-id="53374-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="53374-106">Permissions</span></span>

<span data-ttu-id="53374-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="53374-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="53374-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="53374-109">Permission type</span></span>                        | <span data-ttu-id="53374-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="53374-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="53374-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="53374-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="53374-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="53374-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="53374-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="53374-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53374-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="53374-114">Not supported.</span></span>                           |
| <span data-ttu-id="53374-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="53374-115">Application</span></span>                            | <span data-ttu-id="53374-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="53374-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="53374-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="53374-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerActivityUserDetail(period='{period_value}')
GET /reports/getYammerActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="53374-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="53374-118">Function parameters</span></span>

<span data-ttu-id="53374-119">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="53374-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="53374-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="53374-120">Parameter</span></span> | <span data-ttu-id="53374-121">型</span><span class="sxs-lookup"><span data-stu-id="53374-121">Type</span></span>   | <span data-ttu-id="53374-122">説明</span><span class="sxs-lookup"><span data-stu-id="53374-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="53374-123">period</span><span class="sxs-lookup"><span data-stu-id="53374-123">period</span></span>    | <span data-ttu-id="53374-124">文字列</span><span class="sxs-lookup"><span data-stu-id="53374-124">string</span></span> | <span data-ttu-id="53374-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="53374-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="53374-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="53374-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="53374-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="53374-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="53374-128">date</span><span class="sxs-lookup"><span data-stu-id="53374-128">date</span></span>      | <span data-ttu-id="53374-129">日付</span><span class="sxs-lookup"><span data-stu-id="53374-129">Date</span></span>   | <span data-ttu-id="53374-130">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="53374-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="53374-131">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="53374-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="53374-132">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="53374-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="53374-133">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="53374-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="53374-134">このメソッドは、応答をカスタマイズするための `$format`、`$top`、`$skipToken` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="53374-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="53374-135">既定の出力の種類は、テキストまたは csv です。</span><span class="sxs-lookup"><span data-stu-id="53374-135">The default output type is text/csv.</span></span> <span data-ttu-id="53374-136">ただし、出力の種類を指定する場合は、設定をテキストまたは csv またはアプリケーションまたは json OData $format クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="53374-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="53374-137">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="53374-137">Request headers</span></span>

| <span data-ttu-id="53374-138">名前</span><span class="sxs-lookup"><span data-stu-id="53374-138">Name</span></span>          | <span data-ttu-id="53374-139">説明</span><span class="sxs-lookup"><span data-stu-id="53374-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="53374-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="53374-140">Authorization</span></span> | <span data-ttu-id="53374-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="53374-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="53374-143">応答</span><span class="sxs-lookup"><span data-stu-id="53374-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="53374-144">CSV</span><span class="sxs-lookup"><span data-stu-id="53374-144">CSV</span></span>

<span data-ttu-id="53374-145">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="53374-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="53374-146">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="53374-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="53374-147">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="53374-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="53374-148">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="53374-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="53374-149">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="53374-149">Report Refresh Date</span></span>
- <span data-ttu-id="53374-150">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="53374-150">User Principal Name</span></span>
- <span data-ttu-id="53374-151">表示名</span><span class="sxs-lookup"><span data-stu-id="53374-151">Display Name</span></span>
- <span data-ttu-id="53374-152">ユーザーの状態</span><span class="sxs-lookup"><span data-stu-id="53374-152">User State</span></span>
- <span data-ttu-id="53374-153">状態変更日付</span><span class="sxs-lookup"><span data-stu-id="53374-153">State Change Date</span></span>
- <span data-ttu-id="53374-154">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="53374-154">Last Activity Date</span></span>
- <span data-ttu-id="53374-155">投稿数</span><span class="sxs-lookup"><span data-stu-id="53374-155">Posted Count</span></span>
- <span data-ttu-id="53374-156">読み取り数</span><span class="sxs-lookup"><span data-stu-id="53374-156">Read Count</span></span>
- <span data-ttu-id="53374-157">「いいね!」の数</span><span class="sxs-lookup"><span data-stu-id="53374-157">Liked Count</span></span>
- <span data-ttu-id="53374-158">割り当て済み製品</span><span class="sxs-lookup"><span data-stu-id="53374-158">Assigned Products</span></span>
- <span data-ttu-id="53374-159">レポート期間</span><span class="sxs-lookup"><span data-stu-id="53374-159">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="53374-160">JSON</span><span class="sxs-lookup"><span data-stu-id="53374-160">JSON</span></span>

<span data-ttu-id="53374-161">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に**[yammerActivityUserDetail](../resources/yammeractivityuserdetail.md)** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="53374-161">If successful, this method returns a `200 OK` response code and a **[yammerActivityUserDetail](../resources/yammeractivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="53374-162">この要求の既定のページ サイズは、アイテムは 200 個です。</span><span class="sxs-lookup"><span data-stu-id="53374-162">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="53374-163">例</span><span class="sxs-lookup"><span data-stu-id="53374-163">Example</span></span>

### <a name="csv"></a><span data-ttu-id="53374-164">CSV</span><span class="sxs-lookup"><span data-stu-id="53374-164">CSV</span></span>

<span data-ttu-id="53374-165">次に、CSV を出力する例を示します。</span><span class="sxs-lookup"><span data-stu-id="53374-165">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="53374-166">要求</span><span class="sxs-lookup"><span data-stu-id="53374-166">Request</span></span>

<span data-ttu-id="53374-167">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="53374-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivityuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerActivityUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="53374-168">応答</span><span class="sxs-lookup"><span data-stu-id="53374-168">Response</span></span>

<span data-ttu-id="53374-169">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="53374-169">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="53374-170">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="53374-170">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,User State,State Change Date,Last Activity Date,Posted Count,Read Count,Liked Count,Assigned Products,Report Period
```

### <a name="json"></a><span data-ttu-id="53374-171">JSON</span><span class="sxs-lookup"><span data-stu-id="53374-171">JSON</span></span>

<span data-ttu-id="53374-172">次に、JSON を取得する例を示します。</span><span class="sxs-lookup"><span data-stu-id="53374-172">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="53374-173">要求</span><span class="sxs-lookup"><span data-stu-id="53374-173">Request</span></span>

<span data-ttu-id="53374-174">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="53374-174">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivityuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerActivityUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="53374-175">応答</span><span class="sxs-lookup"><span data-stu-id="53374-175">Response</span></span>

<span data-ttu-id="53374-176">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="53374-176">The following is an example of the response.</span></span>

> <span data-ttu-id="53374-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="53374-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerActivityUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 434

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerActivityUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "displayName": "displayName-value", 
      "userState": "active", 
      "stateChangeDate": "2015-08-26", 
      "lastActivityDate": "2017-09-01", 
      "postedCount": 2, 
      "readCount": 5, 
      "likedCount": 0, 
      "assignedProducts": [
        "OFFICE 365 ENTERPRISE E5"
      ], 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getyammeractivityuserdetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
