---
title: 'reportRoot: getOneDriveUsageFileCounts'
description: すべてのサイトのファイル合計数と、アクティブ ファイルの数を取得します。 ファイルは一定期間中に保存、同期、変更、共有されるとアクティブとみなされます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 5654cc2d8ba9aaaa5f7572a784dc9d002806d0b5
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893609"
---
# <a name="reportroot-getonedriveusagefilecounts"></a><span data-ttu-id="c49f5-104">reportRoot: getOneDriveUsageFileCounts</span><span class="sxs-lookup"><span data-stu-id="c49f5-104">reportRoot: getOneDriveUsageFileCounts</span></span>

<span data-ttu-id="c49f5-105">すべてのサイトのファイル合計数と、アクティブ ファイルの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="c49f5-105">Get the total number of files across all sites and how many are active files.</span></span> <span data-ttu-id="c49f5-106">ファイルは一定期間中に保存、同期、変更、共有されるとアクティブとみなされます。</span><span class="sxs-lookup"><span data-stu-id="c49f5-106">A file is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span>

> <span data-ttu-id="c49f5-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: OneDrive for Business の使用状況](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c49f5-107">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="c49f5-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c49f5-108">Permissions</span></span>

<span data-ttu-id="c49f5-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c49f5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c49f5-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c49f5-111">Permission type</span></span>                        | <span data-ttu-id="c49f5-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c49f5-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="c49f5-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="c49f5-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="c49f5-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c49f5-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="c49f5-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c49f5-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c49f5-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c49f5-116">Not supported.</span></span>                           |
| <span data-ttu-id="c49f5-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c49f5-117">Application</span></span>                            | <span data-ttu-id="c49f5-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c49f5-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="c49f5-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c49f5-119">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c49f5-120">プロトコル</span><span class="sxs-lookup"><span data-stu-id="c49f5-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="c49f5-121">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="c49f5-121">Function parameters</span></span>

<span data-ttu-id="c49f5-122">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="c49f5-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="c49f5-123">パラメーター</span><span class="sxs-lookup"><span data-stu-id="c49f5-123">Parameter</span></span> | <span data-ttu-id="c49f5-124">型</span><span class="sxs-lookup"><span data-stu-id="c49f5-124">Type</span></span>   | <span data-ttu-id="c49f5-125">説明</span><span class="sxs-lookup"><span data-stu-id="c49f5-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="c49f5-126">period</span><span class="sxs-lookup"><span data-stu-id="c49f5-126">period</span></span>    | <span data-ttu-id="c49f5-127">文字列</span><span class="sxs-lookup"><span data-stu-id="c49f5-127">string</span></span> | <span data-ttu-id="c49f5-128">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="c49f5-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="c49f5-129">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="c49f5-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="c49f5-130">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="c49f5-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="c49f5-131">必須。</span><span class="sxs-lookup"><span data-stu-id="c49f5-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="c49f5-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c49f5-132">Request headers</span></span>

| <span data-ttu-id="c49f5-133">名前</span><span class="sxs-lookup"><span data-stu-id="c49f5-133">Name</span></span>          | <span data-ttu-id="c49f5-134">説明</span><span class="sxs-lookup"><span data-stu-id="c49f5-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="c49f5-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="c49f5-135">Authorization</span></span> | <span data-ttu-id="c49f5-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c49f5-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="c49f5-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="c49f5-138">If-None-Match</span></span> | <span data-ttu-id="c49f5-139">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="c49f5-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="c49f5-140">省略可能。</span><span class="sxs-lookup"><span data-stu-id="c49f5-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="c49f5-141">応答</span><span class="sxs-lookup"><span data-stu-id="c49f5-141">Response</span></span>

<span data-ttu-id="c49f5-142">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="c49f5-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="c49f5-143">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="c49f5-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="c49f5-144">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="c49f5-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="c49f5-145">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="c49f5-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="c49f5-146">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="c49f5-146">Report Refresh Date</span></span>
- <span data-ttu-id="c49f5-147">サイトの種類</span><span class="sxs-lookup"><span data-stu-id="c49f5-147">Site Type</span></span>
- <span data-ttu-id="c49f5-148">合計</span><span class="sxs-lookup"><span data-stu-id="c49f5-148">Total</span></span>
- <span data-ttu-id="c49f5-149">アクティブ</span><span class="sxs-lookup"><span data-stu-id="c49f5-149">Active</span></span>
- <span data-ttu-id="c49f5-150">レポート日付</span><span class="sxs-lookup"><span data-stu-id="c49f5-150">Report Date</span></span>
- <span data-ttu-id="c49f5-151">レポート期間</span><span class="sxs-lookup"><span data-stu-id="c49f5-151">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="c49f5-152">例</span><span class="sxs-lookup"><span data-stu-id="c49f5-152">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c49f5-153">要求</span><span class="sxs-lookup"><span data-stu-id="c49f5-153">Request</span></span>

<span data-ttu-id="c49f5-154">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c49f5-154">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getonedriveusagefilecounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOneDriveUsageFileCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c49f5-155">C#</span><span class="sxs-lookup"><span data-stu-id="c49f5-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveusagefilecounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c49f5-156">Javascript</span><span class="sxs-lookup"><span data-stu-id="c49f5-156">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveusagefilecounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c49f5-157">目的-C</span><span class="sxs-lookup"><span data-stu-id="c49f5-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveusagefilecounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c49f5-158">Java</span><span class="sxs-lookup"><span data-stu-id="c49f5-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getonedriveusagefilecounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c49f5-159">応答</span><span class="sxs-lookup"><span data-stu-id="c49f5-159">Response</span></span>

<span data-ttu-id="c49f5-160">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c49f5-160">The following is an example of the response.</span></span>

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

<span data-ttu-id="c49f5-161">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="c49f5-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Total,Active,Report Date,Report Period
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
