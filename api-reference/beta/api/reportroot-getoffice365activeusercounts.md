---
title: 'reportRoot: getOffice365ActiveUserCounts'
description: レポート期間中の日ごとのアクティブ ユーザー数を製品別に取得します。
ms.openlocfilehash: 29cb7a18520774b192d5e9e71b62a7ca86fa9be5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069030"
---
# <a name="reportroot-getoffice365activeusercounts"></a><span data-ttu-id="85c9b-103">reportRoot: getOffice365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="85c9b-103">reportRoot: getOffice365ActiveUserCounts</span></span>

> <span data-ttu-id="85c9b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="85c9b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="85c9b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="85c9b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="85c9b-106">レポート期間中の日ごとのアクティブ ユーザー数を製品別に取得します。</span><span class="sxs-lookup"><span data-stu-id="85c9b-106">Get the count of daily active users in the reporting period by product.</span></span>

> <span data-ttu-id="85c9b-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: アクティブ ユーザー](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="85c9b-107">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="85c9b-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="85c9b-108">Permissions</span></span>

<span data-ttu-id="85c9b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="85c9b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="85c9b-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="85c9b-111">Permission type</span></span>                        | <span data-ttu-id="85c9b-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="85c9b-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="85c9b-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="85c9b-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="85c9b-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="85c9b-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="85c9b-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="85c9b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85c9b-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="85c9b-116">Not supported.</span></span>                           |
| <span data-ttu-id="85c9b-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="85c9b-117">Application</span></span>                            | <span data-ttu-id="85c9b-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="85c9b-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="85c9b-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="85c9b-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="85c9b-120">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="85c9b-120">Function parameters</span></span>

<span data-ttu-id="85c9b-121">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="85c9b-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="85c9b-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="85c9b-122">Parameter</span></span> | <span data-ttu-id="85c9b-123">型</span><span class="sxs-lookup"><span data-stu-id="85c9b-123">Type</span></span>   | <span data-ttu-id="85c9b-124">説明</span><span class="sxs-lookup"><span data-stu-id="85c9b-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="85c9b-125">period</span><span class="sxs-lookup"><span data-stu-id="85c9b-125">period</span></span>    | <span data-ttu-id="85c9b-126">文字列</span><span class="sxs-lookup"><span data-stu-id="85c9b-126">string</span></span> | <span data-ttu-id="85c9b-127">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="85c9b-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="85c9b-128">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="85c9b-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="85c9b-129">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="85c9b-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="85c9b-130">必須。</span><span class="sxs-lookup"><span data-stu-id="85c9b-130">Required.</span></span> |

<span data-ttu-id="85c9b-131">このメソッドをサポートしている、 `$format` 、応答をカスタマイズするのには、 [OData クエリ パラメーター](/graph/query-parameters)です。</span><span class="sxs-lookup"><span data-stu-id="85c9b-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="85c9b-132">既定の出力の種類は、テキストまたは csv です。</span><span class="sxs-lookup"><span data-stu-id="85c9b-132">The default output type is text/csv.</span></span> <span data-ttu-id="85c9b-133">ただし、出力の種類を指定する場合は、設定をテキストまたは csv またはアプリケーションまたは json OData $format クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="85c9b-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="85c9b-134">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="85c9b-134">Request headers</span></span>

| <span data-ttu-id="85c9b-135">名前</span><span class="sxs-lookup"><span data-stu-id="85c9b-135">Name</span></span>          | <span data-ttu-id="85c9b-136">説明</span><span class="sxs-lookup"><span data-stu-id="85c9b-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="85c9b-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="85c9b-137">Authorization</span></span> | <span data-ttu-id="85c9b-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="85c9b-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="85c9b-140">応答</span><span class="sxs-lookup"><span data-stu-id="85c9b-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="85c9b-141">CSV</span><span class="sxs-lookup"><span data-stu-id="85c9b-141">CSV</span></span>

