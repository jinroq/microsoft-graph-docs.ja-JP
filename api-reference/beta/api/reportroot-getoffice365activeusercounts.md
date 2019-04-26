---
title: 'reportRoot: getOffice365ActiveUserCounts'
description: レポート期間中の日ごとのアクティブ ユーザー数を製品別に取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: c8834d59abd186a6a9c20b6ef4a3a6c6674bffba
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33336749"
---
# <a name="reportroot-getoffice365activeusercounts"></a><span data-ttu-id="9df14-103">reportRoot: getOffice365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="9df14-103">reportRoot: getOffice365ActiveUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9df14-104">レポート期間中の日ごとのアクティブ ユーザー数を製品別に取得します。</span><span class="sxs-lookup"><span data-stu-id="9df14-104">Get the count of daily active users in the reporting period by product.</span></span>

> <span data-ttu-id="9df14-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: アクティブ ユーザー](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9df14-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="9df14-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9df14-106">Permissions</span></span>

<span data-ttu-id="9df14-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9df14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9df14-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9df14-109">Permission type</span></span>                        | <span data-ttu-id="9df14-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9df14-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="9df14-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="9df14-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9df14-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9df14-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="9df14-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9df14-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9df14-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9df14-114">Not supported.</span></span>                           |
| <span data-ttu-id="9df14-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9df14-115">Application</span></span>                            | <span data-ttu-id="9df14-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9df14-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="9df14-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9df14-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="9df14-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="9df14-118">Function parameters</span></span>

<span data-ttu-id="9df14-119">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="9df14-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="9df14-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="9df14-120">Parameter</span></span> | <span data-ttu-id="9df14-121">型</span><span class="sxs-lookup"><span data-stu-id="9df14-121">Type</span></span>   | <span data-ttu-id="9df14-122">説明</span><span class="sxs-lookup"><span data-stu-id="9df14-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="9df14-123">period</span><span class="sxs-lookup"><span data-stu-id="9df14-123">period</span></span>    | <span data-ttu-id="9df14-124">文字列</span><span class="sxs-lookup"><span data-stu-id="9df14-124">string</span></span> | <span data-ttu-id="9df14-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="9df14-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="9df14-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="9df14-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="9df14-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="9df14-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="9df14-128">必須。</span><span class="sxs-lookup"><span data-stu-id="9df14-128">Required.</span></span> |

