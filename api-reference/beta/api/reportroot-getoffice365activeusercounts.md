---
title: 'reportRoot: getOffice365ActiveUserCounts'
description: レポート期間中の日ごとのアクティブ ユーザー数を製品別に取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 9b24008a3ea13308f0d83a2ac6a6ef31ece32469
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575315"
---
# <a name="reportroot-getoffice365activeusercounts"></a><span data-ttu-id="f1a21-103">reportRoot: getOffice365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="f1a21-103">reportRoot: getOffice365ActiveUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1a21-104">レポート期間中の日ごとのアクティブ ユーザー数を製品別に取得します。</span><span class="sxs-lookup"><span data-stu-id="f1a21-104">Get the count of daily active users in the reporting period by product.</span></span>

> <span data-ttu-id="f1a21-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: アクティブ ユーザー](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f1a21-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="f1a21-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f1a21-106">Permissions</span></span>

<span data-ttu-id="f1a21-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f1a21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f1a21-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f1a21-109">Permission type</span></span>                        | <span data-ttu-id="f1a21-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f1a21-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="f1a21-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="f1a21-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f1a21-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f1a21-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="f1a21-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f1a21-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1a21-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f1a21-114">Not supported.</span></span>                           |
| <span data-ttu-id="f1a21-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f1a21-115">Application</span></span>                            | <span data-ttu-id="f1a21-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f1a21-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="f1a21-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f1a21-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="f1a21-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="f1a21-118">Function parameters</span></span>

<span data-ttu-id="f1a21-119">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="f1a21-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="f1a21-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="f1a21-120">Parameter</span></span> | <span data-ttu-id="f1a21-121">型</span><span class="sxs-lookup"><span data-stu-id="f1a21-121">Type</span></span>   | <span data-ttu-id="f1a21-122">説明</span><span class="sxs-lookup"><span data-stu-id="f1a21-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="f1a21-123">period</span><span class="sxs-lookup"><span data-stu-id="f1a21-123">period</span></span>    | <span data-ttu-id="f1a21-124">文字列</span><span class="sxs-lookup"><span data-stu-id="f1a21-124">string</span></span> | <span data-ttu-id="f1a21-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="f1a21-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="f1a21-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="f1a21-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="f1a21-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="f1a21-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="f1a21-128">必須。</span><span class="sxs-lookup"><span data-stu-id="f1a21-128">Required.</span></span> |

<span data-ttu-id="f1a21-129">このメソッドをサポートしている、 `$format` 、応答をカスタマイズするのには、 [OData クエリ パラメーター](/graph/query-parameters)です。</span><span class="sxs-lookup"><span data-stu-id="f1a21-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="f1a21-130">既定の出力の種類は、テキストまたは csv です。</span><span class="sxs-lookup"><span data-stu-id="f1a21-130">The default output type is text/csv.</span></span> <span data-ttu-id="f1a21-131">ただし、出力の種類を指定する場合は、設定をテキストまたは csv またはアプリケーションまたは json OData $format クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="f1a21-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f1a21-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f1a21-132">Request headers</span></span>

| <span data-ttu-id="f1a21-133">名前</span><span class="sxs-lookup"><span data-stu-id="f1a21-133">Name</span></span>          | <span data-ttu-id="f1a21-134">説明</span><span class="sxs-lookup"><span data-stu-id="f1a21-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="f1a21-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1a21-135">Authorization</span></span> | <span data-ttu-id="f1a21-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f1a21-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="f1a21-138">応答</span><span class="sxs-lookup"><span data-stu-id="f1a21-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="f1a21-139">CSV</span><span class="sxs-lookup"><span data-stu-id="f1a21-139">CSV</span></span>

