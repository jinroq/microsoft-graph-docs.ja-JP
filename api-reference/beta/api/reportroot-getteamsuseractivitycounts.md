---
title: 'reportRoot: getTeamsUserActivityCounts'
description: アクティビティの種類ごとに、Microsoft Teams アクティビティの数を取得します。 アクティビティの種類は、チーム チャット メッセージ、非公開チャット メッセージ、通話および会議です。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 1f0f3ddd6c9c9e43a46d41d758bb4794072d5071
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514748"
---
# <a name="reportroot-getteamsuseractivitycounts"></a><span data-ttu-id="ce2c3-104">reportRoot: getTeamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="ce2c3-104">reportRoot: getTeamsUserActivityCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce2c3-105">アクティビティの種類ごとに、Microsoft Teams アクティビティの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="ce2c3-105">Get the number of Microsoft Teams activities by activity type.</span></span> <span data-ttu-id="ce2c3-106">アクティビティの種類は、チーム チャット メッセージ、非公開チャット メッセージ、通話および会議です。</span><span class="sxs-lookup"><span data-stu-id="ce2c3-106">The activity types are team chat messages, private chat messages, calls, and meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="ce2c3-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ce2c3-107">Permissions</span></span>

<span data-ttu-id="ce2c3-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ce2c3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ce2c3-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ce2c3-110">Permission type</span></span>                        | <span data-ttu-id="ce2c3-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ce2c3-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ce2c3-112">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="ce2c3-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="ce2c3-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ce2c3-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ce2c3-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ce2c3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce2c3-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ce2c3-115">Not supported.</span></span>                           |
| <span data-ttu-id="ce2c3-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ce2c3-116">Application</span></span>                            | <span data-ttu-id="ce2c3-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ce2c3-117">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="ce2c3-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ce2c3-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="ce2c3-119">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="ce2c3-119">Function parameters</span></span>

<span data-ttu-id="ce2c3-120">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="ce2c3-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="ce2c3-121">パラメーター</span><span class="sxs-lookup"><span data-stu-id="ce2c3-121">Parameter</span></span> | <span data-ttu-id="ce2c3-122">型</span><span class="sxs-lookup"><span data-stu-id="ce2c3-122">Type</span></span>   | <span data-ttu-id="ce2c3-123">説明</span><span class="sxs-lookup"><span data-stu-id="ce2c3-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="ce2c3-124">period</span><span class="sxs-lookup"><span data-stu-id="ce2c3-124">period</span></span>    | <span data-ttu-id="ce2c3-125">文字列</span><span class="sxs-lookup"><span data-stu-id="ce2c3-125">string</span></span> | <span data-ttu-id="ce2c3-126">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="ce2c3-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="ce2c3-127">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="ce2c3-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="ce2c3-128">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="ce2c3-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="ce2c3-129">必須。</span><span class="sxs-lookup"><span data-stu-id="ce2c3-129">Required.</span></span> |

<span data-ttu-id="ce2c3-130">このメソッドをサポートしている、 `$format` 、応答をカスタマイズするのには、 [OData クエリ パラメーター](/graph/query-parameters)です。</span><span class="sxs-lookup"><span data-stu-id="ce2c3-130">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="ce2c3-131">既定の出力の種類は、テキストまたは csv です。</span><span class="sxs-lookup"><span data-stu-id="ce2c3-131">The default output type is text/csv.</span></span> <span data-ttu-id="ce2c3-132">ただし、出力の種類を指定する場合は、設定をテキストまたは csv またはアプリケーションまたは json OData $format クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="ce2c3-132">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ce2c3-133">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ce2c3-133">Request headers</span></span>

| <span data-ttu-id="ce2c3-134">名前</span><span class="sxs-lookup"><span data-stu-id="ce2c3-134">Name</span></span>          | <span data-ttu-id="ce2c3-135">説明</span><span class="sxs-lookup"><span data-stu-id="ce2c3-135">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="ce2c3-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce2c3-136">Authorization</span></span> | <span data-ttu-id="ce2c3-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ce2c3-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="ce2c3-139">応答</span><span class="sxs-lookup"><span data-stu-id="ce2c3-139">Response</span></span>

