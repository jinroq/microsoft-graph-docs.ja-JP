---
title: 'reportRoot: getYammerActivityUserDetail'
description: ユーザー別の Yammer アクティビティに関する詳細を取得します。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 152e275aa794ca01f8b7b6bc7c067cfe536440a6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27929453"
---
# <a name="reportroot-getyammeractivityuserdetail"></a><span data-ttu-id="c6981-103">reportRoot: getYammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="c6981-103">reportRoot: getYammerActivityUserDetail</span></span>

<span data-ttu-id="c6981-104">ユーザー別の Yammer アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="c6981-104">Get details about Yammer activity by user.</span></span>

> <span data-ttu-id="c6981-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer アクティビティ](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c6981-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="permissions"></a><span data-ttu-id="c6981-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c6981-106">Permissions</span></span>

<span data-ttu-id="c6981-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c6981-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c6981-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c6981-109">Permission type</span></span>                        | <span data-ttu-id="c6981-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c6981-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="c6981-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="c6981-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c6981-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6981-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="c6981-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c6981-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6981-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c6981-114">Not supported.</span></span>                           |
| <span data-ttu-id="c6981-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c6981-115">Application</span></span>                            | <span data-ttu-id="c6981-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6981-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="c6981-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c6981-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerActivityUserDetail(period='{period_value}')
GET /reports/getYammerActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="c6981-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="c6981-118">Function parameters</span></span>

<span data-ttu-id="c6981-119">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="c6981-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="c6981-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="c6981-120">Parameter</span></span> | <span data-ttu-id="c6981-121">型</span><span class="sxs-lookup"><span data-stu-id="c6981-121">Type</span></span>   | <span data-ttu-id="c6981-122">説明</span><span class="sxs-lookup"><span data-stu-id="c6981-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="c6981-123">period</span><span class="sxs-lookup"><span data-stu-id="c6981-123">period</span></span>    | <span data-ttu-id="c6981-124">文字列</span><span class="sxs-lookup"><span data-stu-id="c6981-124">string</span></span> | <span data-ttu-id="c6981-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="c6981-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="c6981-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="c6981-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="c6981-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="c6981-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="c6981-128">date</span><span class="sxs-lookup"><span data-stu-id="c6981-128">date</span></span>      | <span data-ttu-id="c6981-129">日付</span><span class="sxs-lookup"><span data-stu-id="c6981-129">Date</span></span>   | <span data-ttu-id="c6981-130">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="c6981-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="c6981-131">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="c6981-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="c6981-132">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="c6981-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="c6981-133">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c6981-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c6981-134">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c6981-134">Request headers</span></span>

| <span data-ttu-id="c6981-135">名前</span><span class="sxs-lookup"><span data-stu-id="c6981-135">Name</span></span>          | <span data-ttu-id="c6981-136">説明</span><span class="sxs-lookup"><span data-stu-id="c6981-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="c6981-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="c6981-137">Authorization</span></span> | <span data-ttu-id="c6981-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c6981-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="c6981-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="c6981-140">If-None-Match</span></span> | <span data-ttu-id="c6981-141">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="c6981-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="c6981-142">省略可能。</span><span class="sxs-lookup"><span data-stu-id="c6981-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="c6981-143">応答</span><span class="sxs-lookup"><span data-stu-id="c6981-143">Response</span></span>

<span data-ttu-id="c6981-144">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="c6981-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="c6981-145">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="c6981-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="c6981-146">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="c6981-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="c6981-147">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="c6981-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="c6981-148">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="c6981-148">Report Refresh Date</span></span>
- <span data-ttu-id="c6981-149">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="c6981-149">User Principal Name</span></span>
- <span data-ttu-id="c6981-150">表示名</span><span class="sxs-lookup"><span data-stu-id="c6981-150">Display Name</span></span>
- <span data-ttu-id="c6981-151">ユーザーの状態</span><span class="sxs-lookup"><span data-stu-id="c6981-151">User State</span></span>
- <span data-ttu-id="c6981-152">状態変更日付</span><span class="sxs-lookup"><span data-stu-id="c6981-152">State Change Date</span></span>
- <span data-ttu-id="c6981-153">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="c6981-153">Last Activity Date</span></span>
- <span data-ttu-id="c6981-154">投稿数</span><span class="sxs-lookup"><span data-stu-id="c6981-154">Posted Count</span></span>
- <span data-ttu-id="c6981-155">読み取り数</span><span class="sxs-lookup"><span data-stu-id="c6981-155">Read Count</span></span>
- <span data-ttu-id="c6981-156">「いいね!」の数</span><span class="sxs-lookup"><span data-stu-id="c6981-156">Liked Count</span></span>
- <span data-ttu-id="c6981-157">割り当て済み製品</span><span class="sxs-lookup"><span data-stu-id="c6981-157">Assigned Products</span></span>
- <span data-ttu-id="c6981-158">レポート期間</span><span class="sxs-lookup"><span data-stu-id="c6981-158">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="c6981-159">例</span><span class="sxs-lookup"><span data-stu-id="c6981-159">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c6981-160">要求</span><span class="sxs-lookup"><span data-stu-id="c6981-160">Request</span></span>

<span data-ttu-id="c6981-161">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c6981-161">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammeractivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerActivityUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="c6981-162">応答</span><span class="sxs-lookup"><span data-stu-id="c6981-162">Response</span></span>

<span data-ttu-id="c6981-163">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c6981-163">The following is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.report" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

#### <a name="request"></a><span data-ttu-id="c6981-164">要求</span><span class="sxs-lookup"><span data-stu-id="c6981-164">Request</span></span>

<span data-ttu-id="c6981-165">場合、`date`パラメーターを指定すると、レポートのスコープは、特定の日に行われた活動をします。</span><span class="sxs-lookup"><span data-stu-id="c6981-165">If the `date` parameter is specified, the report is scoped to activities that took place on the given date.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammeractivityuserdetail_date"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerActivityUserDetail(date='2018-03-05')
```

#### <a name="response"></a><span data-ttu-id="c6981-166">応答</span><span class="sxs-lookup"><span data-stu-id="c6981-166">Response</span></span>

<span data-ttu-id="c6981-167">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c6981-167">The following is an example of the response.</span></span>

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


<span data-ttu-id="c6981-168">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="c6981-168">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,User State,State Change Date,Last Activity Date,Posted Count,Read Count,Liked Count,Assigned Products,Report Period
```
