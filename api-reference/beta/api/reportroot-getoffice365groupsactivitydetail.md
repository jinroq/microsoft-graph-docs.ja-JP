---
title: 'reportRoot: getOffice365GroupsActivityDetail'
description: グループ別の Office 365 グループ アクティビティに関する詳細を取得します。
localization_priority: Normal
ms.openlocfilehash: 02def0c4c2c54a6379ca5770f36d1f7fe5cfa925
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871681"
---
# <a name="reportroot-getoffice365groupsactivitydetail"></a><span data-ttu-id="e77da-103">reportRoot: getOffice365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="e77da-103">reportRoot: getOffice365GroupsActivityDetail</span></span>

> <span data-ttu-id="e77da-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e77da-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e77da-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e77da-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e77da-106">グループ別の Office 365 グループ アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="e77da-106">Get details about Office 365 Groups activity by group.</span></span>

> <span data-ttu-id="e77da-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Office 365 グループ](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e77da-107">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="e77da-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e77da-108">Permissions</span></span>

<span data-ttu-id="e77da-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e77da-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e77da-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e77da-111">Permission type</span></span>                        | <span data-ttu-id="e77da-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e77da-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e77da-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="e77da-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="e77da-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e77da-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e77da-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e77da-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e77da-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e77da-116">Not supported.</span></span>                           |
| <span data-ttu-id="e77da-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e77da-117">Application</span></span>                            | <span data-ttu-id="e77da-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e77da-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="e77da-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e77da-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityDetail(period='{period_value}')
GET /reports/getOffice365GroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="e77da-120">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="e77da-120">Function parameters</span></span>

<span data-ttu-id="e77da-121">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="e77da-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="e77da-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="e77da-122">Parameter</span></span> | <span data-ttu-id="e77da-123">Type</span><span class="sxs-lookup"><span data-stu-id="e77da-123">Type</span></span>   | <span data-ttu-id="e77da-124">説明</span><span class="sxs-lookup"><span data-stu-id="e77da-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="e77da-125">period</span><span class="sxs-lookup"><span data-stu-id="e77da-125">period</span></span>    | <span data-ttu-id="e77da-126">文字列</span><span class="sxs-lookup"><span data-stu-id="e77da-126">string</span></span> | <span data-ttu-id="e77da-127">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="e77da-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="e77da-128">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="e77da-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="e77da-129">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="e77da-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="e77da-130">date</span><span class="sxs-lookup"><span data-stu-id="e77da-130">date</span></span>      | <span data-ttu-id="e77da-131">日付</span><span class="sxs-lookup"><span data-stu-id="e77da-131">Date</span></span>   | <span data-ttu-id="e77da-132">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="e77da-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="e77da-133">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="e77da-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="e77da-134">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="e77da-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="e77da-135">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e77da-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="e77da-136">このメソッドは、応答をカスタマイズするための `$format`、`$top`、`$skipToken` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e77da-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="e77da-137">既定の出力の種類は、テキストまたは csv です。</span><span class="sxs-lookup"><span data-stu-id="e77da-137">The default output type is text/csv.</span></span> <span data-ttu-id="e77da-138">ただし、出力の種類を指定する場合は、設定をテキストまたは csv またはアプリケーションまたは json OData $format クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="e77da-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e77da-139">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e77da-139">Request headers</span></span>

| <span data-ttu-id="e77da-140">名前</span><span class="sxs-lookup"><span data-stu-id="e77da-140">Name</span></span>          | <span data-ttu-id="e77da-141">説明</span><span class="sxs-lookup"><span data-stu-id="e77da-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="e77da-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="e77da-142">Authorization</span></span> | <span data-ttu-id="e77da-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e77da-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="e77da-145">応答</span><span class="sxs-lookup"><span data-stu-id="e77da-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="e77da-146">CSV</span><span class="sxs-lookup"><span data-stu-id="e77da-146">CSV</span></span>

