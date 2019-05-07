---
title: 'reportRoot: getTeamsDeviceUsageUserCounts'
description: デバイスの種類ごとに、Microsoft Teams の日次ユニーク ユーザーの数を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 964c16e41889fe84a260af4f477aa27d8e67e02f
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33603973"
---
# <a name="reportroot-getteamsdeviceusageusercounts"></a><span data-ttu-id="fff3b-103">reportRoot: getTeamsDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="fff3b-103">reportRoot: getTeamsDeviceUsageUserCounts</span></span>

<span data-ttu-id="fff3b-104">デバイスの種類ごとに、Microsoft Teams の日次ユニーク ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="fff3b-104">Get the number of Microsoft Teams daily unique users by device type.</span></span>

## <a name="permissions"></a><span data-ttu-id="fff3b-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fff3b-105">Permissions</span></span>

<span data-ttu-id="fff3b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fff3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fff3b-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fff3b-108">Permission type</span></span>                        | <span data-ttu-id="fff3b-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fff3b-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="fff3b-110">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="fff3b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="fff3b-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fff3b-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="fff3b-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fff3b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fff3b-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fff3b-113">Not supported.</span></span>                           |
| <span data-ttu-id="fff3b-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fff3b-114">Application</span></span>                            | <span data-ttu-id="fff3b-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fff3b-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="fff3b-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fff3b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="fff3b-117">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="fff3b-117">Function parameters</span></span>

<span data-ttu-id="fff3b-118">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="fff3b-118">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="fff3b-119">パラメーター</span><span class="sxs-lookup"><span data-stu-id="fff3b-119">Parameter</span></span> | <span data-ttu-id="fff3b-120">型</span><span class="sxs-lookup"><span data-stu-id="fff3b-120">Type</span></span>   | <span data-ttu-id="fff3b-121">説明</span><span class="sxs-lookup"><span data-stu-id="fff3b-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="fff3b-122">period</span><span class="sxs-lookup"><span data-stu-id="fff3b-122">period</span></span>    | <span data-ttu-id="fff3b-123">文字列</span><span class="sxs-lookup"><span data-stu-id="fff3b-123">string</span></span> | <span data-ttu-id="fff3b-124">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="fff3b-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="fff3b-125">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="fff3b-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="fff3b-126">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="fff3b-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="fff3b-127">必須。</span><span class="sxs-lookup"><span data-stu-id="fff3b-127">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="fff3b-128">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fff3b-128">Request headers</span></span>

| <span data-ttu-id="fff3b-129">名前</span><span class="sxs-lookup"><span data-stu-id="fff3b-129">Name</span></span>          | <span data-ttu-id="fff3b-130">説明</span><span class="sxs-lookup"><span data-stu-id="fff3b-130">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="fff3b-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="fff3b-131">Authorization</span></span> | <span data-ttu-id="fff3b-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="fff3b-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="fff3b-134">応答</span><span class="sxs-lookup"><span data-stu-id="fff3b-134">Response</span></span>

<span data-ttu-id="fff3b-135">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="fff3b-135">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="fff3b-136">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="fff3b-136">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="fff3b-137">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="fff3b-137">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="fff3b-138">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="fff3b-138">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="fff3b-139">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="fff3b-139">Report Refresh Date</span></span>
- <span data-ttu-id="fff3b-140">Web</span><span class="sxs-lookup"><span data-stu-id="fff3b-140">Web</span></span>
- <span data-ttu-id="fff3b-141">Windows スマートフォン</span><span class="sxs-lookup"><span data-stu-id="fff3b-141">Windows Phone</span></span>
- <span data-ttu-id="fff3b-142">Android スマートフォン</span><span class="sxs-lookup"><span data-stu-id="fff3b-142">Android Phone</span></span>
- <span data-ttu-id="fff3b-143">iOS</span><span class="sxs-lookup"><span data-stu-id="fff3b-143">iOS</span></span>
- <span data-ttu-id="fff3b-144">Mac</span><span class="sxs-lookup"><span data-stu-id="fff3b-144">Mac</span></span>
- <span data-ttu-id="fff3b-145">Windows</span><span class="sxs-lookup"><span data-stu-id="fff3b-145">Windows</span></span>
- <span data-ttu-id="fff3b-146">レポート日付</span><span class="sxs-lookup"><span data-stu-id="fff3b-146">Report Date</span></span>
- <span data-ttu-id="fff3b-147">レポート期間</span><span class="sxs-lookup"><span data-stu-id="fff3b-147">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="fff3b-148">例</span><span class="sxs-lookup"><span data-stu-id="fff3b-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="fff3b-149">要求</span><span class="sxs-lookup"><span data-stu-id="fff3b-149">Request</span></span>

<span data-ttu-id="fff3b-150">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fff3b-150">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getTeamsDeviceUsageUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="fff3b-151">応答</span><span class="sxs-lookup"><span data-stu-id="fff3b-151">Response</span></span>

<span data-ttu-id="fff3b-152">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fff3b-152">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="fff3b-153">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="fff3b-153">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="fff3b-154">Visual</span><span class="sxs-lookup"><span data-stu-id="fff3b-154">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getteamsdeviceusageusercounts-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fff3b-155">Java</span><span class="sxs-lookup"><span data-stu-id="fff3b-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getteamsdeviceusageusercounts-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="fff3b-156">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="fff3b-156">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iOS,Mac,Windows,Report Date,Report Period
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
    "Error: /api-reference/v1.0/api/reportroot-getteamsdeviceusageusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getteamsdeviceusageusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
