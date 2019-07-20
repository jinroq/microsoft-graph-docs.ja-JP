---
title: 'reportRoot: getOffice365GroupsActivityDetail'
description: グループ別の Office 365 グループ アクティビティに関する詳細を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: b0435fd85e813942fd5e4a8b087e5a220a934fdd
ms.sourcegitcommit: 6fe086e6a9396a71a82179853547cb7b5e22d980
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/20/2019
ms.locfileid: "35805077"
---
# <a name="reportroot-getoffice365groupsactivitydetail"></a><span data-ttu-id="c70eb-103">reportRoot: getOffice365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="c70eb-103">reportRoot: getOffice365GroupsActivityDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c70eb-104">グループ別の Office 365 グループ アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="c70eb-104">Get details about Office 365 Groups activity by group.</span></span>

> <span data-ttu-id="c70eb-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Office 365 グループ](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c70eb-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="c70eb-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c70eb-106">Permissions</span></span>

<span data-ttu-id="c70eb-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c70eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c70eb-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c70eb-109">Permission type</span></span>                        | <span data-ttu-id="c70eb-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c70eb-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="c70eb-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="c70eb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c70eb-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c70eb-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="c70eb-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c70eb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c70eb-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c70eb-114">Not supported.</span></span>                           |
| <span data-ttu-id="c70eb-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c70eb-115">Application</span></span>                            | <span data-ttu-id="c70eb-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c70eb-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="c70eb-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c70eb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityDetail(period='{period_value}')
GET /reports/getOffice365GroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="c70eb-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="c70eb-118">Function parameters</span></span>

<span data-ttu-id="c70eb-119">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="c70eb-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="c70eb-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="c70eb-120">Parameter</span></span> | <span data-ttu-id="c70eb-121">型</span><span class="sxs-lookup"><span data-stu-id="c70eb-121">Type</span></span>   | <span data-ttu-id="c70eb-122">説明</span><span class="sxs-lookup"><span data-stu-id="c70eb-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="c70eb-123">period</span><span class="sxs-lookup"><span data-stu-id="c70eb-123">period</span></span>    | <span data-ttu-id="c70eb-124">文字列</span><span class="sxs-lookup"><span data-stu-id="c70eb-124">string</span></span> | <span data-ttu-id="c70eb-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="c70eb-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="c70eb-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="c70eb-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="c70eb-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="c70eb-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="c70eb-128">date</span><span class="sxs-lookup"><span data-stu-id="c70eb-128">date</span></span>      | <span data-ttu-id="c70eb-129">日付</span><span class="sxs-lookup"><span data-stu-id="c70eb-129">Date</span></span>   | <span data-ttu-id="c70eb-130">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="c70eb-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="c70eb-131">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="c70eb-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="c70eb-132">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="c70eb-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="c70eb-133">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c70eb-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="c70eb-134">このメソッドは、応答をカスタマイズするための `$format`、`$top`、`$skipToken` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c70eb-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="c70eb-135">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="c70eb-135">The default output type is text/csv.</span></span> <span data-ttu-id="c70eb-136">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="c70eb-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c70eb-137">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c70eb-137">Request headers</span></span>

| <span data-ttu-id="c70eb-138">名前</span><span class="sxs-lookup"><span data-stu-id="c70eb-138">Name</span></span>          | <span data-ttu-id="c70eb-139">説明</span><span class="sxs-lookup"><span data-stu-id="c70eb-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="c70eb-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="c70eb-140">Authorization</span></span> | <span data-ttu-id="c70eb-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c70eb-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="c70eb-143">応答</span><span class="sxs-lookup"><span data-stu-id="c70eb-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="c70eb-144">CSV</span><span class="sxs-lookup"><span data-stu-id="c70eb-144">CSV</span></span>

