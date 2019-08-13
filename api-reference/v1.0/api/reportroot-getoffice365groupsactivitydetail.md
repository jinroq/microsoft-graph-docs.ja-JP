---
title: 'reportRoot: getOffice365GroupsActivityDetail'
description: グループ別の Office 365 グループ アクティビティに関する詳細を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: cb2165cd8e010fe47682853605d6e8724550d6d5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36326651"
---
# <a name="reportroot-getoffice365groupsactivitydetail"></a><span data-ttu-id="117f6-103">reportRoot: getOffice365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="117f6-103">reportRoot: getOffice365GroupsActivityDetail</span></span>

<span data-ttu-id="117f6-104">グループ別の Office 365 グループ アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="117f6-104">Get details about Office 365 Groups activity by group.</span></span>

> <span data-ttu-id="117f6-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Office 365 グループ](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="117f6-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="117f6-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="117f6-106">Permissions</span></span>

<span data-ttu-id="117f6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="117f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="117f6-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="117f6-109">Permission type</span></span>                        | <span data-ttu-id="117f6-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="117f6-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="117f6-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="117f6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="117f6-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="117f6-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="117f6-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="117f6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="117f6-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="117f6-114">Not supported.</span></span>                           |
| <span data-ttu-id="117f6-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="117f6-115">Application</span></span>                            | <span data-ttu-id="117f6-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="117f6-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="117f6-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="117f6-117">HTTP request</span></span>


<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOffice365GroupsActivityDetail(period='{period_value}')
GET /reports/getOffice365GroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="117f6-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="117f6-118">Function parameters</span></span>

<span data-ttu-id="117f6-119">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="117f6-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="117f6-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="117f6-120">Parameter</span></span> | <span data-ttu-id="117f6-121">型</span><span class="sxs-lookup"><span data-stu-id="117f6-121">Type</span></span>   | <span data-ttu-id="117f6-122">説明</span><span class="sxs-lookup"><span data-stu-id="117f6-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="117f6-123">period</span><span class="sxs-lookup"><span data-stu-id="117f6-123">period</span></span>    | <span data-ttu-id="117f6-124">文字列</span><span class="sxs-lookup"><span data-stu-id="117f6-124">string</span></span> | <span data-ttu-id="117f6-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="117f6-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="117f6-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="117f6-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="117f6-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="117f6-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="117f6-128">date</span><span class="sxs-lookup"><span data-stu-id="117f6-128">date</span></span>      | <span data-ttu-id="117f6-129">日付</span><span class="sxs-lookup"><span data-stu-id="117f6-129">Date</span></span>   | <span data-ttu-id="117f6-130">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="117f6-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="117f6-131">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="117f6-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="117f6-132">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="117f6-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="117f6-133">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="117f6-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="117f6-134">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="117f6-134">Request headers</span></span>

| <span data-ttu-id="117f6-135">名前</span><span class="sxs-lookup"><span data-stu-id="117f6-135">Name</span></span>          | <span data-ttu-id="117f6-136">説明</span><span class="sxs-lookup"><span data-stu-id="117f6-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="117f6-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="117f6-137">Authorization</span></span> | <span data-ttu-id="117f6-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="117f6-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="117f6-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="117f6-140">If-None-Match</span></span> | <span data-ttu-id="117f6-141">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="117f6-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="117f6-142">省略可能。</span><span class="sxs-lookup"><span data-stu-id="117f6-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="117f6-143">応答</span><span class="sxs-lookup"><span data-stu-id="117f6-143">Response</span></span>

