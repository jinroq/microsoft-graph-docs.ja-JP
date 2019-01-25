---
title: 'reportRoot: getOneDriveUsageAccountDetail'
description: アカウント別の OneDrive の使用状況に関する詳細を取得します。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 51fe0d89b8ad4e8bb783c901fba101135a296834
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525753"
---
# <a name="reportroot-getonedriveusageaccountdetail"></a><span data-ttu-id="642eb-103">reportRoot: getOneDriveUsageAccountDetail</span><span class="sxs-lookup"><span data-stu-id="642eb-103">reportRoot: getOneDriveUsageAccountDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="642eb-104">アカウント別の OneDrive の使用状況に関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="642eb-104">Get details about OneDrive usage by account.</span></span>

> <span data-ttu-id="642eb-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: OneDrive for Business の使用状況](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="642eb-105">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="642eb-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="642eb-106">Permissions</span></span>

<span data-ttu-id="642eb-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="642eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="642eb-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="642eb-109">Permission type</span></span>                        | <span data-ttu-id="642eb-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="642eb-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="642eb-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="642eb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="642eb-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="642eb-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="642eb-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="642eb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="642eb-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="642eb-114">Not supported.</span></span>                           |
| <span data-ttu-id="642eb-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="642eb-115">Application</span></span>                            | <span data-ttu-id="642eb-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="642eb-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="642eb-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="642eb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageAccountDetail(period='{period_value}')
GET /reports/getOneDriveUsageAccountDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="642eb-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="642eb-118">Function parameters</span></span>

<span data-ttu-id="642eb-119">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="642eb-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="642eb-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="642eb-120">Parameter</span></span> | <span data-ttu-id="642eb-121">型</span><span class="sxs-lookup"><span data-stu-id="642eb-121">Type</span></span>   | <span data-ttu-id="642eb-122">説明</span><span class="sxs-lookup"><span data-stu-id="642eb-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="642eb-123">period</span><span class="sxs-lookup"><span data-stu-id="642eb-123">period</span></span>    | <span data-ttu-id="642eb-124">文字列</span><span class="sxs-lookup"><span data-stu-id="642eb-124">string</span></span> | <span data-ttu-id="642eb-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="642eb-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="642eb-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="642eb-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="642eb-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="642eb-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="642eb-128">date</span><span class="sxs-lookup"><span data-stu-id="642eb-128">date</span></span>      | <span data-ttu-id="642eb-129">日付</span><span class="sxs-lookup"><span data-stu-id="642eb-129">Date</span></span>   | <span data-ttu-id="642eb-130">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="642eb-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="642eb-131">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="642eb-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="642eb-132">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="642eb-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="642eb-133">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="642eb-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="642eb-134">このメソッドは、応答をカスタマイズするための `$format`、`$top`、`$skipToken` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="642eb-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="642eb-135">既定の出力の種類は、テキストまたは csv です。</span><span class="sxs-lookup"><span data-stu-id="642eb-135">The default output type is text/csv.</span></span> <span data-ttu-id="642eb-136">ただし、出力の種類を指定する場合は、設定をテキストまたは csv またはアプリケーションまたは json OData $format クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="642eb-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="642eb-137">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="642eb-137">Request headers</span></span>

| <span data-ttu-id="642eb-138">名前</span><span class="sxs-lookup"><span data-stu-id="642eb-138">Name</span></span>          | <span data-ttu-id="642eb-139">説明</span><span class="sxs-lookup"><span data-stu-id="642eb-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="642eb-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="642eb-140">Authorization</span></span> | <span data-ttu-id="642eb-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="642eb-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="642eb-143">応答</span><span class="sxs-lookup"><span data-stu-id="642eb-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="642eb-144">CSV</span><span class="sxs-lookup"><span data-stu-id="642eb-144">CSV</span></span>

