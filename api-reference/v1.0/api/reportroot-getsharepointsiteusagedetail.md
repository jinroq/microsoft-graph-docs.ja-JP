---
title: 'reportRoot: getSharePointSiteUsageDetail'
description: SharePoint サイトの使用状況に関する詳細を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 20e407dbc089f8ea62cd7b8c0ec63fbedb2d385a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36021847"
---
# <a name="reportroot-getsharepointsiteusagedetail"></a><span data-ttu-id="5b5da-103">reportRoot: getSharePointSiteUsageDetail</span><span class="sxs-lookup"><span data-stu-id="5b5da-103">reportRoot: getSharePointSiteUsageDetail</span></span>

<span data-ttu-id="5b5da-104">SharePoint サイトの使用状況に関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="5b5da-104">Get details about SharePoint site usage.</span></span>

> <span data-ttu-id="5b5da-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: SharePoint サイトの使用状況](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5b5da-105">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="5b5da-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5b5da-106">Permissions</span></span>

<span data-ttu-id="5b5da-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5b5da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5b5da-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5b5da-109">Permission type</span></span>                        | <span data-ttu-id="5b5da-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5b5da-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="5b5da-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="5b5da-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5b5da-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b5da-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="5b5da-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5b5da-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b5da-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5b5da-114">Not supported.</span></span>                           |
| <span data-ttu-id="5b5da-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5b5da-115">Application</span></span>                            | <span data-ttu-id="5b5da-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b5da-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="5b5da-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5b5da-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="5b5da-118">プロトコル</span><span class="sxs-lookup"><span data-stu-id="5b5da-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "samples" } --> 

