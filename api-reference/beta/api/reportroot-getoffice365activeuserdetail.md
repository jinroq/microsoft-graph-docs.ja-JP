---
title: 'reportRoot: getOffice365ActiveUserDetail'
description: Office 365 アクティブ ユーザーに関する詳細を取得します。
localization_priority: Normal
ms.openlocfilehash: dd727648c9b4b0000888a0d45d55737280fc11ba
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882384"
---
# <a name="reportroot-getoffice365activeuserdetail"></a><span data-ttu-id="8e85a-103">reportRoot: getOffice365ActiveUserDetail</span><span class="sxs-lookup"><span data-stu-id="8e85a-103">reportRoot: getOffice365ActiveUserDetail</span></span>

> <span data-ttu-id="8e85a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8e85a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8e85a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8e85a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8e85a-106">Office 365 アクティブ ユーザーに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="8e85a-106">Get details about Office 365 active users.</span></span>

> <span data-ttu-id="8e85a-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: アクティブ ユーザー](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8e85a-107">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="8e85a-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8e85a-108">Permissions</span></span>

<span data-ttu-id="8e85a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8e85a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8e85a-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8e85a-111">Permission type</span></span>                        | <span data-ttu-id="8e85a-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8e85a-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="8e85a-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="8e85a-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="8e85a-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8e85a-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="8e85a-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8e85a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e85a-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8e85a-116">Not supported.</span></span>                           |
| <span data-ttu-id="8e85a-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8e85a-117">Application</span></span>                            | <span data-ttu-id="8e85a-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8e85a-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="8e85a-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8e85a-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserDetail(period='{period_value}')
GET /reports/getOffice365ActiveUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="8e85a-120">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="8e85a-120">Function parameters</span></span>

<span data-ttu-id="8e85a-121">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="8e85a-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="8e85a-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="8e85a-122">Parameter</span></span> | <span data-ttu-id="8e85a-123">Type</span><span class="sxs-lookup"><span data-stu-id="8e85a-123">Type</span></span>   | <span data-ttu-id="8e85a-124">説明</span><span class="sxs-lookup"><span data-stu-id="8e85a-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="8e85a-125">period</span><span class="sxs-lookup"><span data-stu-id="8e85a-125">period</span></span>    | <span data-ttu-id="8e85a-126">文字列</span><span class="sxs-lookup"><span data-stu-id="8e85a-126">string</span></span> | <span data-ttu-id="8e85a-127">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="8e85a-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="8e85a-128">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="8e85a-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="8e85a-129">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="8e85a-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="8e85a-130">date</span><span class="sxs-lookup"><span data-stu-id="8e85a-130">date</span></span>      | <span data-ttu-id="8e85a-131">日付</span><span class="sxs-lookup"><span data-stu-id="8e85a-131">Date</span></span>   | <span data-ttu-id="8e85a-132">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="8e85a-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="8e85a-133">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="8e85a-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="8e85a-134">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="8e85a-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="8e85a-135">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="8e85a-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="8e85a-136">このメソッドは、応答をカスタマイズするための `$format`、`$top`、`$skipToken` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="8e85a-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="8e85a-137">既定の出力の種類は、テキストまたは csv です。</span><span class="sxs-lookup"><span data-stu-id="8e85a-137">The default output type is text/csv.</span></span> <span data-ttu-id="8e85a-138">ただし、出力の種類を指定する場合は、設定をテキストまたは csv またはアプリケーションまたは json OData $format クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="8e85a-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8e85a-139">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8e85a-139">Request headers</span></span>

| <span data-ttu-id="8e85a-140">名前</span><span class="sxs-lookup"><span data-stu-id="8e85a-140">Name</span></span>          | <span data-ttu-id="8e85a-141">説明</span><span class="sxs-lookup"><span data-stu-id="8e85a-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="8e85a-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e85a-142">Authorization</span></span> | <span data-ttu-id="8e85a-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8e85a-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="8e85a-145">応答</span><span class="sxs-lookup"><span data-stu-id="8e85a-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="8e85a-146">CSV</span><span class="sxs-lookup"><span data-stu-id="8e85a-146">CSV</span></span>