<span data-ttu-id="9df14-129">このメソッドは、 `$format`応答をカスタマイズするための[OData クエリパラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="9df14-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="9df14-130">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="9df14-130">The default output type is text/csv.</span></span> <span data-ttu-id="9df14-131">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="9df14-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9df14-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9df14-132">Request headers</span></span>

| <span data-ttu-id="9df14-133">名前</span><span class="sxs-lookup"><span data-stu-id="9df14-133">Name</span></span>          | <span data-ttu-id="9df14-134">説明</span><span class="sxs-lookup"><span data-stu-id="9df14-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="9df14-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="9df14-135">Authorization</span></span> | <span data-ttu-id="9df14-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9df14-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="9df14-138">応答</span><span class="sxs-lookup"><span data-stu-id="9df14-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="9df14-139">CSV</span><span class="sxs-lookup"><span data-stu-id="9df14-139">CSV</span></span>

<span data-ttu-id="9df14-140">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="9df14-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="9df14-141">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="9df14-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="9df14-142">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="9df14-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="9df14-143">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="9df14-143">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="9df14-144">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="9df14-144">Report Refresh Date</span></span>
- <span data-ttu-id="9df14-145">Office 365</span><span class="sxs-lookup"><span data-stu-id="9df14-145">Office 365</span></span>
- <span data-ttu-id="9df14-146">Exchange</span><span class="sxs-lookup"><span data-stu-id="9df14-146">Exchange</span></span>
- <span data-ttu-id="9df14-147">OneDrive</span><span class="sxs-lookup"><span data-stu-id="9df14-147">OneDrive</span></span>
- <span data-ttu-id="9df14-148">SharePoint</span><span class="sxs-lookup"><span data-stu-id="9df14-148">SharePoint</span></span>
- <span data-ttu-id="9df14-149">Skype For Business</span><span class="sxs-lookup"><span data-stu-id="9df14-149">Skype For Business</span></span> 
- <span data-ttu-id="9df14-150">Yammer</span><span class="sxs-lookup"><span data-stu-id="9df14-150">Yammer</span></span>
- <span data-ttu-id="9df14-151">Teams</span><span class="sxs-lookup"><span data-stu-id="9df14-151">Teams</span></span>
- <span data-ttu-id="9df14-152">レポート日付</span><span class="sxs-lookup"><span data-stu-id="9df14-152">Report Date</span></span>
- <span data-ttu-id="9df14-153">レポート期間</span><span class="sxs-lookup"><span data-stu-id="9df14-153">Report Period</span></span>

<span data-ttu-id="9df14-154">次の列は、21vianet が運用している Microsoft graph 中国ではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9df14-154">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="9df14-155">Yammer</span><span class="sxs-lookup"><span data-stu-id="9df14-155">Yammer</span></span>
- <span data-ttu-id="9df14-156">Teams</span><span class="sxs-lookup"><span data-stu-id="9df14-156">Teams</span></span>

### <a name="json"></a><span data-ttu-id="9df14-157">JSON</span><span class="sxs-lookup"><span data-stu-id="9df14-157">JSON</span></span>

<span data-ttu-id="9df14-158">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[office365ActiveUserCounts](../resources/office365activeusercounts.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9df14-158">If successful, this method returns a `200 OK` response code and an **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** object in the response body.</span></span>

<span data-ttu-id="9df14-159">**[office365ActiveUserCounts](../resources/office365activeusercounts.md)** オブジェクトの次のプロパティは、21vianet が運用している Microsoft Graph の中国ではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9df14-159">The following properties in **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="9df14-160">yammer</span><span class="sxs-lookup"><span data-stu-id="9df14-160">yammer</span></span>
- <span data-ttu-id="9df14-161">teams</span><span class="sxs-lookup"><span data-stu-id="9df14-161">teams</span></span>

## <a name="example"></a><span data-ttu-id="9df14-162">例</span><span class="sxs-lookup"><span data-stu-id="9df14-162">Example</span></span>

### <a name="csv"></a><span data-ttu-id="9df14-163">CSV</span><span class="sxs-lookup"><span data-stu-id="9df14-163">CSV</span></span>

<span data-ttu-id="9df14-164">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9df14-164">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="9df14-165">要求</span><span class="sxs-lookup"><span data-stu-id="9df14-165">Request</span></span>

<span data-ttu-id="9df14-166">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9df14-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="9df14-167">応答</span><span class="sxs-lookup"><span data-stu-id="9df14-167">Response</span></span>

<span data-ttu-id="9df14-168">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9df14-168">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="9df14-169">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="9df14-169">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Office 365,Exchange,OneDrive,SharePoint,Skype For Business,Yammer,Teams,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="9df14-170">JSON</span><span class="sxs-lookup"><span data-stu-id="9df14-170">JSON</span></span>

<span data-ttu-id="9df14-171">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="9df14-171">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="9df14-172">要求</span><span class="sxs-lookup"><span data-stu-id="9df14-172">Request</span></span>

<span data-ttu-id="9df14-173">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9df14-173">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="9df14-174">応答</span><span class="sxs-lookup"><span data-stu-id="9df14-174">Response</span></span>

<span data-ttu-id="9df14-175">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9df14-175">The following is an example of the response.</span></span>

> <span data-ttu-id="9df14-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="9df14-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ActiveUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 317

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365ActiveUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "office365": 1718, 
      "exchange": 1429, 
      "oneDrive": 350, 
      "sharePoint": 795, 
      "skypeForBusiness": 251, 
      "yammer": 47, 
      "teams": 10, 
      "reportDate": "2017-08-29", 
      "reportPeriod": "7"
    }
  ]
}
```
