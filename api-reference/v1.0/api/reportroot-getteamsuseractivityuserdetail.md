---
title: 'reportRoot: getTeamsUserActivityUserDetail'
description: ユーザーごとに、Microsoft Teams ユーザー アクティビティの詳細を取得します。
localization_priority: Priority
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 6de0af2b1ec30e21658dc8fa2f4ab6bbb56379db
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369427"
---
# <a name="reportroot-getteamsuseractivityuserdetail"></a><span data-ttu-id="03d34-103">reportRoot: getTeamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="03d34-103">reportRoot: getTeamsUserActivityUserDetail</span></span>

<span data-ttu-id="03d34-104">ユーザーごとに、Microsoft Teams ユーザー アクティビティの詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="03d34-104">Get details about Microsoft Teams user activity by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="03d34-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="03d34-105">Permissions</span></span>

<span data-ttu-id="03d34-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="03d34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="03d34-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="03d34-108">Permission type</span></span>                        | <span data-ttu-id="03d34-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="03d34-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="03d34-110">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="03d34-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="03d34-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="03d34-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="03d34-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="03d34-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03d34-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="03d34-113">Not supported.</span></span>                           |
| <span data-ttu-id="03d34-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="03d34-114">Application</span></span>                            | <span data-ttu-id="03d34-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="03d34-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="03d34-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="03d34-116">HTTP request</span></span>

<!-- { "blockType": "samples" } -->

```http
GET /reports/getTeamsUserActivityUserDetail(period='{period_value}')
GET /reports/getTeamsUserActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="03d34-117">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="03d34-117">Function parameters</span></span>

<span data-ttu-id="03d34-118">要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="03d34-118">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="03d34-119">パラメーター</span><span class="sxs-lookup"><span data-stu-id="03d34-119">Parameter</span></span> | <span data-ttu-id="03d34-120">型</span><span class="sxs-lookup"><span data-stu-id="03d34-120">Type</span></span>   | <span data-ttu-id="03d34-121">説明</span><span class="sxs-lookup"><span data-stu-id="03d34-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="03d34-122">period</span><span class="sxs-lookup"><span data-stu-id="03d34-122">period</span></span>    | <span data-ttu-id="03d34-123">文字列</span><span class="sxs-lookup"><span data-stu-id="03d34-123">string</span></span> | <span data-ttu-id="03d34-124">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="03d34-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="03d34-125">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="03d34-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="03d34-126">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="03d34-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="03d34-127">date</span><span class="sxs-lookup"><span data-stu-id="03d34-127">date</span></span>      | <span data-ttu-id="03d34-128">日付</span><span class="sxs-lookup"><span data-stu-id="03d34-128">Date</span></span>   | <span data-ttu-id="03d34-129">何らかのアクティビティを実行したユーザーを表示する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="03d34-129">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="03d34-130">{date_value} は YYYY-MM-DD の形式にします。</span><span class="sxs-lookup"><span data-stu-id="03d34-130">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="03d34-131">このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="03d34-131">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="03d34-132">**注:** URL に期間または日付を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="03d34-132">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="03d34-133">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="03d34-133">Request headers</span></span>

| <span data-ttu-id="03d34-134">名前</span><span class="sxs-lookup"><span data-stu-id="03d34-134">Name</span></span>          | <span data-ttu-id="03d34-135">説明</span><span class="sxs-lookup"><span data-stu-id="03d34-135">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="03d34-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="03d34-136">Authorization</span></span> | <span data-ttu-id="03d34-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="03d34-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="03d34-139">応答</span><span class="sxs-lookup"><span data-stu-id="03d34-139">Response</span></span>

<span data-ttu-id="03d34-140">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="03d34-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="03d34-141">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="03d34-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="03d34-142">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="03d34-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="03d34-143">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="03d34-143">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="03d34-144">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="03d34-144">Report Refresh Date</span></span>
- <span data-ttu-id="03d34-145">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="03d34-145">User Principal Name</span></span>
- <span data-ttu-id="03d34-146">最後のアクティビティ日付</span><span class="sxs-lookup"><span data-stu-id="03d34-146">Last Activity Date</span></span>
- <span data-ttu-id="03d34-147">削除済み</span><span class="sxs-lookup"><span data-stu-id="03d34-147">Is Deleted</span></span>
- <span data-ttu-id="03d34-148">削除日</span><span class="sxs-lookup"><span data-stu-id="03d34-148">Deleted Date</span></span>
- <span data-ttu-id="03d34-149">割り当て済み製品</span><span class="sxs-lookup"><span data-stu-id="03d34-149">Assigned Products</span></span>
- <span data-ttu-id="03d34-150">チーム チャット メッセージ数</span><span class="sxs-lookup"><span data-stu-id="03d34-150">Team Chat Message Count</span></span>
- <span data-ttu-id="03d34-151">非公開チャット メッセージ数</span><span class="sxs-lookup"><span data-stu-id="03d34-151">Private Chat Message Count</span></span>
- <span data-ttu-id="03d34-152">通話数</span><span class="sxs-lookup"><span data-stu-id="03d34-152">Call Count</span></span>
- <span data-ttu-id="03d34-153">会議数</span><span class="sxs-lookup"><span data-stu-id="03d34-153">Meeting Count</span></span>
- <span data-ttu-id="03d34-154">その他のアクションの有無</span><span class="sxs-lookup"><span data-stu-id="03d34-154">Has Other Action</span></span>
- <span data-ttu-id="03d34-155">レポート期間</span><span class="sxs-lookup"><span data-stu-id="03d34-155">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="03d34-156">例</span><span class="sxs-lookup"><span data-stu-id="03d34-156">Example</span></span>

#### <a name="request"></a><span data-ttu-id="03d34-157">要求</span><span class="sxs-lookup"><span data-stu-id="03d34-157">Request</span></span>

<span data-ttu-id="03d34-158">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="03d34-158">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="03d34-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="03d34-159">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getTeamsUserActivityUserDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="03d34-160">C#</span><span class="sxs-lookup"><span data-stu-id="03d34-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsuseractivityuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="03d34-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="03d34-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsuseractivityuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="03d34-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="03d34-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsuseractivityuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="03d34-163">Java</span><span class="sxs-lookup"><span data-stu-id="03d34-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getteamsuseractivityuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="03d34-164">応答</span><span class="sxs-lookup"><span data-stu-id="03d34-164">Response</span></span>

<span data-ttu-id="03d34-165">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="03d34-165">The following is an example of the response.</span></span>

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

<span data-ttu-id="03d34-166">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="03d34-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Is Deleted,Deleted Date,Assigned Products,Team Chat Message Count,Private Chat Message Count,Call Count,Meeting Count,Has Other Action,Report Period
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