<span data-ttu-id="85c9b-142">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="85c9b-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="85c9b-143">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="85c9b-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="85c9b-144">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="85c9b-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="85c9b-145">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="85c9b-145">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="85c9b-146">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="85c9b-146">Report Refresh Date</span></span>
- <span data-ttu-id="85c9b-147">Office 365</span><span class="sxs-lookup"><span data-stu-id="85c9b-147">Office 365</span></span>
- <span data-ttu-id="85c9b-148">Exchange</span><span class="sxs-lookup"><span data-stu-id="85c9b-148">Exchange</span></span>
- <span data-ttu-id="85c9b-149">OneDrive</span><span class="sxs-lookup"><span data-stu-id="85c9b-149">OneDrive</span></span>
- <span data-ttu-id="85c9b-150">SharePoint</span><span class="sxs-lookup"><span data-stu-id="85c9b-150">SharePoint</span></span>
- <span data-ttu-id="85c9b-151">Skype For Business</span><span class="sxs-lookup"><span data-stu-id="85c9b-151">Skype For Business</span></span> 
- <span data-ttu-id="85c9b-152">Yammer</span><span class="sxs-lookup"><span data-stu-id="85c9b-152">Yammer</span></span>
- <span data-ttu-id="85c9b-153">Teams</span><span class="sxs-lookup"><span data-stu-id="85c9b-153">Teams</span></span>
- <span data-ttu-id="85c9b-154">レポート日付</span><span class="sxs-lookup"><span data-stu-id="85c9b-154">Report Date</span></span>
- <span data-ttu-id="85c9b-155">レポート期間</span><span class="sxs-lookup"><span data-stu-id="85c9b-155">Report Period</span></span>

<span data-ttu-id="85c9b-156">21Vianet によって運営されて、Microsoft Graph 中国では、次の列はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="85c9b-156">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="85c9b-157">Yammer</span><span class="sxs-lookup"><span data-stu-id="85c9b-157">Yammer</span></span>
- <span data-ttu-id="85c9b-158">Teams</span><span class="sxs-lookup"><span data-stu-id="85c9b-158">Teams</span></span>

### <a name="json"></a><span data-ttu-id="85c9b-159">JSON</span><span class="sxs-lookup"><span data-stu-id="85c9b-159">JSON</span></span>

<span data-ttu-id="85c9b-160">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の**[office365ActiveUserCounts](../resources/office365activeusercounts.md)** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="85c9b-160">If successful, this method returns a `200 OK` response code and an **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** object in the response body.</span></span>

<span data-ttu-id="85c9b-161">21Vianet によって運営されて、Microsoft Graph 中国では、 **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** オブジェクトでは、次のプロパティはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="85c9b-161">The following properties in **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="85c9b-162">yammer</span><span class="sxs-lookup"><span data-stu-id="85c9b-162">yammer</span></span>
- <span data-ttu-id="85c9b-163">チーム</span><span class="sxs-lookup"><span data-stu-id="85c9b-163">teams</span></span>

## <a name="example"></a><span data-ttu-id="85c9b-164">使用例</span><span class="sxs-lookup"><span data-stu-id="85c9b-164">Example</span></span>

### <a name="csv"></a><span data-ttu-id="85c9b-165">CSV</span><span class="sxs-lookup"><span data-stu-id="85c9b-165">CSV</span></span>

<span data-ttu-id="85c9b-166">次に、CSV を出力する例を示します。</span><span class="sxs-lookup"><span data-stu-id="85c9b-166">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="85c9b-167">要求</span><span class="sxs-lookup"><span data-stu-id="85c9b-167">Request</span></span>

<span data-ttu-id="85c9b-168">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="85c9b-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="85c9b-169">応答</span><span class="sxs-lookup"><span data-stu-id="85c9b-169">Response</span></span>

<span data-ttu-id="85c9b-170">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="85c9b-170">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="85c9b-171">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="85c9b-171">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="85c9b-172">JSON</span><span class="sxs-lookup"><span data-stu-id="85c9b-172">JSON</span></span>

<span data-ttu-id="85c9b-173">次に、JSON を取得する例を示します。</span><span class="sxs-lookup"><span data-stu-id="85c9b-173">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="85c9b-174">要求</span><span class="sxs-lookup"><span data-stu-id="85c9b-174">Request</span></span>

<span data-ttu-id="85c9b-175">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="85c9b-175">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="85c9b-176">応答</span><span class="sxs-lookup"><span data-stu-id="85c9b-176">Response</span></span>

<span data-ttu-id="85c9b-177">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="85c9b-177">The following is an example of the response.</span></span>

> <span data-ttu-id="85c9b-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="85c9b-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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