<span data-ttu-id="f1a21-140">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="f1a21-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="f1a21-141">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="f1a21-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="f1a21-142">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="f1a21-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="f1a21-143">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="f1a21-143">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="f1a21-144">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="f1a21-144">Report Refresh Date</span></span>
- <span data-ttu-id="f1a21-145">Office 365</span><span class="sxs-lookup"><span data-stu-id="f1a21-145">Office 365</span></span>
- <span data-ttu-id="f1a21-146">Exchange</span><span class="sxs-lookup"><span data-stu-id="f1a21-146">Exchange</span></span>
- <span data-ttu-id="f1a21-147">OneDrive</span><span class="sxs-lookup"><span data-stu-id="f1a21-147">OneDrive</span></span>
- <span data-ttu-id="f1a21-148">SharePoint</span><span class="sxs-lookup"><span data-stu-id="f1a21-148">SharePoint</span></span>
- <span data-ttu-id="f1a21-149">Skype For Business</span><span class="sxs-lookup"><span data-stu-id="f1a21-149">Skype For Business</span></span> 
- <span data-ttu-id="f1a21-150">Yammer</span><span class="sxs-lookup"><span data-stu-id="f1a21-150">Yammer</span></span>
- <span data-ttu-id="f1a21-151">Teams</span><span class="sxs-lookup"><span data-stu-id="f1a21-151">Teams</span></span>
- <span data-ttu-id="f1a21-152">レポート日付</span><span class="sxs-lookup"><span data-stu-id="f1a21-152">Report Date</span></span>
- <span data-ttu-id="f1a21-153">レポート期間</span><span class="sxs-lookup"><span data-stu-id="f1a21-153">Report Period</span></span>

<span data-ttu-id="f1a21-154">21Vianet によって運営されて、Microsoft Graph 中国では、次の列はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f1a21-154">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="f1a21-155">Yammer</span><span class="sxs-lookup"><span data-stu-id="f1a21-155">Yammer</span></span>
- <span data-ttu-id="f1a21-156">Teams</span><span class="sxs-lookup"><span data-stu-id="f1a21-156">Teams</span></span>

### <a name="json"></a><span data-ttu-id="f1a21-157">JSON</span><span class="sxs-lookup"><span data-stu-id="f1a21-157">JSON</span></span>

<span data-ttu-id="f1a21-158">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の**[office365ActiveUserCounts](../resources/office365activeusercounts.md)** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="f1a21-158">If successful, this method returns a `200 OK` response code and an **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** object in the response body.</span></span>

<span data-ttu-id="f1a21-159">21Vianet によって運営されて、Microsoft Graph 中国では、 **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** オブジェクトでは、次のプロパティはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f1a21-159">The following properties in **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="f1a21-160">yammer</span><span class="sxs-lookup"><span data-stu-id="f1a21-160">yammer</span></span>
- <span data-ttu-id="f1a21-161">チーム</span><span class="sxs-lookup"><span data-stu-id="f1a21-161">teams</span></span>

## <a name="example"></a><span data-ttu-id="f1a21-162">例</span><span class="sxs-lookup"><span data-stu-id="f1a21-162">Example</span></span>

### <a name="csv"></a><span data-ttu-id="f1a21-163">CSV</span><span class="sxs-lookup"><span data-stu-id="f1a21-163">CSV</span></span>

<span data-ttu-id="f1a21-164">次に、CSV を出力する例を示します。</span><span class="sxs-lookup"><span data-stu-id="f1a21-164">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="f1a21-165">要求</span><span class="sxs-lookup"><span data-stu-id="f1a21-165">Request</span></span>

<span data-ttu-id="f1a21-166">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f1a21-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="f1a21-167">応答</span><span class="sxs-lookup"><span data-stu-id="f1a21-167">Response</span></span>

<span data-ttu-id="f1a21-168">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f1a21-168">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="f1a21-169">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="f1a21-169">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="f1a21-170">JSON</span><span class="sxs-lookup"><span data-stu-id="f1a21-170">JSON</span></span>

<span data-ttu-id="f1a21-171">次に、JSON を取得する例を示します。</span><span class="sxs-lookup"><span data-stu-id="f1a21-171">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="f1a21-172">要求</span><span class="sxs-lookup"><span data-stu-id="f1a21-172">Request</span></span>

<span data-ttu-id="f1a21-173">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f1a21-173">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="f1a21-174">応答</span><span class="sxs-lookup"><span data-stu-id="f1a21-174">Response</span></span>

<span data-ttu-id="f1a21-175">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f1a21-175">The following is an example of the response.</span></span>

> <span data-ttu-id="f1a21-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f1a21-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getoffice365activeusercounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
