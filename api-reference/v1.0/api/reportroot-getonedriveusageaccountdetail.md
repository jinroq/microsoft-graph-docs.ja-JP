---
title: 'reportRoot: getOneDriveUsageAccountDetail'
description: アカウント別の OneDrive の使用状況に関する詳細を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 2fa19a2bf01d5584cf9f8d5a976119fa19a98719
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36025016"
---
# <a name="reportroot-getonedriveusageaccountdetail"></a><span data-ttu-id="812f4-103">reportRoot: getOneDriveUsageAccountDetail</span><span class="sxs-lookup"><span data-stu-id="812f4-103">reportRoot: getOneDriveUsageAccountDetail</span></span>

<span data-ttu-id="812f4-104">アカウント別の OneDrive の使用状況に関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="812f4-104">Get details about OneDrive usage by account.</span></span>

> <span data-ttu-id="812f4-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: OneDrive for Business の使用状況](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="812f4-105">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="812f4-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="812f4-106">Permissions</span></span>

<span data-ttu-id="812f4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="812f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="812f4-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="812f4-109">Permission type</span></span>                        | <span data-ttu-id="812f4-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="812f4-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="812f4-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="812f4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="812f4-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="812f4-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="812f4-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="812f4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="812f4-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="812f4-114">Not supported.</span></span>                           |
| <span data-ttu-id="812f4-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="812f4-115">Application</span></span>                            | <span data-ttu-id="812f4-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="812f4-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="812f4-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="812f4-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="812f4-118">プロトコル</span><span class="sxs-lookup"><span data-stu-id="812f4-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOneDriveUsageAccountDetail(period='{period_value}')
GET /reports/getOneDriveUsageAccountDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="812f4-119">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="812f4-119">Function parameters</span></span>

<span data-ttu-id="812f4-120">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="812f4-120">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="812f4-121">パラメーター</span><span class="sxs-lookup"><span data-stu-id="812f4-121">Parameter</span></span> | <span data-ttu-id="812f4-122">型</span><span class="sxs-lookup"><span data-stu-id="812f4-122">Type</span></span>   | <span data-ttu-id="812f4-123">説明</span><span class="sxs-lookup"><span data-stu-id="812f4-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="812f4-124">period</span><span class="sxs-lookup"><span data-stu-id="812f4-124">period</span></span>    | <span data-ttu-id="812f4-125">文字列</span><span class="sxs-lookup"><span data-stu-id="812f4-125">string</span></span> | <span data-ttu-id="812f4-126">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="812f4-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="812f4-127">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="812f4-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="812f4-128">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="812f4-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="812f4-129">date</span><span class="sxs-lookup"><span data-stu-id="812f4-129">date</span></span>      | <span data-ttu-id="812f4-130">日付</span><span class="sxs-lookup"><span data-stu-id="812f4-130">Date</span></span>   | <span data-ttu-id="812f4-131">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="812f4-131">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="812f4-132">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="812f4-132">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="812f4-133">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="812f4-133">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="812f4-134">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="812f4-134">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="812f4-135">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="812f4-135">Request headers</span></span>

| <span data-ttu-id="812f4-136">名前</span><span class="sxs-lookup"><span data-stu-id="812f4-136">Name</span></span>          | <span data-ttu-id="812f4-137">説明</span><span class="sxs-lookup"><span data-stu-id="812f4-137">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="812f4-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="812f4-138">Authorization</span></span> | <span data-ttu-id="812f4-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="812f4-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="812f4-141">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="812f4-141">If-None-Match</span></span> | <span data-ttu-id="812f4-142">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="812f4-142">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="812f4-143">省略可能。</span><span class="sxs-lookup"><span data-stu-id="812f4-143">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="812f4-144">応答</span><span class="sxs-lookup"><span data-stu-id="812f4-144">Response</span></span>

<span data-ttu-id="812f4-145">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="812f4-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="812f4-146">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="812f4-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="812f4-147">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="812f4-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="812f4-148">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="812f4-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="812f4-149">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="812f4-149">Report Refresh Date</span></span>
- <span data-ttu-id="812f4-150">サイトの URL</span><span class="sxs-lookup"><span data-stu-id="812f4-150">Site URL</span></span>
- <span data-ttu-id="812f4-151">所有者の表示名</span><span class="sxs-lookup"><span data-stu-id="812f4-151">Owner Display Name</span></span>
- <span data-ttu-id="812f4-152">削除済み</span><span class="sxs-lookup"><span data-stu-id="812f4-152">Is Deleted</span></span>
- <span data-ttu-id="812f4-153">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="812f4-153">Last Activity Date</span></span>
- <span data-ttu-id="812f4-154">ファイル数</span><span class="sxs-lookup"><span data-stu-id="812f4-154">File Count</span></span>
- <span data-ttu-id="812f4-155">アクティブなファイル数</span><span class="sxs-lookup"><span data-stu-id="812f4-155">Active File Count</span></span>
- <span data-ttu-id="812f4-156">使用済みストレージ (バイト)</span><span class="sxs-lookup"><span data-stu-id="812f4-156">Storage Used (Byte)</span></span>
- <span data-ttu-id="812f4-157">割り当て済みストレージ (バイト)</span><span class="sxs-lookup"><span data-stu-id="812f4-157">Storage Allocated (Byte)</span></span>
- <span data-ttu-id="812f4-158">レポート期間</span><span class="sxs-lookup"><span data-stu-id="812f4-158">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="812f4-159">例</span><span class="sxs-lookup"><span data-stu-id="812f4-159">Example</span></span>

#### <a name="request"></a><span data-ttu-id="812f4-160">要求</span><span class="sxs-lookup"><span data-stu-id="812f4-160">Request</span></span>

<span data-ttu-id="812f4-161">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="812f4-161">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getonedriveusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOneDriveUsageAccountDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="812f4-162">C#</span><span class="sxs-lookup"><span data-stu-id="812f4-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveusageuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="812f4-163">Javascript</span><span class="sxs-lookup"><span data-stu-id="812f4-163">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveusageuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="812f4-164">目的-C</span><span class="sxs-lookup"><span data-stu-id="812f4-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveusageuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="812f4-165">Java</span><span class="sxs-lookup"><span data-stu-id="812f4-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getonedriveusageuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="812f4-166">応答</span><span class="sxs-lookup"><span data-stu-id="812f4-166">Response</span></span>

<span data-ttu-id="812f4-167">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="812f4-167">The following is an example of the response.</span></span>

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

<span data-ttu-id="812f4-168">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="812f4-168">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site URL,Owner Display Name,Is Deleted,Last Activity Date,File Count,Active File Count,Storage Used (Byte),Storage Allocated (Byte),Report Period
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
