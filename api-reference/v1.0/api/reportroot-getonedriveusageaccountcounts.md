---
title: 'reportRoot: getOneDriveUsageAccountCounts'
description: アクティブな OneDrive for Business サイトの数の傾向を取得します。 ユーザーがファイルを表示、変更、アップロード、ダウンロード、共有、同期したサイトはすべて、アクティブなサイトとみなされます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: c4e77ff214a5183d18fd4ee3f72d13b20b2a3ab8
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35449597"
---
# <a name="reportroot-getonedriveusageaccountcounts"></a><span data-ttu-id="534e2-104">reportRoot: getOneDriveUsageAccountCounts</span><span class="sxs-lookup"><span data-stu-id="534e2-104">reportRoot: getOneDriveUsageAccountCounts</span></span>

<span data-ttu-id="534e2-105">アクティブな OneDrive for Business サイトの数の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="534e2-105">Get the trend in the number of active OneDrive for Business sites.</span></span> <span data-ttu-id="534e2-106">ユーザーがファイルを表示、変更、アップロード、ダウンロード、共有、同期したサイトはすべて、アクティブなサイトとみなされます。</span><span class="sxs-lookup"><span data-stu-id="534e2-106">Any site on which users viewed, modified, uploaded, downloaded, shared, or synced files is considered an active site.</span></span>

> <span data-ttu-id="534e2-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: OneDrive for Business の使用状況](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="534e2-107">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="534e2-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="534e2-108">Permissions</span></span>

<span data-ttu-id="534e2-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="534e2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="534e2-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="534e2-111">Permission type</span></span>                        | <span data-ttu-id="534e2-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="534e2-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="534e2-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="534e2-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="534e2-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="534e2-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="534e2-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="534e2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="534e2-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="534e2-116">Not supported.</span></span>                           |
| <span data-ttu-id="534e2-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="534e2-117">Application</span></span>                            | <span data-ttu-id="534e2-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="534e2-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="534e2-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="534e2-119">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="534e2-120">プロトコル</span><span class="sxs-lookup"><span data-stu-id="534e2-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageAccountCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="534e2-121">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="534e2-121">Function parameters</span></span>

<span data-ttu-id="534e2-122">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="534e2-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="534e2-123">パラメーター</span><span class="sxs-lookup"><span data-stu-id="534e2-123">Parameter</span></span> | <span data-ttu-id="534e2-124">型</span><span class="sxs-lookup"><span data-stu-id="534e2-124">Type</span></span>   | <span data-ttu-id="534e2-125">説明</span><span class="sxs-lookup"><span data-stu-id="534e2-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="534e2-126">period</span><span class="sxs-lookup"><span data-stu-id="534e2-126">period</span></span>    | <span data-ttu-id="534e2-127">文字列</span><span class="sxs-lookup"><span data-stu-id="534e2-127">string</span></span> | <span data-ttu-id="534e2-128">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="534e2-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="534e2-129">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="534e2-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="534e2-130">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="534e2-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="534e2-131">必須。</span><span class="sxs-lookup"><span data-stu-id="534e2-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="534e2-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="534e2-132">Request headers</span></span>

| <span data-ttu-id="534e2-133">名前</span><span class="sxs-lookup"><span data-stu-id="534e2-133">Name</span></span>          | <span data-ttu-id="534e2-134">説明</span><span class="sxs-lookup"><span data-stu-id="534e2-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="534e2-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="534e2-135">Authorization</span></span> | <span data-ttu-id="534e2-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="534e2-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="534e2-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="534e2-138">If-None-Match</span></span> | <span data-ttu-id="534e2-139">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="534e2-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="534e2-140">省略可能。</span><span class="sxs-lookup"><span data-stu-id="534e2-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="534e2-141">応答</span><span class="sxs-lookup"><span data-stu-id="534e2-141">Response</span></span>

<span data-ttu-id="534e2-142">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="534e2-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="534e2-143">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="534e2-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="534e2-144">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="534e2-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="534e2-145">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="534e2-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="534e2-146">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="534e2-146">Report Refresh Date</span></span>
- <span data-ttu-id="534e2-147">サイトの種類</span><span class="sxs-lookup"><span data-stu-id="534e2-147">Site Type</span></span>
- <span data-ttu-id="534e2-148">合計</span><span class="sxs-lookup"><span data-stu-id="534e2-148">Total</span></span>
- <span data-ttu-id="534e2-149">アクティブ</span><span class="sxs-lookup"><span data-stu-id="534e2-149">Active</span></span>
- <span data-ttu-id="534e2-150">レポート日付</span><span class="sxs-lookup"><span data-stu-id="534e2-150">Report Date</span></span>
- <span data-ttu-id="534e2-151">レポート期間</span><span class="sxs-lookup"><span data-stu-id="534e2-151">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="534e2-152">例</span><span class="sxs-lookup"><span data-stu-id="534e2-152">Example</span></span>

#### <a name="request"></a><span data-ttu-id="534e2-153">要求</span><span class="sxs-lookup"><span data-stu-id="534e2-153">Request</span></span>

<span data-ttu-id="534e2-154">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="534e2-154">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getonedriveusageaccountcounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOneDriveUsageAccountCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="534e2-155">C#</span><span class="sxs-lookup"><span data-stu-id="534e2-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveusageaccountcounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="534e2-156">Javascript</span><span class="sxs-lookup"><span data-stu-id="534e2-156">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveusageaccountcounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="534e2-157">目的-C</span><span class="sxs-lookup"><span data-stu-id="534e2-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveusageaccountcounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="534e2-158">応答</span><span class="sxs-lookup"><span data-stu-id="534e2-158">Response</span></span>

<span data-ttu-id="534e2-159">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="534e2-159">The following is an example of the response.</span></span>

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

<span data-ttu-id="534e2-160">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="534e2-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
