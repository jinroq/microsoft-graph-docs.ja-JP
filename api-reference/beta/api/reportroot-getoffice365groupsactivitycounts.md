---
title: 'reportRoot: getOffice365GroupsActivityCounts'
description: グループ ワークロード全体のグループ活動の数を取得します。
ms.openlocfilehash: 0dfcf2a20344c3f0336f9042b22295c7a9b0e2b9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066277"
---
# <a name="reportroot-getoffice365groupsactivitycounts"></a><span data-ttu-id="31261-103">reportRoot: getOffice365GroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="31261-103">reportRoot: getOffice365GroupsActivityCounts</span></span>

> <span data-ttu-id="31261-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="31261-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="31261-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="31261-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="31261-106">グループ ワークロード全体のグループ活動の数を取得します。</span><span class="sxs-lookup"><span data-stu-id="31261-106">Get the number of group activities across group workloads.</span></span>

> <span data-ttu-id="31261-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Office 365 グループ](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="31261-107">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="31261-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="31261-108">Permissions</span></span>

<span data-ttu-id="31261-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="31261-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="31261-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="31261-111">Permission type</span></span>                        | <span data-ttu-id="31261-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="31261-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="31261-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="31261-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="31261-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="31261-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="31261-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="31261-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31261-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="31261-116">Not supported.</span></span>                           |
| <span data-ttu-id="31261-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="31261-117">Application</span></span>                            | <span data-ttu-id="31261-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="31261-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="31261-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="31261-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="31261-120">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="31261-120">Function parameters</span></span>

<span data-ttu-id="31261-121">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="31261-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="31261-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="31261-122">Parameter</span></span> | <span data-ttu-id="31261-123">型</span><span class="sxs-lookup"><span data-stu-id="31261-123">Type</span></span>   | <span data-ttu-id="31261-124">説明</span><span class="sxs-lookup"><span data-stu-id="31261-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="31261-125">period</span><span class="sxs-lookup"><span data-stu-id="31261-125">period</span></span>    | <span data-ttu-id="31261-126">文字列</span><span class="sxs-lookup"><span data-stu-id="31261-126">string</span></span> | <span data-ttu-id="31261-127">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="31261-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="31261-128">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="31261-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="31261-129">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="31261-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="31261-130">必須。</span><span class="sxs-lookup"><span data-stu-id="31261-130">Required.</span></span> |

<span data-ttu-id="31261-131">このメソッドをサポートしている、 `$format` 、応答をカスタマイズするのには、 [OData クエリ パラメーター](/graph/query-parameters)です。</span><span class="sxs-lookup"><span data-stu-id="31261-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="31261-132">既定の出力の種類は、テキストまたは csv です。</span><span class="sxs-lookup"><span data-stu-id="31261-132">The default output type is text/csv.</span></span> <span data-ttu-id="31261-133">ただし、出力の種類を指定する場合は、設定をテキストまたは csv またはアプリケーションまたは json OData $format クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="31261-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="31261-134">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="31261-134">Request headers</span></span>

| <span data-ttu-id="31261-135">名前</span><span class="sxs-lookup"><span data-stu-id="31261-135">Name</span></span>          | <span data-ttu-id="31261-136">説明</span><span class="sxs-lookup"><span data-stu-id="31261-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="31261-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="31261-137">Authorization</span></span> | <span data-ttu-id="31261-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="31261-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="31261-140">応答</span><span class="sxs-lookup"><span data-stu-id="31261-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="31261-141">CSV</span><span class="sxs-lookup"><span data-stu-id="31261-141">CSV</span></span>

