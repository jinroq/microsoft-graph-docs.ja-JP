---
title: 'reportRoot: getTeamsUserActivityUserCounts'
description: アクティビティの種類ごとに、Microsoft Teams ユーザーの数を取得します。 アクティビティの種類は、チーム チャット メッセージ、非公開チャット メッセージ、通話、または会議の数です。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 6115368b99c1aa8c445e9d6f7e7c307a4b72f8e2
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33336344"
---
# <a name="reportroot-getteamsuseractivityusercounts"></a><span data-ttu-id="e45ff-104">reportRoot: getTeamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="e45ff-104">reportRoot: getTeamsUserActivityUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e45ff-105">アクティビティの種類ごとに、Microsoft Teams ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="e45ff-105">Get the number of Microsoft Teams users by activity type.</span></span> <span data-ttu-id="e45ff-106">アクティビティの種類は、チーム チャット メッセージ、非公開チャット メッセージ、通話、または会議の数です。</span><span class="sxs-lookup"><span data-stu-id="e45ff-106">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="e45ff-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e45ff-107">Permissions</span></span>

<span data-ttu-id="e45ff-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e45ff-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e45ff-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e45ff-110">Permission type</span></span>                        | <span data-ttu-id="e45ff-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e45ff-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e45ff-112">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="e45ff-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="e45ff-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e45ff-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e45ff-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e45ff-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e45ff-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e45ff-115">Not supported.</span></span>                           |
| <span data-ttu-id="e45ff-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e45ff-116">Application</span></span>                            | <span data-ttu-id="e45ff-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e45ff-117">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="e45ff-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e45ff-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="e45ff-119">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="e45ff-119">Function parameters</span></span>

<span data-ttu-id="e45ff-120">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="e45ff-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="e45ff-121">パラメーター</span><span class="sxs-lookup"><span data-stu-id="e45ff-121">Parameter</span></span> | <span data-ttu-id="e45ff-122">型</span><span class="sxs-lookup"><span data-stu-id="e45ff-122">Type</span></span>   | <span data-ttu-id="e45ff-123">説明</span><span class="sxs-lookup"><span data-stu-id="e45ff-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="e45ff-124">period</span><span class="sxs-lookup"><span data-stu-id="e45ff-124">period</span></span>    | <span data-ttu-id="e45ff-125">文字列</span><span class="sxs-lookup"><span data-stu-id="e45ff-125">string</span></span> | <span data-ttu-id="e45ff-126">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="e45ff-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="e45ff-127">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="e45ff-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="e45ff-128">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="e45ff-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="e45ff-129">必須。</span><span class="sxs-lookup"><span data-stu-id="e45ff-129">Required.</span></span> |

<span data-ttu-id="e45ff-130">このメソッドは、 `$format`応答をカスタマイズするための[OData クエリパラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e45ff-130">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="e45ff-131">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="e45ff-131">The default output type is text/csv.</span></span> <span data-ttu-id="e45ff-132">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="e45ff-132">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e45ff-133">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e45ff-133">Request headers</span></span>

| <span data-ttu-id="e45ff-134">名前</span><span class="sxs-lookup"><span data-stu-id="e45ff-134">Name</span></span>          | <span data-ttu-id="e45ff-135">説明</span><span class="sxs-lookup"><span data-stu-id="e45ff-135">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="e45ff-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="e45ff-136">Authorization</span></span> | <span data-ttu-id="e45ff-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e45ff-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="e45ff-139">応答</span><span class="sxs-lookup"><span data-stu-id="e45ff-139">Response</span></span>

### <a name="csv"></a><span data-ttu-id="e45ff-140">CSV</span><span class="sxs-lookup"><span data-stu-id="e45ff-140">CSV</span></span>

<span data-ttu-id="e45ff-141">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="e45ff-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e45ff-142">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="e45ff-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e45ff-143">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="e45ff-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e45ff-144">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="e45ff-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="e45ff-145">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="e45ff-145">Report Refresh Date</span></span>
- <span data-ttu-id="e45ff-146">レポート日付</span><span class="sxs-lookup"><span data-stu-id="e45ff-146">Report Date</span></span>
- <span data-ttu-id="e45ff-147">チーム チャット メッセージ</span><span class="sxs-lookup"><span data-stu-id="e45ff-147">Team Chat Messages</span></span>
- <span data-ttu-id="e45ff-148">非公開チャット メッセージ</span><span class="sxs-lookup"><span data-stu-id="e45ff-148">Private Chat Messages</span></span>
- <span data-ttu-id="e45ff-149">通話</span><span class="sxs-lookup"><span data-stu-id="e45ff-149">Calls</span></span>
- <span data-ttu-id="e45ff-150">会議</span><span class="sxs-lookup"><span data-stu-id="e45ff-150">Meetings</span></span>
- <span data-ttu-id="e45ff-151">その他のアクション</span><span class="sxs-lookup"><span data-stu-id="e45ff-151">Other Actions</span></span>
- <span data-ttu-id="e45ff-152">レポート期間</span><span class="sxs-lookup"><span data-stu-id="e45ff-152">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="e45ff-153">JSON</span><span class="sxs-lookup"><span data-stu-id="e45ff-153">JSON</span></span>

<span data-ttu-id="e45ff-154">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[teamsuseractivityusercounts](../resources/teamsuseractivityusercounts.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e45ff-154">If successful, this method returns a `200 OK` response code and a **[teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e45ff-155">例</span><span class="sxs-lookup"><span data-stu-id="e45ff-155">Example</span></span>

### <a name="csv"></a><span data-ttu-id="e45ff-156">CSV</span><span class="sxs-lookup"><span data-stu-id="e45ff-156">CSV</span></span>

<span data-ttu-id="e45ff-157">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e45ff-157">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="e45ff-158">要求</span><span class="sxs-lookup"><span data-stu-id="e45ff-158">Request</span></span>

<span data-ttu-id="e45ff-159">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e45ff-159">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="e45ff-160">応答</span><span class="sxs-lookup"><span data-stu-id="e45ff-160">Response</span></span>

<span data-ttu-id="e45ff-161">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e45ff-161">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="e45ff-162">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="e45ff-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Team Chat Messages,Private Chat Messages,Calls,Meetings,Other Actions,Report Period
```

### <a name="json"></a><span data-ttu-id="e45ff-163">JSON</span><span class="sxs-lookup"><span data-stu-id="e45ff-163">JSON</span></span>

<span data-ttu-id="e45ff-164">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="e45ff-164">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="e45ff-165">要求</span><span class="sxs-lookup"><span data-stu-id="e45ff-165">Request</span></span>

<span data-ttu-id="e45ff-166">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e45ff-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="e45ff-167">応答</span><span class="sxs-lookup"><span data-stu-id="e45ff-167">Response</span></span>

<span data-ttu-id="e45ff-168">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e45ff-168">The following is an example of the response.</span></span>

> <span data-ttu-id="e45ff-p108">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="e45ff-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsUserActivityUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 291

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsUserActivityUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
      "teamChatMessages": 30, 
      "privateChatMessages": 21, 
      "calls": 6, 
      "meetings": 2, 
      "otherActions": 17, 
      "reportPeriod": "7"
    }
  ]
}
```
