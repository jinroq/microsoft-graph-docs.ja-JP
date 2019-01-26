---
title: 'reportRoot: getSkypeForBusinessOrganizerActivityUserCounts'
description: 一意のユーザー数と組織内のユーザーが開催、企画した電話会議セッションの数と種類に関する使用傾向を取得します。 会議セッションの種類には、IM、オーディオ/ビデオ、アプリケーション共有、Web、サード パーティへのダイヤルイン/ダイヤルアウト、Microsoft へのダイヤルイン/ダイヤルアウトなどがあります。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: af6d72466e58e7b56f3a667ce282d220a638c9f0
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576760"
---
# <a name="reportroot-getskypeforbusinessorganizeractivityusercounts"></a><span data-ttu-id="782d2-104">reportRoot: getSkypeForBusinessOrganizerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="782d2-104">reportRoot: getSkypeForBusinessOrganizerActivityUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="782d2-105">一意のユーザー数と組織内のユーザーが開催、企画した電話会議セッションの数と種類に関する使用傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="782d2-105">Get usage trends on the number of unique users and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="782d2-106">会議セッションの種類には、IM、オーディオ/ビデオ、アプリケーション共有、Web、サード パーティへのダイヤルイン/ダイヤルアウト、Microsoft へのダイヤルイン/ダイヤルアウトなどがあります。</span><span class="sxs-lookup"><span data-stu-id="782d2-106">Types of conference sessions include IM, audio/video, application sharing, web, dial-in/out - 3rd party, and dial-in/out Microsoft.</span></span>

> <span data-ttu-id="782d2-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Skype for Business 電話会議の開催者のアクティビティ](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="782d2-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="permissions"></a><span data-ttu-id="782d2-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="782d2-108">Permissions</span></span>

<span data-ttu-id="782d2-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="782d2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="782d2-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="782d2-111">Permission type</span></span>                        | <span data-ttu-id="782d2-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="782d2-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="782d2-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="782d2-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="782d2-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="782d2-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="782d2-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="782d2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="782d2-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="782d2-116">Not supported.</span></span>                           |
| <span data-ttu-id="782d2-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="782d2-117">Application</span></span>                            | <span data-ttu-id="782d2-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="782d2-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="782d2-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="782d2-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessOrganizerActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="782d2-120">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="782d2-120">Function parameters</span></span>

<span data-ttu-id="782d2-121">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="782d2-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="782d2-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="782d2-122">Parameter</span></span> | <span data-ttu-id="782d2-123">型</span><span class="sxs-lookup"><span data-stu-id="782d2-123">Type</span></span>   | <span data-ttu-id="782d2-124">説明</span><span class="sxs-lookup"><span data-stu-id="782d2-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="782d2-125">period</span><span class="sxs-lookup"><span data-stu-id="782d2-125">period</span></span>    | <span data-ttu-id="782d2-126">文字列</span><span class="sxs-lookup"><span data-stu-id="782d2-126">string</span></span> | <span data-ttu-id="782d2-127">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="782d2-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="782d2-128">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="782d2-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="782d2-129">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="782d2-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="782d2-130">必須。</span><span class="sxs-lookup"><span data-stu-id="782d2-130">Required.</span></span> |

<span data-ttu-id="782d2-131">このメソッドをサポートしている、 `$format` 、応答をカスタマイズするのには、 [OData クエリ パラメーター](/graph/query-parameters)です。</span><span class="sxs-lookup"><span data-stu-id="782d2-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="782d2-132">既定の出力の種類は、テキストまたは csv です。</span><span class="sxs-lookup"><span data-stu-id="782d2-132">The default output type is text/csv.</span></span> <span data-ttu-id="782d2-133">ただし、出力の種類を指定する場合は、設定をテキストまたは csv またはアプリケーションまたは json OData $format クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="782d2-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="782d2-134">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="782d2-134">Request headers</span></span>

| <span data-ttu-id="782d2-135">名前</span><span class="sxs-lookup"><span data-stu-id="782d2-135">Name</span></span>          | <span data-ttu-id="782d2-136">説明</span><span class="sxs-lookup"><span data-stu-id="782d2-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="782d2-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="782d2-137">Authorization</span></span> | <span data-ttu-id="782d2-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="782d2-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="782d2-140">応答</span><span class="sxs-lookup"><span data-stu-id="782d2-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="782d2-141">CSV</span><span class="sxs-lookup"><span data-stu-id="782d2-141">CSV</span></span>

