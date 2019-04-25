---
title: 'reportRoot: getSharePointActivityUserCounts'
description: アクティブ ユーザーの数の傾向を取得します。 ユーザーが一定期間中にファイル アクティビティ (保存、同期、変更、共有) を実行するか、またはページにアクセスすると、そのユーザーはアクティブとみなされます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 15734e15cf13cbbc03fd136d51bbdf9f4ac13ba0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537938"
---
# <a name="reportroot-getsharepointactivityusercounts"></a><span data-ttu-id="11bf2-104">reportRoot: getSharePointActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="11bf2-104">reportRoot: getSharePointActivityUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11bf2-105">アクティブ ユーザーの数の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="11bf2-105">Get the trend in the number of active users.</span></span> <span data-ttu-id="11bf2-106">ユーザーが一定期間中にファイル アクティビティ (保存、同期、変更、共有) を実行するか、またはページにアクセスすると、そのユーザーはアクティブとみなされます。</span><span class="sxs-lookup"><span data-stu-id="11bf2-106">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span>

> <span data-ttu-id="11bf2-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: SharePoint アクティビティ](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="11bf2-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="11bf2-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="11bf2-108">Permissions</span></span>

<span data-ttu-id="11bf2-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="11bf2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="11bf2-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="11bf2-111">Permission type</span></span>                        | <span data-ttu-id="11bf2-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="11bf2-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="11bf2-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="11bf2-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="11bf2-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="11bf2-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="11bf2-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="11bf2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11bf2-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="11bf2-116">Not supported.</span></span>                           |
| <span data-ttu-id="11bf2-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="11bf2-117">Application</span></span>                            | <span data-ttu-id="11bf2-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="11bf2-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="11bf2-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="11bf2-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="11bf2-120">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="11bf2-120">Function parameters</span></span>

<span data-ttu-id="11bf2-121">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="11bf2-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="11bf2-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="11bf2-122">Parameter</span></span> | <span data-ttu-id="11bf2-123">型</span><span class="sxs-lookup"><span data-stu-id="11bf2-123">Type</span></span>   | <span data-ttu-id="11bf2-124">説明</span><span class="sxs-lookup"><span data-stu-id="11bf2-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="11bf2-125">period</span><span class="sxs-lookup"><span data-stu-id="11bf2-125">period</span></span>    | <span data-ttu-id="11bf2-126">文字列</span><span class="sxs-lookup"><span data-stu-id="11bf2-126">string</span></span> | <span data-ttu-id="11bf2-127">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="11bf2-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="11bf2-128">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="11bf2-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="11bf2-129">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="11bf2-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="11bf2-130">必須。</span><span class="sxs-lookup"><span data-stu-id="11bf2-130">Required.</span></span> |

<span data-ttu-id="11bf2-131">このメソッドは、 `$format`応答をカスタマイズするための[OData クエリパラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="11bf2-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="11bf2-132">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="11bf2-132">The default output type is text/csv.</span></span> <span data-ttu-id="11bf2-133">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="11bf2-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="11bf2-134">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="11bf2-134">Request headers</span></span>

| <span data-ttu-id="11bf2-135">名前</span><span class="sxs-lookup"><span data-stu-id="11bf2-135">Name</span></span>          | <span data-ttu-id="11bf2-136">説明</span><span class="sxs-lookup"><span data-stu-id="11bf2-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="11bf2-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="11bf2-137">Authorization</span></span> | <span data-ttu-id="11bf2-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="11bf2-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="11bf2-140">応答</span><span class="sxs-lookup"><span data-stu-id="11bf2-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="11bf2-141">CSV</span><span class="sxs-lookup"><span data-stu-id="11bf2-141">CSV</span></span>

<span data-ttu-id="11bf2-142">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="11bf2-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="11bf2-143">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="11bf2-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="11bf2-144">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="11bf2-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="11bf2-145">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="11bf2-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="11bf2-146">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="11bf2-146">Report Refresh Date</span></span>
- <span data-ttu-id="11bf2-147">アクセスしたページ</span><span class="sxs-lookup"><span data-stu-id="11bf2-147">Visited Page</span></span>
- <span data-ttu-id="11bf2-148">表示済みまたは編集済み</span><span class="sxs-lookup"><span data-stu-id="11bf2-148">Viewed Or Edited</span></span>
- <span data-ttu-id="11bf2-149">同期済み</span><span class="sxs-lookup"><span data-stu-id="11bf2-149">Synced</span></span>
- <span data-ttu-id="11bf2-150">社内で共有済み</span><span class="sxs-lookup"><span data-stu-id="11bf2-150">Shared Internally</span></span>
- <span data-ttu-id="11bf2-151">外部で共有済み</span><span class="sxs-lookup"><span data-stu-id="11bf2-151">Shared Externally</span></span>
- <span data-ttu-id="11bf2-152">レポート日付</span><span class="sxs-lookup"><span data-stu-id="11bf2-152">Report Date</span></span>
- <span data-ttu-id="11bf2-153">レポート期間</span><span class="sxs-lookup"><span data-stu-id="11bf2-153">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="11bf2-154">JSON</span><span class="sxs-lookup"><span data-stu-id="11bf2-154">JSON</span></span>

<span data-ttu-id="11bf2-155">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[sharepointactivityusercounts](../resources/sharepointactivityusercounts.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="11bf2-155">If successful, this method returns a `200 OK` response code and a **[sharePointActivityUserCounts](../resources/sharepointactivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11bf2-156">例</span><span class="sxs-lookup"><span data-stu-id="11bf2-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="11bf2-157">CSV</span><span class="sxs-lookup"><span data-stu-id="11bf2-157">CSV</span></span>

<span data-ttu-id="11bf2-158">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="11bf2-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="11bf2-159">要求</span><span class="sxs-lookup"><span data-stu-id="11bf2-159">Request</span></span>

<span data-ttu-id="11bf2-160">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="11bf2-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="11bf2-161">応答</span><span class="sxs-lookup"><span data-stu-id="11bf2-161">Response</span></span>

<span data-ttu-id="11bf2-162">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="11bf2-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="11bf2-163">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="11bf2-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Visited Page,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="11bf2-164">JSON</span><span class="sxs-lookup"><span data-stu-id="11bf2-164">JSON</span></span>

<span data-ttu-id="11bf2-165">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="11bf2-165">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="11bf2-166">要求</span><span class="sxs-lookup"><span data-stu-id="11bf2-166">Request</span></span>

<span data-ttu-id="11bf2-167">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="11bf2-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="11bf2-168">応答</span><span class="sxs-lookup"><span data-stu-id="11bf2-168">Response</span></span>

<span data-ttu-id="11bf2-169">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="11bf2-169">The following is an example of the response.</span></span>

> <span data-ttu-id="11bf2-p108">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="11bf2-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointActivityUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 302

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.sharePointActivityUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "visitedPage": 56, 
      "viewedOrEdited": 163, 
      "synced": 7, 
      "sharedInternally": 10, 
      "sharedExternally": 1, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getsharepointactivityusercounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
