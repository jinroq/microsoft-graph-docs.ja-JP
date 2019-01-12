---
title: 'reportRoot: getSkypeForBusinessActivityCounts'
description: Skype for Business を介して組織内で行われた会議セッションの開催ユーザー数と参加ユーザー数の傾向を取得します。 レポートには、ピア ツー ピア セッションの数も含まれます。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: e0d666321f7287f817d91a348a4c8c7ad17bf823
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964712"
---
# <a name="reportroot-getskypeforbusinessactivitycounts"></a><span data-ttu-id="4e0f1-104">reportRoot: getSkypeForBusinessActivityCounts</span><span class="sxs-lookup"><span data-stu-id="4e0f1-104">reportRoot: getSkypeForBusinessActivityCounts</span></span>

> <span data-ttu-id="4e0f1-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4e0f1-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4e0f1-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4e0f1-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4e0f1-107">Skype for Business を介して組織内で行われた会議セッションの開催ユーザー数と参加ユーザー数の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="4e0f1-107">Get the trends on how many users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="4e0f1-108">レポートには、ピア ツー ピア セッションの数も含まれます。</span><span class="sxs-lookup"><span data-stu-id="4e0f1-108">The report also includes the number of peer-to-peer sessions.</span></span>

> <span data-ttu-id="4e0f1-109">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Skype for Business アクティビティ](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4e0f1-109">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="4e0f1-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4e0f1-110">Permissions</span></span>

<span data-ttu-id="4e0f1-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4e0f1-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4e0f1-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4e0f1-113">Permission type</span></span>                        | <span data-ttu-id="4e0f1-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4e0f1-114">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="4e0f1-115">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="4e0f1-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="4e0f1-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4e0f1-116">Reports.Read.All</span></span>                         |
| <span data-ttu-id="4e0f1-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4e0f1-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e0f1-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4e0f1-118">Not supported.</span></span>                           |
| <span data-ttu-id="4e0f1-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4e0f1-119">Application</span></span>                            | <span data-ttu-id="4e0f1-120">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4e0f1-120">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="4e0f1-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4e0f1-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="4e0f1-122">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="4e0f1-122">Function parameters</span></span>

<span data-ttu-id="4e0f1-123">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="4e0f1-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="4e0f1-124">パラメーター</span><span class="sxs-lookup"><span data-stu-id="4e0f1-124">Parameter</span></span> | <span data-ttu-id="4e0f1-125">Type</span><span class="sxs-lookup"><span data-stu-id="4e0f1-125">Type</span></span>   | <span data-ttu-id="4e0f1-126">説明</span><span class="sxs-lookup"><span data-stu-id="4e0f1-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="4e0f1-127">period</span><span class="sxs-lookup"><span data-stu-id="4e0f1-127">period</span></span>    | <span data-ttu-id="4e0f1-128">文字列</span><span class="sxs-lookup"><span data-stu-id="4e0f1-128">string</span></span> | <span data-ttu-id="4e0f1-129">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="4e0f1-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="4e0f1-130">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="4e0f1-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="4e0f1-131">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="4e0f1-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="4e0f1-132">必須。</span><span class="sxs-lookup"><span data-stu-id="4e0f1-132">Required.</span></span> |

<span data-ttu-id="4e0f1-133">このメソッドをサポートしている、 `$format` 、応答をカスタマイズするのには、 [OData クエリ パラメーター](/graph/query-parameters)です。</span><span class="sxs-lookup"><span data-stu-id="4e0f1-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="4e0f1-134">既定の出力の種類は、テキストまたは csv です。</span><span class="sxs-lookup"><span data-stu-id="4e0f1-134">The default output type is text/csv.</span></span> <span data-ttu-id="4e0f1-135">ただし、出力の種類を指定する場合は、設定をテキストまたは csv またはアプリケーションまたは json OData $format クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="4e0f1-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4e0f1-136">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4e0f1-136">Request headers</span></span>

| <span data-ttu-id="4e0f1-137">名前</span><span class="sxs-lookup"><span data-stu-id="4e0f1-137">Name</span></span>          | <span data-ttu-id="4e0f1-138">説明</span><span class="sxs-lookup"><span data-stu-id="4e0f1-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="4e0f1-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e0f1-139">Authorization</span></span> | <span data-ttu-id="4e0f1-p107">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4e0f1-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="4e0f1-142">応答</span><span class="sxs-lookup"><span data-stu-id="4e0f1-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="4e0f1-143">CSV</span><span class="sxs-lookup"><span data-stu-id="4e0f1-143">CSV</span></span>

<span data-ttu-id="4e0f1-144">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="4e0f1-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="4e0f1-145">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="4e0f1-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="4e0f1-146">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="4e0f1-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="4e0f1-147">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="4e0f1-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="4e0f1-148">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="4e0f1-148">Report Refresh Date</span></span>
- <span data-ttu-id="4e0f1-149">レポート日付</span><span class="sxs-lookup"><span data-stu-id="4e0f1-149">Report Date</span></span>
- <span data-ttu-id="4e0f1-150">レポート期間</span><span class="sxs-lookup"><span data-stu-id="4e0f1-150">Report Period</span></span>
- <span data-ttu-id="4e0f1-151">ピアツーピア</span><span class="sxs-lookup"><span data-stu-id="4e0f1-151">Peer-to-peer</span></span>
- <span data-ttu-id="4e0f1-152">開催</span><span class="sxs-lookup"><span data-stu-id="4e0f1-152">Organized</span></span>
- <span data-ttu-id="4e0f1-153">参加</span><span class="sxs-lookup"><span data-stu-id="4e0f1-153">Participated</span></span>

### <a name="json"></a><span data-ttu-id="4e0f1-154">JSON</span><span class="sxs-lookup"><span data-stu-id="4e0f1-154">JSON</span></span>

<span data-ttu-id="4e0f1-155">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に**[skypeForBusinessActivityCounts](../resources/skypeforbusinessactivitycounts.md)** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="4e0f1-155">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessActivityCounts](../resources/skypeforbusinessactivitycounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e0f1-156">例</span><span class="sxs-lookup"><span data-stu-id="4e0f1-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="4e0f1-157">CSV</span><span class="sxs-lookup"><span data-stu-id="4e0f1-157">CSV</span></span>

<span data-ttu-id="4e0f1-158">次に、CSV を出力する例を示します。</span><span class="sxs-lookup"><span data-stu-id="4e0f1-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="4e0f1-159">要求</span><span class="sxs-lookup"><span data-stu-id="4e0f1-159">Request</span></span>

<span data-ttu-id="4e0f1-160">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4e0f1-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessactivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="4e0f1-161">応答</span><span class="sxs-lookup"><span data-stu-id="4e0f1-161">Response</span></span>

<span data-ttu-id="4e0f1-162">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4e0f1-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="4e0f1-163">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="4e0f1-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Peer-to-peer,Organized,Participated
```

### <a name="json"></a><span data-ttu-id="4e0f1-164">JSON</span><span class="sxs-lookup"><span data-stu-id="4e0f1-164">JSON</span></span>

<span data-ttu-id="4e0f1-165">次に、JSON を取得する例を示します。</span><span class="sxs-lookup"><span data-stu-id="4e0f1-165">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="4e0f1-166">要求</span><span class="sxs-lookup"><span data-stu-id="4e0f1-166">Request</span></span>

<span data-ttu-id="4e0f1-167">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4e0f1-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessactivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="4e0f1-168">応答</span><span class="sxs-lookup"><span data-stu-id="4e0f1-168">Response</span></span>

<span data-ttu-id="4e0f1-169">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4e0f1-169">The following is an example of the response.</span></span>

> <span data-ttu-id="4e0f1-p109">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="4e0f1-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessActivityCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 264

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessActivityCounts)", 
  "value": [
    {
      "peerToPeer": 3436, 
      "organized": 58, 
      "participated": 209, 
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
