---
title: 'reportRoot: getSkypeForBusinessDeviceUsageUserCounts'
description: Skype for Business アプリを使用して接続した組織内のユーザー数について、使用傾向を取得します。 組織内で Skype for Business クライアント アプリをインストールし、使用したデバイスの種類 (Windows、Windows スマートフォン、Android スマートフォン、iPhone、iPad) の詳細も取得できます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 6af0cd07545d57ccf1278a9f46ce8a157b3184f1
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35276224"
---
# <a name="reportroot-getskypeforbusinessdeviceusageusercounts"></a><span data-ttu-id="9be9c-104">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="9be9c-104">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span></span>

<span data-ttu-id="9be9c-105">Skype for Business アプリを使用して接続した組織内のユーザー数について、使用傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="9be9c-105">Get the usage trends on how many users in your organization have connected using the Skype for Business app.</span></span> <span data-ttu-id="9be9c-106">組織内で Skype for Business クライアント アプリをインストールし、使用したデバイスの種類 (Windows、Windows スマートフォン、Android スマートフォン、iPhone、iPad) の詳細も取得できます。</span><span class="sxs-lookup"><span data-stu-id="9be9c-106">You will also get a breakdown by the type of device (Windows, Windows phone, Android phone, iPhone, or iPad) on which the Skype for Business client app is installed and used across your organization.</span></span>

> <span data-ttu-id="9be9c-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: 使用している Skype for Business クライアント](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9be9c-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="9be9c-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9be9c-108">Permissions</span></span>

<span data-ttu-id="9be9c-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9be9c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9be9c-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9be9c-111">Permission type</span></span>                        | <span data-ttu-id="9be9c-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9be9c-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="9be9c-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="9be9c-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="9be9c-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9be9c-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="9be9c-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9be9c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9be9c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9be9c-116">Not supported.</span></span>                           |
| <span data-ttu-id="9be9c-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9be9c-117">Application</span></span>                            | <span data-ttu-id="9be9c-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9be9c-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="9be9c-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9be9c-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="9be9c-120">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="9be9c-120">Function parameters</span></span>

<span data-ttu-id="9be9c-121">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="9be9c-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="9be9c-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="9be9c-122">Parameter</span></span> | <span data-ttu-id="9be9c-123">型</span><span class="sxs-lookup"><span data-stu-id="9be9c-123">Type</span></span>   | <span data-ttu-id="9be9c-124">説明</span><span class="sxs-lookup"><span data-stu-id="9be9c-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="9be9c-125">period</span><span class="sxs-lookup"><span data-stu-id="9be9c-125">period</span></span>    | <span data-ttu-id="9be9c-126">文字列</span><span class="sxs-lookup"><span data-stu-id="9be9c-126">string</span></span> | <span data-ttu-id="9be9c-127">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="9be9c-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="9be9c-128">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="9be9c-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="9be9c-129">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="9be9c-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="9be9c-130">必須。</span><span class="sxs-lookup"><span data-stu-id="9be9c-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="9be9c-131">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9be9c-131">Request headers</span></span>

| <span data-ttu-id="9be9c-132">名前</span><span class="sxs-lookup"><span data-stu-id="9be9c-132">Name</span></span>          | <span data-ttu-id="9be9c-133">説明</span><span class="sxs-lookup"><span data-stu-id="9be9c-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="9be9c-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="9be9c-134">Authorization</span></span> | <span data-ttu-id="9be9c-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9be9c-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="9be9c-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="9be9c-137">If-None-Match</span></span> | <span data-ttu-id="9be9c-138">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="9be9c-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="9be9c-139">省略可能。</span><span class="sxs-lookup"><span data-stu-id="9be9c-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="9be9c-140">応答</span><span class="sxs-lookup"><span data-stu-id="9be9c-140">Response</span></span>

<span data-ttu-id="9be9c-141">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="9be9c-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="9be9c-142">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="9be9c-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="9be9c-143">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="9be9c-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="9be9c-144">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="9be9c-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="9be9c-145">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="9be9c-145">Report Refresh Date</span></span>
- <span data-ttu-id="9be9c-146">Windows</span><span class="sxs-lookup"><span data-stu-id="9be9c-146">Windows</span></span>
- <span data-ttu-id="9be9c-147">Windows スマートフォン</span><span class="sxs-lookup"><span data-stu-id="9be9c-147">Windows Phone</span></span>
- <span data-ttu-id="9be9c-148">Android スマートフォン</span><span class="sxs-lookup"><span data-stu-id="9be9c-148">Android Phone</span></span>
- <span data-ttu-id="9be9c-149">iPhone</span><span class="sxs-lookup"><span data-stu-id="9be9c-149">iPhone</span></span>
- <span data-ttu-id="9be9c-150">iPad</span><span class="sxs-lookup"><span data-stu-id="9be9c-150">iPad</span></span>
- <span data-ttu-id="9be9c-151">レポート日付</span><span class="sxs-lookup"><span data-stu-id="9be9c-151">Report Date</span></span>
- <span data-ttu-id="9be9c-152">レポート期間</span><span class="sxs-lookup"><span data-stu-id="9be9c-152">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="9be9c-153">例</span><span class="sxs-lookup"><span data-stu-id="9be9c-153">Example</span></span>

#### <a name="request"></a><span data-ttu-id="9be9c-154">要求</span><span class="sxs-lookup"><span data-stu-id="9be9c-154">Request</span></span>

<span data-ttu-id="9be9c-155">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9be9c-155">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessdeviceusageusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessDeviceUsageUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="9be9c-156">応答</span><span class="sxs-lookup"><span data-stu-id="9be9c-156">Response</span></span>

<span data-ttu-id="9be9c-157">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9be9c-157">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="9be9c-158">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="9be9c-158">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="9be9c-159">C#</span><span class="sxs-lookup"><span data-stu-id="9be9c-159">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessdeviceusageusercounts-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9be9c-160">Javascript</span><span class="sxs-lookup"><span data-stu-id="9be9c-160">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessdeviceusageusercounts-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="9be9c-161">目的-C</span><span class="sxs-lookup"><span data-stu-id="9be9c-161">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessdeviceusageusercounts-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="9be9c-162">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="9be9c-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Windows,Windows Phone,Android Phone,iPhone,iPad,Report Date,Report Period
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
    "Error: /api-reference/v1.0/api/reportroot-getskypeforbusinessdeviceusageusercounts.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/reportroot-getskypeforbusinessdeviceusageusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getskypeforbusinessdeviceusageusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
