---
title: 'reportRoot: getYammerActivityCounts'
description: 投稿、読み取り、および " いいね!" を付けられたメッセージの数によって、組織内での Yammer アクティビティの量の傾向を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: c35a841d3f7792d14ec905db484eaaa473d90255
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33603785"
---
# <a name="reportroot-getyammeractivitycounts"></a><span data-ttu-id="cee93-103">reportRoot: getYammerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="cee93-103">reportRoot: getYammerActivityCounts</span></span>

<span data-ttu-id="cee93-104">投稿、読み取り、および " いいね!" を付けられたメッセージの数によって、組織内での Yammer アクティビティの量の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="cee93-104">Get the trends on the amount of Yammer activity in your organization by how many messages were posted, read, and liked.</span></span>

> <span data-ttu-id="cee93-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer アクティビティ](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cee93-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="permissions"></a><span data-ttu-id="cee93-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cee93-106">Permissions</span></span>

<span data-ttu-id="cee93-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cee93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cee93-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cee93-109">Permission type</span></span>                        | <span data-ttu-id="cee93-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cee93-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="cee93-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="cee93-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cee93-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="cee93-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="cee93-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cee93-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cee93-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cee93-114">Not supported.</span></span>                           |
| <span data-ttu-id="cee93-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cee93-115">Application</span></span>                            | <span data-ttu-id="cee93-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="cee93-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="cee93-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cee93-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="cee93-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="cee93-118">Function parameters</span></span>

<span data-ttu-id="cee93-119">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="cee93-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="cee93-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="cee93-120">Parameter</span></span> | <span data-ttu-id="cee93-121">型</span><span class="sxs-lookup"><span data-stu-id="cee93-121">Type</span></span>   | <span data-ttu-id="cee93-122">説明</span><span class="sxs-lookup"><span data-stu-id="cee93-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="cee93-123">period</span><span class="sxs-lookup"><span data-stu-id="cee93-123">period</span></span>    | <span data-ttu-id="cee93-124">文字列</span><span class="sxs-lookup"><span data-stu-id="cee93-124">string</span></span> | <span data-ttu-id="cee93-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="cee93-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="cee93-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="cee93-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="cee93-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="cee93-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="cee93-128">必須。</span><span class="sxs-lookup"><span data-stu-id="cee93-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="cee93-129">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cee93-129">Request headers</span></span>

| <span data-ttu-id="cee93-130">名前</span><span class="sxs-lookup"><span data-stu-id="cee93-130">Name</span></span>          | <span data-ttu-id="cee93-131">説明</span><span class="sxs-lookup"><span data-stu-id="cee93-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="cee93-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="cee93-132">Authorization</span></span> | <span data-ttu-id="cee93-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="cee93-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="cee93-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="cee93-135">If-None-Match</span></span> | <span data-ttu-id="cee93-136">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="cee93-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="cee93-137">省略可能。</span><span class="sxs-lookup"><span data-stu-id="cee93-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="cee93-138">応答</span><span class="sxs-lookup"><span data-stu-id="cee93-138">Response</span></span>

<span data-ttu-id="cee93-139">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="cee93-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="cee93-140">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="cee93-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="cee93-141">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="cee93-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="cee93-142">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="cee93-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="cee93-143">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="cee93-143">Report Refresh Date</span></span>
- <span data-ttu-id="cee93-144">いいね!</span><span class="sxs-lookup"><span data-stu-id="cee93-144">Liked</span></span>
- <span data-ttu-id="cee93-145">投稿</span><span class="sxs-lookup"><span data-stu-id="cee93-145">Posted</span></span>
- <span data-ttu-id="cee93-146">読み取り</span><span class="sxs-lookup"><span data-stu-id="cee93-146">Read</span></span>
- <span data-ttu-id="cee93-147">レポート日付</span><span class="sxs-lookup"><span data-stu-id="cee93-147">Report Date</span></span>
- <span data-ttu-id="cee93-148">レポート期間</span><span class="sxs-lookup"><span data-stu-id="cee93-148">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="cee93-149">例</span><span class="sxs-lookup"><span data-stu-id="cee93-149">Example</span></span>

#### <a name="request"></a><span data-ttu-id="cee93-150">要求</span><span class="sxs-lookup"><span data-stu-id="cee93-150">Request</span></span>

<span data-ttu-id="cee93-151">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cee93-151">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammeractivitycounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerActivityCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="cee93-152">応答</span><span class="sxs-lookup"><span data-stu-id="cee93-152">Response</span></span>

<span data-ttu-id="cee93-153">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cee93-153">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="cee93-154">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="cee93-154">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="cee93-155">Visual</span><span class="sxs-lookup"><span data-stu-id="cee93-155">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getyammeractivitycounts-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cee93-156">Java</span><span class="sxs-lookup"><span data-stu-id="cee93-156">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getyammeractivitycounts-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="cee93-157">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="cee93-157">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Liked,Posted,Read,Report Date,Report Period
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
    "Error: /api-reference/v1.0/api/reportroot-getyammeractivitycounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getyammeractivitycounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