<span data-ttu-id="c70eb-145">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="c70eb-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="c70eb-146">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="c70eb-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="c70eb-147">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="c70eb-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="c70eb-148">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="c70eb-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="c70eb-149">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="c70eb-149">Report Refresh Date</span></span>
- <span data-ttu-id="c70eb-150">グループ表示名</span><span class="sxs-lookup"><span data-stu-id="c70eb-150">Group Display Name</span></span>
- <span data-ttu-id="c70eb-151">削除済み</span><span class="sxs-lookup"><span data-stu-id="c70eb-151">Is Deleted</span></span>
- <span data-ttu-id="c70eb-152">所有者のプリンシパル名</span><span class="sxs-lookup"><span data-stu-id="c70eb-152">Owner Principal Name</span></span>
- <span data-ttu-id="c70eb-153">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="c70eb-153">Last Activity Date</span></span>
- <span data-ttu-id="c70eb-154">グループの種類</span><span class="sxs-lookup"><span data-stu-id="c70eb-154">Group Type</span></span>
- <span data-ttu-id="c70eb-155">メンバー数</span><span class="sxs-lookup"><span data-stu-id="c70eb-155">Member Count</span></span>
- <span data-ttu-id="c70eb-156">外部メンバー数</span><span class="sxs-lookup"><span data-stu-id="c70eb-156">External Member Count</span></span>
- <span data-ttu-id="c70eb-157">Exchange の受信メール数</span><span class="sxs-lookup"><span data-stu-id="c70eb-157">Exchange Received Email Count</span></span>
- <span data-ttu-id="c70eb-158">SharePoint のアクティブなファイル数</span><span class="sxs-lookup"><span data-stu-id="c70eb-158">SharePoint Active File Count</span></span>
- <span data-ttu-id="c70eb-159">Yammer に投稿されたメッセージ数</span><span class="sxs-lookup"><span data-stu-id="c70eb-159">Yammer Posted Message Count</span></span>
- <span data-ttu-id="c70eb-160">Yammer の開封済みメッセージ数</span><span class="sxs-lookup"><span data-stu-id="c70eb-160">Yammer Read Message Count</span></span>
- <span data-ttu-id="c70eb-161">Yammer で「いいね!」されたメッセージ数</span><span class="sxs-lookup"><span data-stu-id="c70eb-161">Yammer Liked Message Count</span></span>
- <span data-ttu-id="c70eb-162">Exchange メールボックスのアイテム合計数</span><span class="sxs-lookup"><span data-stu-id="c70eb-162">Exchange Mailbox Total Item Count</span></span>
- <span data-ttu-id="c70eb-163">使用済み Exchange メールボックス ストレージ (バイト)</span><span class="sxs-lookup"><span data-stu-id="c70eb-163">Exchange Mailbox Storage Used (Byte)</span></span>
- <span data-ttu-id="c70eb-164">SharePoint の合計ファイル数</span><span class="sxs-lookup"><span data-stu-id="c70eb-164">SharePoint Total File Count</span></span>
- <span data-ttu-id="c70eb-165">SharePoint の使用済みサイト ストレージ (バイト)</span><span class="sxs-lookup"><span data-stu-id="c70eb-165">SharePoint Site Storage Used (Byte)</span></span>
- <span data-ttu-id="c70eb-166">グループ Id</span><span class="sxs-lookup"><span data-stu-id="c70eb-166">Group Id</span></span>
- <span data-ttu-id="c70eb-167">レポート期間</span><span class="sxs-lookup"><span data-stu-id="c70eb-167">Report Period</span></span>

<span data-ttu-id="c70eb-168">次の列は、21Vianet が運用している Microsoft Graph 中国ではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c70eb-168">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="c70eb-169">Yammer に投稿されたメッセージ数</span><span class="sxs-lookup"><span data-stu-id="c70eb-169">Yammer Posted Message Count</span></span>
- <span data-ttu-id="c70eb-170">Yammer の開封済みメッセージ数</span><span class="sxs-lookup"><span data-stu-id="c70eb-170">Yammer Read Message Count</span></span>
- <span data-ttu-id="c70eb-171">Yammer で「いいね!」されたメッセージ数</span><span class="sxs-lookup"><span data-stu-id="c70eb-171">Yammer Liked Message Count</span></span>

### <a name="json"></a><span data-ttu-id="c70eb-172">JSON</span><span class="sxs-lookup"><span data-stu-id="c70eb-172">JSON</span></span>

