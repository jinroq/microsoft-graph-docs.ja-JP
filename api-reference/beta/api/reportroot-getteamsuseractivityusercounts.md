---
title: 'reportRoot: getTeamsUserActivityUserCounts'
description: アクティビティの種類ごとに、Microsoft Teams ユーザーの数を取得します。 アクティビティの種類は、チーム チャット メッセージ、非公開チャット メッセージ、通話、または会議の数です。
ms.openlocfilehash: 6eb9f4a59941f05fff0b9dba5ecf7282a163dec7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074546"
---
# <a name="reportroot-getteamsuseractivityusercounts"></a><span data-ttu-id="f6c61-104">reportRoot: getTeamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="f6c61-104">reportRoot: getTeamsUserActivityUserCounts</span></span>

> <span data-ttu-id="f6c61-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f6c61-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f6c61-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f6c61-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f6c61-107">アクティビティの種類ごとに、Microsoft Teams ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="f6c61-107">Get the number of Microsoft Teams users by activity type.</span></span> <span data-ttu-id="f6c61-108">アクティビティの種類は、チーム チャット メッセージ、非公開チャット メッセージ、通話、または会議の数です。</span><span class="sxs-lookup"><span data-stu-id="f6c61-108">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="f6c61-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f6c61-109">Permissions</span></span>

<span data-ttu-id="f6c61-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f6c61-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f6c61-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f6c61-112">Permission type</span></span>                        | <span data-ttu-id="f6c61-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f6c61-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="f6c61-114">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="f6c61-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="f6c61-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f6c61-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="f6c61-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f6c61-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6c61-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f6c61-117">Not supported.</span></span>                           |
| <span data-ttu-id="f6c61-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f6c61-118">Application</span></span>                            | <span data-ttu-id="f6c61-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f6c61-119">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="f6c61-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f6c61-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="f6c61-121">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="f6c61-121">Function parameters</span></span>

<span data-ttu-id="f6c61-122">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="f6c61-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="f6c61-123">パラメーター</span><span class="sxs-lookup"><span data-stu-id="f6c61-123">Parameter</span></span> | <span data-ttu-id="f6c61-124">型</span><span class="sxs-lookup"><span data-stu-id="f6c61-124">Type</span></span>   | <span data-ttu-id="f6c61-125">説明</span><span class="sxs-lookup"><span data-stu-id="f6c61-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="f6c61-126">period</span><span class="sxs-lookup"><span data-stu-id="f6c61-126">period</span></span>    | <span data-ttu-id="f6c61-127">文字列</span><span class="sxs-lookup"><span data-stu-id="f6c61-127">string</span></span> | <span data-ttu-id="f6c61-128">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="f6c61-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="f6c61-129">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="f6c61-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="f6c61-130">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="f6c61-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="f6c61-131">必須。</span><span class="sxs-lookup"><span data-stu-id="f6c61-131">Required.</span></span> |

<span data-ttu-id="f6c61-132">このメソッドをサポートしている、 `$format` 、応答をカスタマイズするのには、 [OData クエリ パラメーター](/graph/query-parameters)です。</span><span class="sxs-lookup"><span data-stu-id="f6c61-132">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="f6c61-133">既定の出力の種類は、テキストまたは csv です。</span><span class="sxs-lookup"><span data-stu-id="f6c61-133">The default output type is text/csv.</span></span> <span data-ttu-id="f6c61-134">ただし、出力の種類を指定する場合は、設定をテキストまたは csv またはアプリケーションまたは json OData $format クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="f6c61-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f6c61-135">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f6c61-135">Request headers</span></span>

| <span data-ttu-id="f6c61-136">名前</span><span class="sxs-lookup"><span data-stu-id="f6c61-136">Name</span></span>          | <span data-ttu-id="f6c61-137">説明</span><span class="sxs-lookup"><span data-stu-id="f6c61-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="f6c61-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6c61-138">Authorization</span></span> | <span data-ttu-id="f6c61-p107">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f6c61-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="f6c61-141">応答</span><span class="sxs-lookup"><span data-stu-id="f6c61-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="f6c61-142">CSV</span><span class="sxs-lookup"><span data-stu-id="f6c61-142">CSV</span></span>

<span data-ttu-id="f6c61-143">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="f6c61-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="f6c61-144">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="f6c61-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="f6c61-145">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="f6c61-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="f6c61-146">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="f6c61-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="f6c61-147">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="f6c61-147">Report Refresh Date</span></span>
- <span data-ttu-id="f6c61-148">レポート日付</span><span class="sxs-lookup"><span data-stu-id="f6c61-148">Report Date</span></span>
- <span data-ttu-id="f6c61-149">チーム チャット メッセージ</span><span class="sxs-lookup"><span data-stu-id="f6c61-149">Team Chat Messages</span></span>
- <span data-ttu-id="f6c61-150">非公開チャット メッセージ</span><span class="sxs-lookup"><span data-stu-id="f6c61-150">Private Chat Messages</span></span>
- <span data-ttu-id="f6c61-151">通話</span><span class="sxs-lookup"><span data-stu-id="f6c61-151">Calls</span></span>
- <span data-ttu-id="f6c61-152">会議</span><span class="sxs-lookup"><span data-stu-id="f6c61-152">Meetings</span></span>
- <span data-ttu-id="f6c61-153">その他のアクション</span><span class="sxs-lookup"><span data-stu-id="f6c61-153">Other Actions</span></span>
- <span data-ttu-id="f6c61-154">レポート期間</span><span class="sxs-lookup"><span data-stu-id="f6c61-154">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="f6c61-155">JSON</span><span class="sxs-lookup"><span data-stu-id="f6c61-155">JSON</span></span>

<span data-ttu-id="f6c61-156">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に**[teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md)** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="f6c61-156">If successful, this method returns a `200 OK` response code and a **[teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6c61-157">使用例</span><span class="sxs-lookup"><span data-stu-id="f6c61-157">Example</span></span>

### <a name="csv"></a><span data-ttu-id="f6c61-158">CSV</span><span class="sxs-lookup"><span data-stu-id="f6c61-158">CSV</span></span>

<span data-ttu-id="f6c61-159">次に、CSV を出力する例を示します。</span><span class="sxs-lookup"><span data-stu-id="f6c61-159">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="f6c61-160">要求</span><span class="sxs-lookup"><span data-stu-id="f6c61-160">Request</span></span>

<span data-ttu-id="f6c61-161">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f6c61-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="f6c61-162">応答</span><span class="sxs-lookup"><span data-stu-id="f6c61-162">Response</span></span>

<span data-ttu-id="f6c61-163">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f6c61-163">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="f6c61-164">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="f6c61-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="f6c61-165">JSON</span><span class="sxs-lookup"><span data-stu-id="f6c61-165">JSON</span></span>

<span data-ttu-id="f6c61-166">次に、JSON を取得する例を示します。</span><span class="sxs-lookup"><span data-stu-id="f6c61-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="f6c61-167">要求</span><span class="sxs-lookup"><span data-stu-id="f6c61-167">Request</span></span>

<span data-ttu-id="f6c61-168">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f6c61-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="f6c61-169">応答</span><span class="sxs-lookup"><span data-stu-id="f6c61-169">Response</span></span>

<span data-ttu-id="f6c61-170">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f6c61-170">The following is an example of the response.</span></span>

> <span data-ttu-id="f6c61-p109">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f6c61-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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