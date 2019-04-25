---
title: 'reportRoot: getOffice365ServicesUserCounts'
description: アクティビティの種類とサービス別のユーザー数を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: f04f892e3bcfe593ebd1d5a4ca04cf70f0dd38e7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32538106"
---
# <a name="reportroot-getoffice365servicesusercounts"></a><span data-ttu-id="10e79-103">reportRoot: getOffice365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="10e79-103">reportRoot: getOffice365ServicesUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10e79-104">アクティビティの種類とサービス別のユーザー数を取得します。</span><span class="sxs-lookup"><span data-stu-id="10e79-104">Get the count of users by activity type and service.</span></span>

> <span data-ttu-id="10e79-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: アクティブ ユーザー](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="10e79-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="10e79-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="10e79-106">Permissions</span></span>

<span data-ttu-id="10e79-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="10e79-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="10e79-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="10e79-109">Permission type</span></span>                        | <span data-ttu-id="10e79-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="10e79-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="10e79-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="10e79-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="10e79-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="10e79-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="10e79-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="10e79-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10e79-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="10e79-114">Not supported.</span></span>                           |
| <span data-ttu-id="10e79-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="10e79-115">Application</span></span>                            | <span data-ttu-id="10e79-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="10e79-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="10e79-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="10e79-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ServicesUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="10e79-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="10e79-118">Function parameters</span></span>

<span data-ttu-id="10e79-119">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="10e79-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="10e79-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="10e79-120">Parameter</span></span> | <span data-ttu-id="10e79-121">型</span><span class="sxs-lookup"><span data-stu-id="10e79-121">Type</span></span>   | <span data-ttu-id="10e79-122">説明</span><span class="sxs-lookup"><span data-stu-id="10e79-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="10e79-123">period</span><span class="sxs-lookup"><span data-stu-id="10e79-123">period</span></span>    | <span data-ttu-id="10e79-124">文字列</span><span class="sxs-lookup"><span data-stu-id="10e79-124">string</span></span> | <span data-ttu-id="10e79-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="10e79-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="10e79-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="10e79-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="10e79-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="10e79-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="10e79-128">必須。</span><span class="sxs-lookup"><span data-stu-id="10e79-128">Required.</span></span> |

