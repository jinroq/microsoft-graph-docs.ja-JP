---
title: 'reportRoot: getSharePointSiteUsageStorage'
description: レポート期間中に割り当てられ、消費したストレージの傾向を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 1503def2d2096dbd575afa21770eeb6a9097989f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36025009"
---
# <a name="reportroot-getsharepointsiteusagestorage"></a><span data-ttu-id="1e949-103">reportRoot: getSharePointSiteUsageStorage</span><span class="sxs-lookup"><span data-stu-id="1e949-103">reportRoot: getSharePointSiteUsageStorage</span></span>

<span data-ttu-id="1e949-104">レポート期間中に割り当てられ、消費したストレージの傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="1e949-104">Get the trend of storage allocated and consumed during the reporting period.</span></span>

> <span data-ttu-id="1e949-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: SharePoint サイトの使用状況](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1e949-105">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="1e949-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1e949-106">Permissions</span></span>

<span data-ttu-id="1e949-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1e949-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1e949-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1e949-109">Permission type</span></span>                        | <span data-ttu-id="1e949-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1e949-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="1e949-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="1e949-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1e949-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1e949-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="1e949-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1e949-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e949-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1e949-114">Not supported.</span></span>                           |
| <span data-ttu-id="1e949-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1e949-115">Application</span></span>                            | <span data-ttu-id="1e949-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1e949-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="1e949-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1e949-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="1e949-118">プロトコル</span><span class="sxs-lookup"><span data-stu-id="1e949-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageStorage(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="1e949-119">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="1e949-119">Function parameters</span></span>

<span data-ttu-id="1e949-120">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="1e949-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="1e949-121">パラメーター</span><span class="sxs-lookup"><span data-stu-id="1e949-121">Parameter</span></span> | <span data-ttu-id="1e949-122">型</span><span class="sxs-lookup"><span data-stu-id="1e949-122">Type</span></span>   | <span data-ttu-id="1e949-123">説明</span><span class="sxs-lookup"><span data-stu-id="1e949-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="1e949-124">period</span><span class="sxs-lookup"><span data-stu-id="1e949-124">period</span></span>    | <span data-ttu-id="1e949-125">文字列</span><span class="sxs-lookup"><span data-stu-id="1e949-125">string</span></span> | <span data-ttu-id="1e949-126">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="1e949-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="1e949-127">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="1e949-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="1e949-128">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="1e949-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="1e949-129">必須。</span><span class="sxs-lookup"><span data-stu-id="1e949-129">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="1e949-130">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1e949-130">Request headers</span></span>

| <span data-ttu-id="1e949-131">名前</span><span class="sxs-lookup"><span data-stu-id="1e949-131">Name</span></span>          | <span data-ttu-id="1e949-132">説明</span><span class="sxs-lookup"><span data-stu-id="1e949-132">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="1e949-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e949-133">Authorization</span></span> | <span data-ttu-id="1e949-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1e949-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="1e949-136">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="1e949-136">If-None-Match</span></span> | <span data-ttu-id="1e949-137">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="1e949-137">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="1e949-138">省略可能。</span><span class="sxs-lookup"><span data-stu-id="1e949-138">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="1e949-139">応答</span><span class="sxs-lookup"><span data-stu-id="1e949-139">Response</span></span>

<span data-ttu-id="1e949-140">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="1e949-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="1e949-141">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="1e949-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="1e949-142">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="1e949-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="1e949-143">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="1e949-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="1e949-144">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="1e949-144">Report Refresh Date</span></span>
- <span data-ttu-id="1e949-145">サイトの種類</span><span class="sxs-lookup"><span data-stu-id="1e949-145">Site Type</span></span>
- <span data-ttu-id="1e949-146">使用済みストレージ (バイト)</span><span class="sxs-lookup"><span data-stu-id="1e949-146">Storage Used (Byte)</span></span>
- <span data-ttu-id="1e949-147">レポート日付</span><span class="sxs-lookup"><span data-stu-id="1e949-147">Report Date</span></span>
- <span data-ttu-id="1e949-148">レポート期間</span><span class="sxs-lookup"><span data-stu-id="1e949-148">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="1e949-149">例</span><span class="sxs-lookup"><span data-stu-id="1e949-149">Example</span></span>

#### <a name="request"></a><span data-ttu-id="1e949-150">要求</span><span class="sxs-lookup"><span data-stu-id="1e949-150">Request</span></span>

<span data-ttu-id="1e949-151">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1e949-151">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getsharepointsiteusagestorage"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointSiteUsageStorage(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1e949-152">C#</span><span class="sxs-lookup"><span data-stu-id="1e949-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointsiteusagestorage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1e949-153">Javascript</span><span class="sxs-lookup"><span data-stu-id="1e949-153">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointsiteusagestorage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1e949-154">目的-C</span><span class="sxs-lookup"><span data-stu-id="1e949-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointsiteusagestorage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1e949-155">Java</span><span class="sxs-lookup"><span data-stu-id="1e949-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getsharepointsiteusagestorage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1e949-156">応答</span><span class="sxs-lookup"><span data-stu-id="1e949-156">Response</span></span>

<span data-ttu-id="1e949-157">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1e949-157">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.report"
} -->

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="1e949-158">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="1e949-158">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Storage Used (Byte),Report Date,Report Period
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
