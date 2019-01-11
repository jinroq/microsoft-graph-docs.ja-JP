---
title: 'reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts'
description: 組織内で実施されたピア ツー ピア セッションの長さ (分数) と種類についての使用傾向を取得します。 セッションの種類には、オーディオとビデオが含まれます。
localization_priority: Normal
ms.openlocfilehash: 05523dd497abff5a6034e9fee669f463696b13b7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842485"
---
# <a name="reportroot-getskypeforbusinesspeertopeeractivityminutecounts"></a><span data-ttu-id="19398-104">reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="19398-104">reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts</span></span>

> <span data-ttu-id="19398-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="19398-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="19398-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="19398-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="19398-107">組織内で実施されたピア ツー ピア セッションの長さ (分数) と種類についての使用傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="19398-107">Get usage trends on the length in minutes and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="19398-108">セッションの種類には、オーディオとビデオが含まれます。</span><span class="sxs-lookup"><span data-stu-id="19398-108">Types of sessions include audio and video.</span></span>

> <span data-ttu-id="19398-109">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Skype for Business ピア ツー ピア アクティビティ](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="19398-109">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="permissions"></a><span data-ttu-id="19398-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="19398-110">Permissions</span></span>

<span data-ttu-id="19398-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="19398-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="19398-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="19398-113">Permission type</span></span>                        | <span data-ttu-id="19398-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="19398-114">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="19398-115">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="19398-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="19398-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="19398-116">Reports.Read.All</span></span>                         |
| <span data-ttu-id="19398-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="19398-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19398-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="19398-118">Not supported.</span></span>                           |
| <span data-ttu-id="19398-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="19398-119">Application</span></span>                            | <span data-ttu-id="19398-120">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="19398-120">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="19398-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="19398-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="19398-122">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="19398-122">Function parameters</span></span>

<span data-ttu-id="19398-123">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="19398-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="19398-124">パラメーター</span><span class="sxs-lookup"><span data-stu-id="19398-124">Parameter</span></span> | <span data-ttu-id="19398-125">Type</span><span class="sxs-lookup"><span data-stu-id="19398-125">Type</span></span>   | <span data-ttu-id="19398-126">説明</span><span class="sxs-lookup"><span data-stu-id="19398-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="19398-127">period</span><span class="sxs-lookup"><span data-stu-id="19398-127">period</span></span>    | <span data-ttu-id="19398-128">文字列</span><span class="sxs-lookup"><span data-stu-id="19398-128">string</span></span> | <span data-ttu-id="19398-129">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="19398-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="19398-130">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="19398-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="19398-131">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="19398-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="19398-132">必須。</span><span class="sxs-lookup"><span data-stu-id="19398-132">Required.</span></span> |

<span data-ttu-id="19398-133">このメソッドをサポートしている、 `$format` 、応答をカスタマイズするのには、 [OData クエリ パラメーター](/graph/query-parameters)です。</span><span class="sxs-lookup"><span data-stu-id="19398-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="19398-134">既定の出力の種類は、テキストまたは csv です。</span><span class="sxs-lookup"><span data-stu-id="19398-134">The default output type is text/csv.</span></span> <span data-ttu-id="19398-135">ただし、出力の種類を指定する場合は、設定をテキストまたは csv またはアプリケーションまたは json OData $format クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="19398-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="19398-136">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="19398-136">Request headers</span></span>

| <span data-ttu-id="19398-137">名前</span><span class="sxs-lookup"><span data-stu-id="19398-137">Name</span></span>          | <span data-ttu-id="19398-138">説明</span><span class="sxs-lookup"><span data-stu-id="19398-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="19398-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="19398-139">Authorization</span></span> | <span data-ttu-id="19398-p107">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="19398-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="19398-142">応答</span><span class="sxs-lookup"><span data-stu-id="19398-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="19398-143">CSV</span><span class="sxs-lookup"><span data-stu-id="19398-143">CSV</span></span>

<span data-ttu-id="19398-144">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="19398-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="19398-145">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="19398-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="19398-146">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="19398-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="19398-147">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="19398-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="19398-148">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="19398-148">Report Refresh Date</span></span>
- <span data-ttu-id="19398-149">レポート日付</span><span class="sxs-lookup"><span data-stu-id="19398-149">Report Date</span></span>
- <span data-ttu-id="19398-150">レポート期間</span><span class="sxs-lookup"><span data-stu-id="19398-150">Report Period</span></span>
- <span data-ttu-id="19398-151">オーディオ</span><span class="sxs-lookup"><span data-stu-id="19398-151">Audio</span></span>
- <span data-ttu-id="19398-152">ビデオ</span><span class="sxs-lookup"><span data-stu-id="19398-152">Video</span></span>

### <a name="json"></a><span data-ttu-id="19398-153">JSON</span><span class="sxs-lookup"><span data-stu-id="19398-153">JSON</span></span>

<span data-ttu-id="19398-154">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に**[skypeForBusinessPeerToPeerActivityMinuteCounts](../resources/skypeforbusinesspeertopeeractivityminutecounts.md)** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="19398-154">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessPeerToPeerActivityMinuteCounts](../resources/skypeforbusinesspeertopeeractivityminutecounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19398-155">例</span><span class="sxs-lookup"><span data-stu-id="19398-155">Example</span></span>

### <a name="csv"></a><span data-ttu-id="19398-156">CSV</span><span class="sxs-lookup"><span data-stu-id="19398-156">CSV</span></span>

<span data-ttu-id="19398-157">次に、CSV を出力する例を示します。</span><span class="sxs-lookup"><span data-stu-id="19398-157">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="19398-158">要求</span><span class="sxs-lookup"><span data-stu-id="19398-158">Request</span></span>

<span data-ttu-id="19398-159">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="19398-159">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinesspeertopeeractivityminutecounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="19398-160">応答</span><span class="sxs-lookup"><span data-stu-id="19398-160">Response</span></span>

<span data-ttu-id="19398-161">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="19398-161">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="19398-162">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="19398-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Audio,Video
```

### <a name="json"></a><span data-ttu-id="19398-163">JSON</span><span class="sxs-lookup"><span data-stu-id="19398-163">JSON</span></span>

<span data-ttu-id="19398-164">次に、JSON を取得する例を示します。</span><span class="sxs-lookup"><span data-stu-id="19398-164">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="19398-165">要求</span><span class="sxs-lookup"><span data-stu-id="19398-165">Request</span></span>

<span data-ttu-id="19398-166">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="19398-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinesspeertopeeractivityminutecounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="19398-167">応答</span><span class="sxs-lookup"><span data-stu-id="19398-167">Response</span></span>

<span data-ttu-id="19398-168">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="19398-168">The following is an example of the response.</span></span>

> <span data-ttu-id="19398-p109">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="19398-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityMinuteCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 251

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessPeerToPeerActivityMinuteCounts)", 
  "value": [
    {
      "audio": 836, 
      "video": 35, 
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
