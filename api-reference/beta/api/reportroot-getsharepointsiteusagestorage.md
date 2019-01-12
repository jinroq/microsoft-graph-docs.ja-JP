---
title: 'reportRoot: getSharePointSiteUsageStorage'
description: レポート期間中に割り当てられ、消費したストレージの傾向を取得します。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: d66400c9b94f72d9ecc3b5d50d4ca92f1f8cb364
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946036"
---
# <a name="reportroot-getsharepointsiteusagestorage"></a><span data-ttu-id="eac40-103">reportRoot: getSharePointSiteUsageStorage</span><span class="sxs-lookup"><span data-stu-id="eac40-103">reportRoot: getSharePointSiteUsageStorage</span></span>

> <span data-ttu-id="eac40-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="eac40-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eac40-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eac40-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="eac40-106">レポート期間中に割り当てられ、消費したストレージの傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="eac40-106">Get the trend of storage allocated and consumed during the reporting period.</span></span>

> <span data-ttu-id="eac40-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: SharePoint サイトの使用状況](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eac40-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="eac40-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="eac40-108">Permissions</span></span>

<span data-ttu-id="eac40-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eac40-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="eac40-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="eac40-111">Permission type</span></span>                        | <span data-ttu-id="eac40-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="eac40-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="eac40-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="eac40-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="eac40-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="eac40-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="eac40-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="eac40-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eac40-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eac40-116">Not supported.</span></span>                           |
| <span data-ttu-id="eac40-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="eac40-117">Application</span></span>                            | <span data-ttu-id="eac40-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="eac40-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="eac40-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="eac40-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageStorage(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="eac40-120">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="eac40-120">Function parameters</span></span>

<span data-ttu-id="eac40-121">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="eac40-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="eac40-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="eac40-122">Parameter</span></span> | <span data-ttu-id="eac40-123">Type</span><span class="sxs-lookup"><span data-stu-id="eac40-123">Type</span></span>   | <span data-ttu-id="eac40-124">説明</span><span class="sxs-lookup"><span data-stu-id="eac40-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="eac40-125">period</span><span class="sxs-lookup"><span data-stu-id="eac40-125">period</span></span>    | <span data-ttu-id="eac40-126">文字列</span><span class="sxs-lookup"><span data-stu-id="eac40-126">string</span></span> | <span data-ttu-id="eac40-127">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="eac40-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="eac40-128">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="eac40-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="eac40-129">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="eac40-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="eac40-130">必須。</span><span class="sxs-lookup"><span data-stu-id="eac40-130">Required.</span></span> |

<span data-ttu-id="eac40-131">このメソッドをサポートしている、 `$format` 、応答をカスタマイズするのには、 [OData クエリ パラメーター](/graph/query-parameters)です。</span><span class="sxs-lookup"><span data-stu-id="eac40-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="eac40-132">既定の出力の種類は、テキストまたは csv です。</span><span class="sxs-lookup"><span data-stu-id="eac40-132">The default output type is text/csv.</span></span> <span data-ttu-id="eac40-133">ただし、出力の種類を指定する場合は、設定をテキストまたは csv またはアプリケーションまたは json OData $format クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="eac40-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eac40-134">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="eac40-134">Request headers</span></span>

| <span data-ttu-id="eac40-135">名前</span><span class="sxs-lookup"><span data-stu-id="eac40-135">Name</span></span>          | <span data-ttu-id="eac40-136">説明</span><span class="sxs-lookup"><span data-stu-id="eac40-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="eac40-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="eac40-137">Authorization</span></span> | <span data-ttu-id="eac40-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="eac40-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="eac40-140">応答</span><span class="sxs-lookup"><span data-stu-id="eac40-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="eac40-141">CSV</span><span class="sxs-lookup"><span data-stu-id="eac40-141">CSV</span></span>

<span data-ttu-id="eac40-142">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="eac40-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="eac40-143">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="eac40-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="eac40-144">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="eac40-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="eac40-145">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="eac40-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="eac40-146">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="eac40-146">Report Refresh Date</span></span>
- <span data-ttu-id="eac40-147">サイトの種類</span><span class="sxs-lookup"><span data-stu-id="eac40-147">Site Type</span></span>
- <span data-ttu-id="eac40-148">使用済みストレージ (バイト)</span><span class="sxs-lookup"><span data-stu-id="eac40-148">Storage Used (Byte)</span></span>
- <span data-ttu-id="eac40-149">レポート日付</span><span class="sxs-lookup"><span data-stu-id="eac40-149">Report Date</span></span>
- <span data-ttu-id="eac40-150">レポート期間</span><span class="sxs-lookup"><span data-stu-id="eac40-150">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="eac40-151">JSON</span><span class="sxs-lookup"><span data-stu-id="eac40-151">JSON</span></span>

<span data-ttu-id="eac40-152">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に**[siteUsageStorage](../resources/siteusagestorage.md)** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="eac40-152">If successful, this method returns a `200 OK` response code and a **[siteUsageStorage](../resources/siteusagestorage.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eac40-153">例</span><span class="sxs-lookup"><span data-stu-id="eac40-153">Example</span></span>

### <a name="csv"></a><span data-ttu-id="eac40-154">CSV</span><span class="sxs-lookup"><span data-stu-id="eac40-154">CSV</span></span>

<span data-ttu-id="eac40-155">次に、CSV を出力する例を示します。</span><span class="sxs-lookup"><span data-stu-id="eac40-155">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="eac40-156">要求</span><span class="sxs-lookup"><span data-stu-id="eac40-156">Request</span></span>

<span data-ttu-id="eac40-157">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="eac40-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagestorage_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageStorage(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="eac40-158">応答</span><span class="sxs-lookup"><span data-stu-id="eac40-158">Response</span></span>

<span data-ttu-id="eac40-159">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="eac40-159">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="eac40-160">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="eac40-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Storage Used (Byte),Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="eac40-161">JSON</span><span class="sxs-lookup"><span data-stu-id="eac40-161">JSON</span></span>

<span data-ttu-id="eac40-162">次に、JSON を取得する例を示します。</span><span class="sxs-lookup"><span data-stu-id="eac40-162">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="eac40-163">要求</span><span class="sxs-lookup"><span data-stu-id="eac40-163">Request</span></span>

<span data-ttu-id="eac40-164">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="eac40-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagestorage_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageStorage(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="eac40-165">応答</span><span class="sxs-lookup"><span data-stu-id="eac40-165">Response</span></span>

<span data-ttu-id="eac40-166">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="eac40-166">The following is an example of the response.</span></span>

> <span data-ttu-id="eac40-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="eac40-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.siteUsageStorage"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 248

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.siteUsageStorage)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteType": "All", 
      "storageUsedInBytes": 171835798971, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
