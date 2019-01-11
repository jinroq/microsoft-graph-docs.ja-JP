---
title: 'reportRoot: getYammerDeviceUsageUserCounts'
description: デバイスの種類別に日次ユーザーの数を取得します。
localization_priority: Normal
ms.openlocfilehash: f4387ac7761f2b2360e8aa4bf9789ba7ecdfef5a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867817"
---
# <a name="reportroot-getyammerdeviceusageusercounts"></a><span data-ttu-id="2a7fa-103">reportRoot: getYammerDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="2a7fa-103">reportRoot: getYammerDeviceUsageUserCounts</span></span>

<span data-ttu-id="2a7fa-104">デバイスの種類別に日次ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="2a7fa-104">Get the number of daily users by device type.</span></span>

> <span data-ttu-id="2a7fa-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer デバイスの使用状況](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2a7fa-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="2a7fa-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2a7fa-106">Permissions</span></span>

<span data-ttu-id="2a7fa-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2a7fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2a7fa-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2a7fa-109">Permission type</span></span>                        | <span data-ttu-id="2a7fa-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2a7fa-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="2a7fa-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="2a7fa-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2a7fa-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2a7fa-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="2a7fa-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2a7fa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a7fa-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2a7fa-114">Not supported.</span></span>                           |
| <span data-ttu-id="2a7fa-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2a7fa-115">Application</span></span>                            | <span data-ttu-id="2a7fa-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2a7fa-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="2a7fa-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2a7fa-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="2a7fa-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="2a7fa-118">Function parameters</span></span>

<span data-ttu-id="2a7fa-119">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="2a7fa-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="2a7fa-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="2a7fa-120">Parameter</span></span> | <span data-ttu-id="2a7fa-121">Type</span><span class="sxs-lookup"><span data-stu-id="2a7fa-121">Type</span></span>   | <span data-ttu-id="2a7fa-122">説明</span><span class="sxs-lookup"><span data-stu-id="2a7fa-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="2a7fa-123">period</span><span class="sxs-lookup"><span data-stu-id="2a7fa-123">period</span></span>    | <span data-ttu-id="2a7fa-124">文字列</span><span class="sxs-lookup"><span data-stu-id="2a7fa-124">string</span></span> | <span data-ttu-id="2a7fa-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="2a7fa-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="2a7fa-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="2a7fa-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="2a7fa-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="2a7fa-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="2a7fa-128">必須。</span><span class="sxs-lookup"><span data-stu-id="2a7fa-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="2a7fa-129">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2a7fa-129">Request headers</span></span>

| <span data-ttu-id="2a7fa-130">名前</span><span class="sxs-lookup"><span data-stu-id="2a7fa-130">Name</span></span>          | <span data-ttu-id="2a7fa-131">説明</span><span class="sxs-lookup"><span data-stu-id="2a7fa-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="2a7fa-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a7fa-132">Authorization</span></span> | <span data-ttu-id="2a7fa-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2a7fa-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="2a7fa-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="2a7fa-135">If-None-Match</span></span> | <span data-ttu-id="2a7fa-136">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="2a7fa-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="2a7fa-137">省略可能。</span><span class="sxs-lookup"><span data-stu-id="2a7fa-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="2a7fa-138">応答</span><span class="sxs-lookup"><span data-stu-id="2a7fa-138">Response</span></span>

<span data-ttu-id="2a7fa-139">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="2a7fa-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="2a7fa-140">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="2a7fa-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="2a7fa-141">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="2a7fa-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="2a7fa-142">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="2a7fa-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="2a7fa-143">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="2a7fa-143">Report Refresh Date</span></span>
- <span data-ttu-id="2a7fa-144">Web</span><span class="sxs-lookup"><span data-stu-id="2a7fa-144">Web</span></span>
- <span data-ttu-id="2a7fa-145">Windows スマートフォン</span><span class="sxs-lookup"><span data-stu-id="2a7fa-145">Windows Phone</span></span>
- <span data-ttu-id="2a7fa-146">Android スマートフォン</span><span class="sxs-lookup"><span data-stu-id="2a7fa-146">Android Phone</span></span>
- <span data-ttu-id="2a7fa-147">iPhone</span><span class="sxs-lookup"><span data-stu-id="2a7fa-147">iPhone</span></span>
- <span data-ttu-id="2a7fa-148">iPad</span><span class="sxs-lookup"><span data-stu-id="2a7fa-148">iPad</span></span>
- <span data-ttu-id="2a7fa-149">その他</span><span class="sxs-lookup"><span data-stu-id="2a7fa-149">Other</span></span>
- <span data-ttu-id="2a7fa-150">レポート日付</span><span class="sxs-lookup"><span data-stu-id="2a7fa-150">Report Date</span></span>
- <span data-ttu-id="2a7fa-151">レポート期間</span><span class="sxs-lookup"><span data-stu-id="2a7fa-151">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="2a7fa-152">例</span><span class="sxs-lookup"><span data-stu-id="2a7fa-152">Example</span></span>

#### <a name="request"></a><span data-ttu-id="2a7fa-153">要求</span><span class="sxs-lookup"><span data-stu-id="2a7fa-153">Request</span></span>

<span data-ttu-id="2a7fa-154">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2a7fa-154">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammerdeviceusageusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerDeviceUsageUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="2a7fa-155">応答</span><span class="sxs-lookup"><span data-stu-id="2a7fa-155">Response</span></span>

<span data-ttu-id="2a7fa-156">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2a7fa-156">The following is an example of the response.</span></span>

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

<span data-ttu-id="2a7fa-157">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="2a7fa-157">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iPhone,iPad,Other,Report Date,Report Period
```
