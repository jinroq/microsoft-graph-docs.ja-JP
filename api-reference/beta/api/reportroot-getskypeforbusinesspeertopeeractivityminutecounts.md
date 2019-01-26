---
title: 'reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts'
description: 組織内で実施されたピア ツー ピア セッションの長さ (分数) と種類についての使用傾向を取得します。 セッションの種類には、オーディオとビデオが含まれます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 775a6c64a49336f3873b0a0dd9837b84b8b9e2cb
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575906"
---
# <a name="reportroot-getskypeforbusinesspeertopeeractivityminutecounts"></a><span data-ttu-id="7debc-104">reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="7debc-104">reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7debc-105">組織内で実施されたピア ツー ピア セッションの長さ (分数) と種類についての使用傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="7debc-105">Get usage trends on the length in minutes and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="7debc-106">セッションの種類には、オーディオとビデオが含まれます。</span><span class="sxs-lookup"><span data-stu-id="7debc-106">Types of sessions include audio and video.</span></span>

> <span data-ttu-id="7debc-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Skype for Business ピア ツー ピア アクティビティ](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7debc-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="permissions"></a><span data-ttu-id="7debc-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7debc-108">Permissions</span></span>

<span data-ttu-id="7debc-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7debc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7debc-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7debc-111">Permission type</span></span>                        | <span data-ttu-id="7debc-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7debc-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="7debc-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="7debc-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="7debc-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7debc-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="7debc-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7debc-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7debc-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7debc-116">Not supported.</span></span>                           |
| <span data-ttu-id="7debc-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7debc-117">Application</span></span>                            | <span data-ttu-id="7debc-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7debc-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="7debc-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7debc-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="7debc-120">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="7debc-120">Function parameters</span></span>

<span data-ttu-id="7debc-121">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="7debc-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="7debc-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="7debc-122">Parameter</span></span> | <span data-ttu-id="7debc-123">型</span><span class="sxs-lookup"><span data-stu-id="7debc-123">Type</span></span>   | <span data-ttu-id="7debc-124">説明</span><span class="sxs-lookup"><span data-stu-id="7debc-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="7debc-125">period</span><span class="sxs-lookup"><span data-stu-id="7debc-125">period</span></span>    | <span data-ttu-id="7debc-126">文字列</span><span class="sxs-lookup"><span data-stu-id="7debc-126">string</span></span> | <span data-ttu-id="7debc-127">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="7debc-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="7debc-128">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="7debc-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="7debc-129">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="7debc-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="7debc-130">必須。</span><span class="sxs-lookup"><span data-stu-id="7debc-130">Required.</span></span> |

<span data-ttu-id="7debc-131">このメソッドをサポートしている、 `$format` 、応答をカスタマイズするのには、 [OData クエリ パラメーター](/graph/query-parameters)です。</span><span class="sxs-lookup"><span data-stu-id="7debc-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="7debc-132">既定の出力の種類は、テキストまたは csv です。</span><span class="sxs-lookup"><span data-stu-id="7debc-132">The default output type is text/csv.</span></span> <span data-ttu-id="7debc-133">ただし、出力の種類を指定する場合は、設定をテキストまたは csv またはアプリケーションまたは json OData $format クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="7debc-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7debc-134">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7debc-134">Request headers</span></span>

| <span data-ttu-id="7debc-135">名前</span><span class="sxs-lookup"><span data-stu-id="7debc-135">Name</span></span>          | <span data-ttu-id="7debc-136">説明</span><span class="sxs-lookup"><span data-stu-id="7debc-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="7debc-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="7debc-137">Authorization</span></span> | <span data-ttu-id="7debc-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7debc-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="7debc-140">応答</span><span class="sxs-lookup"><span data-stu-id="7debc-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="7debc-141">CSV</span><span class="sxs-lookup"><span data-stu-id="7debc-141">CSV</span></span>

<span data-ttu-id="7debc-142">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="7debc-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="7debc-143">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="7debc-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="7debc-144">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="7debc-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="7debc-145">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="7debc-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="7debc-146">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="7debc-146">Report Refresh Date</span></span>
- <span data-ttu-id="7debc-147">レポート日付</span><span class="sxs-lookup"><span data-stu-id="7debc-147">Report Date</span></span>
- <span data-ttu-id="7debc-148">レポート期間</span><span class="sxs-lookup"><span data-stu-id="7debc-148">Report Period</span></span>
- <span data-ttu-id="7debc-149">オーディオ</span><span class="sxs-lookup"><span data-stu-id="7debc-149">Audio</span></span>
- <span data-ttu-id="7debc-150">ビデオ</span><span class="sxs-lookup"><span data-stu-id="7debc-150">Video</span></span>

### <a name="json"></a><span data-ttu-id="7debc-151">JSON</span><span class="sxs-lookup"><span data-stu-id="7debc-151">JSON</span></span>

<span data-ttu-id="7debc-152">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に**[skypeForBusinessPeerToPeerActivityMinuteCounts](../resources/skypeforbusinesspeertopeeractivityminutecounts.md)** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="7debc-152">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessPeerToPeerActivityMinuteCounts](../resources/skypeforbusinesspeertopeeractivityminutecounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7debc-153">例</span><span class="sxs-lookup"><span data-stu-id="7debc-153">Example</span></span>

### <a name="csv"></a><span data-ttu-id="7debc-154">CSV</span><span class="sxs-lookup"><span data-stu-id="7debc-154">CSV</span></span>

<span data-ttu-id="7debc-155">次に、CSV を出力する例を示します。</span><span class="sxs-lookup"><span data-stu-id="7debc-155">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="7debc-156">要求</span><span class="sxs-lookup"><span data-stu-id="7debc-156">Request</span></span>

<span data-ttu-id="7debc-157">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7debc-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinesspeertopeeractivityminutecounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="7debc-158">応答</span><span class="sxs-lookup"><span data-stu-id="7debc-158">Response</span></span>

<span data-ttu-id="7debc-159">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7debc-159">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="7debc-160">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="7debc-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="7debc-161">JSON</span><span class="sxs-lookup"><span data-stu-id="7debc-161">JSON</span></span>

<span data-ttu-id="7debc-162">次に、JSON を取得する例を示します。</span><span class="sxs-lookup"><span data-stu-id="7debc-162">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="7debc-163">要求</span><span class="sxs-lookup"><span data-stu-id="7debc-163">Request</span></span>

<span data-ttu-id="7debc-164">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7debc-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinesspeertopeeractivityminutecounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="7debc-165">応答</span><span class="sxs-lookup"><span data-stu-id="7debc-165">Response</span></span>

<span data-ttu-id="7debc-166">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7debc-166">The following is an example of the response.</span></span>

> <span data-ttu-id="7debc-p108">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="7debc-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinesspeertopeeractivityminutecounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
