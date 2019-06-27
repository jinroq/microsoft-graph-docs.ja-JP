---
title: 'reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts'
description: 組織内で実施されたピア ツー ピア セッションの長さ (分数) と種類についての使用傾向を取得します。 セッションの種類には、オーディオとビデオが含まれます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 5e9affeb4b7903f5e247d2f2998fac2d7af23135
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35277211"
---
# <a name="reportroot-getskypeforbusinesspeertopeeractivityminutecounts"></a><span data-ttu-id="e377d-104">reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="e377d-104">reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts</span></span>

<span data-ttu-id="e377d-105">組織内で実施されたピア ツー ピア セッションの長さ (分数) と種類についての使用傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="e377d-105">Get usage trends on the length in minutes and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="e377d-106">セッションの種類には、オーディオとビデオが含まれます。</span><span class="sxs-lookup"><span data-stu-id="e377d-106">Types of sessions include audio and video.</span></span>

> <span data-ttu-id="e377d-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Skype for Business ピア ツー ピア アクティビティ](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e377d-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="permissions"></a><span data-ttu-id="e377d-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e377d-108">Permissions</span></span>

<span data-ttu-id="e377d-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e377d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e377d-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e377d-111">Permission type</span></span>                        | <span data-ttu-id="e377d-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e377d-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e377d-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="e377d-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="e377d-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e377d-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e377d-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e377d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e377d-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e377d-116">Not supported.</span></span>                           |
| <span data-ttu-id="e377d-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e377d-117">Application</span></span>                            | <span data-ttu-id="e377d-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e377d-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="e377d-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e377d-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="e377d-120">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="e377d-120">Function parameters</span></span>

<span data-ttu-id="e377d-121">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="e377d-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="e377d-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="e377d-122">Parameter</span></span> | <span data-ttu-id="e377d-123">型</span><span class="sxs-lookup"><span data-stu-id="e377d-123">Type</span></span>   | <span data-ttu-id="e377d-124">説明</span><span class="sxs-lookup"><span data-stu-id="e377d-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="e377d-125">period</span><span class="sxs-lookup"><span data-stu-id="e377d-125">period</span></span>    | <span data-ttu-id="e377d-126">文字列</span><span class="sxs-lookup"><span data-stu-id="e377d-126">string</span></span> | <span data-ttu-id="e377d-127">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="e377d-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="e377d-128">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="e377d-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="e377d-129">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="e377d-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="e377d-130">必須。</span><span class="sxs-lookup"><span data-stu-id="e377d-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="e377d-131">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e377d-131">Request headers</span></span>

| <span data-ttu-id="e377d-132">名前</span><span class="sxs-lookup"><span data-stu-id="e377d-132">Name</span></span>          | <span data-ttu-id="e377d-133">説明</span><span class="sxs-lookup"><span data-stu-id="e377d-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="e377d-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="e377d-134">Authorization</span></span> | <span data-ttu-id="e377d-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e377d-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="e377d-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="e377d-137">If-None-Match</span></span> | <span data-ttu-id="e377d-138">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="e377d-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="e377d-139">省略可能。</span><span class="sxs-lookup"><span data-stu-id="e377d-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="e377d-140">応答</span><span class="sxs-lookup"><span data-stu-id="e377d-140">Response</span></span>

<span data-ttu-id="e377d-141">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="e377d-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e377d-142">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="e377d-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e377d-143">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="e377d-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e377d-144">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="e377d-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="e377d-145">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="e377d-145">Report Refresh Date</span></span>
- <span data-ttu-id="e377d-146">レポート日付</span><span class="sxs-lookup"><span data-stu-id="e377d-146">Report Date</span></span>
- <span data-ttu-id="e377d-147">レポート期間</span><span class="sxs-lookup"><span data-stu-id="e377d-147">Report Period</span></span>
- <span data-ttu-id="e377d-148">オーディオ</span><span class="sxs-lookup"><span data-stu-id="e377d-148">Audio</span></span>
- <span data-ttu-id="e377d-149">ビデオ</span><span class="sxs-lookup"><span data-stu-id="e377d-149">Video</span></span>

## <a name="example"></a><span data-ttu-id="e377d-150">例</span><span class="sxs-lookup"><span data-stu-id="e377d-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="e377d-151">要求</span><span class="sxs-lookup"><span data-stu-id="e377d-151">Request</span></span>

<span data-ttu-id="e377d-152">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e377d-152">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinesspeertopeeractivityminutecounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="e377d-153">応答</span><span class="sxs-lookup"><span data-stu-id="e377d-153">Response</span></span>

<span data-ttu-id="e377d-154">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e377d-154">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="e377d-155">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="e377d-155">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e377d-156">C#</span><span class="sxs-lookup"><span data-stu-id="e377d-156">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinesspeertopeeractivityminutecounts-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e377d-157">Javascript</span><span class="sxs-lookup"><span data-stu-id="e377d-157">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinesspeertopeeractivityminutecounts-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e377d-158">目的-C</span><span class="sxs-lookup"><span data-stu-id="e377d-158">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinesspeertopeeractivityminutecounts-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="e377d-159">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="e377d-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Audio,Video
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
    "Error: /api-reference/v1.0/api/reportroot-getskypeforbusinesspeertopeeractivityminutecounts.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/reportroot-getskypeforbusinesspeertopeeractivityminutecounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getskypeforbusinesspeertopeeractivityminutecounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
