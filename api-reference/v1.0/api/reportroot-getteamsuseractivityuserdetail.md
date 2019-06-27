---
title: 'reportRoot: getTeamsUserActivityUserDetail'
description: ユーザーごとに、Microsoft Teams ユーザー アクティビティの詳細を取得します。
localization_priority: Priority
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 1d5fce97a59dae80aab8792dd9b477d08a3bdb3d
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35273200"
---
# <a name="reportroot-getteamsuseractivityuserdetail"></a><span data-ttu-id="42c27-103">reportRoot: getTeamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="42c27-103">reportRoot: getTeamsUserActivityUserDetail</span></span>

<span data-ttu-id="42c27-104">ユーザーごとに、Microsoft Teams ユーザー アクティビティの詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="42c27-104">Get details about Microsoft Teams user activity by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="42c27-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="42c27-105">Permissions</span></span>

<span data-ttu-id="42c27-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="42c27-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="42c27-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="42c27-108">Permission type</span></span>                        | <span data-ttu-id="42c27-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="42c27-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="42c27-110">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="42c27-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="42c27-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="42c27-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="42c27-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="42c27-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42c27-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="42c27-113">Not supported.</span></span>                           |
| <span data-ttu-id="42c27-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="42c27-114">Application</span></span>                            | <span data-ttu-id="42c27-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="42c27-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="42c27-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="42c27-116">HTTP request</span></span>

<!-- { "blockType": "samples" } -->

```http
GET /reports/getTeamsUserActivityUserDetail(period='{period_value}')
GET /reports/getTeamsUserActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="42c27-117">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="42c27-117">Function parameters</span></span>

<span data-ttu-id="42c27-118">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="42c27-118">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="42c27-119">パラメーター</span><span class="sxs-lookup"><span data-stu-id="42c27-119">Parameter</span></span> | <span data-ttu-id="42c27-120">型</span><span class="sxs-lookup"><span data-stu-id="42c27-120">Type</span></span>   | <span data-ttu-id="42c27-121">説明</span><span class="sxs-lookup"><span data-stu-id="42c27-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="42c27-122">period</span><span class="sxs-lookup"><span data-stu-id="42c27-122">period</span></span>    | <span data-ttu-id="42c27-123">文字列</span><span class="sxs-lookup"><span data-stu-id="42c27-123">string</span></span> | <span data-ttu-id="42c27-124">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="42c27-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="42c27-125">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="42c27-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="42c27-126">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="42c27-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="42c27-127">date</span><span class="sxs-lookup"><span data-stu-id="42c27-127">date</span></span>      | <span data-ttu-id="42c27-128">日付</span><span class="sxs-lookup"><span data-stu-id="42c27-128">Date</span></span>   | <span data-ttu-id="42c27-129">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="42c27-129">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="42c27-130">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="42c27-130">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="42c27-131">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="42c27-131">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="42c27-132">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="42c27-132">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="42c27-133">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="42c27-133">Request headers</span></span>

| <span data-ttu-id="42c27-134">名前</span><span class="sxs-lookup"><span data-stu-id="42c27-134">Name</span></span>          | <span data-ttu-id="42c27-135">説明</span><span class="sxs-lookup"><span data-stu-id="42c27-135">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="42c27-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="42c27-136">Authorization</span></span> | <span data-ttu-id="42c27-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="42c27-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="42c27-139">応答</span><span class="sxs-lookup"><span data-stu-id="42c27-139">Response</span></span>

<span data-ttu-id="42c27-140">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="42c27-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="42c27-141">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="42c27-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="42c27-142">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="42c27-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="42c27-143">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="42c27-143">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="42c27-144">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="42c27-144">Report Refresh Date</span></span>
- <span data-ttu-id="42c27-145">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="42c27-145">User Principal Name</span></span>
- <span data-ttu-id="42c27-146">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="42c27-146">Last Activity Date</span></span>
- <span data-ttu-id="42c27-147">削除済み</span><span class="sxs-lookup"><span data-stu-id="42c27-147">Is Deleted</span></span>
- <span data-ttu-id="42c27-148">削除日</span><span class="sxs-lookup"><span data-stu-id="42c27-148">Deleted Date</span></span>
- <span data-ttu-id="42c27-149">割り当て済み製品</span><span class="sxs-lookup"><span data-stu-id="42c27-149">Assigned Products</span></span>
- <span data-ttu-id="42c27-150">チーム チャット メッセージ数</span><span class="sxs-lookup"><span data-stu-id="42c27-150">Team Chat Message Count</span></span>
- <span data-ttu-id="42c27-151">非公開チャット メッセージ数</span><span class="sxs-lookup"><span data-stu-id="42c27-151">Private Chat Message Count</span></span>
- <span data-ttu-id="42c27-152">通話数</span><span class="sxs-lookup"><span data-stu-id="42c27-152">Call Count</span></span>
- <span data-ttu-id="42c27-153">会議数</span><span class="sxs-lookup"><span data-stu-id="42c27-153">Meeting Count</span></span>
- <span data-ttu-id="42c27-154">その他のアクションの有無</span><span class="sxs-lookup"><span data-stu-id="42c27-154">Has Other Action</span></span>
- <span data-ttu-id="42c27-155">レポート期間</span><span class="sxs-lookup"><span data-stu-id="42c27-155">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="42c27-156">例</span><span class="sxs-lookup"><span data-stu-id="42c27-156">Example</span></span>

#### <a name="request"></a><span data-ttu-id="42c27-157">要求</span><span class="sxs-lookup"><span data-stu-id="42c27-157">Request</span></span>

<span data-ttu-id="42c27-158">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="42c27-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getTeamsUserActivityUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="42c27-159">応答</span><span class="sxs-lookup"><span data-stu-id="42c27-159">Response</span></span>

<span data-ttu-id="42c27-160">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="42c27-160">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="42c27-161">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="42c27-161">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="42c27-162">C#</span><span class="sxs-lookup"><span data-stu-id="42c27-162">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getteamsuseractivityuserdetail-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="42c27-163">Javascript</span><span class="sxs-lookup"><span data-stu-id="42c27-163">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getteamsuseractivityuserdetail-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="42c27-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="42c27-164">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getteamsuseractivityuserdetail-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="42c27-165">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="42c27-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Is Deleted,Deleted Date,Assigned Products,Team Chat Message Count,Private Chat Message Count,Call Count,Meeting Count,Has Other Action,Report Period
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
    "Error: /api-reference/v1.0/api/reportroot-getteamsuseractivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/reportroot-getteamsuseractivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getteamsuseractivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
