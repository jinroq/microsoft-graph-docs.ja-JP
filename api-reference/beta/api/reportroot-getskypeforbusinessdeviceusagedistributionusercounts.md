---
title: 'reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts'
description: 組織内でそれぞれ別個のデバイスを使用するユーザーの数を取得します。 このレポートでは、Windows、Windows スマートフォン、Android スマートフォン、iPhone、iPad を含むデバイス別のユーザーの数を表示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: eea7cd939705574189c45f08e83fc3d883f2fe1d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33336556"
---
# <a name="reportroot-getskypeforbusinessdeviceusagedistributionusercounts"></a><span data-ttu-id="5b06d-104">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="5b06d-104">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b06d-105">組織内でそれぞれ別個のデバイスを使用するユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="5b06d-105">Get the number of users using unique devices in your organization.</span></span> <span data-ttu-id="5b06d-106">このレポートでは、Windows、Windows スマートフォン、Android スマートフォン、iPhone、iPad を含むデバイス別のユーザーの数を表示します。</span><span class="sxs-lookup"><span data-stu-id="5b06d-106">The report will show you the number of users per device including Windows, Windows phone, Android phone, iPhone, and iPad.</span></span>

> <span data-ttu-id="5b06d-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: 使用している Skype for Business クライアント](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5b06d-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="5b06d-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5b06d-108">Permissions</span></span>

<span data-ttu-id="5b06d-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5b06d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5b06d-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5b06d-111">Permission type</span></span>                        | <span data-ttu-id="5b06d-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5b06d-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="5b06d-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="5b06d-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="5b06d-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b06d-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="5b06d-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5b06d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b06d-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5b06d-116">Not supported.</span></span>                           |
| <span data-ttu-id="5b06d-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5b06d-117">Application</span></span>                            | <span data-ttu-id="5b06d-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b06d-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="5b06d-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5b06d-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="5b06d-120">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="5b06d-120">Function parameters</span></span>

<span data-ttu-id="5b06d-121">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="5b06d-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="5b06d-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="5b06d-122">Parameter</span></span> | <span data-ttu-id="5b06d-123">型</span><span class="sxs-lookup"><span data-stu-id="5b06d-123">Type</span></span>   | <span data-ttu-id="5b06d-124">説明</span><span class="sxs-lookup"><span data-stu-id="5b06d-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="5b06d-125">period</span><span class="sxs-lookup"><span data-stu-id="5b06d-125">period</span></span>    | <span data-ttu-id="5b06d-126">文字列</span><span class="sxs-lookup"><span data-stu-id="5b06d-126">string</span></span> | <span data-ttu-id="5b06d-127">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="5b06d-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="5b06d-128">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="5b06d-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="5b06d-129">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="5b06d-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="5b06d-130">必須。</span><span class="sxs-lookup"><span data-stu-id="5b06d-130">Required.</span></span> |

<span data-ttu-id="5b06d-131">このメソッドは、 `$format`応答をカスタマイズするための[OData クエリパラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="5b06d-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="5b06d-132">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="5b06d-132">The default output type is text/csv.</span></span> <span data-ttu-id="5b06d-133">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="5b06d-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5b06d-134">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5b06d-134">Request headers</span></span>

| <span data-ttu-id="5b06d-135">名前</span><span class="sxs-lookup"><span data-stu-id="5b06d-135">Name</span></span>          | <span data-ttu-id="5b06d-136">説明</span><span class="sxs-lookup"><span data-stu-id="5b06d-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="5b06d-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b06d-137">Authorization</span></span> | <span data-ttu-id="5b06d-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5b06d-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="5b06d-140">応答</span><span class="sxs-lookup"><span data-stu-id="5b06d-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="5b06d-141">CSV</span><span class="sxs-lookup"><span data-stu-id="5b06d-141">CSV</span></span>

<span data-ttu-id="5b06d-142">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="5b06d-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="5b06d-143">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="5b06d-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="5b06d-144">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="5b06d-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="5b06d-145">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="5b06d-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="5b06d-146">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="5b06d-146">Report Refresh Date</span></span>
- <span data-ttu-id="5b06d-147">Windows</span><span class="sxs-lookup"><span data-stu-id="5b06d-147">Windows</span></span>
- <span data-ttu-id="5b06d-148">Windows スマートフォン</span><span class="sxs-lookup"><span data-stu-id="5b06d-148">Windows Phone</span></span>
- <span data-ttu-id="5b06d-149">Android スマートフォン</span><span class="sxs-lookup"><span data-stu-id="5b06d-149">Android Phone</span></span>
- <span data-ttu-id="5b06d-150">iPhone</span><span class="sxs-lookup"><span data-stu-id="5b06d-150">iPhone</span></span>
- <span data-ttu-id="5b06d-151">iPad</span><span class="sxs-lookup"><span data-stu-id="5b06d-151">iPad</span></span>
- <span data-ttu-id="5b06d-152">レポート期間</span><span class="sxs-lookup"><span data-stu-id="5b06d-152">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="5b06d-153">JSON</span><span class="sxs-lookup"><span data-stu-id="5b06d-153">JSON</span></span>

<span data-ttu-id="5b06d-154">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[skypeForBusinessDeviceUsageDistributionUserCounts](../resources/skypeforbusinessdeviceusagedistributionusercounts.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5b06d-154">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessDeviceUsageDistributionUserCounts](../resources/skypeforbusinessdeviceusagedistributionusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b06d-155">例</span><span class="sxs-lookup"><span data-stu-id="5b06d-155">Example</span></span>

### <a name="csv"></a><span data-ttu-id="5b06d-156">CSV</span><span class="sxs-lookup"><span data-stu-id="5b06d-156">CSV</span></span>

<span data-ttu-id="5b06d-157">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5b06d-157">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="5b06d-158">要求</span><span class="sxs-lookup"><span data-stu-id="5b06d-158">Request</span></span>

<span data-ttu-id="5b06d-159">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5b06d-159">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusagedistributionusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="5b06d-160">応答</span><span class="sxs-lookup"><span data-stu-id="5b06d-160">Response</span></span>

<span data-ttu-id="5b06d-161">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5b06d-161">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="5b06d-162">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="5b06d-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Windows,Windows Phone,Android Phone,iPhone,iPad,Report Period
```

### <a name="json"></a><span data-ttu-id="5b06d-163">JSON</span><span class="sxs-lookup"><span data-stu-id="5b06d-163">JSON</span></span>

<span data-ttu-id="5b06d-164">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="5b06d-164">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="5b06d-165">要求</span><span class="sxs-lookup"><span data-stu-id="5b06d-165">Request</span></span>

<span data-ttu-id="5b06d-166">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5b06d-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusagedistributionusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="5b06d-167">応答</span><span class="sxs-lookup"><span data-stu-id="5b06d-167">Response</span></span>

<span data-ttu-id="5b06d-168">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5b06d-168">The following is an example of the response.</span></span>

> <span data-ttu-id="5b06d-p108">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="5b06d-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageDistributionUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 275

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessDeviceUsageDistributionUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "windows": 122, 
      "windowsPhone": 8, 
      "androidPhone": 19, 
      "iPhone": 28, 
      "iPad": 1, 
      "reportPeriod": "7"
    }
  ]
}
```
