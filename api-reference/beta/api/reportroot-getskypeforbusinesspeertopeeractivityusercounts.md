---
title: 'reportRoot: getSkypeForBusinessPeerToPeerActivityUserCounts'
description: 組織内で実施されたピア ツー ピア セッションの一意のユーザー数と種類について、使用傾向を取得します。 ピア ツー ピア セッションでのセッションの種類には IM、オーディオ、ビデオ、アプリケーション共有、ファイル転送があります。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 1b208c57a18e5803021921d2eee8bb2486ad8bf8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928424"
---
# <a name="reportroot-getskypeforbusinesspeertopeeractivityusercounts"></a><span data-ttu-id="0212b-104">reportRoot: getSkypeForBusinessPeerToPeerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="0212b-104">reportRoot: getSkypeForBusinessPeerToPeerActivityUserCounts</span></span>

> <span data-ttu-id="0212b-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0212b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0212b-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0212b-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0212b-107">組織内で実施されたピア ツー ピア セッションの一意のユーザー数と種類について、使用傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="0212b-107">Get usage trends on the number of unique users and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="0212b-108">ピア ツー ピア セッションでのセッションの種類には IM、オーディオ、ビデオ、アプリケーション共有、ファイル転送があります。</span><span class="sxs-lookup"><span data-stu-id="0212b-108">Types of sessions include IM, audio, video, application sharing, and file transfers in peer-to-peer sessions.</span></span>

