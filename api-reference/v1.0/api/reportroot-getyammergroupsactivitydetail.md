---
title: 'reportRoot: getYammerGroupsActivityDetail'
description: グループ別の Yammer グループ アクティビティに関する詳細を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 827b4bfd785ce3cadca5a71c74970a4012854055
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320223"
---
# <a name="reportroot-getyammergroupsactivitydetail"></a><span data-ttu-id="d66ae-103">reportRoot: getYammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="d66ae-103">reportRoot: getYammerGroupsActivityDetail</span></span>

<span data-ttu-id="d66ae-104">グループ別の Yammer グループ アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="d66ae-104">Get details about Yammer groups activity by group.</span></span>

> <span data-ttu-id="d66ae-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer グループ アクティビティ](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d66ae-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="permissions"></a><span data-ttu-id="d66ae-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d66ae-106">Permissions</span></span>

<span data-ttu-id="d66ae-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d66ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d66ae-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d66ae-109">Permission type</span></span>                        | <span data-ttu-id="d66ae-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d66ae-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="d66ae-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="d66ae-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d66ae-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d66ae-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="d66ae-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d66ae-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d66ae-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d66ae-114">Not supported.</span></span>                           |
| <span data-ttu-id="d66ae-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d66ae-115">Application</span></span>                            | <span data-ttu-id="d66ae-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d66ae-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="d66ae-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d66ae-117">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityDetail(period='{period_value}')
GET /reports/getYammerGroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="d66ae-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="d66ae-118">Function parameters</span></span>

<span data-ttu-id="d66ae-119">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="d66ae-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="d66ae-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="d66ae-120">Parameter</span></span> | <span data-ttu-id="d66ae-121">型</span><span class="sxs-lookup"><span data-stu-id="d66ae-121">Type</span></span>   | <span data-ttu-id="d66ae-122">説明</span><span class="sxs-lookup"><span data-stu-id="d66ae-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="d66ae-123">period</span><span class="sxs-lookup"><span data-stu-id="d66ae-123">period</span></span>    | <span data-ttu-id="d66ae-124">文字列</span><span class="sxs-lookup"><span data-stu-id="d66ae-124">string</span></span> | <span data-ttu-id="d66ae-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="d66ae-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="d66ae-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="d66ae-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="d66ae-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="d66ae-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="d66ae-128">date</span><span class="sxs-lookup"><span data-stu-id="d66ae-128">date</span></span>      | <span data-ttu-id="d66ae-129">日付</span><span class="sxs-lookup"><span data-stu-id="d66ae-129">Date</span></span>   | <span data-ttu-id="d66ae-130">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="d66ae-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="d66ae-131">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="d66ae-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="d66ae-132">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="d66ae-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="d66ae-133">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d66ae-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d66ae-134">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d66ae-134">Request headers</span></span>

| <span data-ttu-id="d66ae-135">名前</span><span class="sxs-lookup"><span data-stu-id="d66ae-135">Name</span></span>          | <span data-ttu-id="d66ae-136">説明</span><span class="sxs-lookup"><span data-stu-id="d66ae-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="d66ae-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="d66ae-137">Authorization</span></span> | <span data-ttu-id="d66ae-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d66ae-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="d66ae-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="d66ae-140">If-None-Match</span></span> | <span data-ttu-id="d66ae-141">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="d66ae-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="d66ae-142">省略可能。</span><span class="sxs-lookup"><span data-stu-id="d66ae-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="d66ae-143">応答</span><span class="sxs-lookup"><span data-stu-id="d66ae-143">Response</span></span>

<span data-ttu-id="d66ae-144">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="d66ae-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="d66ae-145">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="d66ae-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="d66ae-146">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="d66ae-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="d66ae-147">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="d66ae-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="d66ae-148">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="d66ae-148">Report Refresh Date</span></span>
- <span data-ttu-id="d66ae-149">グループ表示名</span><span class="sxs-lookup"><span data-stu-id="d66ae-149">Group Display Name</span></span>
- <span data-ttu-id="d66ae-150">削除済み</span><span class="sxs-lookup"><span data-stu-id="d66ae-150">Is Deleted</span></span>
- <span data-ttu-id="d66ae-151">所有者のプリンシパル名</span><span class="sxs-lookup"><span data-stu-id="d66ae-151">Owner Principal Name</span></span>
- <span data-ttu-id="d66ae-152">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="d66ae-152">Last Activity Date</span></span>
- <span data-ttu-id="d66ae-153">グループの種類</span><span class="sxs-lookup"><span data-stu-id="d66ae-153">Group Type</span></span>
- <span data-ttu-id="d66ae-154">Office 365 接続</span><span class="sxs-lookup"><span data-stu-id="d66ae-154">Office 365 Connected</span></span>
- <span data-ttu-id="d66ae-155">メンバー数</span><span class="sxs-lookup"><span data-stu-id="d66ae-155">Member Count</span></span>
- <span data-ttu-id="d66ae-156">投稿数</span><span class="sxs-lookup"><span data-stu-id="d66ae-156">Posted Count</span></span>
- <span data-ttu-id="d66ae-157">読み取り数</span><span class="sxs-lookup"><span data-stu-id="d66ae-157">Read Count</span></span>
- <span data-ttu-id="d66ae-158">「いいね!」の数</span><span class="sxs-lookup"><span data-stu-id="d66ae-158">Liked Count</span></span>
- <span data-ttu-id="d66ae-159">レポート期間</span><span class="sxs-lookup"><span data-stu-id="d66ae-159">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="d66ae-160">例</span><span class="sxs-lookup"><span data-stu-id="d66ae-160">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d66ae-161">要求</span><span class="sxs-lookup"><span data-stu-id="d66ae-161">Request</span></span>

<span data-ttu-id="d66ae-162">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d66ae-162">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d66ae-163">プロトコル</span><span class="sxs-lookup"><span data-stu-id="d66ae-163">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammergroupsactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerGroupsActivityDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d66ae-164">C#</span><span class="sxs-lookup"><span data-stu-id="d66ae-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammergroupsactivityuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d66ae-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d66ae-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammergroupsactivityuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d66ae-166">目的-C</span><span class="sxs-lookup"><span data-stu-id="d66ae-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammergroupsactivityuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d66ae-167">Java</span><span class="sxs-lookup"><span data-stu-id="d66ae-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getyammergroupsactivityuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d66ae-168">応答</span><span class="sxs-lookup"><span data-stu-id="d66ae-168">Response</span></span>

<span data-ttu-id="d66ae-169">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d66ae-169">The following is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.report" } --> 

```http
HTTP/1.1 302 Found
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

#### <a name="request"></a><span data-ttu-id="d66ae-170">要求</span><span class="sxs-lookup"><span data-stu-id="d66ae-170">Request</span></span>
<span data-ttu-id="d66ae-171">を使用して`date`呼び出された場合、レポートのスコープは、指定された日付のアクティビティに設定されます。</span><span class="sxs-lookup"><span data-stu-id="d66ae-171">If called with a `date`, the report is scoped to activity on the given date.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammergroupsactivityuserdetail_date"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerGroupsActivityDetail(date='2018-03-05')
```

#### <a name="response"></a><span data-ttu-id="d66ae-172">応答</span><span class="sxs-lookup"><span data-stu-id="d66ae-172">Response</span></span>

<span data-ttu-id="d66ae-173">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d66ae-173">The following is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.report" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="d66ae-174">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="d66ae-174">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "ignored"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Group Display Name,Is Deleted,Owner Principal Name,Last Activity Date,Group Type,Office 365 Connected,Member Count,Posted Count,Read Count,Liked Count,Report Period
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
