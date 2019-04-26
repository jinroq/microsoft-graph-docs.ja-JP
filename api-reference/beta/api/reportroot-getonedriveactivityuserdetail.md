---
title: 'reportRoot: getOneDriveActivityUserDetail'
description: ユーザー別の OneDrive アクティビティに関する詳細を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 485b825eabe7723529c7e013d161b4a63ed7786c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33336597"
---
# <a name="reportroot-getonedriveactivityuserdetail"></a><span data-ttu-id="59516-103">reportRoot: getOneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="59516-103">reportRoot: getOneDriveActivityUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59516-104">ユーザー別の OneDrive アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="59516-104">Get details about OneDrive activity by user.</span></span>

> <span data-ttu-id="59516-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: OneDrive for Business のアクティビティ](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="59516-105">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="permissions"></a><span data-ttu-id="59516-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="59516-106">Permissions</span></span>

<span data-ttu-id="59516-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="59516-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="59516-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="59516-109">Permission type</span></span>                        | <span data-ttu-id="59516-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="59516-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="59516-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="59516-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="59516-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="59516-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="59516-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="59516-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59516-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="59516-114">Not supported.</span></span>                           |
| <span data-ttu-id="59516-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="59516-115">Application</span></span>                            | <span data-ttu-id="59516-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="59516-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="59516-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="59516-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveActivityUserDetail(period='{period_value}')
GET /reports/getOneDriveActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="59516-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="59516-118">Function parameters</span></span>

<span data-ttu-id="59516-119">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="59516-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="59516-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="59516-120">Parameter</span></span> | <span data-ttu-id="59516-121">型</span><span class="sxs-lookup"><span data-stu-id="59516-121">Type</span></span>   | <span data-ttu-id="59516-122">説明</span><span class="sxs-lookup"><span data-stu-id="59516-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="59516-123">period</span><span class="sxs-lookup"><span data-stu-id="59516-123">period</span></span>    | <span data-ttu-id="59516-124">文字列</span><span class="sxs-lookup"><span data-stu-id="59516-124">string</span></span> | <span data-ttu-id="59516-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="59516-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="59516-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="59516-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="59516-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="59516-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="59516-128">date</span><span class="sxs-lookup"><span data-stu-id="59516-128">date</span></span>      | <span data-ttu-id="59516-129">日付</span><span class="sxs-lookup"><span data-stu-id="59516-129">Date</span></span>   | <span data-ttu-id="59516-130">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="59516-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="59516-131">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="59516-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="59516-132">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="59516-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="59516-133">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="59516-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="59516-134">このメソッドは、応答をカスタマイズするための `$format`、`$top`、`$skipToken` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="59516-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="59516-135">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="59516-135">The default output type is text/csv.</span></span> <span data-ttu-id="59516-136">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="59516-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="59516-137">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="59516-137">Request headers</span></span>

| <span data-ttu-id="59516-138">名前</span><span class="sxs-lookup"><span data-stu-id="59516-138">Name</span></span>          | <span data-ttu-id="59516-139">説明</span><span class="sxs-lookup"><span data-stu-id="59516-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="59516-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="59516-140">Authorization</span></span> | <span data-ttu-id="59516-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="59516-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="59516-143">応答</span><span class="sxs-lookup"><span data-stu-id="59516-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="59516-144">CSV</span><span class="sxs-lookup"><span data-stu-id="59516-144">CSV</span></span>

<span data-ttu-id="59516-145">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="59516-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="59516-146">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="59516-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="59516-147">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="59516-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="59516-148">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="59516-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="59516-149">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="59516-149">Report Refresh Date</span></span>
- <span data-ttu-id="59516-150">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="59516-150">User Principal Name</span></span>
- <span data-ttu-id="59516-151">削除済み</span><span class="sxs-lookup"><span data-stu-id="59516-151">Is Deleted</span></span>
- <span data-ttu-id="59516-152">削除日</span><span class="sxs-lookup"><span data-stu-id="59516-152">Deleted Date</span></span>
- <span data-ttu-id="59516-153">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="59516-153">Last Activity Date</span></span>
- <span data-ttu-id="59516-154">表示済みまたは編集済みファイルの数</span><span class="sxs-lookup"><span data-stu-id="59516-154">Viewed Or Edited File Count</span></span>
- <span data-ttu-id="59516-155">同期済みファイルの数</span><span class="sxs-lookup"><span data-stu-id="59516-155">Synced File Count</span></span>
- <span data-ttu-id="59516-156">社内で共有済みファイルの数</span><span class="sxs-lookup"><span data-stu-id="59516-156">Shared Internally File Count</span></span>
- <span data-ttu-id="59516-157">外部で共有済みファイルの数</span><span class="sxs-lookup"><span data-stu-id="59516-157">Shared Externally File Count</span></span>
- <span data-ttu-id="59516-158">割り当て済み製品</span><span class="sxs-lookup"><span data-stu-id="59516-158">Assigned Products</span></span>
- <span data-ttu-id="59516-159">レポート期間</span><span class="sxs-lookup"><span data-stu-id="59516-159">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="59516-160">JSON</span><span class="sxs-lookup"><span data-stu-id="59516-160">JSON</span></span>

<span data-ttu-id="59516-161">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[onedrive activityuserdetail](../resources/onedriveactivityuserdetail.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="59516-161">If successful, this method returns a `200 OK` response code and a **[oneDriveActivityUserDetail](../resources/onedriveactivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="59516-162">この要求の既定のページサイズは200アイテムです。</span><span class="sxs-lookup"><span data-stu-id="59516-162">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="59516-163">例</span><span class="sxs-lookup"><span data-stu-id="59516-163">Example</span></span>

### <a name="csv"></a><span data-ttu-id="59516-164">CSV</span><span class="sxs-lookup"><span data-stu-id="59516-164">CSV</span></span>

<span data-ttu-id="59516-165">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="59516-165">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="59516-166">要求</span><span class="sxs-lookup"><span data-stu-id="59516-166">Request</span></span>

<span data-ttu-id="59516-167">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="59516-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveactivityuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveActivityUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="59516-168">応答</span><span class="sxs-lookup"><span data-stu-id="59516-168">Response</span></span>

<span data-ttu-id="59516-169">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="59516-169">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="59516-170">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="59516-170">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Viewed Or Edited File Count,Synced File Count,Shared Internally File Count,Shared Externally File Count,Assigned Products,Report Period
```

### <a name="json"></a><span data-ttu-id="59516-171">JSON</span><span class="sxs-lookup"><span data-stu-id="59516-171">JSON</span></span>

<span data-ttu-id="59516-172">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="59516-172">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="59516-173">要求</span><span class="sxs-lookup"><span data-stu-id="59516-173">Request</span></span>

<span data-ttu-id="59516-174">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="59516-174">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveactivityuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveActivityUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="59516-175">応答</span><span class="sxs-lookup"><span data-stu-id="59516-175">Response</span></span>

<span data-ttu-id="59516-176">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="59516-176">The following is an example of the response.</span></span>

> <span data-ttu-id="59516-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="59516-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oneDriveActivityUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 450

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.oneDriveActivityUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "isDeleted": false, 
      "deletedDate": null, 
      "lastActivityDate": "2017-09-01", 
      "viewedOrEditedFileCount": 1, 
      "syncedFileCount": 0, 
      "sharedInternallyFileCount": 0, 
      "sharedExternallyFileCount": 0, 
      "assignedProducts": [
        "OFFICE 365 ENTERPRISE E5"
      ], 
      "reportPeriod": "7"
    }
  ]
}
```
