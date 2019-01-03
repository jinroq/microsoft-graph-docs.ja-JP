---
title: 'reportRoot: getSkypeForBusinessParticipantActivityCounts'
description: 組織からユーザーが参加した会議セッションの数と種類について、使用傾向を取得します。 会議セッションの種類には、IM、オーディオ/ビデオ、アプリケーション共有、Web、サードパーティへのダイヤルイン/ダイヤルアウトなどがあります。
ms.openlocfilehash: ecb3938330b38492dbee6dd873421c96fbf23d56
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068410"
---
# <a name="reportroot-getskypeforbusinessparticipantactivitycounts"></a><span data-ttu-id="dc0be-104">reportRoot: getSkypeForBusinessParticipantActivityCounts</span><span class="sxs-lookup"><span data-stu-id="dc0be-104">reportRoot: getSkypeForBusinessParticipantActivityCounts</span></span>

> <span data-ttu-id="dc0be-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="dc0be-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dc0be-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dc0be-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dc0be-107">組織からユーザーが参加した会議セッションの数と種類について、使用傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="dc0be-107">Get usage trends on the number and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="dc0be-108">会議セッションの種類には、IM、オーディオ/ビデオ、アプリケーション共有、Web、サードパーティへのダイヤルイン/ダイヤルアウトなどがあります。</span><span class="sxs-lookup"><span data-stu-id="dc0be-108">Types of conference sessions include IM, audio/video, application sharing, web, and dial-in/out - 3rd party.</span></span>

