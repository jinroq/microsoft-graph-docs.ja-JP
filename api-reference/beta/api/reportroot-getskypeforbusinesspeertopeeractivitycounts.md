---
title: 'reportRoot: getSkypeForBusinessPeerToPeerActivityCounts'
description: 組織内で実施されたセッションの数と種類について、使用傾向を取得します。 セッションの種類には IM、オーディオ、ビデオ、アプリケーション共有、ファイル転送があります。
localization_priority: Normal
ms.openlocfilehash: a962a80f2cf1aff70a267a5b52ac429e88286fe2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871709"
---
# <a name="reportroot-getskypeforbusinesspeertopeeractivitycounts"></a><span data-ttu-id="cf6ba-104">reportRoot: getSkypeForBusinessPeerToPeerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="cf6ba-104">reportRoot: getSkypeForBusinessPeerToPeerActivityCounts</span></span>

> <span data-ttu-id="cf6ba-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cf6ba-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cf6ba-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cf6ba-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cf6ba-107">組織内で実施されたセッションの数と種類について、使用傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="cf6ba-107">Get usage trends on the number and type of sessions held in your organization.</span></span> <span data-ttu-id="cf6ba-108">セッションの種類には IM、オーディオ、ビデオ、アプリケーション共有、ファイル転送があります。</span><span class="sxs-lookup"><span data-stu-id="cf6ba-108">Types of sessions include IM, audio, video, application sharing, and file transfer.</span></span>

