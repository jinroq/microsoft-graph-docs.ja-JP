---
title: 'reportRoot: getSharePointSiteUsageSiteCounts'
description: すべてのサイトのファイルの合計数と、アクティブ ファイルの数を取得します。 ファイル (ユーザーまたはシステム) は、一定期間中に保存、同期、変更、共有されるとアクティブとみなされます。
ms.openlocfilehash: 1689b43b4f3e90ca88d61e6b8bd4332d29ad1e5f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066486"
---
# <a name="reportroot-getsharepointsiteusagesitecounts"></a><span data-ttu-id="baed5-104">reportRoot: getSharePointSiteUsageSiteCounts</span><span class="sxs-lookup"><span data-stu-id="baed5-104">reportRoot: getSharePointSiteUsageSiteCounts</span></span>

> <span data-ttu-id="baed5-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="baed5-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="baed5-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="baed5-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="baed5-107">すべてのサイトのファイルの合計数と、アクティブ ファイルの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="baed5-107">Get the total number of files across all sites and the number of active files.</span></span> <span data-ttu-id="baed5-108">ファイル (ユーザーまたはシステム) は、一定期間中に保存、同期、変更、共有されるとアクティブとみなされます。</span><span class="sxs-lookup"><span data-stu-id="baed5-108">A file (user or system) is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span>

> <span data-ttu-id="baed5-109">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: SharePoint サイトの使用状況](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="baed5-109">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="baed5-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="baed5-110">Permissions</span></span>

<span data-ttu-id="baed5-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="baed5-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="baed5-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="baed5-113">Permission type</span></span>                        | <span data-ttu-id="baed5-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="baed5-114">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="baed5-115">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="baed5-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="baed5-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="baed5-116">Reports.Read.All</span></span>                         |
| <span data-ttu-id="baed5-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="baed5-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="baed5-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="baed5-118">Not supported.</span></span>                           |
| <span data-ttu-id="baed5-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="baed5-119">Application</span></span>                            | <span data-ttu-id="baed5-120">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="baed5-120">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="baed5-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="baed5-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageSiteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="baed5-122">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="baed5-122">Function parameters</span></span>

<span data-ttu-id="baed5-123">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="baed5-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="baed5-124">パラメーター</span><span class="sxs-lookup"><span data-stu-id="baed5-124">Parameter</span></span> | <span data-ttu-id="baed5-125">型</span><span class="sxs-lookup"><span data-stu-id="baed5-125">Type</span></span>   | <span data-ttu-id="baed5-126">説明</span><span class="sxs-lookup"><span data-stu-id="baed5-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="baed5-127">period</span><span class="sxs-lookup"><span data-stu-id="baed5-127">period</span></span>    | <span data-ttu-id="baed5-128">文字列</span><span class="sxs-lookup"><span data-stu-id="baed5-128">string</span></span> | <span data-ttu-id="baed5-129">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="baed5-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="baed5-130">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="baed5-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="baed5-131">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="baed5-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="baed5-132">必須。</span><span class="sxs-lookup"><span data-stu-id="baed5-132">Required.</span></span> |

<span data-ttu-id="baed5-133">このメソッドをサポートしている、 `$format` 、応答をカスタマイズするのには、 [OData クエリ パラメーター](/graph/query-parameters)です。</span><span class="sxs-lookup"><span data-stu-id="baed5-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="baed5-134">既定の出力の種類は、テキストまたは csv です。</span><span class="sxs-lookup"><span data-stu-id="baed5-134">The default output type is text/csv.</span></span> <span data-ttu-id="baed5-135">ただし、出力の種類を指定する場合は、設定をテキストまたは csv またはアプリケーションまたは json OData $format クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="baed5-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="baed5-136">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="baed5-136">Request headers</span></span>

| <span data-ttu-id="baed5-137">名前</span><span class="sxs-lookup"><span data-stu-id="baed5-137">Name</span></span>          | <span data-ttu-id="baed5-138">説明</span><span class="sxs-lookup"><span data-stu-id="baed5-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="baed5-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="baed5-139">Authorization</span></span> | <span data-ttu-id="baed5-p107">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="baed5-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="baed5-142">応答</span><span class="sxs-lookup"><span data-stu-id="baed5-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="baed5-143">CSV</span><span class="sxs-lookup"><span data-stu-id="baed5-143">CSV</span></span>

<span data-ttu-id="baed5-144">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="baed5-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="baed5-145">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="baed5-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="baed5-146">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="baed5-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="baed5-147">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="baed5-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="baed5-148">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="baed5-148">Report Refresh Date</span></span>
- <span data-ttu-id="baed5-149">サイトの種類</span><span class="sxs-lookup"><span data-stu-id="baed5-149">Site Type</span></span>
- <span data-ttu-id="baed5-150">合計</span><span class="sxs-lookup"><span data-stu-id="baed5-150">Total</span></span>
- <span data-ttu-id="baed5-151">アクティブ</span><span class="sxs-lookup"><span data-stu-id="baed5-151">Active</span></span>
- <span data-ttu-id="baed5-152">レポート日付</span><span class="sxs-lookup"><span data-stu-id="baed5-152">Report Date</span></span>
- <span data-ttu-id="baed5-153">レポート期間</span><span class="sxs-lookup"><span data-stu-id="baed5-153">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="baed5-154">JSON</span><span class="sxs-lookup"><span data-stu-id="baed5-154">JSON</span></span>

<span data-ttu-id="baed5-155">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に**[sharePointSiteUsageSiteCounts](../resources/sharepointsiteusagesitecounts.md)** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="baed5-155">If successful, this method returns a `200 OK` response code and a **[sharePointSiteUsageSiteCounts](../resources/sharepointsiteusagesitecounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="baed5-156">使用例</span><span class="sxs-lookup"><span data-stu-id="baed5-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="baed5-157">CSV</span><span class="sxs-lookup"><span data-stu-id="baed5-157">CSV</span></span>

<span data-ttu-id="baed5-158">次に、CSV を出力する例を示します。</span><span class="sxs-lookup"><span data-stu-id="baed5-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="baed5-159">要求</span><span class="sxs-lookup"><span data-stu-id="baed5-159">Request</span></span>

<span data-ttu-id="baed5-160">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="baed5-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagesitecounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageSiteCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="baed5-161">応答</span><span class="sxs-lookup"><span data-stu-id="baed5-161">Response</span></span>

<span data-ttu-id="baed5-162">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="baed5-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="baed5-163">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="baed5-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Total,Active,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="baed5-164">JSON</span><span class="sxs-lookup"><span data-stu-id="baed5-164">JSON</span></span>

<span data-ttu-id="baed5-165">次に、JSON を取得する例を示します。</span><span class="sxs-lookup"><span data-stu-id="baed5-165">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="baed5-166">要求</span><span class="sxs-lookup"><span data-stu-id="baed5-166">Request</span></span>

<span data-ttu-id="baed5-167">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="baed5-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagesitecounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageSiteCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="baed5-168">応答</span><span class="sxs-lookup"><span data-stu-id="baed5-168">Response</span></span>

<span data-ttu-id="baed5-169">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="baed5-169">The following is an example of the response.</span></span>

> <span data-ttu-id="baed5-p109">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="baed5-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointSiteUsageSiteCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 251

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.sharePointSiteUsageSiteCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteType": "All", 
      "total": 47, 
      "active": 15, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```