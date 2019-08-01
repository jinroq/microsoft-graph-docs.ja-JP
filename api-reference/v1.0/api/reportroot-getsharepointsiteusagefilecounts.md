---
title: 'reportRoot: getSharePointSiteUsageFileCounts'
description: すべてのサイトのファイルの合計数と、アクティブ ファイルの数を取得します。 ファイル (ユーザーまたはシステム) は、一定期間中に保存、同期、変更、共有されるとアクティブとみなされます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 8c74719cad238d80a156ea88d04b6c29eeddb12b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36021848"
---
# <a name="reportroot-getsharepointsiteusagefilecounts"></a><span data-ttu-id="c2402-104">reportRoot: getSharePointSiteUsageFileCounts</span><span class="sxs-lookup"><span data-stu-id="c2402-104">reportRoot: getSharePointSiteUsageFileCounts</span></span>

<span data-ttu-id="c2402-105">すべてのサイトのファイルの合計数と、アクティブ ファイルの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="c2402-105">Get the total number of files across all sites and the number of active files.</span></span> <span data-ttu-id="c2402-106">ファイル (ユーザーまたはシステム) は、一定期間中に保存、同期、変更、共有されるとアクティブとみなされます。</span><span class="sxs-lookup"><span data-stu-id="c2402-106">A file (user or system) is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span>

> <span data-ttu-id="c2402-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: SharePoint サイトの使用状況](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c2402-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="c2402-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c2402-108">Permissions</span></span>

<span data-ttu-id="c2402-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c2402-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c2402-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c2402-111">Permission type</span></span>                        | <span data-ttu-id="c2402-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c2402-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="c2402-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="c2402-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="c2402-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2402-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="c2402-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c2402-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2402-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c2402-116">Not supported.</span></span>                           |
| <span data-ttu-id="c2402-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c2402-117">Application</span></span>                            | <span data-ttu-id="c2402-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2402-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="c2402-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c2402-119">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c2402-120">プロトコル</span><span class="sxs-lookup"><span data-stu-id="c2402-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="c2402-121">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="c2402-121">Function parameters</span></span>

<span data-ttu-id="c2402-122">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="c2402-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="c2402-123">パラメーター</span><span class="sxs-lookup"><span data-stu-id="c2402-123">Parameter</span></span> | <span data-ttu-id="c2402-124">型</span><span class="sxs-lookup"><span data-stu-id="c2402-124">Type</span></span>   | <span data-ttu-id="c2402-125">説明</span><span class="sxs-lookup"><span data-stu-id="c2402-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="c2402-126">period</span><span class="sxs-lookup"><span data-stu-id="c2402-126">period</span></span>    | <span data-ttu-id="c2402-127">文字列</span><span class="sxs-lookup"><span data-stu-id="c2402-127">string</span></span> | <span data-ttu-id="c2402-128">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="c2402-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="c2402-129">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="c2402-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="c2402-130">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="c2402-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="c2402-131">必須。</span><span class="sxs-lookup"><span data-stu-id="c2402-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="c2402-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c2402-132">Request headers</span></span>

| <span data-ttu-id="c2402-133">名前</span><span class="sxs-lookup"><span data-stu-id="c2402-133">Name</span></span>          | <span data-ttu-id="c2402-134">説明</span><span class="sxs-lookup"><span data-stu-id="c2402-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="c2402-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2402-135">Authorization</span></span> | <span data-ttu-id="c2402-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c2402-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="c2402-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="c2402-138">If-None-Match</span></span> | <span data-ttu-id="c2402-139">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="c2402-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="c2402-140">省略可能。</span><span class="sxs-lookup"><span data-stu-id="c2402-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="c2402-141">応答</span><span class="sxs-lookup"><span data-stu-id="c2402-141">Response</span></span>

<span data-ttu-id="c2402-142">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="c2402-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="c2402-143">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="c2402-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="c2402-144">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="c2402-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="c2402-145">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="c2402-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="c2402-146">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="c2402-146">Report Refresh Date</span></span>
- <span data-ttu-id="c2402-147">サイトの種類</span><span class="sxs-lookup"><span data-stu-id="c2402-147">Site Type</span></span>
- <span data-ttu-id="c2402-148">合計</span><span class="sxs-lookup"><span data-stu-id="c2402-148">Total</span></span>
- <span data-ttu-id="c2402-149">アクティブ</span><span class="sxs-lookup"><span data-stu-id="c2402-149">Active</span></span>
- <span data-ttu-id="c2402-150">レポート日付</span><span class="sxs-lookup"><span data-stu-id="c2402-150">Report Date</span></span>
- <span data-ttu-id="c2402-151">レポート期間</span><span class="sxs-lookup"><span data-stu-id="c2402-151">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="c2402-152">例</span><span class="sxs-lookup"><span data-stu-id="c2402-152">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c2402-153">要求</span><span class="sxs-lookup"><span data-stu-id="c2402-153">Request</span></span>

<span data-ttu-id="c2402-154">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c2402-154">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getsharepointsiteusagefilecounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointSiteUsageFileCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c2402-155">C#</span><span class="sxs-lookup"><span data-stu-id="c2402-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointsiteusagefilecounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c2402-156">Javascript</span><span class="sxs-lookup"><span data-stu-id="c2402-156">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointsiteusagefilecounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c2402-157">目的-C</span><span class="sxs-lookup"><span data-stu-id="c2402-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointsiteusagefilecounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c2402-158">Java</span><span class="sxs-lookup"><span data-stu-id="c2402-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getsharepointsiteusagefilecounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c2402-159">応答</span><span class="sxs-lookup"><span data-stu-id="c2402-159">Response</span></span>

<span data-ttu-id="c2402-160">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c2402-160">The following is an example of the response.</span></span>

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

<span data-ttu-id="c2402-161">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="c2402-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
