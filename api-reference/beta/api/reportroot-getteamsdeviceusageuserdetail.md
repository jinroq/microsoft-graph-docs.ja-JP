---
title: 'reportRoot: getTeamsDeviceUsageUserDetail'
description: ユーザーごとに、Microsoft Teams デバイスの使用状況の詳細を取得します。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 0e24a66905afa0ccb20c30fb4414e621cb4a1683
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522281"
---
# <a name="reportroot-getteamsdeviceusageuserdetail"></a><span data-ttu-id="d8eb6-103">reportRoot: getTeamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="d8eb6-103">reportRoot: getTeamsDeviceUsageUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8eb6-104">ユーザーごとに、Microsoft Teams デバイスの使用状況の詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="d8eb6-104">Get details about Microsoft Teams device usage by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="d8eb6-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d8eb6-105">Permissions</span></span>

<span data-ttu-id="d8eb6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d8eb6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d8eb6-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d8eb6-108">Permission type</span></span>                        | <span data-ttu-id="d8eb6-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d8eb6-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="d8eb6-110">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="d8eb6-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d8eb6-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d8eb6-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="d8eb6-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d8eb6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8eb6-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d8eb6-113">Not supported.</span></span>                           |
| <span data-ttu-id="d8eb6-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d8eb6-114">Application</span></span>                            | <span data-ttu-id="d8eb6-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d8eb6-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="d8eb6-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d8eb6-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageUserDetail(period='D7')
GET /reports/getTeamsDeviceUsageUserDetail(date=2017-09-01)
```

## <a name="function-parameters"></a><span data-ttu-id="d8eb6-117">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="d8eb6-117">Function parameters</span></span>

<span data-ttu-id="d8eb6-118">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="d8eb6-118">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="d8eb6-119">パラメーター</span><span class="sxs-lookup"><span data-stu-id="d8eb6-119">Parameter</span></span> | <span data-ttu-id="d8eb6-120">型</span><span class="sxs-lookup"><span data-stu-id="d8eb6-120">Type</span></span>   | <span data-ttu-id="d8eb6-121">説明</span><span class="sxs-lookup"><span data-stu-id="d8eb6-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="d8eb6-122">period</span><span class="sxs-lookup"><span data-stu-id="d8eb6-122">period</span></span>    | <span data-ttu-id="d8eb6-123">文字列</span><span class="sxs-lookup"><span data-stu-id="d8eb6-123">string</span></span> | <span data-ttu-id="d8eb6-124">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="d8eb6-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="d8eb6-125">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="d8eb6-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="d8eb6-126">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="d8eb6-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="d8eb6-127">date</span><span class="sxs-lookup"><span data-stu-id="d8eb6-127">date</span></span>      | <span data-ttu-id="d8eb6-128">日付</span><span class="sxs-lookup"><span data-stu-id="d8eb6-128">Date</span></span>   | <span data-ttu-id="d8eb6-129">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="d8eb6-129">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="d8eb6-130">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="d8eb6-130">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="d8eb6-131">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="d8eb6-131">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="d8eb6-132">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d8eb6-132">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="d8eb6-133">このメソッドは、応答をカスタマイズするための `$format`、`$top`、`$skipToken` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d8eb6-133">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="d8eb6-134">既定の出力の種類は、テキストまたは csv です。</span><span class="sxs-lookup"><span data-stu-id="d8eb6-134">The default output type is text/csv.</span></span> <span data-ttu-id="d8eb6-135">ただし、出力の種類を指定する場合は、設定をテキストまたは csv またはアプリケーションまたは json OData $format クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="d8eb6-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d8eb6-136">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d8eb6-136">Request headers</span></span>

| <span data-ttu-id="d8eb6-137">名前</span><span class="sxs-lookup"><span data-stu-id="d8eb6-137">Name</span></span>          | <span data-ttu-id="d8eb6-138">説明</span><span class="sxs-lookup"><span data-stu-id="d8eb6-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="d8eb6-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8eb6-139">Authorization</span></span> | <span data-ttu-id="d8eb6-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d8eb6-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="d8eb6-142">応答</span><span class="sxs-lookup"><span data-stu-id="d8eb6-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="d8eb6-143">CSV</span><span class="sxs-lookup"><span data-stu-id="d8eb6-143">CSV</span></span>

<span data-ttu-id="d8eb6-144">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="d8eb6-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="d8eb6-145">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="d8eb6-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="d8eb6-146">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="d8eb6-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="d8eb6-147">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="d8eb6-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="d8eb6-148">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="d8eb6-148">Report Refresh Date</span></span>
- <span data-ttu-id="d8eb6-149">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="d8eb6-149">User Principal Name</span></span>
- <span data-ttu-id="d8eb6-150">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="d8eb6-150">Last Activity Date</span></span>
- <span data-ttu-id="d8eb6-151">削除済み</span><span class="sxs-lookup"><span data-stu-id="d8eb6-151">Is Deleted</span></span>
- <span data-ttu-id="d8eb6-152">削除日</span><span class="sxs-lookup"><span data-stu-id="d8eb6-152">Deleted Date</span></span>
- <span data-ttu-id="d8eb6-153">Web の使用</span><span class="sxs-lookup"><span data-stu-id="d8eb6-153">Used Web</span></span>
- <span data-ttu-id="d8eb6-154">Windows スマートフォンの使用</span><span class="sxs-lookup"><span data-stu-id="d8eb6-154">Used Windows Phone</span></span>
- <span data-ttu-id="d8eb6-155">iOS の使用</span><span class="sxs-lookup"><span data-stu-id="d8eb6-155">Used iOS</span></span>
- <span data-ttu-id="d8eb6-156">Mac の使用</span><span class="sxs-lookup"><span data-stu-id="d8eb6-156">Used Mac</span></span>
- <span data-ttu-id="d8eb6-157">Android スマートフォンの使用</span><span class="sxs-lookup"><span data-stu-id="d8eb6-157">Used Android Phone</span></span>
- <span data-ttu-id="d8eb6-158">Windows の使用</span><span class="sxs-lookup"><span data-stu-id="d8eb6-158">Used Windows</span></span>
- <span data-ttu-id="d8eb6-159">レポート期間</span><span class="sxs-lookup"><span data-stu-id="d8eb6-159">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="d8eb6-160">JSON</span><span class="sxs-lookup"><span data-stu-id="d8eb6-160">JSON</span></span>

<span data-ttu-id="d8eb6-161">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に**[teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md)** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="d8eb6-161">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="d8eb6-162">この要求の既定のページ サイズは、2000 のアイテムです。</span><span class="sxs-lookup"><span data-stu-id="d8eb6-162">The default page size for this request is 2000 items.</span></span>

## <a name="example"></a><span data-ttu-id="d8eb6-163">例</span><span class="sxs-lookup"><span data-stu-id="d8eb6-163">Example</span></span>

### <a name="csv"></a><span data-ttu-id="d8eb6-164">CSV</span><span class="sxs-lookup"><span data-stu-id="d8eb6-164">CSV</span></span>

<span data-ttu-id="d8eb6-165">次に、CSV を出力する例を示します。</span><span class="sxs-lookup"><span data-stu-id="d8eb6-165">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="d8eb6-166">要求</span><span class="sxs-lookup"><span data-stu-id="d8eb6-166">Request</span></span>

<span data-ttu-id="d8eb6-167">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d8eb6-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="d8eb6-168">応答</span><span class="sxs-lookup"><span data-stu-id="d8eb6-168">Response</span></span>

<span data-ttu-id="d8eb6-169">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d8eb6-169">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="d8eb6-170">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="d8eb6-170">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Is Deleted,Deleted Date,Used Web,Used Windows Phone,Used iOS,Used Mac,Used Android Phone,Used Windows,Report Period
```

### <a name="json"></a><span data-ttu-id="d8eb6-171">JSON</span><span class="sxs-lookup"><span data-stu-id="d8eb6-171">JSON</span></span>

<span data-ttu-id="d8eb6-172">次に、JSON を取得する例を示します。</span><span class="sxs-lookup"><span data-stu-id="d8eb6-172">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="d8eb6-173">要求</span><span class="sxs-lookup"><span data-stu-id="d8eb6-173">Request</span></span>

<span data-ttu-id="d8eb6-174">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d8eb6-174">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="d8eb6-175">応答</span><span class="sxs-lookup"><span data-stu-id="d8eb6-175">Response</span></span>

<span data-ttu-id="d8eb6-176">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d8eb6-176">The following is an example of the response.</span></span>

> <span data-ttu-id="d8eb6-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="d8eb6-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 374

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsDeviceUsageUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "lastActivityDate": "2017-09-01", 
      "isDeleted": false, 
      "deletedDate": null, 
      "usedWeb": false, 
      "usedWindowsPhone": false, 
      "usediOS": true, 
      "usedMac": false, 
      "usedAndroidPhone": false, 
      "usedWindows": true, 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getteamsdeviceusageuserdetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
