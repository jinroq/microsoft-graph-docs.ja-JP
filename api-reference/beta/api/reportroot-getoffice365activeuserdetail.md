---
title: 'reportRoot: getOffice365ActiveUserDetail'
description: Office 365 アクティブ ユーザーに関する詳細を取得します。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: ba73993ffdf205e197058afa2d9aea2648e7c877
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518150"
---
# <a name="reportroot-getoffice365activeuserdetail"></a><span data-ttu-id="c8390-103">reportRoot: getOffice365ActiveUserDetail</span><span class="sxs-lookup"><span data-stu-id="c8390-103">reportRoot: getOffice365ActiveUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8390-104">Office 365 アクティブ ユーザーに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="c8390-104">Get details about Office 365 active users.</span></span>

> <span data-ttu-id="c8390-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: アクティブ ユーザー](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c8390-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="c8390-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c8390-106">Permissions</span></span>

<span data-ttu-id="c8390-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c8390-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c8390-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c8390-109">Permission type</span></span>                        | <span data-ttu-id="c8390-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c8390-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="c8390-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="c8390-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c8390-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c8390-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="c8390-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c8390-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8390-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8390-114">Not supported.</span></span>                           |
| <span data-ttu-id="c8390-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c8390-115">Application</span></span>                            | <span data-ttu-id="c8390-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c8390-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="c8390-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c8390-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserDetail(period='{period_value}')
GET /reports/getOffice365ActiveUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="c8390-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="c8390-118">Function parameters</span></span>

<span data-ttu-id="c8390-119">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="c8390-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="c8390-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="c8390-120">Parameter</span></span> | <span data-ttu-id="c8390-121">型</span><span class="sxs-lookup"><span data-stu-id="c8390-121">Type</span></span>   | <span data-ttu-id="c8390-122">説明</span><span class="sxs-lookup"><span data-stu-id="c8390-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="c8390-123">period</span><span class="sxs-lookup"><span data-stu-id="c8390-123">period</span></span>    | <span data-ttu-id="c8390-124">文字列</span><span class="sxs-lookup"><span data-stu-id="c8390-124">string</span></span> | <span data-ttu-id="c8390-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="c8390-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="c8390-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="c8390-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="c8390-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="c8390-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="c8390-128">date</span><span class="sxs-lookup"><span data-stu-id="c8390-128">date</span></span>      | <span data-ttu-id="c8390-129">日付</span><span class="sxs-lookup"><span data-stu-id="c8390-129">Date</span></span>   | <span data-ttu-id="c8390-130">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="c8390-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="c8390-131">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="c8390-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="c8390-132">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="c8390-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="c8390-133">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c8390-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="c8390-134">このメソッドは、応答をカスタマイズするための `$format`、`$top`、`$skipToken` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c8390-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="c8390-135">既定の出力の種類は、テキストまたは csv です。</span><span class="sxs-lookup"><span data-stu-id="c8390-135">The default output type is text/csv.</span></span> <span data-ttu-id="c8390-136">ただし、出力の種類を指定する場合は、設定をテキストまたは csv またはアプリケーションまたは json OData $format クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="c8390-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c8390-137">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c8390-137">Request headers</span></span>

| <span data-ttu-id="c8390-138">名前</span><span class="sxs-lookup"><span data-stu-id="c8390-138">Name</span></span>          | <span data-ttu-id="c8390-139">説明</span><span class="sxs-lookup"><span data-stu-id="c8390-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="c8390-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8390-140">Authorization</span></span> | <span data-ttu-id="c8390-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c8390-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="c8390-143">応答</span><span class="sxs-lookup"><span data-stu-id="c8390-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="c8390-144">CSV</span><span class="sxs-lookup"><span data-stu-id="c8390-144">CSV</span></span>

