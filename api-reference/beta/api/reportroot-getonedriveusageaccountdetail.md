---
title: 'reportRoot: getOneDriveUsageAccountDetail'
description: アカウント別の OneDrive の使用状況に関する詳細を取得します。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 1aa7de008f1791908786111a87c1ab046df7f42e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960302"
---
# <a name="reportroot-getonedriveusageaccountdetail"></a><span data-ttu-id="61a17-103">reportRoot: getOneDriveUsageAccountDetail</span><span class="sxs-lookup"><span data-stu-id="61a17-103">reportRoot: getOneDriveUsageAccountDetail</span></span>

> <span data-ttu-id="61a17-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="61a17-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="61a17-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="61a17-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="61a17-106">アカウント別の OneDrive の使用状況に関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="61a17-106">Get details about OneDrive usage by account.</span></span>

> <span data-ttu-id="61a17-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: OneDrive for Business の使用状況](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="61a17-107">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="61a17-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="61a17-108">Permissions</span></span>

<span data-ttu-id="61a17-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="61a17-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="61a17-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="61a17-111">Permission type</span></span>                        | <span data-ttu-id="61a17-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="61a17-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="61a17-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="61a17-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="61a17-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="61a17-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="61a17-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="61a17-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="61a17-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="61a17-116">Not supported.</span></span>                           |
| <span data-ttu-id="61a17-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="61a17-117">Application</span></span>                            | <span data-ttu-id="61a17-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="61a17-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="61a17-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="61a17-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageAccountDetail(period='{period_value}')
GET /reports/getOneDriveUsageAccountDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="61a17-120">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="61a17-120">Function parameters</span></span>

<span data-ttu-id="61a17-121">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="61a17-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="61a17-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="61a17-122">Parameter</span></span> | <span data-ttu-id="61a17-123">型</span><span class="sxs-lookup"><span data-stu-id="61a17-123">Type</span></span>   | <span data-ttu-id="61a17-124">説明</span><span class="sxs-lookup"><span data-stu-id="61a17-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="61a17-125">period</span><span class="sxs-lookup"><span data-stu-id="61a17-125">period</span></span>    | <span data-ttu-id="61a17-126">文字列</span><span class="sxs-lookup"><span data-stu-id="61a17-126">string</span></span> | <span data-ttu-id="61a17-127">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="61a17-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="61a17-128">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="61a17-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="61a17-129">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="61a17-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="61a17-130">date</span><span class="sxs-lookup"><span data-stu-id="61a17-130">date</span></span>      | <span data-ttu-id="61a17-131">日付</span><span class="sxs-lookup"><span data-stu-id="61a17-131">Date</span></span>   | <span data-ttu-id="61a17-132">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="61a17-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="61a17-133">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="61a17-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="61a17-134">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="61a17-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="61a17-135">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="61a17-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="61a17-136">このメソッドは、応答をカスタマイズするための `$format`、`$top`、`$skipToken` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="61a17-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="61a17-137">既定の出力の種類は、テキストまたは csv です。</span><span class="sxs-lookup"><span data-stu-id="61a17-137">The default output type is text/csv.</span></span> <span data-ttu-id="61a17-138">ただし、出力の種類を指定する場合は、設定をテキストまたは csv またはアプリケーションまたは json OData $format クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="61a17-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="61a17-139">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="61a17-139">Request headers</span></span>

| <span data-ttu-id="61a17-140">名前</span><span class="sxs-lookup"><span data-stu-id="61a17-140">Name</span></span>          | <span data-ttu-id="61a17-141">説明</span><span class="sxs-lookup"><span data-stu-id="61a17-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="61a17-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="61a17-142">Authorization</span></span> | <span data-ttu-id="61a17-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="61a17-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="61a17-145">応答</span><span class="sxs-lookup"><span data-stu-id="61a17-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="61a17-146">CSV</span><span class="sxs-lookup"><span data-stu-id="61a17-146">CSV</span></span>

