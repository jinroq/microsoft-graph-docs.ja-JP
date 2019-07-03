---
title: 'reportRoot: getOffice365ActiveUserDetail'
description: Office 365 アクティブ ユーザーに関する詳細を取得します。
localization_priority: Priority
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: d25a818137352f01407b2cfffa4cab846de4662d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35459224"
---
# <a name="reportroot-getoffice365activeuserdetail"></a><span data-ttu-id="74d20-103">reportRoot: getOffice365ActiveUserDetail</span><span class="sxs-lookup"><span data-stu-id="74d20-103">reportRoot: getOffice365ActiveUserDetail</span></span>

<span data-ttu-id="74d20-104">Office 365 アクティブ ユーザーに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="74d20-104">Get details about Office 365 active users.</span></span>

> <span data-ttu-id="74d20-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: アクティブ ユーザー](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="74d20-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="74d20-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="74d20-106">Permissions</span></span>

<span data-ttu-id="74d20-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="74d20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="74d20-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="74d20-109">Permission type</span></span>                        | <span data-ttu-id="74d20-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="74d20-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="74d20-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="74d20-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="74d20-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="74d20-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="74d20-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="74d20-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74d20-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="74d20-114">Not supported.</span></span>                           |
| <span data-ttu-id="74d20-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="74d20-115">Application</span></span>                            | <span data-ttu-id="74d20-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="74d20-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="74d20-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="74d20-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="74d20-118">HTTP</span><span class="sxs-lookup"><span data-stu-id="74d20-118">--Http</span></span>](#tab/http)
<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOffice365ActiveUserDetail(period='{period_value}')
GET /reports/getOffice365ActiveUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="74d20-119">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="74d20-119">Function parameters</span></span>

<span data-ttu-id="74d20-120">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="74d20-120">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="74d20-121">パラメーター</span><span class="sxs-lookup"><span data-stu-id="74d20-121">Parameter</span></span> | <span data-ttu-id="74d20-122">型</span><span class="sxs-lookup"><span data-stu-id="74d20-122">Type</span></span>   | <span data-ttu-id="74d20-123">説明</span><span class="sxs-lookup"><span data-stu-id="74d20-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="74d20-124">period</span><span class="sxs-lookup"><span data-stu-id="74d20-124">period</span></span>    | <span data-ttu-id="74d20-125">文字列</span><span class="sxs-lookup"><span data-stu-id="74d20-125">string</span></span> | <span data-ttu-id="74d20-126">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="74d20-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="74d20-127">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="74d20-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="74d20-128">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="74d20-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="74d20-129">date</span><span class="sxs-lookup"><span data-stu-id="74d20-129">date</span></span>      | <span data-ttu-id="74d20-130">日付</span><span class="sxs-lookup"><span data-stu-id="74d20-130">Date</span></span>   | <span data-ttu-id="74d20-131">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="74d20-131">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="74d20-132">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="74d20-132">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="74d20-133">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="74d20-133">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="74d20-134">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="74d20-134">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="74d20-135">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="74d20-135">Request headers</span></span>

| <span data-ttu-id="74d20-136">名前</span><span class="sxs-lookup"><span data-stu-id="74d20-136">Name</span></span>          | <span data-ttu-id="74d20-137">説明</span><span class="sxs-lookup"><span data-stu-id="74d20-137">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="74d20-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="74d20-138">Authorization</span></span> | <span data-ttu-id="74d20-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="74d20-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="74d20-141">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="74d20-141">If-None-Match</span></span> | <span data-ttu-id="74d20-142">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="74d20-142">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="74d20-143">省略可能。</span><span class="sxs-lookup"><span data-stu-id="74d20-143">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="74d20-144">応答</span><span class="sxs-lookup"><span data-stu-id="74d20-144">Response</span></span>

