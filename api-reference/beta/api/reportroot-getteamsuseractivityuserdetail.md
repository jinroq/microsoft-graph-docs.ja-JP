---
title: 'reportRoot: getTeamsUserActivityUserDetail'
description: ユーザーごとに、Microsoft Teams ユーザー アクティビティの詳細を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 453be7fcb51aecf3bfd237b0d65708341f169b8b
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33639097"
---
# <a name="reportroot-getteamsuseractivityuserdetail"></a><span data-ttu-id="1e8a6-103">reportRoot: getTeamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="1e8a6-103">reportRoot: getTeamsUserActivityUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e8a6-104">ユーザーごとに、Microsoft Teams ユーザー アクティビティの詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="1e8a6-104">Get details about Microsoft Teams user activity by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="1e8a6-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1e8a6-105">Permissions</span></span>

<span data-ttu-id="1e8a6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1e8a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1e8a6-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1e8a6-108">Permission type</span></span>                        | <span data-ttu-id="1e8a6-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1e8a6-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="1e8a6-110">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="1e8a6-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="1e8a6-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1e8a6-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="1e8a6-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1e8a6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e8a6-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1e8a6-113">Not supported.</span></span>                           |
| <span data-ttu-id="1e8a6-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1e8a6-114">Application</span></span>                            | <span data-ttu-id="1e8a6-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1e8a6-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="1e8a6-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1e8a6-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserDetail(period='D7')
GET /reports/getTeamsUserActivityUserDetail(date=2017-09-01)
```

## <a name="function-parameters"></a><span data-ttu-id="1e8a6-117">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="1e8a6-117">Function parameters</span></span>

<span data-ttu-id="1e8a6-118">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="1e8a6-118">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="1e8a6-119">パラメーター</span><span class="sxs-lookup"><span data-stu-id="1e8a6-119">Parameter</span></span> | <span data-ttu-id="1e8a6-120">型</span><span class="sxs-lookup"><span data-stu-id="1e8a6-120">Type</span></span>   | <span data-ttu-id="1e8a6-121">説明</span><span class="sxs-lookup"><span data-stu-id="1e8a6-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="1e8a6-122">period</span><span class="sxs-lookup"><span data-stu-id="1e8a6-122">period</span></span>    | <span data-ttu-id="1e8a6-123">文字列</span><span class="sxs-lookup"><span data-stu-id="1e8a6-123">string</span></span> | <span data-ttu-id="1e8a6-124">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="1e8a6-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="1e8a6-125">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="1e8a6-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="1e8a6-126">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="1e8a6-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="1e8a6-127">date</span><span class="sxs-lookup"><span data-stu-id="1e8a6-127">date</span></span>      | <span data-ttu-id="1e8a6-128">日付</span><span class="sxs-lookup"><span data-stu-id="1e8a6-128">Date</span></span>   | <span data-ttu-id="1e8a6-129">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="1e8a6-129">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="1e8a6-130">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="1e8a6-130">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="1e8a6-131">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="1e8a6-131">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="1e8a6-132">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1e8a6-132">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="1e8a6-133">このメソッドは、応答をカスタマイズするための `$format`、`$top`、`$skipToken` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="1e8a6-133">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="1e8a6-134">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="1e8a6-134">The default output type is text/csv.</span></span> <span data-ttu-id="1e8a6-135">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="1e8a6-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1e8a6-136">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1e8a6-136">Request headers</span></span>

| <span data-ttu-id="1e8a6-137">名前</span><span class="sxs-lookup"><span data-stu-id="1e8a6-137">Name</span></span>          | <span data-ttu-id="1e8a6-138">説明</span><span class="sxs-lookup"><span data-stu-id="1e8a6-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="1e8a6-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e8a6-139">Authorization</span></span> | <span data-ttu-id="1e8a6-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1e8a6-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="1e8a6-142">応答</span><span class="sxs-lookup"><span data-stu-id="1e8a6-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="1e8a6-143">CSV</span><span class="sxs-lookup"><span data-stu-id="1e8a6-143">CSV</span></span>

<span data-ttu-id="1e8a6-144">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="1e8a6-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="1e8a6-145">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="1e8a6-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="1e8a6-146">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="1e8a6-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="1e8a6-147">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="1e8a6-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="1e8a6-148">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="1e8a6-148">Report Refresh Date</span></span>
- <span data-ttu-id="1e8a6-149">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="1e8a6-149">User Principal Name</span></span>
- <span data-ttu-id="1e8a6-150">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="1e8a6-150">Last Activity Date</span></span>
- <span data-ttu-id="1e8a6-151">削除済み</span><span class="sxs-lookup"><span data-stu-id="1e8a6-151">Is Deleted</span></span>
- <span data-ttu-id="1e8a6-152">削除日</span><span class="sxs-lookup"><span data-stu-id="1e8a6-152">Deleted Date</span></span>
- <span data-ttu-id="1e8a6-153">割り当て済み製品</span><span class="sxs-lookup"><span data-stu-id="1e8a6-153">Assigned Products</span></span>
- <span data-ttu-id="1e8a6-154">チーム チャット メッセージ数</span><span class="sxs-lookup"><span data-stu-id="1e8a6-154">Team Chat Message Count</span></span>
- <span data-ttu-id="1e8a6-155">非公開チャット メッセージ数</span><span class="sxs-lookup"><span data-stu-id="1e8a6-155">Private Chat Message Count</span></span>
- <span data-ttu-id="1e8a6-156">通話数</span><span class="sxs-lookup"><span data-stu-id="1e8a6-156">Call Count</span></span>
- <span data-ttu-id="1e8a6-157">会議数</span><span class="sxs-lookup"><span data-stu-id="1e8a6-157">Meeting Count</span></span>
- <span data-ttu-id="1e8a6-158">その他のアクションの有無</span><span class="sxs-lookup"><span data-stu-id="1e8a6-158">Has Other Action</span></span>
- <span data-ttu-id="1e8a6-159">レポート期間</span><span class="sxs-lookup"><span data-stu-id="1e8a6-159">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="1e8a6-160">JSON</span><span class="sxs-lookup"><span data-stu-id="1e8a6-160">JSON</span></span>

<span data-ttu-id="1e8a6-161">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[Teamsuseractivityuserdetail](../resources/teamsuseractivityuserdetail.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1e8a6-161">If successful, this method returns a `200 OK` response code and a **[teamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="1e8a6-162">この要求の既定のページサイズは2000アイテムです。</span><span class="sxs-lookup"><span data-stu-id="1e8a6-162">The default page size for this request is 2000 items.</span></span>

## <a name="example"></a><span data-ttu-id="1e8a6-163">例</span><span class="sxs-lookup"><span data-stu-id="1e8a6-163">Example</span></span>

### <a name="csv"></a><span data-ttu-id="1e8a6-164">CSV</span><span class="sxs-lookup"><span data-stu-id="1e8a6-164">CSV</span></span>

<span data-ttu-id="1e8a6-165">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1e8a6-165">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="1e8a6-166">要求</span><span class="sxs-lookup"><span data-stu-id="1e8a6-166">Request</span></span>

<span data-ttu-id="1e8a6-167">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1e8a6-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="1e8a6-168">応答</span><span class="sxs-lookup"><span data-stu-id="1e8a6-168">Response</span></span>

<span data-ttu-id="1e8a6-169">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1e8a6-169">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="1e8a6-170">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="1e8a6-170">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1e8a6-171">Visual</span><span class="sxs-lookup"><span data-stu-id="1e8a6-171">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getteamsuseractivityuserdetail_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1e8a6-172">Java</span><span class="sxs-lookup"><span data-stu-id="1e8a6-172">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getteamsuseractivityuserdetail_csv-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="1e8a6-173">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="1e8a6-173">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="1e8a6-174">JSON</span><span class="sxs-lookup"><span data-stu-id="1e8a6-174">JSON</span></span>

<span data-ttu-id="1e8a6-175">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="1e8a6-175">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="1e8a6-176">要求</span><span class="sxs-lookup"><span data-stu-id="1e8a6-176">Request</span></span>

<span data-ttu-id="1e8a6-177">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1e8a6-177">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="1e8a6-178">応答</span><span class="sxs-lookup"><span data-stu-id="1e8a6-178">Response</span></span>

<span data-ttu-id="1e8a6-179">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1e8a6-179">The following is an example of the response.</span></span>

> <span data-ttu-id="1e8a6-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="1e8a6-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="1e8a6-182">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="1e8a6-182">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1e8a6-183">Visual</span><span class="sxs-lookup"><span data-stu-id="1e8a6-183">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getteamsuseractivityuserdetail_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1e8a6-184">Java</span><span class="sxs-lookup"><span data-stu-id="1e8a6-184">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getteamsuseractivityuserdetail_json-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getteamsuseractivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getteamsuseractivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getteamsuseractivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getteamsuseractivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
