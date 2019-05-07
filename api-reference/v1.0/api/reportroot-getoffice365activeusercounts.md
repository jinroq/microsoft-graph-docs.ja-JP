---
title: 'reportRoot: getOffice365ActiveUserCounts'
description: レポート期間中の日ごとのアクティブ ユーザー数を製品別に取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 537058ce5132e4385e08f123f8a3075f87892290
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33606573"
---
# <a name="reportroot-getoffice365activeusercounts"></a><span data-ttu-id="b0856-103">reportRoot: getOffice365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="b0856-103">reportRoot: getOffice365ActiveUserCounts</span></span>

<span data-ttu-id="b0856-104">レポート期間中の日ごとのアクティブ ユーザー数を製品別に取得します。</span><span class="sxs-lookup"><span data-stu-id="b0856-104">Get the count of daily active users in the reporting period by product.</span></span>

> <span data-ttu-id="b0856-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: アクティブ ユーザー](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b0856-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="b0856-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b0856-106">Permissions</span></span>

<span data-ttu-id="b0856-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b0856-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b0856-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b0856-109">Permission type</span></span>                        | <span data-ttu-id="b0856-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b0856-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b0856-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="b0856-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b0856-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b0856-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b0856-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b0856-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0856-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b0856-114">Not supported.</span></span>                           |
| <span data-ttu-id="b0856-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b0856-115">Application</span></span>                            | <span data-ttu-id="b0856-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b0856-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="b0856-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b0856-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="b0856-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="b0856-118">Function parameters</span></span>

<span data-ttu-id="b0856-119">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="b0856-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="b0856-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="b0856-120">Parameter</span></span> | <span data-ttu-id="b0856-121">型</span><span class="sxs-lookup"><span data-stu-id="b0856-121">Type</span></span>   | <span data-ttu-id="b0856-122">説明</span><span class="sxs-lookup"><span data-stu-id="b0856-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b0856-123">period</span><span class="sxs-lookup"><span data-stu-id="b0856-123">period</span></span>    | <span data-ttu-id="b0856-124">文字列</span><span class="sxs-lookup"><span data-stu-id="b0856-124">string</span></span> | <span data-ttu-id="b0856-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="b0856-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b0856-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="b0856-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b0856-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="b0856-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="b0856-128">必須。</span><span class="sxs-lookup"><span data-stu-id="b0856-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="b0856-129">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b0856-129">Request headers</span></span>

| <span data-ttu-id="b0856-130">名前</span><span class="sxs-lookup"><span data-stu-id="b0856-130">Name</span></span>          | <span data-ttu-id="b0856-131">説明</span><span class="sxs-lookup"><span data-stu-id="b0856-131">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="b0856-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0856-132">Authorization</span></span> | <span data-ttu-id="b0856-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b0856-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="b0856-135">応答</span><span class="sxs-lookup"><span data-stu-id="b0856-135">Response</span></span>

<span data-ttu-id="b0856-136">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="b0856-136">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b0856-137">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="b0856-137">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b0856-138">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="b0856-138">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b0856-139">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="b0856-139">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b0856-140">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="b0856-140">Report Refresh Date</span></span>
- <span data-ttu-id="b0856-141">Office 365</span><span class="sxs-lookup"><span data-stu-id="b0856-141">Office 365</span></span>
- <span data-ttu-id="b0856-142">Exchange</span><span class="sxs-lookup"><span data-stu-id="b0856-142">Exchange</span></span>
- <span data-ttu-id="b0856-143">OneDrive</span><span class="sxs-lookup"><span data-stu-id="b0856-143">OneDrive</span></span>
- <span data-ttu-id="b0856-144">SharePoint</span><span class="sxs-lookup"><span data-stu-id="b0856-144">SharePoint</span></span>
- <span data-ttu-id="b0856-145">Skype For Business</span><span class="sxs-lookup"><span data-stu-id="b0856-145">Skype For Business</span></span> 
- <span data-ttu-id="b0856-146">Yammer</span><span class="sxs-lookup"><span data-stu-id="b0856-146">Yammer</span></span>
- <span data-ttu-id="b0856-147">Teams</span><span class="sxs-lookup"><span data-stu-id="b0856-147">Teams</span></span>
- <span data-ttu-id="b0856-148">レポート日付</span><span class="sxs-lookup"><span data-stu-id="b0856-148">Report Date</span></span>
- <span data-ttu-id="b0856-149">レポート期間</span><span class="sxs-lookup"><span data-stu-id="b0856-149">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="b0856-150">例</span><span class="sxs-lookup"><span data-stu-id="b0856-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b0856-151">要求</span><span class="sxs-lookup"><span data-stu-id="b0856-151">Request</span></span>

<span data-ttu-id="b0856-152">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b0856-152">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activeusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActiveUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="b0856-153">応答</span><span class="sxs-lookup"><span data-stu-id="b0856-153">Response</span></span>

<span data-ttu-id="b0856-154">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b0856-154">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="b0856-155">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="b0856-155">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b0856-156">Visual</span><span class="sxs-lookup"><span data-stu-id="b0856-156">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activeusercounts-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b0856-157">Java</span><span class="sxs-lookup"><span data-stu-id="b0856-157">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activeusercounts-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="b0856-158">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="b0856-158">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Office 365,Exchange,OneDrive,SharePoint,Skype For Business,Yammer,Teams,Report Date,Report Period
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
    "Error: /api-reference/v1.0/api/reportroot-getoffice365activeusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getoffice365activeusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
