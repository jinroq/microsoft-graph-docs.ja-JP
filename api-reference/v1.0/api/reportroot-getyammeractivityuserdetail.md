---
title: 'reportRoot: getYammerActivityUserDetail'
description: ユーザー別の Yammer アクティビティに関する詳細を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 6fd8dde2aaa27471229443f3b0c3bc71c83cebb5
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35276840"
---
# <a name="reportroot-getyammeractivityuserdetail"></a><span data-ttu-id="1950d-103">reportRoot: getYammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="1950d-103">reportRoot: getYammerActivityUserDetail</span></span>

<span data-ttu-id="1950d-104">ユーザー別の Yammer アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="1950d-104">Get details about Yammer activity by user.</span></span>

> <span data-ttu-id="1950d-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer アクティビティ](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1950d-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="permissions"></a><span data-ttu-id="1950d-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1950d-106">Permissions</span></span>

<span data-ttu-id="1950d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1950d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1950d-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1950d-109">Permission type</span></span>                        | <span data-ttu-id="1950d-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1950d-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="1950d-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="1950d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1950d-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1950d-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="1950d-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1950d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1950d-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1950d-114">Not supported.</span></span>                           |
| <span data-ttu-id="1950d-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1950d-115">Application</span></span>                            | <span data-ttu-id="1950d-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1950d-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="1950d-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1950d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerActivityUserDetail(period='{period_value}')
GET /reports/getYammerActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="1950d-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="1950d-118">Function parameters</span></span>

<span data-ttu-id="1950d-119">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="1950d-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="1950d-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="1950d-120">Parameter</span></span> | <span data-ttu-id="1950d-121">型</span><span class="sxs-lookup"><span data-stu-id="1950d-121">Type</span></span>   | <span data-ttu-id="1950d-122">説明</span><span class="sxs-lookup"><span data-stu-id="1950d-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="1950d-123">period</span><span class="sxs-lookup"><span data-stu-id="1950d-123">period</span></span>    | <span data-ttu-id="1950d-124">文字列</span><span class="sxs-lookup"><span data-stu-id="1950d-124">string</span></span> | <span data-ttu-id="1950d-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="1950d-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="1950d-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="1950d-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="1950d-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="1950d-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="1950d-128">date</span><span class="sxs-lookup"><span data-stu-id="1950d-128">date</span></span>      | <span data-ttu-id="1950d-129">日付</span><span class="sxs-lookup"><span data-stu-id="1950d-129">Date</span></span>   | <span data-ttu-id="1950d-130">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="1950d-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="1950d-131">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="1950d-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="1950d-132">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="1950d-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="1950d-133">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1950d-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1950d-134">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1950d-134">Request headers</span></span>

| <span data-ttu-id="1950d-135">名前</span><span class="sxs-lookup"><span data-stu-id="1950d-135">Name</span></span>          | <span data-ttu-id="1950d-136">説明</span><span class="sxs-lookup"><span data-stu-id="1950d-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="1950d-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="1950d-137">Authorization</span></span> | <span data-ttu-id="1950d-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1950d-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="1950d-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="1950d-140">If-None-Match</span></span> | <span data-ttu-id="1950d-141">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="1950d-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="1950d-142">省略可能。</span><span class="sxs-lookup"><span data-stu-id="1950d-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="1950d-143">応答</span><span class="sxs-lookup"><span data-stu-id="1950d-143">Response</span></span>

<span data-ttu-id="1950d-144">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="1950d-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="1950d-145">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="1950d-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="1950d-146">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="1950d-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="1950d-147">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="1950d-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="1950d-148">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="1950d-148">Report Refresh Date</span></span>
- <span data-ttu-id="1950d-149">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="1950d-149">User Principal Name</span></span>
- <span data-ttu-id="1950d-150">表示名</span><span class="sxs-lookup"><span data-stu-id="1950d-150">Display Name</span></span>
- <span data-ttu-id="1950d-151">ユーザーの状態</span><span class="sxs-lookup"><span data-stu-id="1950d-151">User State</span></span>
- <span data-ttu-id="1950d-152">状態変更日付</span><span class="sxs-lookup"><span data-stu-id="1950d-152">State Change Date</span></span>
- <span data-ttu-id="1950d-153">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="1950d-153">Last Activity Date</span></span>
- <span data-ttu-id="1950d-154">投稿数</span><span class="sxs-lookup"><span data-stu-id="1950d-154">Posted Count</span></span>
- <span data-ttu-id="1950d-155">読み取り数</span><span class="sxs-lookup"><span data-stu-id="1950d-155">Read Count</span></span>
- <span data-ttu-id="1950d-156">「いいね!」の数</span><span class="sxs-lookup"><span data-stu-id="1950d-156">Liked Count</span></span>
- <span data-ttu-id="1950d-157">割り当て済み製品</span><span class="sxs-lookup"><span data-stu-id="1950d-157">Assigned Products</span></span>
- <span data-ttu-id="1950d-158">レポート期間</span><span class="sxs-lookup"><span data-stu-id="1950d-158">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="1950d-159">例</span><span class="sxs-lookup"><span data-stu-id="1950d-159">Example</span></span>

#### <a name="request"></a><span data-ttu-id="1950d-160">要求</span><span class="sxs-lookup"><span data-stu-id="1950d-160">Request</span></span>

<span data-ttu-id="1950d-161">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1950d-161">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammeractivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerActivityUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="1950d-162">応答</span><span class="sxs-lookup"><span data-stu-id="1950d-162">Response</span></span>

<span data-ttu-id="1950d-163">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1950d-163">The following is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.report" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="1950d-164">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="1950d-164">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1950d-165">C#</span><span class="sxs-lookup"><span data-stu-id="1950d-165">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getyammeractivityuserdetail-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1950d-166">Javascript</span><span class="sxs-lookup"><span data-stu-id="1950d-166">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getyammeractivityuserdetail-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="1950d-167">目的-C</span><span class="sxs-lookup"><span data-stu-id="1950d-167">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getyammeractivityuserdetail-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

#### <a name="request"></a><span data-ttu-id="1950d-168">要求</span><span class="sxs-lookup"><span data-stu-id="1950d-168">Request</span></span>

<span data-ttu-id="1950d-169">`date`パラメーターが指定されている場合、レポートのスコープは、指定された日付に行われたアクティビティになります。</span><span class="sxs-lookup"><span data-stu-id="1950d-169">If the `date` parameter is specified, the report is scoped to activities that took place on the given date.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammeractivityuserdetail_date"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerActivityUserDetail(date='2018-03-05')
```

#### <a name="response"></a><span data-ttu-id="1950d-170">応答</span><span class="sxs-lookup"><span data-stu-id="1950d-170">Response</span></span>

<span data-ttu-id="1950d-171">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1950d-171">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.report"
} -->

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```


<span data-ttu-id="1950d-172">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="1950d-172">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,User State,State Change Date,Last Activity Date,Posted Count,Read Count,Liked Count,Assigned Products,Report Period
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
    "Error: /api-reference/v1.0/api/reportroot-getyammeractivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/reportroot-getyammeractivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getyammeractivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
