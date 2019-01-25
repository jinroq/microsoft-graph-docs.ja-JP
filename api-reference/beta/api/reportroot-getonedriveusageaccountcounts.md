---
title: 'reportRoot: getOneDriveUsageAccountCounts'
description: アクティブな OneDrive for Business サイトの数の傾向を取得します。 ユーザーがファイルを表示、変更、アップロード、ダウンロード、共有、同期したサイトはすべて、アクティブなサイトとみなされます。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: f6fae6f8ab5e94c0ee89a0ee3b88a216d1f0c6c7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529601"
---
# <a name="reportroot-getonedriveusageaccountcounts"></a><span data-ttu-id="81244-104">reportRoot: getOneDriveUsageAccountCounts</span><span class="sxs-lookup"><span data-stu-id="81244-104">reportRoot: getOneDriveUsageAccountCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81244-105">アクティブな OneDrive for Business サイトの数の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="81244-105">Get the trend in the number of active OneDrive for Business sites.</span></span> <span data-ttu-id="81244-106">ユーザーがファイルを表示、変更、アップロード、ダウンロード、共有、同期したサイトはすべて、アクティブなサイトとみなされます。</span><span class="sxs-lookup"><span data-stu-id="81244-106">Any site on which users viewed, modified, uploaded, downloaded, shared, or synced files is considered an active site.</span></span>

> <span data-ttu-id="81244-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: OneDrive for Business の使用状況](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="81244-107">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="81244-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="81244-108">Permissions</span></span>

<span data-ttu-id="81244-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="81244-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="81244-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="81244-111">Permission type</span></span>                        | <span data-ttu-id="81244-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="81244-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="81244-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="81244-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="81244-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="81244-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="81244-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="81244-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81244-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="81244-116">Not supported.</span></span>                           |
| <span data-ttu-id="81244-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="81244-117">Application</span></span>                            | <span data-ttu-id="81244-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="81244-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="81244-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="81244-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageAccountCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="81244-120">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="81244-120">Function parameters</span></span>

<span data-ttu-id="81244-121">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="81244-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="81244-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="81244-122">Parameter</span></span> | <span data-ttu-id="81244-123">型</span><span class="sxs-lookup"><span data-stu-id="81244-123">Type</span></span>   | <span data-ttu-id="81244-124">説明</span><span class="sxs-lookup"><span data-stu-id="81244-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="81244-125">period</span><span class="sxs-lookup"><span data-stu-id="81244-125">period</span></span>    | <span data-ttu-id="81244-126">文字列</span><span class="sxs-lookup"><span data-stu-id="81244-126">string</span></span> | <span data-ttu-id="81244-127">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="81244-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="81244-128">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="81244-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="81244-129">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="81244-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="81244-130">必須。</span><span class="sxs-lookup"><span data-stu-id="81244-130">Required.</span></span> |

<span data-ttu-id="81244-131">このメソッドをサポートしている、 `$format` 、応答をカスタマイズするのには、 [OData クエリ パラメーター](/graph/query-parameters)です。</span><span class="sxs-lookup"><span data-stu-id="81244-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="81244-132">既定の出力の種類は、テキストまたは csv です。</span><span class="sxs-lookup"><span data-stu-id="81244-132">The default output type is text/csv.</span></span> <span data-ttu-id="81244-133">ただし、出力の種類を指定する場合は、設定をテキストまたは csv またはアプリケーションまたは json OData $format クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="81244-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="81244-134">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="81244-134">Request headers</span></span>

| <span data-ttu-id="81244-135">名前</span><span class="sxs-lookup"><span data-stu-id="81244-135">Name</span></span>          | <span data-ttu-id="81244-136">説明</span><span class="sxs-lookup"><span data-stu-id="81244-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="81244-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="81244-137">Authorization</span></span> | <span data-ttu-id="81244-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="81244-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="81244-140">応答</span><span class="sxs-lookup"><span data-stu-id="81244-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="81244-141">CSV</span><span class="sxs-lookup"><span data-stu-id="81244-141">CSV</span></span>

<span data-ttu-id="81244-142">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="81244-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="81244-143">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="81244-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="81244-144">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="81244-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="81244-145">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="81244-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="81244-146">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="81244-146">Report Refresh Date</span></span>
- <span data-ttu-id="81244-147">サイトの種類</span><span class="sxs-lookup"><span data-stu-id="81244-147">Site Type</span></span>
- <span data-ttu-id="81244-148">合計</span><span class="sxs-lookup"><span data-stu-id="81244-148">Total</span></span>
- <span data-ttu-id="81244-149">アクティブ</span><span class="sxs-lookup"><span data-stu-id="81244-149">Active</span></span>
- <span data-ttu-id="81244-150">レポート日付</span><span class="sxs-lookup"><span data-stu-id="81244-150">Report Date</span></span>
- <span data-ttu-id="81244-151">レポート期間</span><span class="sxs-lookup"><span data-stu-id="81244-151">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="81244-152">JSON</span><span class="sxs-lookup"><span data-stu-id="81244-152">JSON</span></span>

<span data-ttu-id="81244-153">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に**[oneDriveUsageAccountCounts](../resources/onedriveusageaccountcounts.md)** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="81244-153">If successful, this method returns a `200 OK` response code and a **[oneDriveUsageAccountCounts](../resources/onedriveusageaccountcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81244-154">例</span><span class="sxs-lookup"><span data-stu-id="81244-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="81244-155">CSV</span><span class="sxs-lookup"><span data-stu-id="81244-155">CSV</span></span>

<span data-ttu-id="81244-156">次に、CSV を出力する例を示します。</span><span class="sxs-lookup"><span data-stu-id="81244-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="81244-157">要求</span><span class="sxs-lookup"><span data-stu-id="81244-157">Request</span></span>

<span data-ttu-id="81244-158">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="81244-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountcounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="81244-159">応答</span><span class="sxs-lookup"><span data-stu-id="81244-159">Response</span></span>

<span data-ttu-id="81244-160">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="81244-160">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="81244-161">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="81244-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="81244-162">JSON</span><span class="sxs-lookup"><span data-stu-id="81244-162">JSON</span></span>

<span data-ttu-id="81244-163">次に、JSON を取得する例を示します。</span><span class="sxs-lookup"><span data-stu-id="81244-163">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="81244-164">要求</span><span class="sxs-lookup"><span data-stu-id="81244-164">Request</span></span>

<span data-ttu-id="81244-165">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="81244-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountcounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="81244-166">応答</span><span class="sxs-lookup"><span data-stu-id="81244-166">Response</span></span>

<span data-ttu-id="81244-167">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="81244-167">The following is an example of the response.</span></span>

> <span data-ttu-id="81244-p108">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="81244-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oneDriveUsageAccountCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 249

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.oneDriveUsageAccountCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteType": "All", 
      "total": 207, 
      "active": 89, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getonedriveusageaccountcounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
