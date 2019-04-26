---
title: 'reportRoot: getTeamsDeviceUsageUserCounts'
description: デバイスの種類ごとに、Microsoft Teams の日次ユニーク ユーザーの数を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 3e196ef562c9a34b511242f31b75241ee1fa7963
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33331787"
---
# <a name="reportroot-getteamsdeviceusageusercounts"></a><span data-ttu-id="d03e8-103">reportRoot: getTeamsDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="d03e8-103">reportRoot: getTeamsDeviceUsageUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d03e8-104">デバイスの種類ごとに、Microsoft Teams の日次ユニーク ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="d03e8-104">Get the number of Microsoft Teams daily unique users by device type.</span></span>

## <a name="permissions"></a><span data-ttu-id="d03e8-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d03e8-105">Permissions</span></span>

<span data-ttu-id="d03e8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d03e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d03e8-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d03e8-108">Permission type</span></span>                        | <span data-ttu-id="d03e8-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d03e8-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="d03e8-110">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="d03e8-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d03e8-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d03e8-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="d03e8-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d03e8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d03e8-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d03e8-113">Not supported.</span></span>                           |
| <span data-ttu-id="d03e8-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d03e8-114">Application</span></span>                            | <span data-ttu-id="d03e8-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d03e8-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="d03e8-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d03e8-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="d03e8-117">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="d03e8-117">Function parameters</span></span>

<span data-ttu-id="d03e8-118">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="d03e8-118">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="d03e8-119">パラメーター</span><span class="sxs-lookup"><span data-stu-id="d03e8-119">Parameter</span></span> | <span data-ttu-id="d03e8-120">型</span><span class="sxs-lookup"><span data-stu-id="d03e8-120">Type</span></span>   | <span data-ttu-id="d03e8-121">説明</span><span class="sxs-lookup"><span data-stu-id="d03e8-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="d03e8-122">period</span><span class="sxs-lookup"><span data-stu-id="d03e8-122">period</span></span>    | <span data-ttu-id="d03e8-123">文字列</span><span class="sxs-lookup"><span data-stu-id="d03e8-123">string</span></span> | <span data-ttu-id="d03e8-124">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="d03e8-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="d03e8-125">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="d03e8-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="d03e8-126">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="d03e8-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="d03e8-127">必須。</span><span class="sxs-lookup"><span data-stu-id="d03e8-127">Required.</span></span> |

<span data-ttu-id="d03e8-128">このメソッドは、 `$format`応答をカスタマイズするための[OData クエリパラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d03e8-128">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="d03e8-129">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="d03e8-129">The default output type is text/csv.</span></span> <span data-ttu-id="d03e8-130">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="d03e8-130">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d03e8-131">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d03e8-131">Request headers</span></span>

| <span data-ttu-id="d03e8-132">名前</span><span class="sxs-lookup"><span data-stu-id="d03e8-132">Name</span></span>          | <span data-ttu-id="d03e8-133">説明</span><span class="sxs-lookup"><span data-stu-id="d03e8-133">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="d03e8-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="d03e8-134">Authorization</span></span> | <span data-ttu-id="d03e8-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d03e8-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="d03e8-137">応答</span><span class="sxs-lookup"><span data-stu-id="d03e8-137">Response</span></span>

### <a name="csv"></a><span data-ttu-id="d03e8-138">CSV</span><span class="sxs-lookup"><span data-stu-id="d03e8-138">CSV</span></span>

<span data-ttu-id="d03e8-139">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="d03e8-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="d03e8-140">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="d03e8-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="d03e8-141">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="d03e8-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="d03e8-142">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="d03e8-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="d03e8-143">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="d03e8-143">Report Refresh Date</span></span>
- <span data-ttu-id="d03e8-144">Web</span><span class="sxs-lookup"><span data-stu-id="d03e8-144">Web</span></span>
- <span data-ttu-id="d03e8-145">Windows スマートフォン</span><span class="sxs-lookup"><span data-stu-id="d03e8-145">Windows Phone</span></span>
- <span data-ttu-id="d03e8-146">Android スマートフォン</span><span class="sxs-lookup"><span data-stu-id="d03e8-146">Android Phone</span></span>
- <span data-ttu-id="d03e8-147">iOS</span><span class="sxs-lookup"><span data-stu-id="d03e8-147">iOS</span></span>
- <span data-ttu-id="d03e8-148">Mac</span><span class="sxs-lookup"><span data-stu-id="d03e8-148">Mac</span></span>
- <span data-ttu-id="d03e8-149">Windows</span><span class="sxs-lookup"><span data-stu-id="d03e8-149">Windows</span></span>
- <span data-ttu-id="d03e8-150">レポート日付</span><span class="sxs-lookup"><span data-stu-id="d03e8-150">Report Date</span></span>
- <span data-ttu-id="d03e8-151">レポート期間</span><span class="sxs-lookup"><span data-stu-id="d03e8-151">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="d03e8-152">JSON</span><span class="sxs-lookup"><span data-stu-id="d03e8-152">JSON</span></span>

<span data-ttu-id="d03e8-153">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[teamsdevice使い方 user計数](../resources/teamsdeviceusageusercounts.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d03e8-153">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageUserCounts](../resources/teamsdeviceusageusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d03e8-154">例</span><span class="sxs-lookup"><span data-stu-id="d03e8-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="d03e8-155">CSV</span><span class="sxs-lookup"><span data-stu-id="d03e8-155">CSV</span></span>

<span data-ttu-id="d03e8-156">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d03e8-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="d03e8-157">要求</span><span class="sxs-lookup"><span data-stu-id="d03e8-157">Request</span></span>

<span data-ttu-id="d03e8-158">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d03e8-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="d03e8-159">応答</span><span class="sxs-lookup"><span data-stu-id="d03e8-159">Response</span></span>

<span data-ttu-id="d03e8-160">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d03e8-160">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="d03e8-161">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="d03e8-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iOS,Mac,Windows,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="d03e8-162">JSON</span><span class="sxs-lookup"><span data-stu-id="d03e8-162">JSON</span></span>

<span data-ttu-id="d03e8-163">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="d03e8-163">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="d03e8-164">要求</span><span class="sxs-lookup"><span data-stu-id="d03e8-164">Request</span></span>

<span data-ttu-id="d03e8-165">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d03e8-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="d03e8-166">応答</span><span class="sxs-lookup"><span data-stu-id="d03e8-166">Response</span></span>

<span data-ttu-id="d03e8-167">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d03e8-167">The following is an example of the response.</span></span>

> <span data-ttu-id="d03e8-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="d03e8-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 269

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsDeviceUsageUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "web": 13, 
      "windowsPhone": 0, 
      "androidPhone": 22, 
      "ios": 75, 
      "mac": 16, 
      "windows": 257, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