<span data-ttu-id="c70eb-173">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c70eb-173">If successful, this method returns a `200 OK` response code and an **[office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** object in the response body.</span></span>

<span data-ttu-id="c70eb-174">**[Office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** オブジェクトの次のプロパティは、21vianet が運用している Microsoft Graph の中国ではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c70eb-174">The following properties in **[office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="c70eb-175">yammerPostedMessageCount</span><span class="sxs-lookup"><span data-stu-id="c70eb-175">yammerPostedMessageCount</span></span>
- <span data-ttu-id="c70eb-176">yammerReadMessageCount</span><span class="sxs-lookup"><span data-stu-id="c70eb-176">yammerReadMessageCount</span></span>
- <span data-ttu-id="c70eb-177">yammerLikedMessageCount</span><span class="sxs-lookup"><span data-stu-id="c70eb-177">yammerLikedMessageCount</span></span>

<span data-ttu-id="c70eb-178">この要求の既定のページサイズは200アイテムです。</span><span class="sxs-lookup"><span data-stu-id="c70eb-178">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="c70eb-179">例</span><span class="sxs-lookup"><span data-stu-id="c70eb-179">Example</span></span>

### <a name="csv"></a><span data-ttu-id="c70eb-180">CSV</span><span class="sxs-lookup"><span data-stu-id="c70eb-180">CSV</span></span>

<span data-ttu-id="c70eb-181">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c70eb-181">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="c70eb-182">要求</span><span class="sxs-lookup"><span data-stu-id="c70eb-182">Request</span></span>

<span data-ttu-id="c70eb-183">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c70eb-183">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c70eb-184">プロトコル</span><span class="sxs-lookup"><span data-stu-id="c70eb-184">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitydetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c70eb-185">C#</span><span class="sxs-lookup"><span data-stu-id="c70eb-185">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365groupsactivitydetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c70eb-186">Javascript</span><span class="sxs-lookup"><span data-stu-id="c70eb-186">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365groupsactivitydetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c70eb-187">目的-C</span><span class="sxs-lookup"><span data-stu-id="c70eb-187">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365groupsactivitydetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c70eb-188">応答</span><span class="sxs-lookup"><span data-stu-id="c70eb-188">Response</span></span>

<span data-ttu-id="c70eb-189">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c70eb-189">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="c70eb-190">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="c70eb-190">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Group Display Name,Is Deleted,Owner Principal Name,Last Activity Date,Group Type,Member Count,External Member Count,Exchange Received Email Count,SharePoint Active File Count,Yammer Posted Message Count,Yammer Read Message Count,Yammer Liked Message Count,Exchange Mailbox Total Item Count,Exchange Mailbox Storage Used (Byte),SharePoint Total File Count,SharePoint Site Storage Used (Byte),Group Id,Report Period
```

### <a name="json"></a><span data-ttu-id="c70eb-191">JSON</span><span class="sxs-lookup"><span data-stu-id="c70eb-191">JSON</span></span>

<span data-ttu-id="c70eb-192">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="c70eb-192">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="c70eb-193">要求</span><span class="sxs-lookup"><span data-stu-id="c70eb-193">Request</span></span>

<span data-ttu-id="c70eb-194">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c70eb-194">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c70eb-195">プロトコル</span><span class="sxs-lookup"><span data-stu-id="c70eb-195">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitydetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c70eb-196">C#</span><span class="sxs-lookup"><span data-stu-id="c70eb-196">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365groupsactivitydetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c70eb-197">Javascript</span><span class="sxs-lookup"><span data-stu-id="c70eb-197">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365groupsactivitydetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c70eb-198">目的-C</span><span class="sxs-lookup"><span data-stu-id="c70eb-198">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365groupsactivitydetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c70eb-199">応答</span><span class="sxs-lookup"><span data-stu-id="c70eb-199">Response</span></span>

<span data-ttu-id="c70eb-200">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c70eb-200">The following is an example of the response.</span></span>

> <span data-ttu-id="c70eb-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="c70eb-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "groupId": "0003cf63-7ff3-4471-b24b-50ffbfb8b5d2",
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
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