<span data-ttu-id="c8390-145">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="c8390-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="c8390-146">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="c8390-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="c8390-147">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="c8390-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="c8390-148">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="c8390-148">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="c8390-149">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="c8390-149">Report Refresh Date</span></span>
- <span data-ttu-id="c8390-150">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="c8390-150">User Principal Name</span></span>
- <span data-ttu-id="c8390-151">表示名</span><span class="sxs-lookup"><span data-stu-id="c8390-151">Display Name</span></span>
- <span data-ttu-id="c8390-152">削除済み</span><span class="sxs-lookup"><span data-stu-id="c8390-152">Is Deleted</span></span>
- <span data-ttu-id="c8390-153">削除日</span><span class="sxs-lookup"><span data-stu-id="c8390-153">Deleted Date</span></span>
- <span data-ttu-id="c8390-154">Exchange ライセンスがある</span><span class="sxs-lookup"><span data-stu-id="c8390-154">Has Exchange License</span></span>
- <span data-ttu-id="c8390-155">OneDrive ライセンスがある</span><span class="sxs-lookup"><span data-stu-id="c8390-155">Has OneDrive License</span></span>
- <span data-ttu-id="c8390-156">SharePoint ライセンスがある</span><span class="sxs-lookup"><span data-stu-id="c8390-156">Has SharePoint License</span></span>
- <span data-ttu-id="c8390-157">Skype for Business ライセンスがある</span><span class="sxs-lookup"><span data-stu-id="c8390-157">Has Skype For Business License</span></span>
- <span data-ttu-id="c8390-158">Yammer ライセンスがある</span><span class="sxs-lookup"><span data-stu-id="c8390-158">Has Yammer License</span></span>
- <span data-ttu-id="c8390-159">Teams ライセンスがある</span><span class="sxs-lookup"><span data-stu-id="c8390-159">Has Teams License</span></span>
- <span data-ttu-id="c8390-160">Exchange の最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="c8390-160">Exchange Last Activity Date</span></span>
- <span data-ttu-id="c8390-161">OneDrive の最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="c8390-161">OneDrive Last Activity Date</span></span>
- <span data-ttu-id="c8390-162">SharePoint の最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="c8390-162">SharePoint Last Activity Date</span></span>
- <span data-ttu-id="c8390-163">Skype For Business の最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="c8390-163">Skype For Business Last Activity Date</span></span>
- <span data-ttu-id="c8390-164">Yammer の最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="c8390-164">Yammer Last Activity Date</span></span>
- <span data-ttu-id="c8390-165">Teams の最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="c8390-165">Teams Last Activity Date</span></span>
- <span data-ttu-id="c8390-166">Exchange のライセンス割り当て日</span><span class="sxs-lookup"><span data-stu-id="c8390-166">Exchange License Assign Date</span></span>
- <span data-ttu-id="c8390-167">OneDrive のライセンス割り当て日</span><span class="sxs-lookup"><span data-stu-id="c8390-167">OneDrive License Assign Date</span></span>
- <span data-ttu-id="c8390-168">SharePoint のライセンス割り当て日</span><span class="sxs-lookup"><span data-stu-id="c8390-168">SharePoint License Assign Date</span></span>
- <span data-ttu-id="c8390-169">Skype For Business のライセンス割り当て日</span><span class="sxs-lookup"><span data-stu-id="c8390-169">Skype For Business License Assign Date</span></span>
- <span data-ttu-id="c8390-170">Yammer のライセンス割り当て日</span><span class="sxs-lookup"><span data-stu-id="c8390-170">Yammer License Assign Date</span></span>
- <span data-ttu-id="c8390-171">Teams のライセンス割り当て日</span><span class="sxs-lookup"><span data-stu-id="c8390-171">Teams License Assign Date</span></span>
- <span data-ttu-id="c8390-172">割り当て済み製品</span><span class="sxs-lookup"><span data-stu-id="c8390-172">Assigned Products</span></span>

<span data-ttu-id="c8390-173">21Vianet によって運営されて、Microsoft Graph 中国では、次の列はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8390-173">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="c8390-174">Yammer ライセンスがある</span><span class="sxs-lookup"><span data-stu-id="c8390-174">Has Yammer License</span></span>
- <span data-ttu-id="c8390-175">Teams ライセンスがある</span><span class="sxs-lookup"><span data-stu-id="c8390-175">Has Teams License</span></span>
- <span data-ttu-id="c8390-176">Yammer の最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="c8390-176">Yammer Last Activity Date</span></span>
- <span data-ttu-id="c8390-177">Teams の最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="c8390-177">Teams Last Activity Date</span></span>
- <span data-ttu-id="c8390-178">Yammer のライセンス割り当て日</span><span class="sxs-lookup"><span data-stu-id="c8390-178">Yammer License Assign Date</span></span>
- <span data-ttu-id="c8390-179">Teams のライセンス割り当て日</span><span class="sxs-lookup"><span data-stu-id="c8390-179">Teams License Assign Date</span></span>

### <a name="json"></a><span data-ttu-id="c8390-180">JSON</span><span class="sxs-lookup"><span data-stu-id="c8390-180">JSON</span></span>

