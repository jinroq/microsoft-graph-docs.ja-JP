---
title: 'reportRoot: getOffice365GroupsActivityDetail'
description: グループ別の Office 365 グループ アクティビティに関する詳細を取得します。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: c70f8ccdb2d27c96a652c0db4d16ee0ca70ec132
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983591"
---
# <a name="reportroot-getoffice365groupsactivitydetail"></a><span data-ttu-id="d047d-103">reportRoot: getOffice365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="d047d-103">reportRoot: getOffice365GroupsActivityDetail</span></span>

> <span data-ttu-id="d047d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d047d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d047d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d047d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d047d-106">グループ別の Office 365 グループ アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="d047d-106">Get details about Office 365 Groups activity by group.</span></span>

> <span data-ttu-id="d047d-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Office 365 グループ](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d047d-107">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="d047d-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d047d-108">Permissions</span></span>

<span data-ttu-id="d047d-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d047d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d047d-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d047d-111">Permission type</span></span>                        | <span data-ttu-id="d047d-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d047d-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="d047d-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="d047d-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="d047d-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d047d-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="d047d-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d047d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d047d-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d047d-116">Not supported.</span></span>                           |
| <span data-ttu-id="d047d-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d047d-117">Application</span></span>                            | <span data-ttu-id="d047d-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d047d-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="d047d-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d047d-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityDetail(period='{period_value}')
GET /reports/getOffice365GroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="d047d-120">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="d047d-120">Function parameters</span></span>

<span data-ttu-id="d047d-121">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="d047d-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="d047d-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="d047d-122">Parameter</span></span> | <span data-ttu-id="d047d-123">型</span><span class="sxs-lookup"><span data-stu-id="d047d-123">Type</span></span>   | <span data-ttu-id="d047d-124">説明</span><span class="sxs-lookup"><span data-stu-id="d047d-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="d047d-125">period</span><span class="sxs-lookup"><span data-stu-id="d047d-125">period</span></span>    | <span data-ttu-id="d047d-126">文字列</span><span class="sxs-lookup"><span data-stu-id="d047d-126">string</span></span> | <span data-ttu-id="d047d-127">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="d047d-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="d047d-128">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="d047d-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="d047d-129">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="d047d-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="d047d-130">date</span><span class="sxs-lookup"><span data-stu-id="d047d-130">date</span></span>      | <span data-ttu-id="d047d-131">日付</span><span class="sxs-lookup"><span data-stu-id="d047d-131">Date</span></span>   | <span data-ttu-id="d047d-132">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="d047d-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="d047d-133">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="d047d-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="d047d-134">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="d047d-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="d047d-135">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d047d-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="d047d-136">このメソッドは、応答をカスタマイズするための `$format`、`$top`、`$skipToken` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d047d-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="d047d-137">既定の出力の種類は、テキストまたは csv です。</span><span class="sxs-lookup"><span data-stu-id="d047d-137">The default output type is text/csv.</span></span> <span data-ttu-id="d047d-138">ただし、出力の種類を指定する場合は、設定をテキストまたは csv またはアプリケーションまたは json OData $format クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="d047d-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d047d-139">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d047d-139">Request headers</span></span>

| <span data-ttu-id="d047d-140">名前</span><span class="sxs-lookup"><span data-stu-id="d047d-140">Name</span></span>          | <span data-ttu-id="d047d-141">説明</span><span class="sxs-lookup"><span data-stu-id="d047d-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="d047d-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="d047d-142">Authorization</span></span> | <span data-ttu-id="d047d-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d047d-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="d047d-145">応答</span><span class="sxs-lookup"><span data-stu-id="d047d-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="d047d-146">CSV</span><span class="sxs-lookup"><span data-stu-id="d047d-146">CSV</span></span>

