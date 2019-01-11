---
title: 'reportRoot: getSharePointActivityUserCounts'
description: アクティブ ユーザーの数の傾向を取得します。 ユーザーが一定期間中にファイル アクティビティ (保存、同期、変更、共有) を実行するか、またはページにアクセスすると、そのユーザーはアクティブとみなされます。
localization_priority: Normal
ms.openlocfilehash: 356f079a1d0836b6cd824a30d6882ed12f0155fd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842204"
---
# <a name="reportroot-getsharepointactivityusercounts"></a><span data-ttu-id="1f593-104">reportRoot: getSharePointActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="1f593-104">reportRoot: getSharePointActivityUserCounts</span></span>

> <span data-ttu-id="1f593-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1f593-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1f593-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1f593-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1f593-107">アクティブ ユーザーの数の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="1f593-107">Get the trend in the number of active users.</span></span> <span data-ttu-id="1f593-108">ユーザーが一定期間中にファイル アクティビティ (保存、同期、変更、共有) を実行するか、またはページにアクセスすると、そのユーザーはアクティブとみなされます。</span><span class="sxs-lookup"><span data-stu-id="1f593-108">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span>

> <span data-ttu-id="1f593-109">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: SharePoint アクティビティ](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1f593-109">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="1f593-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1f593-110">Permissions</span></span>

<span data-ttu-id="1f593-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1f593-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1f593-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1f593-113">Permission type</span></span>                        | <span data-ttu-id="1f593-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1f593-114">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="1f593-115">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="1f593-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="1f593-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1f593-116">Reports.Read.All</span></span>                         |
| <span data-ttu-id="1f593-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1f593-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f593-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1f593-118">Not supported.</span></span>                           |
| <span data-ttu-id="1f593-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1f593-119">Application</span></span>                            | <span data-ttu-id="1f593-120">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1f593-120">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="1f593-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1f593-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="1f593-122">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="1f593-122">Function parameters</span></span>

<span data-ttu-id="1f593-123">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="1f593-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="1f593-124">パラメーター</span><span class="sxs-lookup"><span data-stu-id="1f593-124">Parameter</span></span> | <span data-ttu-id="1f593-125">Type</span><span class="sxs-lookup"><span data-stu-id="1f593-125">Type</span></span>   | <span data-ttu-id="1f593-126">説明</span><span class="sxs-lookup"><span data-stu-id="1f593-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="1f593-127">period</span><span class="sxs-lookup"><span data-stu-id="1f593-127">period</span></span>    | <span data-ttu-id="1f593-128">文字列</span><span class="sxs-lookup"><span data-stu-id="1f593-128">string</span></span> | <span data-ttu-id="1f593-129">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="1f593-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="1f593-130">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="1f593-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="1f593-131">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="1f593-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="1f593-132">必須。</span><span class="sxs-lookup"><span data-stu-id="1f593-132">Required.</span></span> |

<span data-ttu-id="1f593-133">このメソッドをサポートしている、 `$format` 、応答をカスタマイズするのには、 [OData クエリ パラメーター](/graph/query-parameters)です。</span><span class="sxs-lookup"><span data-stu-id="1f593-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="1f593-134">既定の出力の種類は、テキストまたは csv です。</span><span class="sxs-lookup"><span data-stu-id="1f593-134">The default output type is text/csv.</span></span> <span data-ttu-id="1f593-135">ただし、出力の種類を指定する場合は、設定をテキストまたは csv またはアプリケーションまたは json OData $format クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="1f593-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1f593-136">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1f593-136">Request headers</span></span>

| <span data-ttu-id="1f593-137">名前</span><span class="sxs-lookup"><span data-stu-id="1f593-137">Name</span></span>          | <span data-ttu-id="1f593-138">説明</span><span class="sxs-lookup"><span data-stu-id="1f593-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="1f593-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f593-139">Authorization</span></span> | <span data-ttu-id="1f593-p107">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1f593-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="1f593-142">応答</span><span class="sxs-lookup"><span data-stu-id="1f593-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="1f593-143">CSV</span><span class="sxs-lookup"><span data-stu-id="1f593-143">CSV</span></span>

<span data-ttu-id="1f593-144">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="1f593-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="1f593-145">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="1f593-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="1f593-146">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="1f593-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="1f593-147">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="1f593-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="1f593-148">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="1f593-148">Report Refresh Date</span></span>
- <span data-ttu-id="1f593-149">アクセスしたページ</span><span class="sxs-lookup"><span data-stu-id="1f593-149">Visited Page</span></span>
- <span data-ttu-id="1f593-150">表示済みまたは編集済み</span><span class="sxs-lookup"><span data-stu-id="1f593-150">Viewed Or Edited</span></span>
- <span data-ttu-id="1f593-151">同期済み</span><span class="sxs-lookup"><span data-stu-id="1f593-151">Synced</span></span>
- <span data-ttu-id="1f593-152">社内で共有済み</span><span class="sxs-lookup"><span data-stu-id="1f593-152">Shared Internally</span></span>
- <span data-ttu-id="1f593-153">外部で共有済み</span><span class="sxs-lookup"><span data-stu-id="1f593-153">Shared Externally</span></span>
- <span data-ttu-id="1f593-154">レポート日付</span><span class="sxs-lookup"><span data-stu-id="1f593-154">Report Date</span></span>
- <span data-ttu-id="1f593-155">レポート期間</span><span class="sxs-lookup"><span data-stu-id="1f593-155">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="1f593-156">JSON</span><span class="sxs-lookup"><span data-stu-id="1f593-156">JSON</span></span>

<span data-ttu-id="1f593-157">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に**[sharePointActivityUserCounts](../resources/sharepointactivityusercounts.md)** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="1f593-157">If successful, this method returns a `200 OK` response code and a **[sharePointActivityUserCounts](../resources/sharepointactivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f593-158">例</span><span class="sxs-lookup"><span data-stu-id="1f593-158">Example</span></span>

### <a name="csv"></a><span data-ttu-id="1f593-159">CSV</span><span class="sxs-lookup"><span data-stu-id="1f593-159">CSV</span></span>

<span data-ttu-id="1f593-160">次に、CSV を出力する例を示します。</span><span class="sxs-lookup"><span data-stu-id="1f593-160">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="1f593-161">要求</span><span class="sxs-lookup"><span data-stu-id="1f593-161">Request</span></span>

<span data-ttu-id="1f593-162">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1f593-162">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="1f593-163">応答</span><span class="sxs-lookup"><span data-stu-id="1f593-163">Response</span></span>

<span data-ttu-id="1f593-164">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1f593-164">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="1f593-165">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="1f593-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="1f593-166">JSON</span><span class="sxs-lookup"><span data-stu-id="1f593-166">JSON</span></span>

<span data-ttu-id="1f593-167">次に、JSON を取得する例を示します。</span><span class="sxs-lookup"><span data-stu-id="1f593-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="1f593-168">要求</span><span class="sxs-lookup"><span data-stu-id="1f593-168">Request</span></span>

<span data-ttu-id="1f593-169">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1f593-169">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="1f593-170">応答</span><span class="sxs-lookup"><span data-stu-id="1f593-170">Response</span></span>

<span data-ttu-id="1f593-171">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1f593-171">The following is an example of the response.</span></span>

> <span data-ttu-id="1f593-p109">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="1f593-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
