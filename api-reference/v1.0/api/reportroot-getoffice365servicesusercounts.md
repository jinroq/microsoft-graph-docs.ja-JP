---
title: 'reportRoot: getOffice365ServicesUserCounts'
description: アクティビティの種類とサービス別のユーザー数を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 9cf9af433e99db343e1ed5678f497b6d23aa7cd9
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33605000"
---
# <a name="reportroot-getoffice365servicesusercounts"></a><span data-ttu-id="828a4-103">reportRoot: getOffice365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="828a4-103">reportRoot: getOffice365ServicesUserCounts</span></span>

<span data-ttu-id="828a4-104">アクティビティの種類とサービス別のユーザー数を取得します。</span><span class="sxs-lookup"><span data-stu-id="828a4-104">Get the count of users by activity type and service.</span></span>

> <span data-ttu-id="828a4-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: アクティブ ユーザー](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="828a4-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="828a4-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="828a4-106">Permissions</span></span>

<span data-ttu-id="828a4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="828a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="828a4-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="828a4-109">Permission type</span></span>                        | <span data-ttu-id="828a4-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="828a4-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="828a4-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="828a4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="828a4-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="828a4-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="828a4-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="828a4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="828a4-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="828a4-114">Not supported.</span></span>                           |
| <span data-ttu-id="828a4-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="828a4-115">Application</span></span>                            | <span data-ttu-id="828a4-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="828a4-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="828a4-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="828a4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ServicesUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="828a4-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="828a4-118">Function parameters</span></span>

<span data-ttu-id="828a4-119">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="828a4-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="828a4-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="828a4-120">Parameter</span></span> | <span data-ttu-id="828a4-121">型</span><span class="sxs-lookup"><span data-stu-id="828a4-121">Type</span></span>   | <span data-ttu-id="828a4-122">説明</span><span class="sxs-lookup"><span data-stu-id="828a4-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="828a4-123">period</span><span class="sxs-lookup"><span data-stu-id="828a4-123">period</span></span>    | <span data-ttu-id="828a4-124">文字列</span><span class="sxs-lookup"><span data-stu-id="828a4-124">string</span></span> | <span data-ttu-id="828a4-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="828a4-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="828a4-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="828a4-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="828a4-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="828a4-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="828a4-128">必須。</span><span class="sxs-lookup"><span data-stu-id="828a4-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="828a4-129">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="828a4-129">Request headers</span></span>

| <span data-ttu-id="828a4-130">名前</span><span class="sxs-lookup"><span data-stu-id="828a4-130">Name</span></span>          | <span data-ttu-id="828a4-131">説明</span><span class="sxs-lookup"><span data-stu-id="828a4-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="828a4-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="828a4-132">Authorization</span></span> | <span data-ttu-id="828a4-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="828a4-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="828a4-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="828a4-135">If-None-Match</span></span> | <span data-ttu-id="828a4-136">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="828a4-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="828a4-137">省略可能。</span><span class="sxs-lookup"><span data-stu-id="828a4-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="828a4-138">応答</span><span class="sxs-lookup"><span data-stu-id="828a4-138">Response</span></span>

<span data-ttu-id="828a4-139">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="828a4-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="828a4-140">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="828a4-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="828a4-141">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="828a4-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="828a4-142">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="828a4-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="828a4-143">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="828a4-143">Report Refresh Date</span></span>
- <span data-ttu-id="828a4-144">Exchange アクティブ</span><span class="sxs-lookup"><span data-stu-id="828a4-144">Exchange Active</span></span>
- <span data-ttu-id="828a4-145">Exchange 非アクティブ</span><span class="sxs-lookup"><span data-stu-id="828a4-145">Exchange Inactive</span></span>
- <span data-ttu-id="828a4-146">OneDrive アクティブ</span><span class="sxs-lookup"><span data-stu-id="828a4-146">OneDrive Active</span></span>
- <span data-ttu-id="828a4-147">OneDrive 非アクティブ</span><span class="sxs-lookup"><span data-stu-id="828a4-147">OneDrive Inactive</span></span>
- <span data-ttu-id="828a4-148">SharePoint アクティブ</span><span class="sxs-lookup"><span data-stu-id="828a4-148">SharePoint Active</span></span>
- <span data-ttu-id="828a4-149">SharePoint 非アクティブ</span><span class="sxs-lookup"><span data-stu-id="828a4-149">SharePoint Inactive</span></span>
- <span data-ttu-id="828a4-150">Skype For Business アクティブ</span><span class="sxs-lookup"><span data-stu-id="828a4-150">Skype For Business Active</span></span>
- <span data-ttu-id="828a4-151">Skype For Business 非アクティブ</span><span class="sxs-lookup"><span data-stu-id="828a4-151">Skype For Business Inactive</span></span>
- <span data-ttu-id="828a4-152">Yammer アクティブ</span><span class="sxs-lookup"><span data-stu-id="828a4-152">Yammer Active</span></span>
- <span data-ttu-id="828a4-153">Yammer 非アクティブ</span><span class="sxs-lookup"><span data-stu-id="828a4-153">Yammer Inactive</span></span>
- <span data-ttu-id="828a4-154">Teams アクティブ</span><span class="sxs-lookup"><span data-stu-id="828a4-154">Teams Active</span></span>
- <span data-ttu-id="828a4-155">Teams 非アクティブ</span><span class="sxs-lookup"><span data-stu-id="828a4-155">Teams Inactive</span></span>
- <span data-ttu-id="828a4-156">レポート期間</span><span class="sxs-lookup"><span data-stu-id="828a4-156">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="828a4-157">例</span><span class="sxs-lookup"><span data-stu-id="828a4-157">Example</span></span>

#### <a name="request"></a><span data-ttu-id="828a4-158">要求</span><span class="sxs-lookup"><span data-stu-id="828a4-158">Request</span></span>

<span data-ttu-id="828a4-159">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="828a4-159">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365servicesusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ServicesUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="828a4-160">応答</span><span class="sxs-lookup"><span data-stu-id="828a4-160">Response</span></span>

<span data-ttu-id="828a4-161">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="828a4-161">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="828a4-162">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="828a4-162">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="828a4-163">Visual</span><span class="sxs-lookup"><span data-stu-id="828a4-163">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365servicesusercounts-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="828a4-164">Java</span><span class="sxs-lookup"><span data-stu-id="828a4-164">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365servicesusercounts-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="828a4-165">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="828a4-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Exchange Active,Exchange Inactive,OneDrive Active,OneDrive Inactive,SharePoint Active,SharePoint Inactive,Skype For Business Active,Skype For Business Inactive,Yammer Active,Yammer Inactive,Teams Active,Teams Inactive,Report Period
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
    "Error: /api-reference/v1.0/api/reportroot-getoffice365servicesusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getoffice365servicesusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
