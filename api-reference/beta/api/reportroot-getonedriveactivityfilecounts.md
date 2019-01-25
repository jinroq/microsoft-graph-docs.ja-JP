---
title: 'reportRoot: getOneDriveActivityFileCounts'
description: いずれかの OneDrive アカウントに対してファイル操作を実行した、一意のライセンス ユーザーの数を取得します。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: e3a5d9cd840d47fd950330758e64b33625052904
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518353"
---
# <a name="reportroot-getonedriveactivityfilecounts"></a><span data-ttu-id="bae07-103">reportRoot: getOneDriveActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="bae07-103">reportRoot: getOneDriveActivityFileCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bae07-104">いずれかの OneDrive アカウントに対してファイル操作を実行した、一意のライセンス ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="bae07-104">Get the number of unique, licensed users that performed file interactions against any OneDrive account.</span></span>

> <span data-ttu-id="bae07-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: OneDrive for Business のアクティビティ](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bae07-105">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="permissions"></a><span data-ttu-id="bae07-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bae07-106">Permissions</span></span>

<span data-ttu-id="bae07-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bae07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bae07-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bae07-109">Permission type</span></span>                        | <span data-ttu-id="bae07-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bae07-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="bae07-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="bae07-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="bae07-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bae07-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="bae07-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bae07-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bae07-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bae07-114">Not supported.</span></span>                           |
| <span data-ttu-id="bae07-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bae07-115">Application</span></span>                            | <span data-ttu-id="bae07-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bae07-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="bae07-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bae07-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveActivityFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="bae07-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="bae07-118">Function parameters</span></span>

<span data-ttu-id="bae07-119">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="bae07-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="bae07-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="bae07-120">Parameter</span></span> | <span data-ttu-id="bae07-121">型</span><span class="sxs-lookup"><span data-stu-id="bae07-121">Type</span></span>   | <span data-ttu-id="bae07-122">説明</span><span class="sxs-lookup"><span data-stu-id="bae07-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="bae07-123">period</span><span class="sxs-lookup"><span data-stu-id="bae07-123">period</span></span>    | <span data-ttu-id="bae07-124">文字列</span><span class="sxs-lookup"><span data-stu-id="bae07-124">string</span></span> | <span data-ttu-id="bae07-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="bae07-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="bae07-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="bae07-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="bae07-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="bae07-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="bae07-128">必須。</span><span class="sxs-lookup"><span data-stu-id="bae07-128">Required.</span></span> |

<span data-ttu-id="bae07-129">このメソッドをサポートしている、 `$format` 、応答をカスタマイズするのには、 [OData クエリ パラメーター](/graph/query-parameters)です。</span><span class="sxs-lookup"><span data-stu-id="bae07-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="bae07-130">既定の出力の種類は、テキストまたは csv です。</span><span class="sxs-lookup"><span data-stu-id="bae07-130">The default output type is text/csv.</span></span> <span data-ttu-id="bae07-131">ただし、出力の種類を指定する場合は、設定をテキストまたは csv またはアプリケーションまたは json OData $format クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="bae07-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bae07-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bae07-132">Request headers</span></span>

| <span data-ttu-id="bae07-133">名前</span><span class="sxs-lookup"><span data-stu-id="bae07-133">Name</span></span>          | <span data-ttu-id="bae07-134">説明</span><span class="sxs-lookup"><span data-stu-id="bae07-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="bae07-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="bae07-135">Authorization</span></span> | <span data-ttu-id="bae07-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="bae07-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="bae07-138">応答</span><span class="sxs-lookup"><span data-stu-id="bae07-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="bae07-139">CSV</span><span class="sxs-lookup"><span data-stu-id="bae07-139">CSV</span></span>

<span data-ttu-id="bae07-140">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="bae07-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="bae07-141">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="bae07-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="bae07-142">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="bae07-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="bae07-143">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="bae07-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="bae07-144">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="bae07-144">Report Refresh Date</span></span>
- <span data-ttu-id="bae07-145">表示済みまたは編集済み</span><span class="sxs-lookup"><span data-stu-id="bae07-145">Viewed Or Edited</span></span>
- <span data-ttu-id="bae07-146">同期済み</span><span class="sxs-lookup"><span data-stu-id="bae07-146">Synced</span></span>
- <span data-ttu-id="bae07-147">社内で共有済み</span><span class="sxs-lookup"><span data-stu-id="bae07-147">Shared Internally</span></span>
- <span data-ttu-id="bae07-148">外部で共有済み</span><span class="sxs-lookup"><span data-stu-id="bae07-148">Shared Externally</span></span>
- <span data-ttu-id="bae07-149">レポート日付</span><span class="sxs-lookup"><span data-stu-id="bae07-149">Report Date</span></span>
- <span data-ttu-id="bae07-150">レポート期間</span><span class="sxs-lookup"><span data-stu-id="bae07-150">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="bae07-151">JSON</span><span class="sxs-lookup"><span data-stu-id="bae07-151">JSON</span></span>

<span data-ttu-id="bae07-152">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に**[siteActivitySummary](../resources/siteactivitysummary.md)** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="bae07-152">If successful, this method returns a `200 OK` response code and a **[siteActivitySummary](../resources/siteactivitysummary.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bae07-153">例</span><span class="sxs-lookup"><span data-stu-id="bae07-153">Example</span></span>

### <a name="csv"></a><span data-ttu-id="bae07-154">CSV</span><span class="sxs-lookup"><span data-stu-id="bae07-154">CSV</span></span>

<span data-ttu-id="bae07-155">次に、CSV を出力する例を示します。</span><span class="sxs-lookup"><span data-stu-id="bae07-155">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="bae07-156">要求</span><span class="sxs-lookup"><span data-stu-id="bae07-156">Request</span></span>

<span data-ttu-id="bae07-157">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="bae07-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveactivityfilecounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveActivityFileCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="bae07-158">応答</span><span class="sxs-lookup"><span data-stu-id="bae07-158">Response</span></span>

<span data-ttu-id="bae07-159">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="bae07-159">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="bae07-160">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="bae07-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="bae07-161">JSON</span><span class="sxs-lookup"><span data-stu-id="bae07-161">JSON</span></span>

<span data-ttu-id="bae07-162">次に、JSON を取得する例を示します。</span><span class="sxs-lookup"><span data-stu-id="bae07-162">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="bae07-163">要求</span><span class="sxs-lookup"><span data-stu-id="bae07-163">Request</span></span>

<span data-ttu-id="bae07-164">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="bae07-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveactivityfilecounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveActivityFileCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="bae07-165">応答</span><span class="sxs-lookup"><span data-stu-id="bae07-165">Response</span></span>

<span data-ttu-id="bae07-166">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="bae07-166">The following is an example of the response.</span></span>

> <span data-ttu-id="bae07-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="bae07-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.siteActivitySummary"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 280

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.siteActivitySummary)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "viewedOrEdited": 1997, 
      "synced": 24756, 
      "sharedInternally": 7, 
      "sharedExternally": 0, 
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
    "Error: /api-reference/beta/api/reportroot-getonedriveactivityfilecounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