<span data-ttu-id="10e79-129">このメソッドは、 `$format`応答をカスタマイズするための[OData クエリパラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="10e79-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="10e79-130">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="10e79-130">The default output type is text/csv.</span></span> <span data-ttu-id="10e79-131">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="10e79-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="10e79-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="10e79-132">Request headers</span></span>

| <span data-ttu-id="10e79-133">名前</span><span class="sxs-lookup"><span data-stu-id="10e79-133">Name</span></span>          | <span data-ttu-id="10e79-134">説明</span><span class="sxs-lookup"><span data-stu-id="10e79-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="10e79-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="10e79-135">Authorization</span></span> | <span data-ttu-id="10e79-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="10e79-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="10e79-138">応答</span><span class="sxs-lookup"><span data-stu-id="10e79-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="10e79-139">CSV</span><span class="sxs-lookup"><span data-stu-id="10e79-139">CSV</span></span>

<span data-ttu-id="10e79-140">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="10e79-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="10e79-141">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="10e79-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="10e79-142">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="10e79-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="10e79-143">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="10e79-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="10e79-144">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="10e79-144">Report Refresh Date</span></span>
- <span data-ttu-id="10e79-145">Exchange アクティブ</span><span class="sxs-lookup"><span data-stu-id="10e79-145">Exchange Active</span></span>
- <span data-ttu-id="10e79-146">Exchange 非アクティブ</span><span class="sxs-lookup"><span data-stu-id="10e79-146">Exchange Inactive</span></span>
- <span data-ttu-id="10e79-147">OneDrive アクティブ</span><span class="sxs-lookup"><span data-stu-id="10e79-147">OneDrive Active</span></span>
- <span data-ttu-id="10e79-148">OneDrive 非アクティブ</span><span class="sxs-lookup"><span data-stu-id="10e79-148">OneDrive Inactive</span></span>
- <span data-ttu-id="10e79-149">SharePoint アクティブ</span><span class="sxs-lookup"><span data-stu-id="10e79-149">SharePoint Active</span></span>
- <span data-ttu-id="10e79-150">SharePoint 非アクティブ</span><span class="sxs-lookup"><span data-stu-id="10e79-150">SharePoint Inactive</span></span>
- <span data-ttu-id="10e79-151">Skype For Business アクティブ</span><span class="sxs-lookup"><span data-stu-id="10e79-151">Skype For Business Active</span></span>
- <span data-ttu-id="10e79-152">Skype For Business 非アクティブ</span><span class="sxs-lookup"><span data-stu-id="10e79-152">Skype For Business Inactive</span></span>
- <span data-ttu-id="10e79-153">Yammer アクティブ</span><span class="sxs-lookup"><span data-stu-id="10e79-153">Yammer Active</span></span>
- <span data-ttu-id="10e79-154">Yammer 非アクティブ</span><span class="sxs-lookup"><span data-stu-id="10e79-154">Yammer Inactive</span></span>
- <span data-ttu-id="10e79-155">Teams アクティブ</span><span class="sxs-lookup"><span data-stu-id="10e79-155">Teams Active</span></span>
- <span data-ttu-id="10e79-156">Teams 非アクティブ</span><span class="sxs-lookup"><span data-stu-id="10e79-156">Teams Inactive</span></span>
- <span data-ttu-id="10e79-157">Office 365 のアクティブ</span><span class="sxs-lookup"><span data-stu-id="10e79-157">Office 365 Active</span></span>
- <span data-ttu-id="10e79-158">Office 365 の非アクティブ</span><span class="sxs-lookup"><span data-stu-id="10e79-158">Office 365 Inactive</span></span>
- <span data-ttu-id="10e79-159">レポート期間</span><span class="sxs-lookup"><span data-stu-id="10e79-159">Report Period</span></span>

<span data-ttu-id="10e79-160">次の列は、21vianet が運用している Microsoft graph 中国ではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="10e79-160">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="10e79-161">Yammer アクティブ</span><span class="sxs-lookup"><span data-stu-id="10e79-161">Yammer Active</span></span>
- <span data-ttu-id="10e79-162">Yammer 非アクティブ</span><span class="sxs-lookup"><span data-stu-id="10e79-162">Yammer Inactive</span></span>
- <span data-ttu-id="10e79-163">Teams アクティブ</span><span class="sxs-lookup"><span data-stu-id="10e79-163">Teams Active</span></span>
- <span data-ttu-id="10e79-164">Teams 非アクティブ</span><span class="sxs-lookup"><span data-stu-id="10e79-164">Teams Inactive</span></span>

### <a name="json"></a><span data-ttu-id="10e79-165">JSON</span><span class="sxs-lookup"><span data-stu-id="10e79-165">JSON</span></span>

<span data-ttu-id="10e79-166">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="10e79-166">If successful, this method returns a `200 OK` response code and an **[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** object in the response body.</span></span>

<span data-ttu-id="10e79-167">**[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** オブジェクトの次のプロパティは、21vianet が運用している Microsoft Graph の中国ではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="10e79-167">The following properties in **[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="10e79-168">yammerActive</span><span class="sxs-lookup"><span data-stu-id="10e79-168">yammerActive</span></span>
- <span data-ttu-id="10e79-169">yammerInactive</span><span class="sxs-lookup"><span data-stu-id="10e79-169">yammerInactive</span></span>
- <span data-ttu-id="10e79-170">teamsactive</span><span class="sxs-lookup"><span data-stu-id="10e79-170">teamsActive</span></span>
- <span data-ttu-id="10e79-171">teamsinactive</span><span class="sxs-lookup"><span data-stu-id="10e79-171">teamsInactive</span></span>

## <a name="example"></a><span data-ttu-id="10e79-172">例</span><span class="sxs-lookup"><span data-stu-id="10e79-172">Example</span></span>

### <a name="csv"></a><span data-ttu-id="10e79-173">CSV</span><span class="sxs-lookup"><span data-stu-id="10e79-173">CSV</span></span>

<span data-ttu-id="10e79-174">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="10e79-174">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="10e79-175">要求</span><span class="sxs-lookup"><span data-stu-id="10e79-175">Request</span></span>

<span data-ttu-id="10e79-176">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="10e79-176">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365servicesusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ServicesUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="10e79-177">応答</span><span class="sxs-lookup"><span data-stu-id="10e79-177">Response</span></span>

<span data-ttu-id="10e79-178">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="10e79-178">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="10e79-179">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="10e79-179">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Exchange Active,Exchange Inactive,OneDrive Active,OneDrive Inactive,SharePoint Active,SharePoint Inactive,Skype For Business Active,Skype For Business Inactive,Yammer Active,Yammer Inactive,Teams Active,Teams Inactive,Report Period
```

### <a name="json"></a><span data-ttu-id="10e79-180">JSON</span><span class="sxs-lookup"><span data-stu-id="10e79-180">JSON</span></span> 

<span data-ttu-id="10e79-181">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="10e79-181">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="10e79-182">要求</span><span class="sxs-lookup"><span data-stu-id="10e79-182">Request</span></span>

<span data-ttu-id="10e79-183">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="10e79-183">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365servicesusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ServicesUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="10e79-184">応答</span><span class="sxs-lookup"><span data-stu-id="10e79-184">Response</span></span>

<span data-ttu-id="10e79-185">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="10e79-185">The following is an example of the response.</span></span>

> <span data-ttu-id="10e79-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="10e79-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ServicesUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 458

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365ServicesUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "exchangeActive": 2591, 
      "exchangeInactive": 1426, 
      "oneDriveActive": 1800, 
      "oneDriveInactive": 2451, 
      "sharePointActive": 2286, 
      "sharePointInactive": 1815, 
      "skypeForBusinessActive": 2463, 
      "skypeForBusinessInactive": 1947, 
      "yammerActive": 473, 
      "yammerInactive": 2526, 
      "teamsActive": 846, 
      "teamsInactive": 1960, 
      "office365Active": 2791,
      "office365Inactive": 503,
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getoffice365servicesusercounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
