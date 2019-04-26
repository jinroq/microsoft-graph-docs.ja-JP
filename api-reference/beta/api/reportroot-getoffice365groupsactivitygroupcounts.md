---
title: 'reportRoot: getOffice365GroupsActivityGroupCounts'
description: グループの日次合計数と、そのうちのアクティブなグループの数を、電子メールでの会話、Yammer の投稿、SharePoint ファイルのアクティビティに基づいて取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 825a25f60b476e04477c8146530154167cc6a870
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33336691"
---
# <a name="reportroot-getoffice365groupsactivitygroupcounts"></a><span data-ttu-id="daebd-103">reportRoot: getOffice365GroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="daebd-103">reportRoot: getOffice365GroupsActivityGroupCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="daebd-104">グループの日次合計数と、そのうちのアクティブなグループの数を、電子メールでの会話、Yammer の投稿、SharePoint ファイルのアクティビティに基づいて取得します。</span><span class="sxs-lookup"><span data-stu-id="daebd-104">Get the daily total number of groups and how many of them were active based on email conversations, Yammer posts, and SharePoint file activities.</span></span>

> <span data-ttu-id="daebd-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Office 365 グループ](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="daebd-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="daebd-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="daebd-106">Permissions</span></span>

<span data-ttu-id="daebd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="daebd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="daebd-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="daebd-109">Permission type</span></span>                        | <span data-ttu-id="daebd-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="daebd-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="daebd-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="daebd-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="daebd-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="daebd-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="daebd-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="daebd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="daebd-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="daebd-114">Not supported.</span></span>                           |
| <span data-ttu-id="daebd-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="daebd-115">Application</span></span>                            | <span data-ttu-id="daebd-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="daebd-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="daebd-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="daebd-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityGroupCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="daebd-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="daebd-118">Function parameters</span></span>

<span data-ttu-id="daebd-119">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="daebd-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="daebd-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="daebd-120">Parameter</span></span> | <span data-ttu-id="daebd-121">型</span><span class="sxs-lookup"><span data-stu-id="daebd-121">Type</span></span>   | <span data-ttu-id="daebd-122">説明</span><span class="sxs-lookup"><span data-stu-id="daebd-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="daebd-123">period</span><span class="sxs-lookup"><span data-stu-id="daebd-123">period</span></span>    | <span data-ttu-id="daebd-124">文字列</span><span class="sxs-lookup"><span data-stu-id="daebd-124">string</span></span> | <span data-ttu-id="daebd-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="daebd-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="daebd-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="daebd-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="daebd-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="daebd-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="daebd-128">必須。</span><span class="sxs-lookup"><span data-stu-id="daebd-128">Required.</span></span> |

<span data-ttu-id="daebd-129">このメソッドは、 `$format`応答をカスタマイズするための[OData クエリパラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="daebd-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="daebd-130">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="daebd-130">The default output type is text/csv.</span></span> <span data-ttu-id="daebd-131">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="daebd-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="daebd-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="daebd-132">Request headers</span></span>

| <span data-ttu-id="daebd-133">名前</span><span class="sxs-lookup"><span data-stu-id="daebd-133">Name</span></span>          | <span data-ttu-id="daebd-134">説明</span><span class="sxs-lookup"><span data-stu-id="daebd-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="daebd-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="daebd-135">Authorization</span></span> | <span data-ttu-id="daebd-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="daebd-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="daebd-138">応答</span><span class="sxs-lookup"><span data-stu-id="daebd-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="daebd-139">CSV</span><span class="sxs-lookup"><span data-stu-id="daebd-139">CSV</span></span>

<span data-ttu-id="daebd-140">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="daebd-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="daebd-141">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="daebd-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="daebd-142">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="daebd-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="daebd-143">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="daebd-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="daebd-144">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="daebd-144">Report Refresh Date</span></span>
- <span data-ttu-id="daebd-145">合計</span><span class="sxs-lookup"><span data-stu-id="daebd-145">Total</span></span>
- <span data-ttu-id="daebd-146">アクティブ</span><span class="sxs-lookup"><span data-stu-id="daebd-146">Active</span></span>
- <span data-ttu-id="daebd-147">レポート日付</span><span class="sxs-lookup"><span data-stu-id="daebd-147">Report Date</span></span>
- <span data-ttu-id="daebd-148">レポート期間</span><span class="sxs-lookup"><span data-stu-id="daebd-148">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="daebd-149">JSON</span><span class="sxs-lookup"><span data-stu-id="daebd-149">JSON</span></span>

<span data-ttu-id="daebd-150">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[office365GroupsActivityGroupCounts](../resources/office365groupsactivitygroupcounts.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="daebd-150">If successful, this method returns a `200 OK` response code and an **[office365GroupsActivityGroupCounts](../resources/office365groupsactivitygroupcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="daebd-151">例</span><span class="sxs-lookup"><span data-stu-id="daebd-151">Example</span></span>

### <a name="csv"></a><span data-ttu-id="daebd-152">CSV</span><span class="sxs-lookup"><span data-stu-id="daebd-152">CSV</span></span>

<span data-ttu-id="daebd-153">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="daebd-153">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="daebd-154">要求</span><span class="sxs-lookup"><span data-stu-id="daebd-154">Request</span></span>

<span data-ttu-id="daebd-155">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="daebd-155">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitygroupcounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityGroupCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="daebd-156">応答</span><span class="sxs-lookup"><span data-stu-id="daebd-156">Response</span></span>

<span data-ttu-id="daebd-157">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="daebd-157">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="daebd-158">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="daebd-158">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Total,Active,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="daebd-159">JSON</span><span class="sxs-lookup"><span data-stu-id="daebd-159">JSON</span></span>

<span data-ttu-id="daebd-160">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="daebd-160">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="daebd-161">要求</span><span class="sxs-lookup"><span data-stu-id="daebd-161">Request</span></span>

<span data-ttu-id="daebd-162">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="daebd-162">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitygroupcounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityGroupCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="daebd-163">応答</span><span class="sxs-lookup"><span data-stu-id="daebd-163">Response</span></span>

<span data-ttu-id="daebd-164">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="daebd-164">The following is an example of the response.</span></span>

> <span data-ttu-id="daebd-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="daebd-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365GroupsActivityGroupCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 240

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365GroupsActivityGroupCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "total": 5344, 
      "active": 0, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