<span data-ttu-id="117f6-144">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="117f6-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="117f6-145">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="117f6-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="117f6-146">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="117f6-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="117f6-147">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="117f6-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="117f6-148">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="117f6-148">Report Refresh Date</span></span>
- <span data-ttu-id="117f6-149">グループ表示名</span><span class="sxs-lookup"><span data-stu-id="117f6-149">Group Display Name</span></span>
- <span data-ttu-id="117f6-150">削除済み</span><span class="sxs-lookup"><span data-stu-id="117f6-150">Is Deleted</span></span>
- <span data-ttu-id="117f6-151">所有者のプリンシパル名</span><span class="sxs-lookup"><span data-stu-id="117f6-151">Owner Principal Name</span></span>
- <span data-ttu-id="117f6-152">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="117f6-152">Last Activity Date</span></span>
- <span data-ttu-id="117f6-153">グループの種類</span><span class="sxs-lookup"><span data-stu-id="117f6-153">Group Type</span></span>
- <span data-ttu-id="117f6-154">メンバー数</span><span class="sxs-lookup"><span data-stu-id="117f6-154">Member Count</span></span>
- <span data-ttu-id="117f6-155">外部メンバー数</span><span class="sxs-lookup"><span data-stu-id="117f6-155">External Member Count</span></span>
- <span data-ttu-id="117f6-156">Exchange の受信メール数</span><span class="sxs-lookup"><span data-stu-id="117f6-156">Exchange Received Email Count</span></span>
- <span data-ttu-id="117f6-157">SharePoint のアクティブなファイル数</span><span class="sxs-lookup"><span data-stu-id="117f6-157">SharePoint Active File Count</span></span>
- <span data-ttu-id="117f6-158">Yammer に投稿されたメッセージ数</span><span class="sxs-lookup"><span data-stu-id="117f6-158">Yammer Posted Message Count</span></span>
- <span data-ttu-id="117f6-159">Yammer の開封済みメッセージ数</span><span class="sxs-lookup"><span data-stu-id="117f6-159">Yammer Read Message Count</span></span>
- <span data-ttu-id="117f6-160">Yammer で「いいね!」されたメッセージ数</span><span class="sxs-lookup"><span data-stu-id="117f6-160">Yammer Liked Message Count</span></span>
- <span data-ttu-id="117f6-161">Exchange メールボックスのアイテム合計数</span><span class="sxs-lookup"><span data-stu-id="117f6-161">Exchange Mailbox Total Item Count</span></span>
- <span data-ttu-id="117f6-162">使用済み Exchange メールボックス ストレージ (バイト)</span><span class="sxs-lookup"><span data-stu-id="117f6-162">Exchange Mailbox Storage Used (Byte)</span></span>
- <span data-ttu-id="117f6-163">SharePoint の合計ファイル数</span><span class="sxs-lookup"><span data-stu-id="117f6-163">SharePoint Total File Count</span></span>
- <span data-ttu-id="117f6-164">SharePoint の使用済みサイト ストレージ (バイト)</span><span class="sxs-lookup"><span data-stu-id="117f6-164">SharePoint Site Storage Used (Byte)</span></span>
- <span data-ttu-id="117f6-165">レポート期間</span><span class="sxs-lookup"><span data-stu-id="117f6-165">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="117f6-166">例</span><span class="sxs-lookup"><span data-stu-id="117f6-166">Example</span></span>

#### <a name="request"></a><span data-ttu-id="117f6-167">要求</span><span class="sxs-lookup"><span data-stu-id="117f6-167">Request</span></span>

<span data-ttu-id="117f6-168">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="117f6-168">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="117f6-169">プロトコル</span><span class="sxs-lookup"><span data-stu-id="117f6-169">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365groupsactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365GroupsActivityDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="117f6-170">C#</span><span class="sxs-lookup"><span data-stu-id="117f6-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365groupsactivityuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="117f6-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="117f6-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365groupsactivityuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="117f6-172">目的-C</span><span class="sxs-lookup"><span data-stu-id="117f6-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365groupsactivityuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="117f6-173">Java</span><span class="sxs-lookup"><span data-stu-id="117f6-173">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getoffice365groupsactivityuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="117f6-174">応答</span><span class="sxs-lookup"><span data-stu-id="117f6-174">Response</span></span>

<span data-ttu-id="117f6-175">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="117f6-175">The following is an example of the response.</span></span>

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

<span data-ttu-id="117f6-176">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="117f6-176">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Group Display Name,Is Deleted,Owner Principal Name,Last Activity Date,Group Type,Member Count,Guest Count,Exchange Received Email Count,SharePoint Active File Count,Yammer Posted Message Count,Yammer Read Message Count,Yammer Liked Message Count,Exchange Mailbox Total Item Count,Exchange Mailbox Storage Used (Byte),SharePoint Total File Count,SharePoint Site Storage Used (Byte),Report Period
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
