---
title: 'reportRoot: getYammerGroupsActivityDetail'
description: グループ別の Yammer グループ アクティビティに関する詳細を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 1fde8accb02cc09f5a4f2eace2d585eef737f1d9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35975712"
---
# <a name="reportroot-getyammergroupsactivitydetail"></a><span data-ttu-id="0c45f-103">reportRoot: getYammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="0c45f-103">reportRoot: getYammerGroupsActivityDetail</span></span>

<span data-ttu-id="0c45f-104">グループ別の Yammer グループ アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="0c45f-104">Get details about Yammer groups activity by group.</span></span>

> <span data-ttu-id="0c45f-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer グループ アクティビティ](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0c45f-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="permissions"></a><span data-ttu-id="0c45f-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0c45f-106">Permissions</span></span>

<span data-ttu-id="0c45f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0c45f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0c45f-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0c45f-109">Permission type</span></span>                        | <span data-ttu-id="0c45f-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0c45f-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="0c45f-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="0c45f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0c45f-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0c45f-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="0c45f-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0c45f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c45f-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0c45f-114">Not supported.</span></span>                           |
| <span data-ttu-id="0c45f-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0c45f-115">Application</span></span>                            | <span data-ttu-id="0c45f-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0c45f-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="0c45f-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0c45f-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0c45f-118">プロトコル</span><span class="sxs-lookup"><span data-stu-id="0c45f-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityDetail(period='{period_value}')
GET /reports/getYammerGroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="0c45f-119">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="0c45f-119">Function parameters</span></span>

<span data-ttu-id="0c45f-120">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="0c45f-120">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="0c45f-121">パラメーター</span><span class="sxs-lookup"><span data-stu-id="0c45f-121">Parameter</span></span> | <span data-ttu-id="0c45f-122">型</span><span class="sxs-lookup"><span data-stu-id="0c45f-122">Type</span></span>   | <span data-ttu-id="0c45f-123">説明</span><span class="sxs-lookup"><span data-stu-id="0c45f-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="0c45f-124">period</span><span class="sxs-lookup"><span data-stu-id="0c45f-124">period</span></span>    | <span data-ttu-id="0c45f-125">文字列</span><span class="sxs-lookup"><span data-stu-id="0c45f-125">string</span></span> | <span data-ttu-id="0c45f-126">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="0c45f-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="0c45f-127">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="0c45f-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="0c45f-128">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="0c45f-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="0c45f-129">date</span><span class="sxs-lookup"><span data-stu-id="0c45f-129">date</span></span>      | <span data-ttu-id="0c45f-130">日付</span><span class="sxs-lookup"><span data-stu-id="0c45f-130">Date</span></span>   | <span data-ttu-id="0c45f-131">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="0c45f-131">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="0c45f-132">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="0c45f-132">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="0c45f-133">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="0c45f-133">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="0c45f-134">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="0c45f-134">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0c45f-135">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0c45f-135">Request headers</span></span>

| <span data-ttu-id="0c45f-136">名前</span><span class="sxs-lookup"><span data-stu-id="0c45f-136">Name</span></span>          | <span data-ttu-id="0c45f-137">説明</span><span class="sxs-lookup"><span data-stu-id="0c45f-137">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="0c45f-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c45f-138">Authorization</span></span> | <span data-ttu-id="0c45f-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0c45f-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="0c45f-141">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="0c45f-141">If-None-Match</span></span> | <span data-ttu-id="0c45f-142">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="0c45f-142">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="0c45f-143">省略可能。</span><span class="sxs-lookup"><span data-stu-id="0c45f-143">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="0c45f-144">応答</span><span class="sxs-lookup"><span data-stu-id="0c45f-144">Response</span></span>

<span data-ttu-id="0c45f-145">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="0c45f-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="0c45f-146">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="0c45f-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="0c45f-147">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="0c45f-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="0c45f-148">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="0c45f-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="0c45f-149">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="0c45f-149">Report Refresh Date</span></span>
- <span data-ttu-id="0c45f-150">グループ表示名</span><span class="sxs-lookup"><span data-stu-id="0c45f-150">Group Display Name</span></span>
- <span data-ttu-id="0c45f-151">削除済み</span><span class="sxs-lookup"><span data-stu-id="0c45f-151">Is Deleted</span></span>
- <span data-ttu-id="0c45f-152">所有者のプリンシパル名</span><span class="sxs-lookup"><span data-stu-id="0c45f-152">Owner Principal Name</span></span>
- <span data-ttu-id="0c45f-153">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="0c45f-153">Last Activity Date</span></span>
- <span data-ttu-id="0c45f-154">グループの種類</span><span class="sxs-lookup"><span data-stu-id="0c45f-154">Group Type</span></span>
- <span data-ttu-id="0c45f-155">Office 365 接続</span><span class="sxs-lookup"><span data-stu-id="0c45f-155">Office 365 Connected</span></span>
- <span data-ttu-id="0c45f-156">メンバー数</span><span class="sxs-lookup"><span data-stu-id="0c45f-156">Member Count</span></span>
- <span data-ttu-id="0c45f-157">投稿数</span><span class="sxs-lookup"><span data-stu-id="0c45f-157">Posted Count</span></span>
- <span data-ttu-id="0c45f-158">読み取り数</span><span class="sxs-lookup"><span data-stu-id="0c45f-158">Read Count</span></span>
- <span data-ttu-id="0c45f-159">「いいね!」の数</span><span class="sxs-lookup"><span data-stu-id="0c45f-159">Liked Count</span></span>
- <span data-ttu-id="0c45f-160">レポート期間</span><span class="sxs-lookup"><span data-stu-id="0c45f-160">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="0c45f-161">例</span><span class="sxs-lookup"><span data-stu-id="0c45f-161">Example</span></span>

#### <a name="request"></a><span data-ttu-id="0c45f-162">要求</span><span class="sxs-lookup"><span data-stu-id="0c45f-162">Request</span></span>

<span data-ttu-id="0c45f-163">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0c45f-163">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammergroupsactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerGroupsActivityDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0c45f-164">C#</span><span class="sxs-lookup"><span data-stu-id="0c45f-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammergroupsactivityuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0c45f-165">Javascript</span><span class="sxs-lookup"><span data-stu-id="0c45f-165">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammergroupsactivityuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0c45f-166">目的-C</span><span class="sxs-lookup"><span data-stu-id="0c45f-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammergroupsactivityuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0c45f-167">Java</span><span class="sxs-lookup"><span data-stu-id="0c45f-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getyammergroupsactivityuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0c45f-168">応答</span><span class="sxs-lookup"><span data-stu-id="0c45f-168">Response</span></span>

<span data-ttu-id="0c45f-169">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0c45f-169">The following is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.report" } --> 

```http
HTTP/1.1 302 Found
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

#### <a name="request"></a><span data-ttu-id="0c45f-170">要求</span><span class="sxs-lookup"><span data-stu-id="0c45f-170">Request</span></span>
<span data-ttu-id="0c45f-171">を使用して`date`呼び出された場合、レポートのスコープは、指定された日付のアクティビティに設定されます。</span><span class="sxs-lookup"><span data-stu-id="0c45f-171">If called with a `date`, the report is scoped to activity on the given date.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammergroupsactivityuserdetail_date"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerGroupsActivityDetail(date='2018-03-05')
```

#### <a name="response"></a><span data-ttu-id="0c45f-172">応答</span><span class="sxs-lookup"><span data-stu-id="0c45f-172">Response</span></span>

<span data-ttu-id="0c45f-173">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0c45f-173">The following is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.report" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="0c45f-174">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="0c45f-174">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