<span data-ttu-id="d047d-147">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="d047d-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="d047d-148">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="d047d-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="d047d-149">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="d047d-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="d047d-150">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="d047d-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="d047d-151">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="d047d-151">Report Refresh Date</span></span>
- <span data-ttu-id="d047d-152">グループ表示名</span><span class="sxs-lookup"><span data-stu-id="d047d-152">Group Display Name</span></span>
- <span data-ttu-id="d047d-153">削除済み</span><span class="sxs-lookup"><span data-stu-id="d047d-153">Is Deleted</span></span>
- <span data-ttu-id="d047d-154">所有者のプリンシパル名</span><span class="sxs-lookup"><span data-stu-id="d047d-154">Owner Principal Name</span></span>
- <span data-ttu-id="d047d-155">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="d047d-155">Last Activity Date</span></span>
- <span data-ttu-id="d047d-156">グループの種類</span><span class="sxs-lookup"><span data-stu-id="d047d-156">Group Type</span></span>
- <span data-ttu-id="d047d-157">メンバー数</span><span class="sxs-lookup"><span data-stu-id="d047d-157">Member Count</span></span>
- <span data-ttu-id="d047d-158">外部メンバー数</span><span class="sxs-lookup"><span data-stu-id="d047d-158">External Member Count</span></span>
- <span data-ttu-id="d047d-159">Exchange の受信メール数</span><span class="sxs-lookup"><span data-stu-id="d047d-159">Exchange Received Email Count</span></span>
- <span data-ttu-id="d047d-160">SharePoint のアクティブなファイル数</span><span class="sxs-lookup"><span data-stu-id="d047d-160">SharePoint Active File Count</span></span>
- <span data-ttu-id="d047d-161">Yammer に投稿されたメッセージ数</span><span class="sxs-lookup"><span data-stu-id="d047d-161">Yammer Posted Message Count</span></span>
- <span data-ttu-id="d047d-162">Yammer の開封済みメッセージ数</span><span class="sxs-lookup"><span data-stu-id="d047d-162">Yammer Read Message Count</span></span>
- <span data-ttu-id="d047d-163">Yammer で「いいね!」されたメッセージ数</span><span class="sxs-lookup"><span data-stu-id="d047d-163">Yammer Liked Message Count</span></span>
- <span data-ttu-id="d047d-164">Exchange メールボックスのアイテム合計数</span><span class="sxs-lookup"><span data-stu-id="d047d-164">Exchange Mailbox Total Item Count</span></span>
- <span data-ttu-id="d047d-165">使用済み Exchange メールボックス ストレージ (バイト)</span><span class="sxs-lookup"><span data-stu-id="d047d-165">Exchange Mailbox Storage Used (Byte)</span></span>
- <span data-ttu-id="d047d-166">SharePoint の合計ファイル数</span><span class="sxs-lookup"><span data-stu-id="d047d-166">SharePoint Total File Count</span></span>
- <span data-ttu-id="d047d-167">SharePoint の使用済みサイト ストレージ (バイト)</span><span class="sxs-lookup"><span data-stu-id="d047d-167">SharePoint Site Storage Used (Byte)</span></span>
- <span data-ttu-id="d047d-168">レポート期間</span><span class="sxs-lookup"><span data-stu-id="d047d-168">Report Period</span></span>

<span data-ttu-id="d047d-169">21Vianet によって運営されて、Microsoft Graph 中国では、次の列はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d047d-169">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="d047d-170">Yammer に投稿されたメッセージ数</span><span class="sxs-lookup"><span data-stu-id="d047d-170">Yammer Posted Message Count</span></span>
- <span data-ttu-id="d047d-171">Yammer の開封済みメッセージ数</span><span class="sxs-lookup"><span data-stu-id="d047d-171">Yammer Read Message Count</span></span>
- <span data-ttu-id="d047d-172">Yammer で「いいね!」されたメッセージ数</span><span class="sxs-lookup"><span data-stu-id="d047d-172">Yammer Liked Message Count</span></span>

### <a name="json"></a><span data-ttu-id="d047d-173">JSON</span><span class="sxs-lookup"><span data-stu-id="d047d-173">JSON</span></span>

<span data-ttu-id="d047d-174">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の**[office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="d047d-174">If successful, this method returns a `200 OK` response code and an **[office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** object in the response body.</span></span>

<span data-ttu-id="d047d-175">21Vianet によって運営されて、Microsoft Graph 中国では、 **[office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** オブジェクトでは、次のプロパティはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d047d-175">The following properties in **[office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="d047d-176">yammerPostedMessageCount</span><span class="sxs-lookup"><span data-stu-id="d047d-176">yammerPostedMessageCount</span></span>
- <span data-ttu-id="d047d-177">yammerReadMessageCount</span><span class="sxs-lookup"><span data-stu-id="d047d-177">yammerReadMessageCount</span></span>
- <span data-ttu-id="d047d-178">yammerLikedMessageCount</span><span class="sxs-lookup"><span data-stu-id="d047d-178">yammerLikedMessageCount</span></span>

<span data-ttu-id="d047d-179">この要求の既定のページ サイズは、アイテムは 200 個です。</span><span class="sxs-lookup"><span data-stu-id="d047d-179">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="d047d-180">例</span><span class="sxs-lookup"><span data-stu-id="d047d-180">Example</span></span>

### <a name="csv"></a><span data-ttu-id="d047d-181">CSV</span><span class="sxs-lookup"><span data-stu-id="d047d-181">CSV</span></span>

<span data-ttu-id="d047d-182">次に、CSV を出力する例を示します。</span><span class="sxs-lookup"><span data-stu-id="d047d-182">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="d047d-183">要求</span><span class="sxs-lookup"><span data-stu-id="d047d-183">Request</span></span>

<span data-ttu-id="d047d-184">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d047d-184">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitydetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="d047d-185">応答</span><span class="sxs-lookup"><span data-stu-id="d047d-185">Response</span></span>

<span data-ttu-id="d047d-186">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d047d-186">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="d047d-187">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="d047d-187">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="d047d-188">JSON</span><span class="sxs-lookup"><span data-stu-id="d047d-188">JSON</span></span>

<span data-ttu-id="d047d-189">次に、JSON を取得する例を示します。</span><span class="sxs-lookup"><span data-stu-id="d047d-189">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="d047d-190">要求</span><span class="sxs-lookup"><span data-stu-id="d047d-190">Request</span></span>

<span data-ttu-id="d047d-191">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d047d-191">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitydetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="d047d-192">応答</span><span class="sxs-lookup"><span data-stu-id="d047d-192">Response</span></span>

<span data-ttu-id="d047d-193">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d047d-193">The following is an example of the response.</span></span>

> <span data-ttu-id="d047d-p108">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="d047d-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
