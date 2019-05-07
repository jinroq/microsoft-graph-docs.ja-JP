---
title: 'reportRoot: getOffice365GroupsActivityDetail'
description: グループ別の Office 365 グループ アクティビティに関する詳細を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: cf5519f5093647ba8f855cb6f0467ab2c898545c
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33639412"
---
# <a name="reportroot-getoffice365groupsactivitydetail"></a><span data-ttu-id="74ecc-103">reportRoot: getOffice365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="74ecc-103">reportRoot: getOffice365GroupsActivityDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74ecc-104">グループ別の Office 365 グループ アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="74ecc-104">Get details about Office 365 Groups activity by group.</span></span>

> <span data-ttu-id="74ecc-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Office 365 グループ](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="74ecc-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="74ecc-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="74ecc-106">Permissions</span></span>

<span data-ttu-id="74ecc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="74ecc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="74ecc-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="74ecc-109">Permission type</span></span>                        | <span data-ttu-id="74ecc-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="74ecc-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="74ecc-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="74ecc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="74ecc-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="74ecc-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="74ecc-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="74ecc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74ecc-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="74ecc-114">Not supported.</span></span>                           |
| <span data-ttu-id="74ecc-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="74ecc-115">Application</span></span>                            | <span data-ttu-id="74ecc-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="74ecc-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="74ecc-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="74ecc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityDetail(period='{period_value}')
GET /reports/getOffice365GroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="74ecc-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="74ecc-118">Function parameters</span></span>

<span data-ttu-id="74ecc-119">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="74ecc-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="74ecc-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="74ecc-120">Parameter</span></span> | <span data-ttu-id="74ecc-121">型</span><span class="sxs-lookup"><span data-stu-id="74ecc-121">Type</span></span>   | <span data-ttu-id="74ecc-122">説明</span><span class="sxs-lookup"><span data-stu-id="74ecc-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="74ecc-123">period</span><span class="sxs-lookup"><span data-stu-id="74ecc-123">period</span></span>    | <span data-ttu-id="74ecc-124">文字列</span><span class="sxs-lookup"><span data-stu-id="74ecc-124">string</span></span> | <span data-ttu-id="74ecc-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="74ecc-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="74ecc-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="74ecc-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="74ecc-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="74ecc-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="74ecc-128">date</span><span class="sxs-lookup"><span data-stu-id="74ecc-128">date</span></span>      | <span data-ttu-id="74ecc-129">日付</span><span class="sxs-lookup"><span data-stu-id="74ecc-129">Date</span></span>   | <span data-ttu-id="74ecc-130">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="74ecc-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="74ecc-131">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="74ecc-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="74ecc-132">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="74ecc-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="74ecc-133">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="74ecc-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="74ecc-134">このメソッドは、応答をカスタマイズするための `$format`、`$top`、`$skipToken` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="74ecc-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="74ecc-135">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="74ecc-135">The default output type is text/csv.</span></span> <span data-ttu-id="74ecc-136">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="74ecc-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="74ecc-137">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="74ecc-137">Request headers</span></span>

| <span data-ttu-id="74ecc-138">名前</span><span class="sxs-lookup"><span data-stu-id="74ecc-138">Name</span></span>          | <span data-ttu-id="74ecc-139">説明</span><span class="sxs-lookup"><span data-stu-id="74ecc-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="74ecc-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="74ecc-140">Authorization</span></span> | <span data-ttu-id="74ecc-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="74ecc-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="74ecc-143">応答</span><span class="sxs-lookup"><span data-stu-id="74ecc-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="74ecc-144">CSV</span><span class="sxs-lookup"><span data-stu-id="74ecc-144">CSV</span></span>

