---
title: 'reportRoot: getOffice365ServicesUserCounts'
description: アクティビティの種類とサービス別のユーザー数を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: d349ce28ee903934fd84135a871aeeebd0771969
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36422301"
---
# <a name="reportroot-getoffice365servicesusercounts"></a><span data-ttu-id="87535-103">reportRoot: getOffice365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="87535-103">reportRoot: getOffice365ServicesUserCounts</span></span>

<span data-ttu-id="87535-104">アクティビティの種類とサービス別のユーザー数を取得します。</span><span class="sxs-lookup"><span data-stu-id="87535-104">Get the count of users by activity type and service.</span></span>

> <span data-ttu-id="87535-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: アクティブ ユーザー](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="87535-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="87535-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="87535-106">Permissions</span></span>

<span data-ttu-id="87535-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="87535-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="87535-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="87535-109">Permission type</span></span>                        | <span data-ttu-id="87535-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="87535-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="87535-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="87535-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="87535-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="87535-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="87535-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="87535-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87535-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="87535-114">Not supported.</span></span>                           |
| <span data-ttu-id="87535-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="87535-115">Application</span></span>                            | <span data-ttu-id="87535-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="87535-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="87535-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="87535-117">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ServicesUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="87535-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="87535-118">Function parameters</span></span>

<span data-ttu-id="87535-119">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="87535-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="87535-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="87535-120">Parameter</span></span> | <span data-ttu-id="87535-121">型</span><span class="sxs-lookup"><span data-stu-id="87535-121">Type</span></span>   | <span data-ttu-id="87535-122">説明</span><span class="sxs-lookup"><span data-stu-id="87535-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="87535-123">period</span><span class="sxs-lookup"><span data-stu-id="87535-123">period</span></span>    | <span data-ttu-id="87535-124">文字列</span><span class="sxs-lookup"><span data-stu-id="87535-124">string</span></span> | <span data-ttu-id="87535-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="87535-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="87535-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="87535-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="87535-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="87535-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="87535-128">必須。</span><span class="sxs-lookup"><span data-stu-id="87535-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="87535-129">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="87535-129">Request headers</span></span>

| <span data-ttu-id="87535-130">名前</span><span class="sxs-lookup"><span data-stu-id="87535-130">Name</span></span>          | <span data-ttu-id="87535-131">説明</span><span class="sxs-lookup"><span data-stu-id="87535-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="87535-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="87535-132">Authorization</span></span> | <span data-ttu-id="87535-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="87535-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="87535-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="87535-135">If-None-Match</span></span> | <span data-ttu-id="87535-136">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="87535-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="87535-137">省略可能。</span><span class="sxs-lookup"><span data-stu-id="87535-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="87535-138">応答</span><span class="sxs-lookup"><span data-stu-id="87535-138">Response</span></span>

<span data-ttu-id="87535-139">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="87535-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="87535-140">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="87535-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="87535-141">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="87535-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="87535-142">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="87535-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="87535-143">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="87535-143">Report Refresh Date</span></span>
- <span data-ttu-id="87535-144">Exchange アクティブ</span><span class="sxs-lookup"><span data-stu-id="87535-144">Exchange Active</span></span>
- <span data-ttu-id="87535-145">Exchange 非アクティブ</span><span class="sxs-lookup"><span data-stu-id="87535-145">Exchange Inactive</span></span>
- <span data-ttu-id="87535-146">OneDrive アクティブ</span><span class="sxs-lookup"><span data-stu-id="87535-146">OneDrive Active</span></span>
- <span data-ttu-id="87535-147">OneDrive 非アクティブ</span><span class="sxs-lookup"><span data-stu-id="87535-147">OneDrive Inactive</span></span>
- <span data-ttu-id="87535-148">SharePoint アクティブ</span><span class="sxs-lookup"><span data-stu-id="87535-148">SharePoint Active</span></span>
- <span data-ttu-id="87535-149">SharePoint 非アクティブ</span><span class="sxs-lookup"><span data-stu-id="87535-149">SharePoint Inactive</span></span>
- <span data-ttu-id="87535-150">Skype For Business アクティブ</span><span class="sxs-lookup"><span data-stu-id="87535-150">Skype For Business Active</span></span>
- <span data-ttu-id="87535-151">Skype For Business 非アクティブ</span><span class="sxs-lookup"><span data-stu-id="87535-151">Skype For Business Inactive</span></span>
- <span data-ttu-id="87535-152">Yammer アクティブ</span><span class="sxs-lookup"><span data-stu-id="87535-152">Yammer Active</span></span>
- <span data-ttu-id="87535-153">Yammer 非アクティブ</span><span class="sxs-lookup"><span data-stu-id="87535-153">Yammer Inactive</span></span>
- <span data-ttu-id="87535-154">Teams アクティブ</span><span class="sxs-lookup"><span data-stu-id="87535-154">Teams Active</span></span>
- <span data-ttu-id="87535-155">Teams 非アクティブ</span><span class="sxs-lookup"><span data-stu-id="87535-155">Teams Inactive</span></span>
- <span data-ttu-id="87535-156">Office 365 のアクティブ</span><span class="sxs-lookup"><span data-stu-id="87535-156">Office 365 Active</span></span>
- <span data-ttu-id="87535-157">Office 365 の非アクティブ</span><span class="sxs-lookup"><span data-stu-id="87535-157">Office 365 Inactive</span></span>
- <span data-ttu-id="87535-158">レポート期間</span><span class="sxs-lookup"><span data-stu-id="87535-158">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="87535-159">例</span><span class="sxs-lookup"><span data-stu-id="87535-159">Example</span></span>

#### <a name="request"></a><span data-ttu-id="87535-160">要求</span><span class="sxs-lookup"><span data-stu-id="87535-160">Request</span></span>

<span data-ttu-id="87535-161">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="87535-161">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="87535-162">プロトコル</span><span class="sxs-lookup"><span data-stu-id="87535-162">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365servicesusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ServicesUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="87535-163">C#</span><span class="sxs-lookup"><span data-stu-id="87535-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365servicesusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="87535-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="87535-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365servicesusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="87535-165">目的-C</span><span class="sxs-lookup"><span data-stu-id="87535-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365servicesusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="87535-166">Java</span><span class="sxs-lookup"><span data-stu-id="87535-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getoffice365servicesusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="87535-167">応答</span><span class="sxs-lookup"><span data-stu-id="87535-167">Response</span></span>

<span data-ttu-id="87535-168">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="87535-168">The following is an example of the response.</span></span>

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

<span data-ttu-id="87535-169">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="87535-169">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Exchange Active,Exchange Inactive,OneDrive Active,OneDrive Inactive,SharePoint Active,SharePoint Inactive,Skype For Business Active,Skype For Business Inactive,Yammer Active,Yammer Inactive,Teams Active,Teams Inactive,Office 365 Active,Office 365 Inactive,Report Period
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
