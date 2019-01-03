---
title: 'reportRoot: getOneDriveUsageAccountCounts'
description: アクティブな OneDrive for Business サイトの数の傾向を取得します。 ユーザーがファイルを表示、変更、アップロード、ダウンロード、共有、同期したサイトはすべて、アクティブなサイトとみなされます。
ms.openlocfilehash: 146cd3f2be17e74f16b9254fb621ac23bc0d33e0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074470"
---
# <a name="reportroot-getonedriveusageaccountcounts"></a><span data-ttu-id="c0d5b-104">reportRoot: getOneDriveUsageAccountCounts</span><span class="sxs-lookup"><span data-stu-id="c0d5b-104">reportRoot: getOneDriveUsageAccountCounts</span></span>

> <span data-ttu-id="c0d5b-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c0d5b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c0d5b-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c0d5b-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c0d5b-107">アクティブな OneDrive for Business サイトの数の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="c0d5b-107">Get the trend in the number of active OneDrive for Business sites.</span></span> <span data-ttu-id="c0d5b-108">ユーザーがファイルを表示、変更、アップロード、ダウンロード、共有、同期したサイトはすべて、アクティブなサイトとみなされます。</span><span class="sxs-lookup"><span data-stu-id="c0d5b-108">Any site on which users viewed, modified, uploaded, downloaded, shared, or synced files is considered an active site.</span></span>