> <span data-ttu-id="dc0be-109">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Skype for Business 電話会議の参加者のアクティビティ](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dc0be-109">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="permissions"></a><span data-ttu-id="dc0be-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="dc0be-110">Permissions</span></span>

<span data-ttu-id="dc0be-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dc0be-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dc0be-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dc0be-113">Permission type</span></span>                        | <span data-ttu-id="dc0be-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="dc0be-114">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="dc0be-115">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="dc0be-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="dc0be-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="dc0be-116">Reports.Read.All</span></span>                         |
| <span data-ttu-id="dc0be-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dc0be-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc0be-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dc0be-118">Not supported.</span></span>                           |
| <span data-ttu-id="dc0be-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dc0be-119">Application</span></span>                            | <span data-ttu-id="dc0be-120">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="dc0be-120">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="dc0be-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dc0be-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessParticipantActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="dc0be-122">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="dc0be-122">Function parameters</span></span>

<span data-ttu-id="dc0be-123">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="dc0be-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="dc0be-124">パラメーター</span><span class="sxs-lookup"><span data-stu-id="dc0be-124">Parameter</span></span> | <span data-ttu-id="dc0be-125">型</span><span class="sxs-lookup"><span data-stu-id="dc0be-125">Type</span></span>   | <span data-ttu-id="dc0be-126">説明</span><span class="sxs-lookup"><span data-stu-id="dc0be-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="dc0be-127">period</span><span class="sxs-lookup"><span data-stu-id="dc0be-127">period</span></span>    | <span data-ttu-id="dc0be-128">文字列</span><span class="sxs-lookup"><span data-stu-id="dc0be-128">string</span></span> | <span data-ttu-id="dc0be-129">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="dc0be-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="dc0be-130">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="dc0be-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="dc0be-131">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="dc0be-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="dc0be-132">必須。</span><span class="sxs-lookup"><span data-stu-id="dc0be-132">Required.</span></span> |

<span data-ttu-id="dc0be-133">このメソッドをサポートしている、 `$format` 、応答をカスタマイズするのには、 [OData クエリ パラメーター](/graph/query-parameters)です。</span><span class="sxs-lookup"><span data-stu-id="dc0be-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="dc0be-134">既定の出力の種類は、テキストまたは csv です。</span><span class="sxs-lookup"><span data-stu-id="dc0be-134">The default output type is text/csv.</span></span> <span data-ttu-id="dc0be-135">ただし、出力の種類を指定する場合は、設定をテキストまたは csv またはアプリケーションまたは json OData $format クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="dc0be-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dc0be-136">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dc0be-136">Request headers</span></span>

| <span data-ttu-id="dc0be-137">名前</span><span class="sxs-lookup"><span data-stu-id="dc0be-137">Name</span></span>          | <span data-ttu-id="dc0be-138">説明</span><span class="sxs-lookup"><span data-stu-id="dc0be-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="dc0be-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="dc0be-139">Authorization</span></span> | <span data-ttu-id="dc0be-p107">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="dc0be-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="dc0be-142">応答</span><span class="sxs-lookup"><span data-stu-id="dc0be-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="dc0be-143">CSV</span><span class="sxs-lookup"><span data-stu-id="dc0be-143">CSV</span></span>

<span data-ttu-id="dc0be-144">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="dc0be-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="dc0be-145">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="dc0be-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="dc0be-146">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="dc0be-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="dc0be-147">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="dc0be-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="dc0be-148">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="dc0be-148">Report Refresh Date</span></span>
- <span data-ttu-id="dc0be-149">レポート日付</span><span class="sxs-lookup"><span data-stu-id="dc0be-149">Report Date</span></span>
- <span data-ttu-id="dc0be-150">レポート期間</span><span class="sxs-lookup"><span data-stu-id="dc0be-150">Report Period</span></span>
- <span data-ttu-id="dc0be-151">IM</span><span class="sxs-lookup"><span data-stu-id="dc0be-151">IM</span></span>
- <span data-ttu-id="dc0be-152">オーディオ/ビデオ</span><span class="sxs-lookup"><span data-stu-id="dc0be-152">Audio/Video</span></span>
- <span data-ttu-id="dc0be-153">アプリ共有</span><span class="sxs-lookup"><span data-stu-id="dc0be-153">App Sharing</span></span>
- <span data-ttu-id="dc0be-154">Web</span><span class="sxs-lookup"><span data-stu-id="dc0be-154">Web</span></span>
- <span data-ttu-id="dc0be-155">サード パーティのダイヤルイン/アウト</span><span class="sxs-lookup"><span data-stu-id="dc0be-155">Dial-in/out 3rd Party</span></span>

### <a name="json"></a><span data-ttu-id="dc0be-156">JSON</span><span class="sxs-lookup"><span data-stu-id="dc0be-156">JSON</span></span>

<span data-ttu-id="dc0be-157">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に**[skypeForBusinessParticipantActivityCounts](../resources/skypeforbusinessparticipantactivitycounts.md)** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="dc0be-157">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessParticipantActivityCounts](../resources/skypeforbusinessparticipantactivitycounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc0be-158">使用例</span><span class="sxs-lookup"><span data-stu-id="dc0be-158">Example</span></span>

### <a name="csv"></a><span data-ttu-id="dc0be-159">CSV</span><span class="sxs-lookup"><span data-stu-id="dc0be-159">CSV</span></span>

<span data-ttu-id="dc0be-160">次に、CSV を出力する例を示します。</span><span class="sxs-lookup"><span data-stu-id="dc0be-160">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="dc0be-161">要求</span><span class="sxs-lookup"><span data-stu-id="dc0be-161">Request</span></span>

<span data-ttu-id="dc0be-162">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="dc0be-162">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessparticipantactivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessParticipantActivityCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="dc0be-163">応答</span><span class="sxs-lookup"><span data-stu-id="dc0be-163">Response</span></span>

<span data-ttu-id="dc0be-164">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="dc0be-164">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="dc0be-165">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="dc0be-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio/Video,App Sharing,Web,Dial-in/out 3rd Party
```

### <a name="json"></a><span data-ttu-id="dc0be-166">JSON</span><span class="sxs-lookup"><span data-stu-id="dc0be-166">JSON</span></span>

<span data-ttu-id="dc0be-167">次に、JSON を取得する例を示します。</span><span class="sxs-lookup"><span data-stu-id="dc0be-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="dc0be-168">要求</span><span class="sxs-lookup"><span data-stu-id="dc0be-168">Request</span></span>

<span data-ttu-id="dc0be-169">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="dc0be-169">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessparticipantactivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessParticipantActivityCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="dc0be-170">応答</span><span class="sxs-lookup"><span data-stu-id="dc0be-170">Response</span></span>

<span data-ttu-id="dc0be-171">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="dc0be-171">The following is an example of the response.</span></span>

> <span data-ttu-id="dc0be-p109">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="dc0be-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessParticipantActivityCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 296

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessParticipantActivityCounts)", 
  "value": [
    {
      "im": 162, 
      "audioVideo": 156, 
      "appSharing": 45, 
      "web": 12, 
      "dialInOut3rdParty": 2, 
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```