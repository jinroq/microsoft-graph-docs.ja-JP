---
title: 'reportRoot: getTeamsDeviceUsageDistributionUserCounts'
description: デバイスの種類ごとに、選択した期間の Microsoft Teams のユニーク ユーザーの数を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 5f50634d8107d95af6708361a88284122325b5ef
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574832"
---
# <a name="reportroot-getteamsdeviceusagedistributionusercounts"></a><span data-ttu-id="8a8f4-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="8a8f4-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span></span>

<span data-ttu-id="8a8f4-104">デバイスの種類ごとに、選択した期間の Microsoft Teams のユニーク ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="8a8f4-104">Get the number of Microsoft Teams unique users by device type over the selected time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="8a8f4-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8a8f4-105">Permissions</span></span>

<span data-ttu-id="8a8f4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8a8f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8a8f4-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8a8f4-108">Permission type</span></span>                        | <span data-ttu-id="8a8f4-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8a8f4-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="8a8f4-110">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="8a8f4-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8a8f4-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8a8f4-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="8a8f4-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8a8f4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a8f4-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8a8f4-113">Not supported.</span></span>                           |
| <span data-ttu-id="8a8f4-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8a8f4-114">Application</span></span>                            | <span data-ttu-id="8a8f4-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8a8f4-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="8a8f4-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8a8f4-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="8a8f4-117">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="8a8f4-117">Function parameters</span></span>

<span data-ttu-id="8a8f4-118">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="8a8f4-118">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="8a8f4-119">パラメーター</span><span class="sxs-lookup"><span data-stu-id="8a8f4-119">Parameter</span></span> | <span data-ttu-id="8a8f4-120">型</span><span class="sxs-lookup"><span data-stu-id="8a8f4-120">Type</span></span>   | <span data-ttu-id="8a8f4-121">説明</span><span class="sxs-lookup"><span data-stu-id="8a8f4-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="8a8f4-122">period</span><span class="sxs-lookup"><span data-stu-id="8a8f4-122">period</span></span>    | <span data-ttu-id="8a8f4-123">文字列</span><span class="sxs-lookup"><span data-stu-id="8a8f4-123">string</span></span> | <span data-ttu-id="8a8f4-124">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="8a8f4-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="8a8f4-125">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="8a8f4-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="8a8f4-126">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="8a8f4-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="8a8f4-127">必須。</span><span class="sxs-lookup"><span data-stu-id="8a8f4-127">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="8a8f4-128">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8a8f4-128">Request headers</span></span>

| <span data-ttu-id="8a8f4-129">名前</span><span class="sxs-lookup"><span data-stu-id="8a8f4-129">Name</span></span>          | <span data-ttu-id="8a8f4-130">説明</span><span class="sxs-lookup"><span data-stu-id="8a8f4-130">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="8a8f4-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a8f4-131">Authorization</span></span> | <span data-ttu-id="8a8f4-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8a8f4-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="8a8f4-134">応答</span><span class="sxs-lookup"><span data-stu-id="8a8f4-134">Response</span></span>

<span data-ttu-id="8a8f4-135">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="8a8f4-135">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="8a8f4-136">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="8a8f4-136">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="8a8f4-137">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="8a8f4-137">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="8a8f4-138">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="8a8f4-138">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="8a8f4-139">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="8a8f4-139">Report Refresh Date</span></span>
- <span data-ttu-id="8a8f4-140">Web</span><span class="sxs-lookup"><span data-stu-id="8a8f4-140">Web</span></span>
- <span data-ttu-id="8a8f4-141">Windows スマートフォン</span><span class="sxs-lookup"><span data-stu-id="8a8f4-141">Windows Phone</span></span>
- <span data-ttu-id="8a8f4-142">Android スマートフォン</span><span class="sxs-lookup"><span data-stu-id="8a8f4-142">Android Phone</span></span>
- <span data-ttu-id="8a8f4-143">iOS</span><span class="sxs-lookup"><span data-stu-id="8a8f4-143">iOS</span></span>
- <span data-ttu-id="8a8f4-144">Mac</span><span class="sxs-lookup"><span data-stu-id="8a8f4-144">Mac</span></span>
- <span data-ttu-id="8a8f4-145">Windows</span><span class="sxs-lookup"><span data-stu-id="8a8f4-145">Windows</span></span>
- <span data-ttu-id="8a8f4-146">レポート期間</span><span class="sxs-lookup"><span data-stu-id="8a8f4-146">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="8a8f4-147">例</span><span class="sxs-lookup"><span data-stu-id="8a8f4-147">Example</span></span>

#### <a name="request"></a><span data-ttu-id="8a8f4-148">要求</span><span class="sxs-lookup"><span data-stu-id="8a8f4-148">Request</span></span>

<span data-ttu-id="8a8f4-149">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8a8f4-149">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="8a8f4-150">応答</span><span class="sxs-lookup"><span data-stu-id="8a8f4-150">Response</span></span>

<span data-ttu-id="8a8f4-151">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8a8f4-151">The following is an example of the response.</span></span>

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

<span data-ttu-id="8a8f4-152">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="8a8f4-152">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iOS,Mac,Windows,Report Period
```
