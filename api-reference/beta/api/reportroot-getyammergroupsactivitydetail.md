---
title: 'reportRoot: getYammerGroupsActivityDetail'
description: グループ別の Yammer グループ アクティビティに関する詳細を取得します。
ms.openlocfilehash: c13e7160d667d479f4f4ecf17287934bb9c78aa5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066786"
---
# <a name="reportroot-getyammergroupsactivitydetail"></a><span data-ttu-id="a251d-103">reportRoot: getYammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="a251d-103">reportRoot: getYammerGroupsActivityDetail</span></span>

> <span data-ttu-id="a251d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a251d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a251d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a251d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a251d-106">グループ別の Yammer グループ アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="a251d-106">Get details about Yammer groups activity by group.</span></span>

> <span data-ttu-id="a251d-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer グループ アクティビティ](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a251d-107">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="permissions"></a><span data-ttu-id="a251d-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a251d-108">Permissions</span></span>

<span data-ttu-id="a251d-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a251d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a251d-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a251d-111">Permission type</span></span>                        | <span data-ttu-id="a251d-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a251d-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="a251d-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="a251d-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="a251d-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a251d-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="a251d-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a251d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a251d-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a251d-116">Not supported.</span></span>                           |
| <span data-ttu-id="a251d-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a251d-117">Application</span></span>                            | <span data-ttu-id="a251d-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a251d-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="a251d-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a251d-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityDetail(period='{period_value}')
GET /reports/getYammerGroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="a251d-120">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="a251d-120">Function parameters</span></span>

<span data-ttu-id="a251d-121">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="a251d-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="a251d-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="a251d-122">Parameter</span></span> | <span data-ttu-id="a251d-123">型</span><span class="sxs-lookup"><span data-stu-id="a251d-123">Type</span></span>   | <span data-ttu-id="a251d-124">説明</span><span class="sxs-lookup"><span data-stu-id="a251d-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="a251d-125">period</span><span class="sxs-lookup"><span data-stu-id="a251d-125">period</span></span>    | <span data-ttu-id="a251d-126">文字列</span><span class="sxs-lookup"><span data-stu-id="a251d-126">string</span></span> | <span data-ttu-id="a251d-127">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="a251d-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="a251d-128">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="a251d-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="a251d-129">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="a251d-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="a251d-130">date</span><span class="sxs-lookup"><span data-stu-id="a251d-130">date</span></span>      | <span data-ttu-id="a251d-131">日付</span><span class="sxs-lookup"><span data-stu-id="a251d-131">Date</span></span>   | <span data-ttu-id="a251d-132">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="a251d-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="a251d-133">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="a251d-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="a251d-134">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="a251d-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="a251d-135">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a251d-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="a251d-136">このメソッドは、応答をカスタマイズするための `$format`、`$top`、`$skipToken` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="a251d-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="a251d-137">既定の出力の種類は、テキストまたは csv です。</span><span class="sxs-lookup"><span data-stu-id="a251d-137">The default output type is text/csv.</span></span> <span data-ttu-id="a251d-138">ただし、出力の種類を指定する場合は、設定をテキストまたは csv またはアプリケーションまたは json OData $format クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="a251d-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a251d-139">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a251d-139">Request headers</span></span>

| <span data-ttu-id="a251d-140">名前</span><span class="sxs-lookup"><span data-stu-id="a251d-140">Name</span></span>          | <span data-ttu-id="a251d-141">説明</span><span class="sxs-lookup"><span data-stu-id="a251d-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="a251d-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="a251d-142">Authorization</span></span> | <span data-ttu-id="a251d-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a251d-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="a251d-145">応答</span><span class="sxs-lookup"><span data-stu-id="a251d-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="a251d-146">CSV</span><span class="sxs-lookup"><span data-stu-id="a251d-146">CSV</span></span>

