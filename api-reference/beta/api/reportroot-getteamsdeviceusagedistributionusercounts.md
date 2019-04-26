---
title: 'reportRoot: getTeamsDeviceUsageDistributionUserCounts'
description: デバイスの種類ごとに、選択した期間の Microsoft Teams のユニーク ユーザーの数を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 397592a7333a9aee9435a3e2e073645d6e5cacd0
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33336454"
---
# <a name="reportroot-getteamsdeviceusagedistributionusercounts"></a><span data-ttu-id="bbc46-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="bbc46-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bbc46-104">デバイスの種類ごとに、選択した期間の Microsoft Teams のユニーク ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="bbc46-104">Get the number of Microsoft Teams unique users by device type over the selected time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="bbc46-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bbc46-105">Permissions</span></span>

<span data-ttu-id="bbc46-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bbc46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bbc46-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bbc46-108">Permission type</span></span>                        | <span data-ttu-id="bbc46-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bbc46-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="bbc46-110">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="bbc46-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="bbc46-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bbc46-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="bbc46-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bbc46-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bbc46-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bbc46-113">Not supported.</span></span>                           |
| <span data-ttu-id="bbc46-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bbc46-114">Application</span></span>                            | <span data-ttu-id="bbc46-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bbc46-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="bbc46-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bbc46-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="bbc46-117">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="bbc46-117">Function parameters</span></span>

<span data-ttu-id="bbc46-118">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="bbc46-118">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="bbc46-119">パラメーター</span><span class="sxs-lookup"><span data-stu-id="bbc46-119">Parameter</span></span> | <span data-ttu-id="bbc46-120">型</span><span class="sxs-lookup"><span data-stu-id="bbc46-120">Type</span></span>   | <span data-ttu-id="bbc46-121">説明</span><span class="sxs-lookup"><span data-stu-id="bbc46-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="bbc46-122">period</span><span class="sxs-lookup"><span data-stu-id="bbc46-122">period</span></span>    | <span data-ttu-id="bbc46-123">文字列</span><span class="sxs-lookup"><span data-stu-id="bbc46-123">string</span></span> | <span data-ttu-id="bbc46-124">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="bbc46-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="bbc46-125">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="bbc46-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="bbc46-126">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="bbc46-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="bbc46-127">必須。</span><span class="sxs-lookup"><span data-stu-id="bbc46-127">Required.</span></span> |

<span data-ttu-id="bbc46-128">このメソッドは、 `$format`応答をカスタマイズするための[OData クエリパラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="bbc46-128">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="bbc46-129">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="bbc46-129">The default output type is text/csv.</span></span> <span data-ttu-id="bbc46-130">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="bbc46-130">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bbc46-131">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bbc46-131">Request headers</span></span>

| <span data-ttu-id="bbc46-132">名前</span><span class="sxs-lookup"><span data-stu-id="bbc46-132">Name</span></span>          | <span data-ttu-id="bbc46-133">説明</span><span class="sxs-lookup"><span data-stu-id="bbc46-133">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="bbc46-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="bbc46-134">Authorization</span></span> | <span data-ttu-id="bbc46-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="bbc46-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="bbc46-137">応答</span><span class="sxs-lookup"><span data-stu-id="bbc46-137">Response</span></span>

### <a name="csv"></a><span data-ttu-id="bbc46-138">CSV</span><span class="sxs-lookup"><span data-stu-id="bbc46-138">CSV</span></span>

<span data-ttu-id="bbc46-139">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="bbc46-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="bbc46-140">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="bbc46-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="bbc46-141">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="bbc46-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="bbc46-142">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="bbc46-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="bbc46-143">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="bbc46-143">Report Refresh Date</span></span>
- <span data-ttu-id="bbc46-144">Web</span><span class="sxs-lookup"><span data-stu-id="bbc46-144">Web</span></span>
- <span data-ttu-id="bbc46-145">Windows スマートフォン</span><span class="sxs-lookup"><span data-stu-id="bbc46-145">Windows Phone</span></span>
- <span data-ttu-id="bbc46-146">Android スマートフォン</span><span class="sxs-lookup"><span data-stu-id="bbc46-146">Android Phone</span></span>
- <span data-ttu-id="bbc46-147">iOS</span><span class="sxs-lookup"><span data-stu-id="bbc46-147">iOS</span></span>
- <span data-ttu-id="bbc46-148">Mac</span><span class="sxs-lookup"><span data-stu-id="bbc46-148">Mac</span></span>
- <span data-ttu-id="bbc46-149">Windows</span><span class="sxs-lookup"><span data-stu-id="bbc46-149">Windows</span></span>
- <span data-ttu-id="bbc46-150">レポート期間</span><span class="sxs-lookup"><span data-stu-id="bbc46-150">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="bbc46-151">JSON</span><span class="sxs-lookup"><span data-stu-id="bbc46-151">JSON</span></span>

<span data-ttu-id="bbc46-152">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="bbc46-152">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bbc46-153">例</span><span class="sxs-lookup"><span data-stu-id="bbc46-153">Example</span></span>

### <a name="csv"></a><span data-ttu-id="bbc46-154">CSV</span><span class="sxs-lookup"><span data-stu-id="bbc46-154">CSV</span></span>

<span data-ttu-id="bbc46-155">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="bbc46-155">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="bbc46-156">要求</span><span class="sxs-lookup"><span data-stu-id="bbc46-156">Request</span></span>

<span data-ttu-id="bbc46-157">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="bbc46-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="bbc46-158">応答</span><span class="sxs-lookup"><span data-stu-id="bbc46-158">Response</span></span>

<span data-ttu-id="bbc46-159">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="bbc46-159">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="bbc46-160">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="bbc46-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iOS,Mac,Windows,Report Period
```

### <a name="json"></a><span data-ttu-id="bbc46-161">JSON</span><span class="sxs-lookup"><span data-stu-id="bbc46-161">JSON</span></span>

<span data-ttu-id="bbc46-162">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="bbc46-162">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="bbc46-163">要求</span><span class="sxs-lookup"><span data-stu-id="bbc46-163">Request</span></span>

<span data-ttu-id="bbc46-164">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="bbc46-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="bbc46-165">応答</span><span class="sxs-lookup"><span data-stu-id="bbc46-165">Response</span></span>

<span data-ttu-id="bbc46-166">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="bbc46-166">The following is an example of the response.</span></span>

> <span data-ttu-id="bbc46-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="bbc46-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsDeviceUsageDistributionUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 243

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsDeviceUsageDistributionUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "web": 51, 
      "windowsPhone": 2, 
      "androidPhone": 34, 
      "ios": 76, 
      "mac": 40, 
      "windows": 491, 
      "reportPeriod": "7"
    }
  ]
}
```