<span data-ttu-id="8e85a-147">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="8e85a-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="8e85a-148">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="8e85a-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="8e85a-149">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="8e85a-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="8e85a-150">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="8e85a-150">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="8e85a-151">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="8e85a-151">Report Refresh Date</span></span>
- <span data-ttu-id="8e85a-152">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="8e85a-152">User Principal Name</span></span>
- <span data-ttu-id="8e85a-153">表示名</span><span class="sxs-lookup"><span data-stu-id="8e85a-153">Display Name</span></span>
- <span data-ttu-id="8e85a-154">削除済み</span><span class="sxs-lookup"><span data-stu-id="8e85a-154">Is Deleted</span></span>
- <span data-ttu-id="8e85a-155">削除日</span><span class="sxs-lookup"><span data-stu-id="8e85a-155">Deleted Date</span></span>
- <span data-ttu-id="8e85a-156">Exchange ライセンスがある</span><span class="sxs-lookup"><span data-stu-id="8e85a-156">Has Exchange License</span></span>
- <span data-ttu-id="8e85a-157">OneDrive ライセンスがある</span><span class="sxs-lookup"><span data-stu-id="8e85a-157">Has OneDrive License</span></span>
- <span data-ttu-id="8e85a-158">SharePoint ライセンスがある</span><span class="sxs-lookup"><span data-stu-id="8e85a-158">Has SharePoint License</span></span>
- <span data-ttu-id="8e85a-159">Skype for Business ライセンスがある</span><span class="sxs-lookup"><span data-stu-id="8e85a-159">Has Skype For Business License</span></span>
- <span data-ttu-id="8e85a-160">Yammer ライセンスがある</span><span class="sxs-lookup"><span data-stu-id="8e85a-160">Has Yammer License</span></span>
- <span data-ttu-id="8e85a-161">Teams ライセンスがある</span><span class="sxs-lookup"><span data-stu-id="8e85a-161">Has Teams License</span></span>
- <span data-ttu-id="8e85a-162">Exchange の最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="8e85a-162">Exchange Last Activity Date</span></span>
- <span data-ttu-id="8e85a-163">OneDrive の最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="8e85a-163">OneDrive Last Activity Date</span></span>
- <span data-ttu-id="8e85a-164">SharePoint の最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="8e85a-164">SharePoint Last Activity Date</span></span>
- <span data-ttu-id="8e85a-165">Skype For Business の最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="8e85a-165">Skype For Business Last Activity Date</span></span>
- <span data-ttu-id="8e85a-166">Yammer の最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="8e85a-166">Yammer Last Activity Date</span></span>
- <span data-ttu-id="8e85a-167">Teams の最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="8e85a-167">Teams Last Activity Date</span></span>
- <span data-ttu-id="8e85a-168">Exchange のライセンス割り当て日</span><span class="sxs-lookup"><span data-stu-id="8e85a-168">Exchange License Assign Date</span></span>
- <span data-ttu-id="8e85a-169">OneDrive のライセンス割り当て日</span><span class="sxs-lookup"><span data-stu-id="8e85a-169">OneDrive License Assign Date</span></span>
- <span data-ttu-id="8e85a-170">SharePoint のライセンス割り当て日</span><span class="sxs-lookup"><span data-stu-id="8e85a-170">SharePoint License Assign Date</span></span>
- <span data-ttu-id="8e85a-171">Skype For Business のライセンス割り当て日</span><span class="sxs-lookup"><span data-stu-id="8e85a-171">Skype For Business License Assign Date</span></span>
- <span data-ttu-id="8e85a-172">Yammer のライセンス割り当て日</span><span class="sxs-lookup"><span data-stu-id="8e85a-172">Yammer License Assign Date</span></span>
- <span data-ttu-id="8e85a-173">Teams のライセンス割り当て日</span><span class="sxs-lookup"><span data-stu-id="8e85a-173">Teams License Assign Date</span></span>
- <span data-ttu-id="8e85a-174">割り当て済み製品</span><span class="sxs-lookup"><span data-stu-id="8e85a-174">Assigned Products</span></span>