<span data-ttu-id="782d2-142">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="782d2-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="782d2-143">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="782d2-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="782d2-144">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="782d2-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="782d2-145">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="782d2-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="782d2-146">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="782d2-146">Report Refresh Date</span></span>
- <span data-ttu-id="782d2-147">レポート日付</span><span class="sxs-lookup"><span data-stu-id="782d2-147">Report Date</span></span>
- <span data-ttu-id="782d2-148">レポート期間</span><span class="sxs-lookup"><span data-stu-id="782d2-148">Report Period</span></span>
- <span data-ttu-id="782d2-149">IM</span><span class="sxs-lookup"><span data-stu-id="782d2-149">IM</span></span>
- <span data-ttu-id="782d2-150">オーディオ/ビデオ</span><span class="sxs-lookup"><span data-stu-id="782d2-150">Audio/Video</span></span>
- <span data-ttu-id="782d2-151">アプリ共有</span><span class="sxs-lookup"><span data-stu-id="782d2-151">App Sharing</span></span>
- <span data-ttu-id="782d2-152">Web</span><span class="sxs-lookup"><span data-stu-id="782d2-152">Web</span></span>
- <span data-ttu-id="782d2-153">サード パーティのダイヤルイン/アウト</span><span class="sxs-lookup"><span data-stu-id="782d2-153">Dial-in/out 3rd Party</span></span>
- <span data-ttu-id="782d2-154">Microsoft へのダイヤルイン/アウト</span><span class="sxs-lookup"><span data-stu-id="782d2-154">Dial-in/out Microsoft</span></span>

### <a name="json"></a><span data-ttu-id="782d2-155">JSON</span><span class="sxs-lookup"><span data-stu-id="782d2-155">JSON</span></span>

<span data-ttu-id="782d2-156">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に**[skypeForBusinessOrganizerActivityUserCounts](../resources/skypeforbusinessorganizeractivityusercounts.md)** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="782d2-156">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessOrganizerActivityUserCounts](../resources/skypeforbusinessorganizeractivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="782d2-157">例</span><span class="sxs-lookup"><span data-stu-id="782d2-157">Example</span></span>

### <a name="csv"></a><span data-ttu-id="782d2-158">CSV</span><span class="sxs-lookup"><span data-stu-id="782d2-158">CSV</span></span>

<span data-ttu-id="782d2-159">次に、CSV を出力する例を示します。</span><span class="sxs-lookup"><span data-stu-id="782d2-159">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="782d2-160">要求</span><span class="sxs-lookup"><span data-stu-id="782d2-160">Request</span></span>

<span data-ttu-id="782d2-161">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="782d2-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessorganizeractivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessOrganizerActivityUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="782d2-162">応答</span><span class="sxs-lookup"><span data-stu-id="782d2-162">Response</span></span>

<span data-ttu-id="782d2-163">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="782d2-163">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="782d2-164">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="782d2-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio/Video,App Sharing,Web,Dial-in/out 3rd Party,Dial-in/out Microsoft
```

### <a name="json"></a><span data-ttu-id="782d2-165">JSON</span><span class="sxs-lookup"><span data-stu-id="782d2-165">JSON</span></span>

<span data-ttu-id="782d2-166">次に、JSON を取得する例を示します。</span><span class="sxs-lookup"><span data-stu-id="782d2-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="782d2-167">要求</span><span class="sxs-lookup"><span data-stu-id="782d2-167">Request</span></span>

<span data-ttu-id="782d2-168">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="782d2-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessorganizeractivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessOrganizerActivityUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="782d2-169">応答</span><span class="sxs-lookup"><span data-stu-id="782d2-169">Response</span></span>

<span data-ttu-id="782d2-170">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="782d2-170">The following is an example of the response.</span></span>

> <span data-ttu-id="782d2-p108">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="782d2-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessOrganizerActivityUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 319

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessOrganizerActivityUserCounts)", 
  "value": [
    {
      "im": 37, 
      "audioVideo": 42, 
      "appSharing": 35, 
      "web": 3, 
      "dialInOut3rdParty": 0, 
      "dialInOutMicrosoft": 36, 
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
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessorganizeractivityusercounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