<span data-ttu-id="74ecc-145">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="74ecc-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="74ecc-146">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="74ecc-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="74ecc-147">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="74ecc-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="74ecc-148">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="74ecc-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="74ecc-149">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="74ecc-149">Report Refresh Date</span></span>
- <span data-ttu-id="74ecc-150">グループ表示名</span><span class="sxs-lookup"><span data-stu-id="74ecc-150">Group Display Name</span></span>
- <span data-ttu-id="74ecc-151">削除済み</span><span class="sxs-lookup"><span data-stu-id="74ecc-151">Is Deleted</span></span>
- <span data-ttu-id="74ecc-152">所有者のプリンシパル名</span><span class="sxs-lookup"><span data-stu-id="74ecc-152">Owner Principal Name</span></span>
- <span data-ttu-id="74ecc-153">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="74ecc-153">Last Activity Date</span></span>
- <span data-ttu-id="74ecc-154">グループの種類</span><span class="sxs-lookup"><span data-stu-id="74ecc-154">Group Type</span></span>
- <span data-ttu-id="74ecc-155">メンバー数</span><span class="sxs-lookup"><span data-stu-id="74ecc-155">Member Count</span></span>
- <span data-ttu-id="74ecc-156">外部メンバー数</span><span class="sxs-lookup"><span data-stu-id="74ecc-156">External Member Count</span></span>
- <span data-ttu-id="74ecc-157">Exchange の受信メール数</span><span class="sxs-lookup"><span data-stu-id="74ecc-157">Exchange Received Email Count</span></span>
- <span data-ttu-id="74ecc-158">SharePoint のアクティブなファイル数</span><span class="sxs-lookup"><span data-stu-id="74ecc-158">SharePoint Active File Count</span></span>
- <span data-ttu-id="74ecc-159">Yammer に投稿されたメッセージ数</span><span class="sxs-lookup"><span data-stu-id="74ecc-159">Yammer Posted Message Count</span></span>
- <span data-ttu-id="74ecc-160">Yammer の開封済みメッセージ数</span><span class="sxs-lookup"><span data-stu-id="74ecc-160">Yammer Read Message Count</span></span>
- <span data-ttu-id="74ecc-161">Yammer で「いいね!」されたメッセージ数</span><span class="sxs-lookup"><span data-stu-id="74ecc-161">Yammer Liked Message Count</span></span>
- <span data-ttu-id="74ecc-162">Exchange メールボックスのアイテム合計数</span><span class="sxs-lookup"><span data-stu-id="74ecc-162">Exchange Mailbox Total Item Count</span></span>
- <span data-ttu-id="74ecc-163">使用済み Exchange メールボックス ストレージ (バイト)</span><span class="sxs-lookup"><span data-stu-id="74ecc-163">Exchange Mailbox Storage Used (Byte)</span></span>
- <span data-ttu-id="74ecc-164">SharePoint の合計ファイル数</span><span class="sxs-lookup"><span data-stu-id="74ecc-164">SharePoint Total File Count</span></span>
- <span data-ttu-id="74ecc-165">SharePoint の使用済みサイト ストレージ (バイト)</span><span class="sxs-lookup"><span data-stu-id="74ecc-165">SharePoint Site Storage Used (Byte)</span></span>
- <span data-ttu-id="74ecc-166">レポート期間</span><span class="sxs-lookup"><span data-stu-id="74ecc-166">Report Period</span></span>

<span data-ttu-id="74ecc-167">次の列は、21Vianet が運用している Microsoft Graph 中国ではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="74ecc-167">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="74ecc-168">Yammer に投稿されたメッセージ数</span><span class="sxs-lookup"><span data-stu-id="74ecc-168">Yammer Posted Message Count</span></span>
- <span data-ttu-id="74ecc-169">Yammer の開封済みメッセージ数</span><span class="sxs-lookup"><span data-stu-id="74ecc-169">Yammer Read Message Count</span></span>
- <span data-ttu-id="74ecc-170">Yammer で「いいね!」されたメッセージ数</span><span class="sxs-lookup"><span data-stu-id="74ecc-170">Yammer Liked Message Count</span></span>

### <a name="json"></a><span data-ttu-id="74ecc-171">JSON</span><span class="sxs-lookup"><span data-stu-id="74ecc-171">JSON</span></span>