> <span data-ttu-id="cf6ba-109">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Skype for Business ピア ツー ピア アクティビティ](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cf6ba-109">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="permissions"></a><span data-ttu-id="cf6ba-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cf6ba-110">Permissions</span></span>

<span data-ttu-id="cf6ba-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cf6ba-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cf6ba-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cf6ba-113">Permission type</span></span>                        | <span data-ttu-id="cf6ba-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cf6ba-114">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="cf6ba-115">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="cf6ba-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="cf6ba-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf6ba-116">Reports.Read.All</span></span>                         |
| <span data-ttu-id="cf6ba-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cf6ba-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf6ba-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cf6ba-118">Not supported.</span></span>                           |
| <span data-ttu-id="cf6ba-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cf6ba-119">Application</span></span>                            | <span data-ttu-id="cf6ba-120">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf6ba-120">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="cf6ba-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cf6ba-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessPeerToPeerActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="cf6ba-122">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="cf6ba-122">Function parameters</span></span>

<span data-ttu-id="cf6ba-123">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="cf6ba-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="cf6ba-124">パラメーター</span><span class="sxs-lookup"><span data-stu-id="cf6ba-124">Parameter</span></span> | <span data-ttu-id="cf6ba-125">Type</span><span class="sxs-lookup"><span data-stu-id="cf6ba-125">Type</span></span>   | <span data-ttu-id="cf6ba-126">説明</span><span class="sxs-lookup"><span data-stu-id="cf6ba-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="cf6ba-127">period</span><span class="sxs-lookup"><span data-stu-id="cf6ba-127">period</span></span>    | <span data-ttu-id="cf6ba-128">文字列</span><span class="sxs-lookup"><span data-stu-id="cf6ba-128">string</span></span> | <span data-ttu-id="cf6ba-129">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="cf6ba-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="cf6ba-130">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="cf6ba-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="cf6ba-131">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="cf6ba-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="cf6ba-132">必須。</span><span class="sxs-lookup"><span data-stu-id="cf6ba-132">Required.</span></span> |

<span data-ttu-id="cf6ba-133">このメソッドをサポートしている、 `$format` 、応答をカスタマイズするのには、 [OData クエリ パラメーター](/graph/query-parameters)です。</span><span class="sxs-lookup"><span data-stu-id="cf6ba-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="cf6ba-134">既定の出力の種類は、テキストまたは csv です。</span><span class="sxs-lookup"><span data-stu-id="cf6ba-134">The default output type is text/csv.</span></span> <span data-ttu-id="cf6ba-135">ただし、出力の種類を指定する場合は、設定をテキストまたは csv またはアプリケーションまたは json OData $format クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="cf6ba-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cf6ba-136">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cf6ba-136">Request headers</span></span>

| <span data-ttu-id="cf6ba-137">名前</span><span class="sxs-lookup"><span data-stu-id="cf6ba-137">Name</span></span>          | <span data-ttu-id="cf6ba-138">説明</span><span class="sxs-lookup"><span data-stu-id="cf6ba-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="cf6ba-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf6ba-139">Authorization</span></span> | <span data-ttu-id="cf6ba-p107">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="cf6ba-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="cf6ba-142">応答</span><span class="sxs-lookup"><span data-stu-id="cf6ba-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="cf6ba-143">CSV</span><span class="sxs-lookup"><span data-stu-id="cf6ba-143">CSV</span></span>

<span data-ttu-id="cf6ba-144">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="cf6ba-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="cf6ba-145">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="cf6ba-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="cf6ba-146">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="cf6ba-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="cf6ba-147">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="cf6ba-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="cf6ba-148">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="cf6ba-148">Report Refresh Date</span></span>
- <span data-ttu-id="cf6ba-149">レポート日付</span><span class="sxs-lookup"><span data-stu-id="cf6ba-149">Report Date</span></span>
- <span data-ttu-id="cf6ba-150">レポート期間</span><span class="sxs-lookup"><span data-stu-id="cf6ba-150">Report Period</span></span>
- <span data-ttu-id="cf6ba-151">IM</span><span class="sxs-lookup"><span data-stu-id="cf6ba-151">IM</span></span>
- <span data-ttu-id="cf6ba-152">オーディオ</span><span class="sxs-lookup"><span data-stu-id="cf6ba-152">Audio</span></span>
- <span data-ttu-id="cf6ba-153">ビデオ</span><span class="sxs-lookup"><span data-stu-id="cf6ba-153">Video</span></span>
- <span data-ttu-id="cf6ba-154">アプリ共有</span><span class="sxs-lookup"><span data-stu-id="cf6ba-154">App Sharing</span></span>
- <span data-ttu-id="cf6ba-155">ファイル転送</span><span class="sxs-lookup"><span data-stu-id="cf6ba-155">File Transfer</span></span>

### <a name="json"></a><span data-ttu-id="cf6ba-156">JSON</span><span class="sxs-lookup"><span data-stu-id="cf6ba-156">JSON</span></span>

<span data-ttu-id="cf6ba-157">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に**[skypeForBusinessPeerToPeerActivityCounts](../resources/skypeforbusinesspeertopeeractivitycounts.md)** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="cf6ba-157">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessPeerToPeerActivityCounts](../resources/skypeforbusinesspeertopeeractivitycounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf6ba-158">例</span><span class="sxs-lookup"><span data-stu-id="cf6ba-158">Example</span></span>

### <a name="csv"></a><span data-ttu-id="cf6ba-159">CSV</span><span class="sxs-lookup"><span data-stu-id="cf6ba-159">CSV</span></span>

<span data-ttu-id="cf6ba-160">次に、CSV を出力する例を示します。</span><span class="sxs-lookup"><span data-stu-id="cf6ba-160">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="cf6ba-161">要求</span><span class="sxs-lookup"><span data-stu-id="cf6ba-161">Request</span></span>

<span data-ttu-id="cf6ba-162">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cf6ba-162">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinesspeertopeeractivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="cf6ba-163">応答</span><span class="sxs-lookup"><span data-stu-id="cf6ba-163">Response</span></span>

<span data-ttu-id="cf6ba-164">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cf6ba-164">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="cf6ba-165">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="cf6ba-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio,Video,App Sharing,File Transfer
```

### <a name="json"></a><span data-ttu-id="cf6ba-166">JSON</span><span class="sxs-lookup"><span data-stu-id="cf6ba-166">JSON</span></span>

<span data-ttu-id="cf6ba-167">次に、JSON を取得する例を示します。</span><span class="sxs-lookup"><span data-stu-id="cf6ba-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="cf6ba-168">要求</span><span class="sxs-lookup"><span data-stu-id="cf6ba-168">Request</span></span>

<span data-ttu-id="cf6ba-169">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cf6ba-169">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinesspeertopeeractivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="cf6ba-170">応答</span><span class="sxs-lookup"><span data-stu-id="cf6ba-170">Response</span></span>

<span data-ttu-id="cf6ba-171">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cf6ba-171">The following is an example of the response.</span></span>

> <span data-ttu-id="cf6ba-p109">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="cf6ba-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 288

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessPeerToPeerActivityCounts)", 
  "value": [
    {
      "im": 1177, 
      "audio": 107, 
      "video": 7, 
      "appSharing": 74, 
      "fileTransfer": 24, 
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