```http
GET /reports/getSharePointSiteUsageDetail(period='{period_value}')
GET /reports/getSharePointSiteUsageDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="5b5da-119">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="5b5da-119">Function parameters</span></span>

<span data-ttu-id="5b5da-120">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="5b5da-120">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="5b5da-121">パラメーター</span><span class="sxs-lookup"><span data-stu-id="5b5da-121">Parameter</span></span> | <span data-ttu-id="5b5da-122">型</span><span class="sxs-lookup"><span data-stu-id="5b5da-122">Type</span></span>   | <span data-ttu-id="5b5da-123">説明</span><span class="sxs-lookup"><span data-stu-id="5b5da-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="5b5da-124">period</span><span class="sxs-lookup"><span data-stu-id="5b5da-124">period</span></span>    | <span data-ttu-id="5b5da-125">文字列</span><span class="sxs-lookup"><span data-stu-id="5b5da-125">string</span></span> | <span data-ttu-id="5b5da-126">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="5b5da-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="5b5da-127">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="5b5da-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="5b5da-128">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="5b5da-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="5b5da-129">date</span><span class="sxs-lookup"><span data-stu-id="5b5da-129">date</span></span>      | <span data-ttu-id="5b5da-130">日付</span><span class="sxs-lookup"><span data-stu-id="5b5da-130">Date</span></span>   | <span data-ttu-id="5b5da-131">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="5b5da-131">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="5b5da-132">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="5b5da-132">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="5b5da-133">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="5b5da-133">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="5b5da-134">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="5b5da-134">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5b5da-135">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5b5da-135">Request headers</span></span>

| <span data-ttu-id="5b5da-136">名前</span><span class="sxs-lookup"><span data-stu-id="5b5da-136">Name</span></span>          | <span data-ttu-id="5b5da-137">説明</span><span class="sxs-lookup"><span data-stu-id="5b5da-137">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="5b5da-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b5da-138">Authorization</span></span> | <span data-ttu-id="5b5da-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5b5da-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="5b5da-141">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="5b5da-141">If-None-Match</span></span> | <span data-ttu-id="5b5da-142">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="5b5da-142">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="5b5da-143">省略可能。</span><span class="sxs-lookup"><span data-stu-id="5b5da-143">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="5b5da-144">応答</span><span class="sxs-lookup"><span data-stu-id="5b5da-144">Response</span></span>

<span data-ttu-id="5b5da-145">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="5b5da-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="5b5da-146">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="5b5da-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="5b5da-147">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="5b5da-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="5b5da-148">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="5b5da-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="5b5da-149">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="5b5da-149">Report Refresh Date</span></span>
- <span data-ttu-id="5b5da-150">サイト Id</span><span class="sxs-lookup"><span data-stu-id="5b5da-150">Site Id</span></span>
- <span data-ttu-id="5b5da-151">サイトの URL</span><span class="sxs-lookup"><span data-stu-id="5b5da-151">Site URL</span></span>
- <span data-ttu-id="5b5da-152">所有者の表示名</span><span class="sxs-lookup"><span data-stu-id="5b5da-152">Owner Display Name</span></span>
- <span data-ttu-id="5b5da-153">削除済み</span><span class="sxs-lookup"><span data-stu-id="5b5da-153">Is Deleted</span></span>
- <span data-ttu-id="5b5da-154">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="5b5da-154">Last Activity Date</span></span>
- <span data-ttu-id="5b5da-155">ファイル数</span><span class="sxs-lookup"><span data-stu-id="5b5da-155">File Count</span></span>
- <span data-ttu-id="5b5da-156">アクティブなファイル数</span><span class="sxs-lookup"><span data-stu-id="5b5da-156">Active File Count</span></span>
- <span data-ttu-id="5b5da-157">ページ ビューの数</span><span class="sxs-lookup"><span data-stu-id="5b5da-157">Page View Count</span></span>
- <span data-ttu-id="5b5da-158">アクセスしたページ数</span><span class="sxs-lookup"><span data-stu-id="5b5da-158">Visited Page Count</span></span>
- <span data-ttu-id="5b5da-159">使用済みストレージ (バイト)</span><span class="sxs-lookup"><span data-stu-id="5b5da-159">Storage Used (Byte)</span></span>
- <span data-ttu-id="5b5da-160">割り当て済みストレージ (バイト)</span><span class="sxs-lookup"><span data-stu-id="5b5da-160">Storage Allocated (Byte)</span></span>
- <span data-ttu-id="5b5da-161">ルート Web テンプレート</span><span class="sxs-lookup"><span data-stu-id="5b5da-161">Root Web Template</span></span>
- <span data-ttu-id="5b5da-162">レポート期間</span><span class="sxs-lookup"><span data-stu-id="5b5da-162">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="5b5da-163">例</span><span class="sxs-lookup"><span data-stu-id="5b5da-163">Example</span></span>

#### <a name="request"></a><span data-ttu-id="5b5da-164">要求</span><span class="sxs-lookup"><span data-stu-id="5b5da-164">Request</span></span>

<span data-ttu-id="5b5da-165">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5b5da-165">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getsharepointsiteusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointSiteUsageDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5b5da-166">C#</span><span class="sxs-lookup"><span data-stu-id="5b5da-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointsiteusageuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5b5da-167">Javascript</span><span class="sxs-lookup"><span data-stu-id="5b5da-167">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointsiteusageuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5b5da-168">目的-C</span><span class="sxs-lookup"><span data-stu-id="5b5da-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointsiteusageuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="5b5da-169">Java</span><span class="sxs-lookup"><span data-stu-id="5b5da-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getsharepointsiteusageuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5b5da-170">応答</span><span class="sxs-lookup"><span data-stu-id="5b5da-170">Response</span></span>

<span data-ttu-id="5b5da-171">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5b5da-171">The following is an example of the response.</span></span>

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

<span data-ttu-id="5b5da-172">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="5b5da-172">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Id,Site URL,Owner Display Name,Is Deleted,Last Activity Date,File Count,Active File Count,Page View Count,Visited Page Count,Storage Used (Byte),Storage Allocated (Byte),Root Web Template,Report Period
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
