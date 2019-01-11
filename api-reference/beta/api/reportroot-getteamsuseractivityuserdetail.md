---
title: 'reportRoot: getTeamsUserActivityUserDetail'
description: ユーザーごとに、Microsoft Teams ユーザー アクティビティの詳細を取得します。
localization_priority: Normal
ms.openlocfilehash: 7c007acc9988db8dc9e4e7bfdf2440178b1ca445
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815338"
---
# <a name="reportroot-getteamsuseractivityuserdetail"></a><span data-ttu-id="a3658-103">reportRoot: getTeamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="a3658-103">reportRoot: getTeamsUserActivityUserDetail</span></span>

> <span data-ttu-id="a3658-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a3658-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a3658-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a3658-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a3658-106">ユーザーごとに、Microsoft Teams ユーザー アクティビティの詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="a3658-106">Get details about Microsoft Teams user activity by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="a3658-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a3658-107">Permissions</span></span>

<span data-ttu-id="a3658-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a3658-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a3658-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a3658-110">Permission type</span></span>                        | <span data-ttu-id="a3658-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a3658-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="a3658-112">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="a3658-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a3658-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a3658-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="a3658-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a3658-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3658-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a3658-115">Not supported.</span></span>                           |
| <span data-ttu-id="a3658-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a3658-116">Application</span></span>                            | <span data-ttu-id="a3658-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a3658-117">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="a3658-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a3658-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserDetail(period='D7')
GET /reports/getTeamsUserActivityUserDetail(date=2017-09-01)
```

## <a name="function-parameters"></a><span data-ttu-id="a3658-119">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="a3658-119">Function parameters</span></span>

<span data-ttu-id="a3658-120">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="a3658-120">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="a3658-121">パラメーター</span><span class="sxs-lookup"><span data-stu-id="a3658-121">Parameter</span></span> | <span data-ttu-id="a3658-122">Type</span><span class="sxs-lookup"><span data-stu-id="a3658-122">Type</span></span>   | <span data-ttu-id="a3658-123">説明</span><span class="sxs-lookup"><span data-stu-id="a3658-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="a3658-124">period</span><span class="sxs-lookup"><span data-stu-id="a3658-124">period</span></span>    | <span data-ttu-id="a3658-125">文字列</span><span class="sxs-lookup"><span data-stu-id="a3658-125">string</span></span> | <span data-ttu-id="a3658-126">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="a3658-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="a3658-127">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="a3658-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="a3658-128">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="a3658-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="a3658-129">date</span><span class="sxs-lookup"><span data-stu-id="a3658-129">date</span></span>      | <span data-ttu-id="a3658-130">日付</span><span class="sxs-lookup"><span data-stu-id="a3658-130">Date</span></span>   | <span data-ttu-id="a3658-131">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="a3658-131">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="a3658-132">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="a3658-132">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="a3658-133">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="a3658-133">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="a3658-134">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a3658-134">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="a3658-135">このメソッドは、応答をカスタマイズするための `$format`、`$top`、`$skipToken` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="a3658-135">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="a3658-136">既定の出力の種類は、テキストまたは csv です。</span><span class="sxs-lookup"><span data-stu-id="a3658-136">The default output type is text/csv.</span></span> <span data-ttu-id="a3658-137">ただし、出力の種類を指定する場合は、設定をテキストまたは csv またはアプリケーションまたは json OData $format クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="a3658-137">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a3658-138">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a3658-138">Request headers</span></span>

| <span data-ttu-id="a3658-139">名前</span><span class="sxs-lookup"><span data-stu-id="a3658-139">Name</span></span>          | <span data-ttu-id="a3658-140">説明</span><span class="sxs-lookup"><span data-stu-id="a3658-140">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="a3658-141">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3658-141">Authorization</span></span> | <span data-ttu-id="a3658-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a3658-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="a3658-144">応答</span><span class="sxs-lookup"><span data-stu-id="a3658-144">Response</span></span>

### <a name="csv"></a><span data-ttu-id="a3658-145">CSV</span><span class="sxs-lookup"><span data-stu-id="a3658-145">CSV</span></span>

<span data-ttu-id="a3658-146">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="a3658-146">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="a3658-147">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="a3658-147">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="a3658-148">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="a3658-148">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="a3658-149">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="a3658-149">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="a3658-150">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="a3658-150">Report Refresh Date</span></span>
- <span data-ttu-id="a3658-151">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="a3658-151">User Principal Name</span></span>
- <span data-ttu-id="a3658-152">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="a3658-152">Last Activity Date</span></span>
- <span data-ttu-id="a3658-153">削除済み</span><span class="sxs-lookup"><span data-stu-id="a3658-153">Is Deleted</span></span>
- <span data-ttu-id="a3658-154">削除日</span><span class="sxs-lookup"><span data-stu-id="a3658-154">Deleted Date</span></span>
- <span data-ttu-id="a3658-155">割り当て済み製品</span><span class="sxs-lookup"><span data-stu-id="a3658-155">Assigned Products</span></span>
- <span data-ttu-id="a3658-156">チーム チャット メッセージ数</span><span class="sxs-lookup"><span data-stu-id="a3658-156">Team Chat Message Count</span></span>
- <span data-ttu-id="a3658-157">非公開チャット メッセージ数</span><span class="sxs-lookup"><span data-stu-id="a3658-157">Private Chat Message Count</span></span>
- <span data-ttu-id="a3658-158">通話数</span><span class="sxs-lookup"><span data-stu-id="a3658-158">Call Count</span></span>
- <span data-ttu-id="a3658-159">会議数</span><span class="sxs-lookup"><span data-stu-id="a3658-159">Meeting Count</span></span>
- <span data-ttu-id="a3658-160">その他のアクションの有無</span><span class="sxs-lookup"><span data-stu-id="a3658-160">Has Other Action</span></span>
- <span data-ttu-id="a3658-161">レポート期間</span><span class="sxs-lookup"><span data-stu-id="a3658-161">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="a3658-162">JSON</span><span class="sxs-lookup"><span data-stu-id="a3658-162">JSON</span></span>

<span data-ttu-id="a3658-163">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に**[teamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md)** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="a3658-163">If successful, this method returns a `200 OK` response code and a **[teamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="a3658-164">この要求の既定のページ サイズは、2000 のアイテムです。</span><span class="sxs-lookup"><span data-stu-id="a3658-164">The default page size for this request is 2000 items.</span></span>

## <a name="example"></a><span data-ttu-id="a3658-165">例</span><span class="sxs-lookup"><span data-stu-id="a3658-165">Example</span></span>

### <a name="csv"></a><span data-ttu-id="a3658-166">CSV</span><span class="sxs-lookup"><span data-stu-id="a3658-166">CSV</span></span>

<span data-ttu-id="a3658-167">次に、CSV を出力する例を示します。</span><span class="sxs-lookup"><span data-stu-id="a3658-167">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="a3658-168">要求</span><span class="sxs-lookup"><span data-stu-id="a3658-168">Request</span></span>

<span data-ttu-id="a3658-169">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a3658-169">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="a3658-170">応答</span><span class="sxs-lookup"><span data-stu-id="a3658-170">Response</span></span>

<span data-ttu-id="a3658-171">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a3658-171">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="a3658-172">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="a3658-172">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Is Deleted,Deleted Date,Assigned Products,Team Chat Message Count,Private Chat Message Count,Call Count,Meeting Count,Has Other Action,Report Period
```

### <a name="json"></a><span data-ttu-id="a3658-173">JSON</span><span class="sxs-lookup"><span data-stu-id="a3658-173">JSON</span></span>

<span data-ttu-id="a3658-174">次に、JSON を取得する例を示します。</span><span class="sxs-lookup"><span data-stu-id="a3658-174">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="a3658-175">要求</span><span class="sxs-lookup"><span data-stu-id="a3658-175">Request</span></span>

<span data-ttu-id="a3658-176">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a3658-176">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="a3658-177">応答</span><span class="sxs-lookup"><span data-stu-id="a3658-177">Response</span></span>

<span data-ttu-id="a3658-178">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a3658-178">The following is an example of the response.</span></span>

> <span data-ttu-id="a3658-p108">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="a3658-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsUserActivityUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 452

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsUserActivityUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "lastActivityDate": "2017-09-01", 
      "isDeleted": false, 
      "deletedDate": null, 
      "assignedProducts": [
        "OFFICE 365 ENTERPRISE E5"
      ], 
      "teamChatMessageCount": 0, 
      "privateChatMessageCount": 49, 
      "callCount": 2, 
      "meetingCount": 0, 
      "hasOtherAction": true, 
      "reportPeriod": "7"
    }
  ]
}
```
