---
title: 'reportRoot: getYammerDeviceUsageUserCounts'
description: デバイスの種類別に日次ユーザーの数を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: fc304242a44bd46e8127c7c2be966852484c3873
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561384"
---
# <a name="reportroot-getyammerdeviceusageusercounts"></a><span data-ttu-id="49fc3-103">reportRoot: getYammerDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="49fc3-103">reportRoot: getYammerDeviceUsageUserCounts</span></span>

<span data-ttu-id="49fc3-104">デバイスの種類別に日次ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="49fc3-104">Get the number of daily users by device type.</span></span>

> <span data-ttu-id="49fc3-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer デバイスの使用状況](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="49fc3-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="49fc3-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="49fc3-106">Permissions</span></span>

<span data-ttu-id="49fc3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="49fc3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="49fc3-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="49fc3-109">Permission type</span></span>                        | <span data-ttu-id="49fc3-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="49fc3-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="49fc3-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="49fc3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="49fc3-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="49fc3-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="49fc3-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="49fc3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49fc3-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="49fc3-114">Not supported.</span></span>                           |
| <span data-ttu-id="49fc3-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="49fc3-115">Application</span></span>                            | <span data-ttu-id="49fc3-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="49fc3-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="49fc3-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="49fc3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="49fc3-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="49fc3-118">Function parameters</span></span>

<span data-ttu-id="49fc3-119">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="49fc3-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="49fc3-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="49fc3-120">Parameter</span></span> | <span data-ttu-id="49fc3-121">型</span><span class="sxs-lookup"><span data-stu-id="49fc3-121">Type</span></span>   | <span data-ttu-id="49fc3-122">説明</span><span class="sxs-lookup"><span data-stu-id="49fc3-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="49fc3-123">period</span><span class="sxs-lookup"><span data-stu-id="49fc3-123">period</span></span>    | <span data-ttu-id="49fc3-124">文字列</span><span class="sxs-lookup"><span data-stu-id="49fc3-124">string</span></span> | <span data-ttu-id="49fc3-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="49fc3-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="49fc3-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="49fc3-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="49fc3-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="49fc3-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="49fc3-128">必須。</span><span class="sxs-lookup"><span data-stu-id="49fc3-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="49fc3-129">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="49fc3-129">Request headers</span></span>

| <span data-ttu-id="49fc3-130">名前</span><span class="sxs-lookup"><span data-stu-id="49fc3-130">Name</span></span>          | <span data-ttu-id="49fc3-131">説明</span><span class="sxs-lookup"><span data-stu-id="49fc3-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="49fc3-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="49fc3-132">Authorization</span></span> | <span data-ttu-id="49fc3-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="49fc3-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="49fc3-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="49fc3-135">If-None-Match</span></span> | <span data-ttu-id="49fc3-136">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="49fc3-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="49fc3-137">省略可能。</span><span class="sxs-lookup"><span data-stu-id="49fc3-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="49fc3-138">応答</span><span class="sxs-lookup"><span data-stu-id="49fc3-138">Response</span></span>

<span data-ttu-id="49fc3-139">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="49fc3-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="49fc3-140">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="49fc3-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="49fc3-141">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="49fc3-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="49fc3-142">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="49fc3-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="49fc3-143">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="49fc3-143">Report Refresh Date</span></span>
- <span data-ttu-id="49fc3-144">Web</span><span class="sxs-lookup"><span data-stu-id="49fc3-144">Web</span></span>
- <span data-ttu-id="49fc3-145">Windows スマートフォン</span><span class="sxs-lookup"><span data-stu-id="49fc3-145">Windows Phone</span></span>
- <span data-ttu-id="49fc3-146">Android スマートフォン</span><span class="sxs-lookup"><span data-stu-id="49fc3-146">Android Phone</span></span>
- <span data-ttu-id="49fc3-147">iPhone</span><span class="sxs-lookup"><span data-stu-id="49fc3-147">iPhone</span></span>
- <span data-ttu-id="49fc3-148">iPad</span><span class="sxs-lookup"><span data-stu-id="49fc3-148">iPad</span></span>
- <span data-ttu-id="49fc3-149">その他</span><span class="sxs-lookup"><span data-stu-id="49fc3-149">Other</span></span>
- <span data-ttu-id="49fc3-150">レポート日付</span><span class="sxs-lookup"><span data-stu-id="49fc3-150">Report Date</span></span>
- <span data-ttu-id="49fc3-151">レポート期間</span><span class="sxs-lookup"><span data-stu-id="49fc3-151">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="49fc3-152">例</span><span class="sxs-lookup"><span data-stu-id="49fc3-152">Example</span></span>

#### <a name="request"></a><span data-ttu-id="49fc3-153">要求</span><span class="sxs-lookup"><span data-stu-id="49fc3-153">Request</span></span>

<span data-ttu-id="49fc3-154">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="49fc3-154">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammerdeviceusageusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerDeviceUsageUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="49fc3-155">応答</span><span class="sxs-lookup"><span data-stu-id="49fc3-155">Response</span></span>

<span data-ttu-id="49fc3-156">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="49fc3-156">The following is an example of the response.</span></span>

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

<span data-ttu-id="49fc3-157">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="49fc3-157">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iPhone,iPad,Other,Report Date,Report Period
```