> <span data-ttu-id="c0d5b-109">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: OneDrive for Business の使用状況](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c0d5b-109">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="c0d5b-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c0d5b-110">Permissions</span></span>

<span data-ttu-id="c0d5b-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c0d5b-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c0d5b-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c0d5b-113">Permission type</span></span>                        | <span data-ttu-id="c0d5b-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c0d5b-114">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="c0d5b-115">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="c0d5b-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="c0d5b-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0d5b-116">Reports.Read.All</span></span>                         |
| <span data-ttu-id="c0d5b-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c0d5b-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0d5b-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c0d5b-118">Not supported.</span></span>                           |
| <span data-ttu-id="c0d5b-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c0d5b-119">Application</span></span>                            | <span data-ttu-id="c0d5b-120">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0d5b-120">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="c0d5b-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c0d5b-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageAccountCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="c0d5b-122">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="c0d5b-122">Function parameters</span></span>

<span data-ttu-id="c0d5b-123">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="c0d5b-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="c0d5b-124">パラメーター</span><span class="sxs-lookup"><span data-stu-id="c0d5b-124">Parameter</span></span> | <span data-ttu-id="c0d5b-125">型</span><span class="sxs-lookup"><span data-stu-id="c0d5b-125">Type</span></span>   | <span data-ttu-id="c0d5b-126">説明</span><span class="sxs-lookup"><span data-stu-id="c0d5b-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="c0d5b-127">period</span><span class="sxs-lookup"><span data-stu-id="c0d5b-127">period</span></span>    | <span data-ttu-id="c0d5b-128">文字列</span><span class="sxs-lookup"><span data-stu-id="c0d5b-128">string</span></span> | <span data-ttu-id="c0d5b-129">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="c0d5b-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="c0d5b-130">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="c0d5b-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="c0d5b-131">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="c0d5b-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="c0d5b-132">必須。</span><span class="sxs-lookup"><span data-stu-id="c0d5b-132">Required.</span></span> |

<span data-ttu-id="c0d5b-133">このメソッドをサポートしている、 `$format` 、応答をカスタマイズするのには、 [OData クエリ パラメーター](/graph/query-parameters)です。</span><span class="sxs-lookup"><span data-stu-id="c0d5b-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="c0d5b-134">既定の出力の種類は、テキストまたは csv です。</span><span class="sxs-lookup"><span data-stu-id="c0d5b-134">The default output type is text/csv.</span></span> <span data-ttu-id="c0d5b-135">ただし、出力の種類を指定する場合は、設定をテキストまたは csv またはアプリケーションまたは json OData $format クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="c0d5b-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c0d5b-136">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c0d5b-136">Request headers</span></span>

| <span data-ttu-id="c0d5b-137">名前</span><span class="sxs-lookup"><span data-stu-id="c0d5b-137">Name</span></span>          | <span data-ttu-id="c0d5b-138">説明</span><span class="sxs-lookup"><span data-stu-id="c0d5b-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="c0d5b-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0d5b-139">Authorization</span></span> | <span data-ttu-id="c0d5b-p107">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c0d5b-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="c0d5b-142">応答</span><span class="sxs-lookup"><span data-stu-id="c0d5b-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="c0d5b-143">CSV</span><span class="sxs-lookup"><span data-stu-id="c0d5b-143">CSV</span></span>

<span data-ttu-id="c0d5b-144">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="c0d5b-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="c0d5b-145">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="c0d5b-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="c0d5b-146">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="c0d5b-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="c0d5b-147">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="c0d5b-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="c0d5b-148">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="c0d5b-148">Report Refresh Date</span></span>
- <span data-ttu-id="c0d5b-149">サイトの種類</span><span class="sxs-lookup"><span data-stu-id="c0d5b-149">Site Type</span></span>
- <span data-ttu-id="c0d5b-150">合計</span><span class="sxs-lookup"><span data-stu-id="c0d5b-150">Total</span></span>
- <span data-ttu-id="c0d5b-151">アクティブ</span><span class="sxs-lookup"><span data-stu-id="c0d5b-151">Active</span></span>
- <span data-ttu-id="c0d5b-152">レポート日付</span><span class="sxs-lookup"><span data-stu-id="c0d5b-152">Report Date</span></span>
- <span data-ttu-id="c0d5b-153">レポート期間</span><span class="sxs-lookup"><span data-stu-id="c0d5b-153">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="c0d5b-154">JSON</span><span class="sxs-lookup"><span data-stu-id="c0d5b-154">JSON</span></span>

<span data-ttu-id="c0d5b-155">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に**[oneDriveUsageAccountCounts](../resources/onedriveusageaccountcounts.md)** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="c0d5b-155">If successful, this method returns a `200 OK` response code and a **[oneDriveUsageAccountCounts](../resources/onedriveusageaccountcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0d5b-156">使用例</span><span class="sxs-lookup"><span data-stu-id="c0d5b-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="c0d5b-157">CSV</span><span class="sxs-lookup"><span data-stu-id="c0d5b-157">CSV</span></span>

<span data-ttu-id="c0d5b-158">次に、CSV を出力する例を示します。</span><span class="sxs-lookup"><span data-stu-id="c0d5b-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="c0d5b-159">要求</span><span class="sxs-lookup"><span data-stu-id="c0d5b-159">Request</span></span>

<span data-ttu-id="c0d5b-160">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c0d5b-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountcounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="c0d5b-161">応答</span><span class="sxs-lookup"><span data-stu-id="c0d5b-161">Response</span></span>

<span data-ttu-id="c0d5b-162">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c0d5b-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="c0d5b-163">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="c0d5b-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="c0d5b-164">JSON</span><span class="sxs-lookup"><span data-stu-id="c0d5b-164">JSON</span></span>

<span data-ttu-id="c0d5b-165">次に、JSON を取得する例を示します。</span><span class="sxs-lookup"><span data-stu-id="c0d5b-165">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="c0d5b-166">要求</span><span class="sxs-lookup"><span data-stu-id="c0d5b-166">Request</span></span>

<span data-ttu-id="c0d5b-167">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c0d5b-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountcounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="c0d5b-168">応答</span><span class="sxs-lookup"><span data-stu-id="c0d5b-168">Response</span></span>

<span data-ttu-id="c0d5b-169">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c0d5b-169">The following is an example of the response.</span></span>

> <span data-ttu-id="c0d5b-p109">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="c0d5b-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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