### <a name="csv"></a><span data-ttu-id="ce2c3-140">CSV</span><span class="sxs-lookup"><span data-stu-id="ce2c3-140">CSV</span></span>

<span data-ttu-id="ce2c3-141">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="ce2c3-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ce2c3-142">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="ce2c3-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ce2c3-143">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="ce2c3-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ce2c3-144">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="ce2c3-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="ce2c3-145">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="ce2c3-145">Report Refresh Date</span></span>
- <span data-ttu-id="ce2c3-146">レポート日付</span><span class="sxs-lookup"><span data-stu-id="ce2c3-146">Report Date</span></span>
- <span data-ttu-id="ce2c3-147">チーム チャット メッセージ</span><span class="sxs-lookup"><span data-stu-id="ce2c3-147">Team Chat Messages</span></span>
- <span data-ttu-id="ce2c3-148">非公開チャット メッセージ</span><span class="sxs-lookup"><span data-stu-id="ce2c3-148">Private Chat Messages</span></span>
- <span data-ttu-id="ce2c3-149">通話</span><span class="sxs-lookup"><span data-stu-id="ce2c3-149">Calls</span></span>
- <span data-ttu-id="ce2c3-150">会議</span><span class="sxs-lookup"><span data-stu-id="ce2c3-150">Meetings</span></span>
- <span data-ttu-id="ce2c3-151">レポート期間</span><span class="sxs-lookup"><span data-stu-id="ce2c3-151">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="ce2c3-152">JSON</span><span class="sxs-lookup"><span data-stu-id="ce2c3-152">JSON</span></span>

<span data-ttu-id="ce2c3-153">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に**[teamsUserActivityCounts](../resources/teamsuseractivitycounts.md)** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="ce2c3-153">If successful, this method returns a `200 OK` response code and a **[teamsUserActivityCounts](../resources/teamsuseractivitycounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce2c3-154">例</span><span class="sxs-lookup"><span data-stu-id="ce2c3-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="ce2c3-155">CSV</span><span class="sxs-lookup"><span data-stu-id="ce2c3-155">CSV</span></span>

<span data-ttu-id="ce2c3-156">次に、CSV を出力する例を示します。</span><span class="sxs-lookup"><span data-stu-id="ce2c3-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="ce2c3-157">要求</span><span class="sxs-lookup"><span data-stu-id="ce2c3-157">Request</span></span>

<span data-ttu-id="ce2c3-158">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ce2c3-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="ce2c3-159">応答</span><span class="sxs-lookup"><span data-stu-id="ce2c3-159">Response</span></span>

<span data-ttu-id="ce2c3-160">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ce2c3-160">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
<span data-ttu-id="ce2c3-161">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="ce2c3-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Team Chat Messages,Private Chat Messages,Calls,Meetings,Report Period
```

### <a name="json"></a><span data-ttu-id="ce2c3-162">JSON</span><span class="sxs-lookup"><span data-stu-id="ce2c3-162">JSON</span></span>

<span data-ttu-id="ce2c3-163">次に、JSON を取得する例を示します。</span><span class="sxs-lookup"><span data-stu-id="ce2c3-163">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="ce2c3-164">要求</span><span class="sxs-lookup"><span data-stu-id="ce2c3-164">Request</span></span>

<span data-ttu-id="ce2c3-165">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ce2c3-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="ce2c3-166">応答</span><span class="sxs-lookup"><span data-stu-id="ce2c3-166">Response</span></span>

<span data-ttu-id="ce2c3-167">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ce2c3-167">The following is an example of the response.</span></span>

> <span data-ttu-id="ce2c3-p108">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="ce2c3-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsUserActivityCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 277

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsUserActivityCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
      "teamChatMessages": 26, 
      "privateChatMessages": 17, 
      "calls": 4, 
      "meetings": 0, 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getteamsuseractivitycounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