<span data-ttu-id="74ecc-172">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="74ecc-172">If successful, this method returns a `200 OK` response code and an **[office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** object in the response body.</span></span>

<span data-ttu-id="74ecc-173">**[Office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** オブジェクトの次のプロパティは、21vianet が運用している Microsoft Graph の中国ではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="74ecc-173">The following properties in **[office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="74ecc-174">yammerPostedMessageCount</span><span class="sxs-lookup"><span data-stu-id="74ecc-174">yammerPostedMessageCount</span></span>
- <span data-ttu-id="74ecc-175">yammerReadMessageCount</span><span class="sxs-lookup"><span data-stu-id="74ecc-175">yammerReadMessageCount</span></span>
- <span data-ttu-id="74ecc-176">yammerLikedMessageCount</span><span class="sxs-lookup"><span data-stu-id="74ecc-176">yammerLikedMessageCount</span></span>

<span data-ttu-id="74ecc-177">この要求の既定のページサイズは200アイテムです。</span><span class="sxs-lookup"><span data-stu-id="74ecc-177">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="74ecc-178">例</span><span class="sxs-lookup"><span data-stu-id="74ecc-178">Example</span></span>

### <a name="csv"></a><span data-ttu-id="74ecc-179">CSV</span><span class="sxs-lookup"><span data-stu-id="74ecc-179">CSV</span></span>

<span data-ttu-id="74ecc-180">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="74ecc-180">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="74ecc-181">要求</span><span class="sxs-lookup"><span data-stu-id="74ecc-181">Request</span></span>

<span data-ttu-id="74ecc-182">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="74ecc-182">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitydetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="74ecc-183">応答</span><span class="sxs-lookup"><span data-stu-id="74ecc-183">Response</span></span>

<span data-ttu-id="74ecc-184">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="74ecc-184">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="74ecc-185">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="74ecc-185">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="74ecc-186">Visual</span><span class="sxs-lookup"><span data-stu-id="74ecc-186">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365groupsactivitydetail_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="74ecc-187">Java</span><span class="sxs-lookup"><span data-stu-id="74ecc-187">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365groupsactivitydetail_csv-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="74ecc-188">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="74ecc-188">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Group Display Name,Is Deleted,Owner Principal Name,Last Activity Date,Group Type,Member Count,External Member Count,Exchange Received Email Count,SharePoint Active File Count,Yammer Posted Message Count,Yammer Read Message Count,Yammer Liked Message Count,Exchange Mailbox Total Item Count,Exchange Mailbox Storage Used (Byte),SharePoint Total File Count,SharePoint Site Storage Used (Byte),Report Period
```

### <a name="json"></a><span data-ttu-id="74ecc-189">JSON</span><span class="sxs-lookup"><span data-stu-id="74ecc-189">JSON</span></span>

<span data-ttu-id="74ecc-190">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="74ecc-190">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="74ecc-191">要求</span><span class="sxs-lookup"><span data-stu-id="74ecc-191">Request</span></span>

<span data-ttu-id="74ecc-192">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="74ecc-192">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitydetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="74ecc-193">応答</span><span class="sxs-lookup"><span data-stu-id="74ecc-193">Response</span></span>

<span data-ttu-id="74ecc-194">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="74ecc-194">The following is an example of the response.</span></span>

> <span data-ttu-id="74ecc-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="74ecc-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365GroupsActivityDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 674

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365GroupsActivityDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "groupDisplayName": "groupDisplayName-value", 
      "isDeleted": false, 
      "ownerPrincipalName": "ownerDisplayName-value", 
      "lastActivityDate": "2017-08-31", 
      "groupType": "Private", 
      "memberCount": 5, 
      "externalMemberCount": 0, 
      "exchangeReceivedEmailCount": 341, 
      "sharePointActiveFileCount": 0, 
      "yammerPostedMessageCount": 0, 
      "yammerReadMessageCount": 0, 
      "yammerLikedMessageCount": 0, 
      "exchangeMailboxTotalItemCount": 343, 
      "exchangeMailboxStorageUsedInBytes": 3724609, 
      "sharePointTotalFileCount": 0, 
      "sharePointSiteStorageUsedInBytes": 0, 
      "reportPeriod": "30"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="74ecc-197">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="74ecc-197">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="74ecc-198">Visual</span><span class="sxs-lookup"><span data-stu-id="74ecc-198">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365groupsactivitydetail_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="74ecc-199">Java</span><span class="sxs-lookup"><span data-stu-id="74ecc-199">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365groupsactivitydetail_json-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getoffice365groupsactivitydetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getoffice365groupsactivitydetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getoffice365groupsactivitydetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getoffice365groupsactivitydetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