<span data-ttu-id="31261-142">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="31261-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="31261-143">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="31261-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="31261-144">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="31261-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="31261-145">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="31261-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="31261-146">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="31261-146">Report Refresh Date</span></span>
- <span data-ttu-id="31261-147">受信した Exchange の電子メール</span><span class="sxs-lookup"><span data-stu-id="31261-147">Exchange Emails Received</span></span>
- <span data-ttu-id="31261-148">投稿された Yammer メッセージ</span><span class="sxs-lookup"><span data-stu-id="31261-148">Yammer Messages Posted</span></span>
- <span data-ttu-id="31261-149">読み取られた Yammer メッセージ</span><span class="sxs-lookup"><span data-stu-id="31261-149">Yammer Messages Read</span></span>
- <span data-ttu-id="31261-150">「いいね!」された Yammer メッセージ</span><span class="sxs-lookup"><span data-stu-id="31261-150">Yammer Messages Liked</span></span>
- <span data-ttu-id="31261-151">レポート日付</span><span class="sxs-lookup"><span data-stu-id="31261-151">Report Date</span></span>
- <span data-ttu-id="31261-152">レポート期間</span><span class="sxs-lookup"><span data-stu-id="31261-152">Report Period</span></span>

<span data-ttu-id="31261-153">21Vianet によって運営されて、Microsoft Graph 中国では、次の列はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="31261-153">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="31261-154">投稿された Yammer メッセージ</span><span class="sxs-lookup"><span data-stu-id="31261-154">Yammer Messages Posted</span></span>
- <span data-ttu-id="31261-155">読み取られた Yammer メッセージ</span><span class="sxs-lookup"><span data-stu-id="31261-155">Yammer Messages Read</span></span>
- <span data-ttu-id="31261-156">「いいね!」された Yammer メッセージ</span><span class="sxs-lookup"><span data-stu-id="31261-156">Yammer Messages Liked</span></span>

### <a name="json"></a><span data-ttu-id="31261-157">JSON</span><span class="sxs-lookup"><span data-stu-id="31261-157">JSON</span></span>

<span data-ttu-id="31261-158">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の**[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="31261-158">If successful, this method returns a `200 OK` response code and an **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** object in the response body.</span></span>

<span data-ttu-id="31261-159">21Vianet によって運営されて、Microsoft Graph 中国では、 **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** オブジェクトでは、次のプロパティはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="31261-159">The following properties in **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="31261-160">yammerMessagesPosted</span><span class="sxs-lookup"><span data-stu-id="31261-160">yammerMessagesPosted</span></span>
- <span data-ttu-id="31261-161">yammerMessagesRead</span><span class="sxs-lookup"><span data-stu-id="31261-161">yammerMessagesRead</span></span>
- <span data-ttu-id="31261-162">yammerMessagesLiked</span><span class="sxs-lookup"><span data-stu-id="31261-162">yammerMessagesLiked</span></span>

## <a name="example"></a><span data-ttu-id="31261-163">使用例</span><span class="sxs-lookup"><span data-stu-id="31261-163">Example</span></span>

### <a name="csv"></a><span data-ttu-id="31261-164">CSV</span><span class="sxs-lookup"><span data-stu-id="31261-164">CSV</span></span>

<span data-ttu-id="31261-165">次に、CSV を出力する例を示します。</span><span class="sxs-lookup"><span data-stu-id="31261-165">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="31261-166">要求</span><span class="sxs-lookup"><span data-stu-id="31261-166">Request</span></span>

<span data-ttu-id="31261-167">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="31261-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="31261-168">応答</span><span class="sxs-lookup"><span data-stu-id="31261-168">Response</span></span>

<span data-ttu-id="31261-169">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="31261-169">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="31261-170">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="31261-170">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Exchange Emails Received,Yammer Messages Posted,Yammer Messages Read,Yammer Messages Liked,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="31261-171">JSON</span><span class="sxs-lookup"><span data-stu-id="31261-171">JSON</span></span>

<span data-ttu-id="31261-172">次に、JSON を取得する例を示します。</span><span class="sxs-lookup"><span data-stu-id="31261-172">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="31261-173">要求</span><span class="sxs-lookup"><span data-stu-id="31261-173">Request</span></span>

<span data-ttu-id="31261-174">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="31261-174">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="31261-175">応答</span><span class="sxs-lookup"><span data-stu-id="31261-175">Response</span></span>

<span data-ttu-id="31261-176">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="31261-176">The following is an example of the response.</span></span>

> <span data-ttu-id="31261-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="31261-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365GroupsActivityCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 310

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365GroupsActivityCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "exchangeEmailsReceived": 0, 
      "yammerMessagesPosted": 0, 
      "yammerMessagesRead": 0, 
      "yammerMessagesLiked": 0, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
