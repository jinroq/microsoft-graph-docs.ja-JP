---
title: 'reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts'
description: 組織内でそれぞれ別個のデバイスを使用するユーザーの数を取得します。 このレポートでは、Windows、Windows スマートフォン、Android スマートフォン、iPhone、iPad を含むデバイス別のユーザーの数を表示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 6fa19922b928e1d743b69869110ba96ce4a82b56
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35276238"
---
# <a name="reportroot-getskypeforbusinessdeviceusagedistributionusercounts"></a><span data-ttu-id="60a3e-104">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="60a3e-104">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span></span>

<span data-ttu-id="60a3e-105">組織内でそれぞれ別個のデバイスを使用するユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="60a3e-105">Get the number of users using unique devices in your organization.</span></span> <span data-ttu-id="60a3e-106">このレポートでは、Windows、Windows スマートフォン、Android スマートフォン、iPhone、iPad を含むデバイス別のユーザーの数を表示します。</span><span class="sxs-lookup"><span data-stu-id="60a3e-106">The report will show you the number of users per device including Windows, Windows phone, Android phone, iPhone, and iPad.</span></span>

> <span data-ttu-id="60a3e-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: 使用している Skype for Business クライアント](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="60a3e-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="60a3e-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="60a3e-108">Permissions</span></span>

<span data-ttu-id="60a3e-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="60a3e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="60a3e-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="60a3e-111">Permission type</span></span>                        | <span data-ttu-id="60a3e-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="60a3e-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="60a3e-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="60a3e-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="60a3e-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="60a3e-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="60a3e-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="60a3e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60a3e-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="60a3e-116">Not supported.</span></span>                           |
| <span data-ttu-id="60a3e-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="60a3e-117">Application</span></span>                            | <span data-ttu-id="60a3e-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="60a3e-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="60a3e-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="60a3e-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="60a3e-120">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="60a3e-120">Function parameters</span></span>

<span data-ttu-id="60a3e-121">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="60a3e-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="60a3e-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="60a3e-122">Parameter</span></span> | <span data-ttu-id="60a3e-123">型</span><span class="sxs-lookup"><span data-stu-id="60a3e-123">Type</span></span>   | <span data-ttu-id="60a3e-124">説明</span><span class="sxs-lookup"><span data-stu-id="60a3e-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="60a3e-125">period</span><span class="sxs-lookup"><span data-stu-id="60a3e-125">period</span></span>    | <span data-ttu-id="60a3e-126">文字列</span><span class="sxs-lookup"><span data-stu-id="60a3e-126">string</span></span> | <span data-ttu-id="60a3e-127">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="60a3e-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="60a3e-128">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="60a3e-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="60a3e-129">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="60a3e-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="60a3e-130">必須。</span><span class="sxs-lookup"><span data-stu-id="60a3e-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="60a3e-131">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="60a3e-131">Request headers</span></span>

| <span data-ttu-id="60a3e-132">名前</span><span class="sxs-lookup"><span data-stu-id="60a3e-132">Name</span></span>          | <span data-ttu-id="60a3e-133">説明</span><span class="sxs-lookup"><span data-stu-id="60a3e-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="60a3e-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="60a3e-134">Authorization</span></span> | <span data-ttu-id="60a3e-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="60a3e-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="60a3e-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="60a3e-137">If-None-Match</span></span> | <span data-ttu-id="60a3e-138">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="60a3e-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="60a3e-139">省略可能。</span><span class="sxs-lookup"><span data-stu-id="60a3e-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="60a3e-140">応答</span><span class="sxs-lookup"><span data-stu-id="60a3e-140">Response</span></span>

<span data-ttu-id="60a3e-141">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="60a3e-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="60a3e-142">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="60a3e-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="60a3e-143">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="60a3e-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="60a3e-144">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="60a3e-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="60a3e-145">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="60a3e-145">Report Refresh Date</span></span>
- <span data-ttu-id="60a3e-146">Windows</span><span class="sxs-lookup"><span data-stu-id="60a3e-146">Windows</span></span>
- <span data-ttu-id="60a3e-147">Windows スマートフォン</span><span class="sxs-lookup"><span data-stu-id="60a3e-147">Windows Phone</span></span>
- <span data-ttu-id="60a3e-148">Android スマートフォン</span><span class="sxs-lookup"><span data-stu-id="60a3e-148">Android Phone</span></span>
- <span data-ttu-id="60a3e-149">iPhone</span><span class="sxs-lookup"><span data-stu-id="60a3e-149">iPhone</span></span>
- <span data-ttu-id="60a3e-150">iPad</span><span class="sxs-lookup"><span data-stu-id="60a3e-150">iPad</span></span>
- <span data-ttu-id="60a3e-151">レポート期間</span><span class="sxs-lookup"><span data-stu-id="60a3e-151">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="60a3e-152">例</span><span class="sxs-lookup"><span data-stu-id="60a3e-152">Example</span></span>

#### <a name="request"></a><span data-ttu-id="60a3e-153">要求</span><span class="sxs-lookup"><span data-stu-id="60a3e-153">Request</span></span>

<span data-ttu-id="60a3e-154">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="60a3e-154">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessdeviceusagedistributionusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="60a3e-155">応答</span><span class="sxs-lookup"><span data-stu-id="60a3e-155">Response</span></span>

<span data-ttu-id="60a3e-156">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="60a3e-156">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="60a3e-157">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="60a3e-157">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="60a3e-158">C#</span><span class="sxs-lookup"><span data-stu-id="60a3e-158">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessdeviceusagedistributionusercounts-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="60a3e-159">Javascript</span><span class="sxs-lookup"><span data-stu-id="60a3e-159">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessdeviceusagedistributionusercounts-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="60a3e-160">目的-C</span><span class="sxs-lookup"><span data-stu-id="60a3e-160">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessdeviceusagedistributionusercounts-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="60a3e-161">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="60a3e-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Windows,Windows Phone,Android Phone,iPhone,iPad,Report Period
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
    "Error: /api-reference/v1.0/api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