> <span data-ttu-id="0212b-109">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Skype for Business ピア ツー ピア アクティビティ](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0212b-109">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="permissions"></a><span data-ttu-id="0212b-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0212b-110">Permissions</span></span>

<span data-ttu-id="0212b-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0212b-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0212b-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0212b-113">Permission type</span></span>                        | <span data-ttu-id="0212b-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0212b-114">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="0212b-115">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="0212b-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="0212b-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0212b-116">Reports.Read.All</span></span>                         |
| <span data-ttu-id="0212b-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0212b-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0212b-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0212b-118">Not supported.</span></span>                           |
| <span data-ttu-id="0212b-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0212b-119">Application</span></span>                            | <span data-ttu-id="0212b-120">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0212b-120">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="0212b-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0212b-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessPeerToPeerActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="0212b-122">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="0212b-122">Function parameters</span></span>

<span data-ttu-id="0212b-123">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="0212b-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="0212b-124">パラメーター</span><span class="sxs-lookup"><span data-stu-id="0212b-124">Parameter</span></span> | <span data-ttu-id="0212b-125">Type</span><span class="sxs-lookup"><span data-stu-id="0212b-125">Type</span></span>   | <span data-ttu-id="0212b-126">説明</span><span class="sxs-lookup"><span data-stu-id="0212b-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="0212b-127">period</span><span class="sxs-lookup"><span data-stu-id="0212b-127">period</span></span>    | <span data-ttu-id="0212b-128">文字列</span><span class="sxs-lookup"><span data-stu-id="0212b-128">string</span></span> | <span data-ttu-id="0212b-129">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="0212b-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="0212b-130">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="0212b-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="0212b-131">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="0212b-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="0212b-132">必須。</span><span class="sxs-lookup"><span data-stu-id="0212b-132">Required.</span></span> |

<span data-ttu-id="0212b-133">このメソッドをサポートしている、 `$format` 、応答をカスタマイズするのには、 [OData クエリ パラメーター](/graph/query-parameters)です。</span><span class="sxs-lookup"><span data-stu-id="0212b-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="0212b-134">既定の出力の種類は、テキストまたは csv です。</span><span class="sxs-lookup"><span data-stu-id="0212b-134">The default output type is text/csv.</span></span> <span data-ttu-id="0212b-135">ただし、出力の種類を指定する場合は、設定をテキストまたは csv またはアプリケーションまたは json OData $format クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="0212b-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0212b-136">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0212b-136">Request headers</span></span>

| <span data-ttu-id="0212b-137">名前</span><span class="sxs-lookup"><span data-stu-id="0212b-137">Name</span></span>          | <span data-ttu-id="0212b-138">説明</span><span class="sxs-lookup"><span data-stu-id="0212b-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="0212b-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="0212b-139">Authorization</span></span> | <span data-ttu-id="0212b-p107">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0212b-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="0212b-142">応答</span><span class="sxs-lookup"><span data-stu-id="0212b-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="0212b-143">CSV</span><span class="sxs-lookup"><span data-stu-id="0212b-143">CSV</span></span>

<span data-ttu-id="0212b-144">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="0212b-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="0212b-145">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="0212b-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="0212b-146">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="0212b-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="0212b-147">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="0212b-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="0212b-148">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="0212b-148">Report Refresh Date</span></span>
- <span data-ttu-id="0212b-149">レポート日付</span><span class="sxs-lookup"><span data-stu-id="0212b-149">Report Date</span></span>
- <span data-ttu-id="0212b-150">レポート期間</span><span class="sxs-lookup"><span data-stu-id="0212b-150">Report Period</span></span>
- <span data-ttu-id="0212b-151">IM</span><span class="sxs-lookup"><span data-stu-id="0212b-151">IM</span></span>
- <span data-ttu-id="0212b-152">オーディオ</span><span class="sxs-lookup"><span data-stu-id="0212b-152">Audio</span></span>
- <span data-ttu-id="0212b-153">ビデオ</span><span class="sxs-lookup"><span data-stu-id="0212b-153">Video</span></span>
- <span data-ttu-id="0212b-154">アプリ共有</span><span class="sxs-lookup"><span data-stu-id="0212b-154">App Sharing</span></span>
- <span data-ttu-id="0212b-155">ファイル転送</span><span class="sxs-lookup"><span data-stu-id="0212b-155">File Transfer</span></span>

### <a name="json"></a><span data-ttu-id="0212b-156">JSON</span><span class="sxs-lookup"><span data-stu-id="0212b-156">JSON</span></span>

<span data-ttu-id="0212b-157">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に**[skypeForBusinessPeerToPeerActivityUserCounts](../resources/skypeforbusinesspeertopeeractivityusercounts.md)** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="0212b-157">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessPeerToPeerActivityUserCounts](../resources/skypeforbusinesspeertopeeractivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0212b-158">例</span><span class="sxs-lookup"><span data-stu-id="0212b-158">Example</span></span>

### <a name="csv"></a><span data-ttu-id="0212b-159">CSV</span><span class="sxs-lookup"><span data-stu-id="0212b-159">CSV</span></span>

<span data-ttu-id="0212b-160">次に、CSV を出力する例を示します。</span><span class="sxs-lookup"><span data-stu-id="0212b-160">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="0212b-161">要求</span><span class="sxs-lookup"><span data-stu-id="0212b-161">Request</span></span>

<span data-ttu-id="0212b-162">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0212b-162">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinesspeertopeeractivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="0212b-163">応答</span><span class="sxs-lookup"><span data-stu-id="0212b-163">Response</span></span>

<span data-ttu-id="0212b-164">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0212b-164">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="0212b-165">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="0212b-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="0212b-166">JSON</span><span class="sxs-lookup"><span data-stu-id="0212b-166">JSON</span></span>

<span data-ttu-id="0212b-167">次に、JSON を取得する例を示します。</span><span class="sxs-lookup"><span data-stu-id="0212b-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="0212b-168">要求</span><span class="sxs-lookup"><span data-stu-id="0212b-168">Request</span></span>

<span data-ttu-id="0212b-169">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0212b-169">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinesspeertopeeractivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="0212b-170">応答</span><span class="sxs-lookup"><span data-stu-id="0212b-170">Response</span></span>

<span data-ttu-id="0212b-171">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0212b-171">The following is an example of the response.</span></span>

> <span data-ttu-id="0212b-p109">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="0212b-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 290

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessPeerToPeerActivityUserCounts)", 
  "value": [
    {
      "im": 379, 
      "audio": 42, 
      "video": 2, 
      "appSharing": 34, 
      "fileTransfer": 36, 
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
