---
title: 'reportRoot: getOffice365GroupsActivityCounts'
description: グループ ワークロード全体のグループ活動の数を取得します。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 85eab0e6fa7d4e0c541e8745144662fa4631fb4e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508644"
---
# <a name="reportroot-getoffice365groupsactivitycounts"></a><span data-ttu-id="de079-103">reportRoot: getOffice365GroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="de079-103">reportRoot: getOffice365GroupsActivityCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de079-104">グループ ワークロード全体のグループ活動の数を取得します。</span><span class="sxs-lookup"><span data-stu-id="de079-104">Get the number of group activities across group workloads.</span></span>

> <span data-ttu-id="de079-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Office 365 グループ](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="de079-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="de079-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="de079-106">Permissions</span></span>

<span data-ttu-id="de079-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="de079-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="de079-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="de079-109">Permission type</span></span>                        | <span data-ttu-id="de079-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="de079-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="de079-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="de079-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="de079-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="de079-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="de079-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="de079-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de079-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="de079-114">Not supported.</span></span>                           |
| <span data-ttu-id="de079-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="de079-115">Application</span></span>                            | <span data-ttu-id="de079-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="de079-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="de079-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="de079-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="de079-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="de079-118">Function parameters</span></span>

<span data-ttu-id="de079-119">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="de079-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="de079-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="de079-120">Parameter</span></span> | <span data-ttu-id="de079-121">型</span><span class="sxs-lookup"><span data-stu-id="de079-121">Type</span></span>   | <span data-ttu-id="de079-122">説明</span><span class="sxs-lookup"><span data-stu-id="de079-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="de079-123">period</span><span class="sxs-lookup"><span data-stu-id="de079-123">period</span></span>    | <span data-ttu-id="de079-124">文字列</span><span class="sxs-lookup"><span data-stu-id="de079-124">string</span></span> | <span data-ttu-id="de079-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="de079-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="de079-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="de079-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="de079-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="de079-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="de079-128">必須。</span><span class="sxs-lookup"><span data-stu-id="de079-128">Required.</span></span> |

<span data-ttu-id="de079-129">このメソッドをサポートしている、 `$format` 、応答をカスタマイズするのには、 [OData クエリ パラメーター](/graph/query-parameters)です。</span><span class="sxs-lookup"><span data-stu-id="de079-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="de079-130">既定の出力の種類は、テキストまたは csv です。</span><span class="sxs-lookup"><span data-stu-id="de079-130">The default output type is text/csv.</span></span> <span data-ttu-id="de079-131">ただし、出力の種類を指定する場合は、設定をテキストまたは csv またはアプリケーションまたは json OData $format クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="de079-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="de079-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="de079-132">Request headers</span></span>

| <span data-ttu-id="de079-133">名前</span><span class="sxs-lookup"><span data-stu-id="de079-133">Name</span></span>          | <span data-ttu-id="de079-134">説明</span><span class="sxs-lookup"><span data-stu-id="de079-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="de079-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="de079-135">Authorization</span></span> | <span data-ttu-id="de079-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="de079-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="de079-138">応答</span><span class="sxs-lookup"><span data-stu-id="de079-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="de079-139">CSV</span><span class="sxs-lookup"><span data-stu-id="de079-139">CSV</span></span>

<span data-ttu-id="de079-140">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="de079-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="de079-141">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="de079-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="de079-142">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="de079-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="de079-143">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="de079-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="de079-144">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="de079-144">Report Refresh Date</span></span>
- <span data-ttu-id="de079-145">受信した Exchange の電子メール</span><span class="sxs-lookup"><span data-stu-id="de079-145">Exchange Emails Received</span></span>
- <span data-ttu-id="de079-146">投稿された Yammer メッセージ</span><span class="sxs-lookup"><span data-stu-id="de079-146">Yammer Messages Posted</span></span>
- <span data-ttu-id="de079-147">読み取られた Yammer メッセージ</span><span class="sxs-lookup"><span data-stu-id="de079-147">Yammer Messages Read</span></span>
- <span data-ttu-id="de079-148">「いいね!」された Yammer メッセージ</span><span class="sxs-lookup"><span data-stu-id="de079-148">Yammer Messages Liked</span></span>
- <span data-ttu-id="de079-149">レポート日付</span><span class="sxs-lookup"><span data-stu-id="de079-149">Report Date</span></span>
- <span data-ttu-id="de079-150">レポート期間</span><span class="sxs-lookup"><span data-stu-id="de079-150">Report Period</span></span>

<span data-ttu-id="de079-151">21Vianet によって運営されて、Microsoft Graph 中国では、次の列はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="de079-151">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="de079-152">投稿された Yammer メッセージ</span><span class="sxs-lookup"><span data-stu-id="de079-152">Yammer Messages Posted</span></span>
- <span data-ttu-id="de079-153">読み取られた Yammer メッセージ</span><span class="sxs-lookup"><span data-stu-id="de079-153">Yammer Messages Read</span></span>
- <span data-ttu-id="de079-154">「いいね!」された Yammer メッセージ</span><span class="sxs-lookup"><span data-stu-id="de079-154">Yammer Messages Liked</span></span>

### <a name="json"></a><span data-ttu-id="de079-155">JSON</span><span class="sxs-lookup"><span data-stu-id="de079-155">JSON</span></span>

<span data-ttu-id="de079-156">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の**[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="de079-156">If successful, this method returns a `200 OK` response code and an **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** object in the response body.</span></span>

<span data-ttu-id="de079-157">21Vianet によって運営されて、Microsoft Graph 中国では、 **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** オブジェクトでは、次のプロパティはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="de079-157">The following properties in **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="de079-158">yammerMessagesPosted</span><span class="sxs-lookup"><span data-stu-id="de079-158">yammerMessagesPosted</span></span>
- <span data-ttu-id="de079-159">yammerMessagesRead</span><span class="sxs-lookup"><span data-stu-id="de079-159">yammerMessagesRead</span></span>
- <span data-ttu-id="de079-160">yammerMessagesLiked</span><span class="sxs-lookup"><span data-stu-id="de079-160">yammerMessagesLiked</span></span>

## <a name="example"></a><span data-ttu-id="de079-161">例</span><span class="sxs-lookup"><span data-stu-id="de079-161">Example</span></span>

### <a name="csv"></a><span data-ttu-id="de079-162">CSV</span><span class="sxs-lookup"><span data-stu-id="de079-162">CSV</span></span>

<span data-ttu-id="de079-163">次に、CSV を出力する例を示します。</span><span class="sxs-lookup"><span data-stu-id="de079-163">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="de079-164">要求</span><span class="sxs-lookup"><span data-stu-id="de079-164">Request</span></span>

<span data-ttu-id="de079-165">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="de079-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="de079-166">応答</span><span class="sxs-lookup"><span data-stu-id="de079-166">Response</span></span>

<span data-ttu-id="de079-167">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="de079-167">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="de079-168">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="de079-168">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="de079-169">JSON</span><span class="sxs-lookup"><span data-stu-id="de079-169">JSON</span></span>

<span data-ttu-id="de079-170">次に、JSON を取得する例を示します。</span><span class="sxs-lookup"><span data-stu-id="de079-170">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="de079-171">要求</span><span class="sxs-lookup"><span data-stu-id="de079-171">Request</span></span>

<span data-ttu-id="de079-172">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="de079-172">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="de079-173">応答</span><span class="sxs-lookup"><span data-stu-id="de079-173">Response</span></span>

<span data-ttu-id="de079-174">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="de079-174">The following is an example of the response.</span></span>

> <span data-ttu-id="de079-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="de079-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getoffice365groupsactivitycounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