<span data-ttu-id="642eb-145">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="642eb-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="642eb-146">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="642eb-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="642eb-147">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="642eb-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="642eb-148">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="642eb-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="642eb-149">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="642eb-149">Report Refresh Date</span></span>
- <span data-ttu-id="642eb-150">サイトの URL</span><span class="sxs-lookup"><span data-stu-id="642eb-150">Site URL</span></span>
- <span data-ttu-id="642eb-151">所有者の表示名</span><span class="sxs-lookup"><span data-stu-id="642eb-151">Owner Display Name</span></span>
- <span data-ttu-id="642eb-152">削除済み</span><span class="sxs-lookup"><span data-stu-id="642eb-152">Is Deleted</span></span>
- <span data-ttu-id="642eb-153">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="642eb-153">Last Activity Date</span></span>
- <span data-ttu-id="642eb-154">ファイル数</span><span class="sxs-lookup"><span data-stu-id="642eb-154">File Count</span></span>
- <span data-ttu-id="642eb-155">アクティブなファイル数</span><span class="sxs-lookup"><span data-stu-id="642eb-155">Active File Count</span></span>
- <span data-ttu-id="642eb-156">使用済みストレージ (バイト)</span><span class="sxs-lookup"><span data-stu-id="642eb-156">Storage Used (Byte)</span></span>
- <span data-ttu-id="642eb-157">割り当て済みストレージ (バイト)</span><span class="sxs-lookup"><span data-stu-id="642eb-157">Storage Allocated (Byte)</span></span>
- <span data-ttu-id="642eb-158">レポート期間</span><span class="sxs-lookup"><span data-stu-id="642eb-158">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="642eb-159">JSON</span><span class="sxs-lookup"><span data-stu-id="642eb-159">JSON</span></span>

<span data-ttu-id="642eb-160">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に**[oneDriveUsageAccountDetail](../resources/onedriveusageaccountdetail.md)** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="642eb-160">If successful, this method returns a `200 OK` response code and a **[oneDriveUsageAccountDetail](../resources/onedriveusageaccountdetail.md)** object in the response body.</span></span>

<span data-ttu-id="642eb-161">この要求の既定のページ サイズは、アイテムは 200 個です。</span><span class="sxs-lookup"><span data-stu-id="642eb-161">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="642eb-162">例</span><span class="sxs-lookup"><span data-stu-id="642eb-162">Example</span></span>

<span data-ttu-id="642eb-163">次に、CSV を出力する例を示します。</span><span class="sxs-lookup"><span data-stu-id="642eb-163">The following is an example that outputs CSV.</span></span>

### <a name="csv"></a><span data-ttu-id="642eb-164">CSV</span><span class="sxs-lookup"><span data-stu-id="642eb-164">CSV</span></span>

#### <a name="request"></a><span data-ttu-id="642eb-165">要求</span><span class="sxs-lookup"><span data-stu-id="642eb-165">Request</span></span>

<span data-ttu-id="642eb-166">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="642eb-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="642eb-167">応答</span><span class="sxs-lookup"><span data-stu-id="642eb-167">Response</span></span>

<span data-ttu-id="642eb-168">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="642eb-168">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="642eb-169">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="642eb-169">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site URL,Owner Display Name,Is Deleted,Last Activity Date,File Count,Active File Count,Storage Used (Byte),Storage Allocated (Byte),Report Period
```

### <a name="json"></a><span data-ttu-id="642eb-170">JSON</span><span class="sxs-lookup"><span data-stu-id="642eb-170">JSON</span></span>

<span data-ttu-id="642eb-171">次に、JSON を取得する例を示します。</span><span class="sxs-lookup"><span data-stu-id="642eb-171">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="642eb-172">要求</span><span class="sxs-lookup"><span data-stu-id="642eb-172">Request</span></span>

<span data-ttu-id="642eb-173">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="642eb-173">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="642eb-174">応答</span><span class="sxs-lookup"><span data-stu-id="642eb-174">Response</span></span>

<span data-ttu-id="642eb-175">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="642eb-175">The following is an example of the response.</span></span>

> <span data-ttu-id="642eb-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="642eb-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oneDriveUsageAccountDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 400

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.oneDriveUsageAccountDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteUrl": "siteUrl-value", 
      "ownerDisplayName": "ownerDisplayName-value", 
      "isDeleted": false, 
      "lastActivityDate": "2017-09-01", 
      "fileCount": 9, 
      "activeFileCount": 5, 
      "storageUsedInBytes": 12190375, 
      "storageAllocatedInBytes": 549755813880, 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getonedriveusageaccountdetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