<span data-ttu-id="8e85a-175">21Vianet によって運営されて、Microsoft Graph 中国では、次の列はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8e85a-175">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="8e85a-176">Yammer ライセンスがある</span><span class="sxs-lookup"><span data-stu-id="8e85a-176">Has Yammer License</span></span>
- <span data-ttu-id="8e85a-177">Teams ライセンスがある</span><span class="sxs-lookup"><span data-stu-id="8e85a-177">Has Teams License</span></span>
- <span data-ttu-id="8e85a-178">Yammer の最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="8e85a-178">Yammer Last Activity Date</span></span>
- <span data-ttu-id="8e85a-179">Teams の最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="8e85a-179">Teams Last Activity Date</span></span>
- <span data-ttu-id="8e85a-180">Yammer のライセンス割り当て日</span><span class="sxs-lookup"><span data-stu-id="8e85a-180">Yammer License Assign Date</span></span>
- <span data-ttu-id="8e85a-181">Teams のライセンス割り当て日</span><span class="sxs-lookup"><span data-stu-id="8e85a-181">Teams License Assign Date</span></span>

### <a name="json"></a><span data-ttu-id="8e85a-182">JSON</span><span class="sxs-lookup"><span data-stu-id="8e85a-182">JSON</span></span>

<span data-ttu-id="8e85a-183">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の**[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="8e85a-183">If successful, this method returns a `200 OK` response code and an **[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="8e85a-184">21Vianet によって運営されて、Microsoft Graph 中国では、 **[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** オブジェクトでは、次のプロパティはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8e85a-184">The following properties in **[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="8e85a-185">hasYammerLicense</span><span class="sxs-lookup"><span data-stu-id="8e85a-185">hasYammerLicense</span></span>
- <span data-ttu-id="8e85a-186">hasTeamsLicense</span><span class="sxs-lookup"><span data-stu-id="8e85a-186">hasTeamsLicense</span></span>
- <span data-ttu-id="8e85a-187">yammerLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="8e85a-187">yammerLastActivityDate</span></span>
- <span data-ttu-id="8e85a-188">teamsLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="8e85a-188">teamsLastActivityDate</span></span>
- <span data-ttu-id="8e85a-189">yammerLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="8e85a-189">yammerLicenseAssignDate</span></span>
- <span data-ttu-id="8e85a-190">teamsLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="8e85a-190">teamsLicenseAssignDate</span></span>

<span data-ttu-id="8e85a-191">この要求の既定のページ サイズは、アイテムは 200 個です。</span><span class="sxs-lookup"><span data-stu-id="8e85a-191">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="8e85a-192">例</span><span class="sxs-lookup"><span data-stu-id="8e85a-192">Example</span></span>

### <a name="csv"></a><span data-ttu-id="8e85a-193">CSV</span><span class="sxs-lookup"><span data-stu-id="8e85a-193">CSV</span></span>

<span data-ttu-id="8e85a-194">次に、CSV を出力する例を示します。</span><span class="sxs-lookup"><span data-stu-id="8e85a-194">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="8e85a-195">要求</span><span class="sxs-lookup"><span data-stu-id="8e85a-195">Request</span></span>

<span data-ttu-id="8e85a-196">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8e85a-196">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="8e85a-197">応答</span><span class="sxs-lookup"><span data-stu-id="8e85a-197">Response</span></span>

<span data-ttu-id="8e85a-198">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8e85a-198">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="8e85a-199">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="8e85a-199">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="8e85a-200">JSON</span><span class="sxs-lookup"><span data-stu-id="8e85a-200">JSON</span></span>

<span data-ttu-id="8e85a-201">次に、JSON を取得する例を示します。</span><span class="sxs-lookup"><span data-stu-id="8e85a-201">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="8e85a-202">要求</span><span class="sxs-lookup"><span data-stu-id="8e85a-202">Request</span></span>

<span data-ttu-id="8e85a-203">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8e85a-203">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="8e85a-204">応答</span><span class="sxs-lookup"><span data-stu-id="8e85a-204">Response</span></span>

<span data-ttu-id="8e85a-205">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8e85a-205">The following is an example of the response.</span></span>

> <span data-ttu-id="8e85a-p108">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="8e85a-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