<span data-ttu-id="74d20-145">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="74d20-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="74d20-146">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="74d20-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="74d20-147">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="74d20-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="74d20-148">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="74d20-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="74d20-149">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="74d20-149">Report Refresh Date</span></span>
- <span data-ttu-id="74d20-150">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="74d20-150">User Principal Name</span></span>
- <span data-ttu-id="74d20-151">表示名</span><span class="sxs-lookup"><span data-stu-id="74d20-151">Display Name</span></span>
- <span data-ttu-id="74d20-152">削除済み</span><span class="sxs-lookup"><span data-stu-id="74d20-152">Is Deleted</span></span>
- <span data-ttu-id="74d20-153">削除日</span><span class="sxs-lookup"><span data-stu-id="74d20-153">Deleted Date</span></span>
- <span data-ttu-id="74d20-154">Exchange ライセンスがある</span><span class="sxs-lookup"><span data-stu-id="74d20-154">Has Exchange License</span></span>
- <span data-ttu-id="74d20-155">OneDrive ライセンスがある</span><span class="sxs-lookup"><span data-stu-id="74d20-155">Has OneDrive License</span></span>
- <span data-ttu-id="74d20-156">SharePoint ライセンスがある</span><span class="sxs-lookup"><span data-stu-id="74d20-156">Has SharePoint License</span></span>
- <span data-ttu-id="74d20-157">Skype for Business ライセンスがある</span><span class="sxs-lookup"><span data-stu-id="74d20-157">Has Skype For Business License</span></span>
- <span data-ttu-id="74d20-158">Yammer ライセンスがある</span><span class="sxs-lookup"><span data-stu-id="74d20-158">Has Yammer License</span></span>
- <span data-ttu-id="74d20-159">Teams ライセンスがある</span><span class="sxs-lookup"><span data-stu-id="74d20-159">Has Teams License</span></span>
- <span data-ttu-id="74d20-160">Exchange の最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="74d20-160">Exchange Last Activity Date</span></span>
- <span data-ttu-id="74d20-161">OneDrive の最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="74d20-161">OneDrive Last Activity Date</span></span>
- <span data-ttu-id="74d20-162">SharePoint の最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="74d20-162">SharePoint Last Activity Date</span></span>
- <span data-ttu-id="74d20-163">Skype For Business の最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="74d20-163">Skype For Business Last Activity Date</span></span>
- <span data-ttu-id="74d20-164">Yammer の最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="74d20-164">Yammer Last Activity Date</span></span>
- <span data-ttu-id="74d20-165">Teams の最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="74d20-165">Teams Last Activity Date</span></span>
- <span data-ttu-id="74d20-166">Exchange のライセンス割り当て日</span><span class="sxs-lookup"><span data-stu-id="74d20-166">Exchange License Assign Date</span></span>
- <span data-ttu-id="74d20-167">OneDrive のライセンス割り当て日</span><span class="sxs-lookup"><span data-stu-id="74d20-167">OneDrive License Assign Date</span></span>
- <span data-ttu-id="74d20-168">SharePoint のライセンス割り当て日</span><span class="sxs-lookup"><span data-stu-id="74d20-168">SharePoint License Assign Date</span></span>
- <span data-ttu-id="74d20-169">Skype For Business のライセンス割り当て日</span><span class="sxs-lookup"><span data-stu-id="74d20-169">Skype For Business License Assign Date</span></span>
- <span data-ttu-id="74d20-170">Yammer のライセンス割り当て日</span><span class="sxs-lookup"><span data-stu-id="74d20-170">Yammer License Assign Date</span></span>
- <span data-ttu-id="74d20-171">Teams のライセンス割り当て日</span><span class="sxs-lookup"><span data-stu-id="74d20-171">Teams License Assign Date</span></span>
- <span data-ttu-id="74d20-172">割り当て済み製品</span><span class="sxs-lookup"><span data-stu-id="74d20-172">Assigned Products</span></span>

## <a name="example"></a><span data-ttu-id="74d20-173">例</span><span class="sxs-lookup"><span data-stu-id="74d20-173">Example</span></span>

#### <a name="request"></a><span data-ttu-id="74d20-174">要求</span><span class="sxs-lookup"><span data-stu-id="74d20-174">Request</span></span>

<span data-ttu-id="74d20-175">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="74d20-175">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activeuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActiveUserDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="74d20-176">C#</span><span class="sxs-lookup"><span data-stu-id="74d20-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activeuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="74d20-177">Javascript</span><span class="sxs-lookup"><span data-stu-id="74d20-177">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activeuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="74d20-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="74d20-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activeuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="74d20-179">応答</span><span class="sxs-lookup"><span data-stu-id="74d20-179">Response</span></span>

<span data-ttu-id="74d20-180">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="74d20-180">The following is an example of the response.</span></span>

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

<span data-ttu-id="74d20-181">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="74d20-181">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Has Exchange License,Has OneDrive License,Has SharePoint License,Has Skype For Business License,Has Yammer License,Has Teams License,Exchange Last Activity Date,OneDrive Last Activity Date,SharePoint Last Activity Date,Skype For Business Last Activity Date,Yammer Last Activity Date,Teams Last Activity Date,Exchange License Assign Date,OneDrive License Assign Date,SharePoint License Assign Date,Skype For Business License Assign Date,Yammer License Assign Date,Teams License Assign Date,Assigned Products
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