<span data-ttu-id="e77da-147">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="e77da-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e77da-148">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="e77da-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e77da-149">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="e77da-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e77da-150">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="e77da-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="e77da-151">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="e77da-151">Report Refresh Date</span></span>
- <span data-ttu-id="e77da-152">グループ表示名</span><span class="sxs-lookup"><span data-stu-id="e77da-152">Group Display Name</span></span>
- <span data-ttu-id="e77da-153">削除済み</span><span class="sxs-lookup"><span data-stu-id="e77da-153">Is Deleted</span></span>
- <span data-ttu-id="e77da-154">所有者のプリンシパル名</span><span class="sxs-lookup"><span data-stu-id="e77da-154">Owner Principal Name</span></span>
- <span data-ttu-id="e77da-155">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="e77da-155">Last Activity Date</span></span>
- <span data-ttu-id="e77da-156">グループの種類</span><span class="sxs-lookup"><span data-stu-id="e77da-156">Group Type</span></span>
- <span data-ttu-id="e77da-157">メンバー数</span><span class="sxs-lookup"><span data-stu-id="e77da-157">Member Count</span></span>
- <span data-ttu-id="e77da-158">外部メンバー数</span><span class="sxs-lookup"><span data-stu-id="e77da-158">External Member Count</span></span>
- <span data-ttu-id="e77da-159">Exchange の受信メール数</span><span class="sxs-lookup"><span data-stu-id="e77da-159">Exchange Received Email Count</span></span>
- <span data-ttu-id="e77da-160">SharePoint のアクティブなファイル数</span><span class="sxs-lookup"><span data-stu-id="e77da-160">SharePoint Active File Count</span></span>
- <span data-ttu-id="e77da-161">Yammer に投稿されたメッセージ数</span><span class="sxs-lookup"><span data-stu-id="e77da-161">Yammer Posted Message Count</span></span>
- <span data-ttu-id="e77da-162">Yammer の開封済みメッセージ数</span><span class="sxs-lookup"><span data-stu-id="e77da-162">Yammer Read Message Count</span></span>
- <span data-ttu-id="e77da-163">Yammer で「いいね!」されたメッセージ数</span><span class="sxs-lookup"><span data-stu-id="e77da-163">Yammer Liked Message Count</span></span>
- <span data-ttu-id="e77da-164">Exchange メールボックスのアイテム合計数</span><span class="sxs-lookup"><span data-stu-id="e77da-164">Exchange Mailbox Total Item Count</span></span>
- <span data-ttu-id="e77da-165">使用済み Exchange メールボックス ストレージ (バイト)</span><span class="sxs-lookup"><span data-stu-id="e77da-165">Exchange Mailbox Storage Used (Byte)</span></span>
- <span data-ttu-id="e77da-166">SharePoint の合計ファイル数</span><span class="sxs-lookup"><span data-stu-id="e77da-166">SharePoint Total File Count</span></span>
- <span data-ttu-id="e77da-167">SharePoint の使用済みサイト ストレージ (バイト)</span><span class="sxs-lookup"><span data-stu-id="e77da-167">SharePoint Site Storage Used (Byte)</span></span>
- <span data-ttu-id="e77da-168">レポート期間</span><span class="sxs-lookup"><span data-stu-id="e77da-168">Report Period</span></span>

<span data-ttu-id="e77da-169">21Vianet によって運営されて、Microsoft Graph 中国では、次の列はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e77da-169">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="e77da-170">Yammer に投稿されたメッセージ数</span><span class="sxs-lookup"><span data-stu-id="e77da-170">Yammer Posted Message Count</span></span>
- <span data-ttu-id="e77da-171">Yammer の開封済みメッセージ数</span><span class="sxs-lookup"><span data-stu-id="e77da-171">Yammer Read Message Count</span></span>
- <span data-ttu-id="e77da-172">Yammer で「いいね!」されたメッセージ数</span><span class="sxs-lookup"><span data-stu-id="e77da-172">Yammer Liked Message Count</span></span>

### <a name="json"></a><span data-ttu-id="e77da-173">JSON</span><span class="sxs-lookup"><span data-stu-id="e77da-173">JSON</span></span>

<span data-ttu-id="e77da-174">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の**[office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="e77da-174">If successful, this method returns a `200 OK` response code and an **[office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** object in the response body.</span></span>

<span data-ttu-id="e77da-175">21Vianet によって運営されて、Microsoft Graph 中国では、 **[office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** オブジェクトでは、次のプロパティはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e77da-175">The following properties in **[office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="e77da-176">yammerPostedMessageCount</span><span class="sxs-lookup"><span data-stu-id="e77da-176">yammerPostedMessageCount</span></span>
- <span data-ttu-id="e77da-177">yammerReadMessageCount</span><span class="sxs-lookup"><span data-stu-id="e77da-177">yammerReadMessageCount</span></span>
- <span data-ttu-id="e77da-178">yammerLikedMessageCount</span><span class="sxs-lookup"><span data-stu-id="e77da-178">yammerLikedMessageCount</span></span>

<span data-ttu-id="e77da-179">この要求の既定のページ サイズは、アイテムは 200 個です。</span><span class="sxs-lookup"><span data-stu-id="e77da-179">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="e77da-180">例</span><span class="sxs-lookup"><span data-stu-id="e77da-180">Example</span></span>

### <a name="csv"></a><span data-ttu-id="e77da-181">CSV</span><span class="sxs-lookup"><span data-stu-id="e77da-181">CSV</span></span>

<span data-ttu-id="e77da-182">次に、CSV を出力する例を示します。</span><span class="sxs-lookup"><span data-stu-id="e77da-182">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="e77da-183">要求</span><span class="sxs-lookup"><span data-stu-id="e77da-183">Request</span></span>

<span data-ttu-id="e77da-184">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e77da-184">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitydetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="e77da-185">応答</span><span class="sxs-lookup"><span data-stu-id="e77da-185">Response</span></span>

<span data-ttu-id="e77da-186">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e77da-186">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="e77da-187">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="e77da-187">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="e77da-188">JSON</span><span class="sxs-lookup"><span data-stu-id="e77da-188">JSON</span></span>

<span data-ttu-id="e77da-189">次に、JSON を取得する例を示します。</span><span class="sxs-lookup"><span data-stu-id="e77da-189">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="e77da-190">要求</span><span class="sxs-lookup"><span data-stu-id="e77da-190">Request</span></span>

<span data-ttu-id="e77da-191">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e77da-191">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitydetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="e77da-192">応答</span><span class="sxs-lookup"><span data-stu-id="e77da-192">Response</span></span>

<span data-ttu-id="e77da-193">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e77da-193">The following is an example of the response.</span></span>

> <span data-ttu-id="e77da-p108">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="e77da-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