<span data-ttu-id="a251d-147">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="a251d-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="a251d-148">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="a251d-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="a251d-149">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="a251d-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="a251d-150">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="a251d-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="a251d-151">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="a251d-151">Report Refresh Date</span></span>
- <span data-ttu-id="a251d-152">グループ表示名</span><span class="sxs-lookup"><span data-stu-id="a251d-152">Group Display Name</span></span>
- <span data-ttu-id="a251d-153">削除済み</span><span class="sxs-lookup"><span data-stu-id="a251d-153">Is Deleted</span></span>
- <span data-ttu-id="a251d-154">所有者のプリンシパル名</span><span class="sxs-lookup"><span data-stu-id="a251d-154">Owner Principal Name</span></span>
- <span data-ttu-id="a251d-155">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="a251d-155">Last Activity Date</span></span>
- <span data-ttu-id="a251d-156">グループの種類</span><span class="sxs-lookup"><span data-stu-id="a251d-156">Group Type</span></span>
- <span data-ttu-id="a251d-157">Office 365 接続</span><span class="sxs-lookup"><span data-stu-id="a251d-157">Office 365 Connected</span></span>
- <span data-ttu-id="a251d-158">メンバー数</span><span class="sxs-lookup"><span data-stu-id="a251d-158">Member Count</span></span>
- <span data-ttu-id="a251d-159">投稿数</span><span class="sxs-lookup"><span data-stu-id="a251d-159">Posted Count</span></span>
- <span data-ttu-id="a251d-160">読み取り数</span><span class="sxs-lookup"><span data-stu-id="a251d-160">Read Count</span></span>
- <span data-ttu-id="a251d-161">「いいね!」の数</span><span class="sxs-lookup"><span data-stu-id="a251d-161">Liked Count</span></span>
- <span data-ttu-id="a251d-162">レポート期間</span><span class="sxs-lookup"><span data-stu-id="a251d-162">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="a251d-163">JSON</span><span class="sxs-lookup"><span data-stu-id="a251d-163">JSON</span></span>

<span data-ttu-id="a251d-164">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に**[yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md)** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="a251d-164">If successful, this method returns a `200 OK` response code and a **[yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md)** object in the response body.</span></span>

<span data-ttu-id="a251d-165">この要求の既定のページ サイズは、アイテムは 200 個です。</span><span class="sxs-lookup"><span data-stu-id="a251d-165">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="a251d-166">使用例</span><span class="sxs-lookup"><span data-stu-id="a251d-166">Example</span></span>

### <a name="csv"></a><span data-ttu-id="a251d-167">CSV</span><span class="sxs-lookup"><span data-stu-id="a251d-167">CSV</span></span>

<span data-ttu-id="a251d-168">次に、CSV を出力する例を示します。</span><span class="sxs-lookup"><span data-stu-id="a251d-168">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="a251d-169">要求</span><span class="sxs-lookup"><span data-stu-id="a251d-169">Request</span></span>

<span data-ttu-id="a251d-170">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a251d-170">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitydetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="a251d-171">応答</span><span class="sxs-lookup"><span data-stu-id="a251d-171">Response</span></span>

<span data-ttu-id="a251d-172">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a251d-172">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="a251d-173">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="a251d-173">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Group Display Name,Is Deleted,Owner Principal Name,Last Activity Date,Group Type,Office 365 Connected,Member Count,Posted Count,Read Count,Liked Count,Report Period
```

### <a name="json"></a><span data-ttu-id="a251d-174">JSON</span><span class="sxs-lookup"><span data-stu-id="a251d-174">JSON</span></span>

<span data-ttu-id="a251d-175">次に、JSON を取得する例を示します。</span><span class="sxs-lookup"><span data-stu-id="a251d-175">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="a251d-176">要求</span><span class="sxs-lookup"><span data-stu-id="a251d-176">Request</span></span>

<span data-ttu-id="a251d-177">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a251d-177">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitydetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="a251d-178">応答</span><span class="sxs-lookup"><span data-stu-id="a251d-178">Response</span></span>

<span data-ttu-id="a251d-179">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a251d-179">The following is an example of the response.</span></span>

> <span data-ttu-id="a251d-p108">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="a251d-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerGroupsActivityDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 441

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerGroupsActivityDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "groupDisplayName": "groupDisplayName-value", 
      "isDeleted": false, 
      "ownerPrincipalName": "ownerPrincipalName-value", 
      "lastActivityDate": "2017-08-30", 
      "groupType": "private", 
      "office365Connected": true, 
      "memberCount": 176, 
      "postedCount": 15, 
      "readCount": 24, 
      "likedCount": 3, 
      "reportPeriod": "7"
    }
  ]
}
```