<span data-ttu-id="c8390-181">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の**[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="c8390-181">If successful, this method returns a `200 OK` response code and an **[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="c8390-182">21Vianet によって運営されて、Microsoft Graph 中国では、 **[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** オブジェクトでは、次のプロパティはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8390-182">The following properties in **[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="c8390-183">hasYammerLicense</span><span class="sxs-lookup"><span data-stu-id="c8390-183">hasYammerLicense</span></span>
- <span data-ttu-id="c8390-184">hasTeamsLicense</span><span class="sxs-lookup"><span data-stu-id="c8390-184">hasTeamsLicense</span></span>
- <span data-ttu-id="c8390-185">yammerLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="c8390-185">yammerLastActivityDate</span></span>
- <span data-ttu-id="c8390-186">teamsLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="c8390-186">teamsLastActivityDate</span></span>
- <span data-ttu-id="c8390-187">yammerLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="c8390-187">yammerLicenseAssignDate</span></span>
- <span data-ttu-id="c8390-188">teamsLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="c8390-188">teamsLicenseAssignDate</span></span>

<span data-ttu-id="c8390-189">この要求の既定のページ サイズは、アイテムは 200 個です。</span><span class="sxs-lookup"><span data-stu-id="c8390-189">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="c8390-190">例</span><span class="sxs-lookup"><span data-stu-id="c8390-190">Example</span></span>

### <a name="csv"></a><span data-ttu-id="c8390-191">CSV</span><span class="sxs-lookup"><span data-stu-id="c8390-191">CSV</span></span>

<span data-ttu-id="c8390-192">次に、CSV を出力する例を示します。</span><span class="sxs-lookup"><span data-stu-id="c8390-192">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="c8390-193">要求</span><span class="sxs-lookup"><span data-stu-id="c8390-193">Request</span></span>

<span data-ttu-id="c8390-194">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c8390-194">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="c8390-195">応答</span><span class="sxs-lookup"><span data-stu-id="c8390-195">Response</span></span>

<span data-ttu-id="c8390-196">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c8390-196">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="c8390-197">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="c8390-197">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Has Exchange License,Has OneDrive License,Has SharePoint License,Has Skype For Business License,Has Yammer License,Has Teams License,Exchange Last Activity Date,OneDrive Last Activity Date,SharePoint Last Activity Date,Skype For Business Last Activity Date,Yammer Last Activity Date,Teams Last Activity Date,Exchange License Assign Date,OneDrive License Assign Date,SharePoint License Assign Date,Skype For Business License Assign Date,Yammer License Assign Date,Teams License Assign Date,Assigned Products
```

### <a name="json"></a><span data-ttu-id="c8390-198">JSON</span><span class="sxs-lookup"><span data-stu-id="c8390-198">JSON</span></span>

<span data-ttu-id="c8390-199">次に、JSON を取得する例を示します。</span><span class="sxs-lookup"><span data-stu-id="c8390-199">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="c8390-200">要求</span><span class="sxs-lookup"><span data-stu-id="c8390-200">Request</span></span>

<span data-ttu-id="c8390-201">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c8390-201">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="c8390-202">応答</span><span class="sxs-lookup"><span data-stu-id="c8390-202">Response</span></span>

<span data-ttu-id="c8390-203">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c8390-203">The following is an example of the response.</span></span>

> <span data-ttu-id="c8390-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="c8390-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ActiveUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 853

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365ActiveUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userprincipalname-value", 
      "displayName": "displayname-value", 
      "isDeleted": false, 
      "deletedDate": null, 
      "hasExchangeLicense": true, 
      "hasOneDriveLicense": false, 
      "hasSharePointLicense": false, 
      "hasSkypeForBusinessLicense": false, 
      "hasYammerLicense": false, 
      "hasTeamsLicense": false, 
      "exchangeLastActivityDate": "2017-08-30", 
      "oneDriveLastActivityDate": null, 
      "sharePointLastActivityDate": null, 
      "skypeForBusinessLastActivityDate": null, 
      "yammerLastActivityDate": null, 
      "teamsLastActivityDate": null, 
      "exchangeLicenseAssignDate": "2016-05-03", 
      "oneDriveLicenseAssignDate": null, 
      "sharePointLicenseAssignDate": null, 
      "skypeForBusinessLicenseAssignDate": null, 
      "yammerLicenseAssignDate": null, 
      "teamsLicenseAssignDate": null, 
      "assignedProducts": [
        "OFFICE 365 ENTERPRISE E5"
      ]
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getoffice365activeuserdetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