<span data-ttu-id="61a17-147">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="61a17-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="61a17-148">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="61a17-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="61a17-149">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="61a17-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="61a17-150">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="61a17-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="61a17-151">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="61a17-151">Report Refresh Date</span></span>
- <span data-ttu-id="61a17-152">サイトの URL</span><span class="sxs-lookup"><span data-stu-id="61a17-152">Site URL</span></span>
- <span data-ttu-id="61a17-153">所有者の表示名</span><span class="sxs-lookup"><span data-stu-id="61a17-153">Owner Display Name</span></span>
- <span data-ttu-id="61a17-154">削除済み</span><span class="sxs-lookup"><span data-stu-id="61a17-154">Is Deleted</span></span>
- <span data-ttu-id="61a17-155">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="61a17-155">Last Activity Date</span></span>
- <span data-ttu-id="61a17-156">ファイル数</span><span class="sxs-lookup"><span data-stu-id="61a17-156">File Count</span></span>
- <span data-ttu-id="61a17-157">アクティブなファイル数</span><span class="sxs-lookup"><span data-stu-id="61a17-157">Active File Count</span></span>
- <span data-ttu-id="61a17-158">使用済みストレージ (バイト)</span><span class="sxs-lookup"><span data-stu-id="61a17-158">Storage Used (Byte)</span></span>
- <span data-ttu-id="61a17-159">割り当て済みストレージ (バイト)</span><span class="sxs-lookup"><span data-stu-id="61a17-159">Storage Allocated (Byte)</span></span>
- <span data-ttu-id="61a17-160">レポート期間</span><span class="sxs-lookup"><span data-stu-id="61a17-160">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="61a17-161">JSON</span><span class="sxs-lookup"><span data-stu-id="61a17-161">JSON</span></span>

<span data-ttu-id="61a17-162">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に**[oneDriveUsageAccountDetail](../resources/onedriveusageaccountdetail.md)** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="61a17-162">If successful, this method returns a `200 OK` response code and a **[oneDriveUsageAccountDetail](../resources/onedriveusageaccountdetail.md)** object in the response body.</span></span>

<span data-ttu-id="61a17-163">この要求の既定のページ サイズは、アイテムは 200 個です。</span><span class="sxs-lookup"><span data-stu-id="61a17-163">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="61a17-164">例</span><span class="sxs-lookup"><span data-stu-id="61a17-164">Example</span></span>

<span data-ttu-id="61a17-165">次に、CSV を出力する例を示します。</span><span class="sxs-lookup"><span data-stu-id="61a17-165">The following is an example that outputs CSV.</span></span>

### <a name="csv"></a><span data-ttu-id="61a17-166">CSV</span><span class="sxs-lookup"><span data-stu-id="61a17-166">CSV</span></span>

#### <a name="request"></a><span data-ttu-id="61a17-167">要求</span><span class="sxs-lookup"><span data-stu-id="61a17-167">Request</span></span>

<span data-ttu-id="61a17-168">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="61a17-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="61a17-169">応答</span><span class="sxs-lookup"><span data-stu-id="61a17-169">Response</span></span>

<span data-ttu-id="61a17-170">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="61a17-170">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="61a17-171">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="61a17-171">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="61a17-172">JSON</span><span class="sxs-lookup"><span data-stu-id="61a17-172">JSON</span></span>

<span data-ttu-id="61a17-173">次に、JSON を取得する例を示します。</span><span class="sxs-lookup"><span data-stu-id="61a17-173">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="61a17-174">要求</span><span class="sxs-lookup"><span data-stu-id="61a17-174">Request</span></span>

<span data-ttu-id="61a17-175">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="61a17-175">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="61a17-176">応答</span><span class="sxs-lookup"><span data-stu-id="61a17-176">Response</span></span>

<span data-ttu-id="61a17-177">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="61a17-177">The following is an example of the response.</span></span>

> <span data-ttu-id="61a17-p108">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="61a17-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
