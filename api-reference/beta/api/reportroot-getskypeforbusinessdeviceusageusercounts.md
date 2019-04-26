---
title: 'reportRoot: getSkypeForBusinessDeviceUsageUserCounts'
description: Skype for Business アプリを使用して接続した組織内のユーザー数について、使用傾向を取得します。 組織内で Skype for Business クライアント アプリをインストールし、使用したデバイスの種類 (Windows、Windows スマートフォン、Android スマートフォン、iPhone、iPad) の詳細も取得できます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 379446dc0eb317c30ee1339a46331fdfd1c0f9e0
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33332148"
---
# <a name="reportroot-getskypeforbusinessdeviceusageusercounts"></a><span data-ttu-id="7870b-104">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="7870b-104">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7870b-105">Skype for Business アプリを使用して接続した組織内のユーザー数について、使用傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="7870b-105">Get the usage trends on how many users in your organization have connected using the Skype for Business app.</span></span> <span data-ttu-id="7870b-106">組織内で Skype for Business クライアント アプリをインストールし、使用したデバイスの種類 (Windows、Windows スマートフォン、Android スマートフォン、iPhone、iPad) の詳細も取得できます。</span><span class="sxs-lookup"><span data-stu-id="7870b-106">You will also get a breakdown by the type of device (Windows, Windows phone, Android phone, iPhone, or iPad) on which the Skype for Business client app is installed and used across your organization.</span></span>

> <span data-ttu-id="7870b-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: 使用している Skype for Business クライアント](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7870b-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="7870b-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7870b-108">Permissions</span></span>

<span data-ttu-id="7870b-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7870b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7870b-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7870b-111">Permission type</span></span>                        | <span data-ttu-id="7870b-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7870b-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="7870b-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="7870b-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="7870b-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7870b-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="7870b-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7870b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7870b-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7870b-116">Not supported.</span></span>                           |
| <span data-ttu-id="7870b-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7870b-117">Application</span></span>                            | <span data-ttu-id="7870b-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7870b-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="7870b-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7870b-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="7870b-120">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="7870b-120">Function parameters</span></span>

<span data-ttu-id="7870b-121">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="7870b-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="7870b-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="7870b-122">Parameter</span></span> | <span data-ttu-id="7870b-123">型</span><span class="sxs-lookup"><span data-stu-id="7870b-123">Type</span></span>   | <span data-ttu-id="7870b-124">説明</span><span class="sxs-lookup"><span data-stu-id="7870b-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="7870b-125">period</span><span class="sxs-lookup"><span data-stu-id="7870b-125">period</span></span>    | <span data-ttu-id="7870b-126">文字列</span><span class="sxs-lookup"><span data-stu-id="7870b-126">string</span></span> | <span data-ttu-id="7870b-127">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="7870b-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="7870b-128">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="7870b-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="7870b-129">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="7870b-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="7870b-130">必須。</span><span class="sxs-lookup"><span data-stu-id="7870b-130">Required.</span></span> |

<span data-ttu-id="7870b-131">このメソッドは、 `$format`応答をカスタマイズするための[OData クエリパラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="7870b-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="7870b-132">既定の出力の種類は、text/csv です。</span><span class="sxs-lookup"><span data-stu-id="7870b-132">The default output type is text/csv.</span></span> <span data-ttu-id="7870b-133">ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。</span><span class="sxs-lookup"><span data-stu-id="7870b-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7870b-134">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7870b-134">Request headers</span></span>

| <span data-ttu-id="7870b-135">名前</span><span class="sxs-lookup"><span data-stu-id="7870b-135">Name</span></span>          | <span data-ttu-id="7870b-136">説明</span><span class="sxs-lookup"><span data-stu-id="7870b-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="7870b-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="7870b-137">Authorization</span></span> | <span data-ttu-id="7870b-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7870b-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="7870b-140">応答</span><span class="sxs-lookup"><span data-stu-id="7870b-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="7870b-141">CSV</span><span class="sxs-lookup"><span data-stu-id="7870b-141">CSV</span></span>

<span data-ttu-id="7870b-142">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="7870b-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="7870b-143">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="7870b-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="7870b-144">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="7870b-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="7870b-145">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="7870b-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="7870b-146">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="7870b-146">Report Refresh Date</span></span>
- <span data-ttu-id="7870b-147">Windows</span><span class="sxs-lookup"><span data-stu-id="7870b-147">Windows</span></span>
- <span data-ttu-id="7870b-148">Windows スマートフォン</span><span class="sxs-lookup"><span data-stu-id="7870b-148">Windows Phone</span></span>
- <span data-ttu-id="7870b-149">Android スマートフォン</span><span class="sxs-lookup"><span data-stu-id="7870b-149">Android Phone</span></span>
- <span data-ttu-id="7870b-150">iPhone</span><span class="sxs-lookup"><span data-stu-id="7870b-150">iPhone</span></span>
- <span data-ttu-id="7870b-151">iPad</span><span class="sxs-lookup"><span data-stu-id="7870b-151">iPad</span></span>
- <span data-ttu-id="7870b-152">レポート日付</span><span class="sxs-lookup"><span data-stu-id="7870b-152">Report Date</span></span>
- <span data-ttu-id="7870b-153">レポート期間</span><span class="sxs-lookup"><span data-stu-id="7870b-153">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="7870b-154">JSON</span><span class="sxs-lookup"><span data-stu-id="7870b-154">JSON</span></span>

<span data-ttu-id="7870b-155">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[skypeforbusinessdevice使い方 user計数](../resources/skypeforbusinessdeviceusageusercounts.md)** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7870b-155">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessDeviceUsageUserCounts](../resources/skypeforbusinessdeviceusageusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7870b-156">例</span><span class="sxs-lookup"><span data-stu-id="7870b-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="7870b-157">CSV</span><span class="sxs-lookup"><span data-stu-id="7870b-157">CSV</span></span>

<span data-ttu-id="7870b-158">CSV を出力する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7870b-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="7870b-159">要求</span><span class="sxs-lookup"><span data-stu-id="7870b-159">Request</span></span>

<span data-ttu-id="7870b-160">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7870b-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusageusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="7870b-161">応答</span><span class="sxs-lookup"><span data-stu-id="7870b-161">Response</span></span>

<span data-ttu-id="7870b-162">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7870b-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="7870b-163">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="7870b-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Windows,Windows Phone,Android Phone,iPhone,iPad,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="7870b-164">JSON</span><span class="sxs-lookup"><span data-stu-id="7870b-164">JSON</span></span>

<span data-ttu-id="7870b-165">次の例は、JSON を返します。</span><span class="sxs-lookup"><span data-stu-id="7870b-165">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="7870b-166">要求</span><span class="sxs-lookup"><span data-stu-id="7870b-166">Request</span></span>

<span data-ttu-id="7870b-167">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7870b-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusageusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="7870b-168">応答</span><span class="sxs-lookup"><span data-stu-id="7870b-168">Response</span></span>

<span data-ttu-id="7870b-169">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7870b-169">The following is an example of the response.</span></span>

> <span data-ttu-id="7870b-p108">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="7870b-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 289

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessDeviceUsageUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "windows": 403, 
      "windowsPhone": 2, 
      "androidPhone": 13, 
      "iPhone": 26, 
      "iPad": 0, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
