---
title: 'reportRoot: getTeamsUserActivityUserCounts'
description: アクティビティの種類ごとに、Microsoft Teams ユーザーの数を取得します。 アクティビティの種類は、チーム チャット メッセージ、非公開チャット メッセージ、通話、または会議の数です。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 8154d734e97662c4bcae93d3de2c97d3c2e58cea
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35886658"
---
# <a name="reportroot-getteamsuseractivityusercounts"></a><span data-ttu-id="8e267-104">reportRoot: getTeamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="8e267-104">reportRoot: getTeamsUserActivityUserCounts</span></span>

<span data-ttu-id="8e267-105">アクティビティの種類ごとに、Microsoft Teams ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="8e267-105">Get the number of Microsoft Teams users by activity type.</span></span> <span data-ttu-id="8e267-106">アクティビティの種類は、チーム チャット メッセージ、非公開チャット メッセージ、通話、または会議の数です。</span><span class="sxs-lookup"><span data-stu-id="8e267-106">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e267-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8e267-107">Permissions</span></span>

<span data-ttu-id="8e267-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8e267-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8e267-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8e267-110">Permission type</span></span>                        | <span data-ttu-id="8e267-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8e267-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="8e267-112">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="8e267-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="8e267-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8e267-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="8e267-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8e267-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e267-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8e267-115">Not supported.</span></span>                           |
| <span data-ttu-id="8e267-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8e267-116">Application</span></span>                            | <span data-ttu-id="8e267-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8e267-117">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="8e267-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8e267-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="8e267-119">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="8e267-119">Function parameters</span></span>

<span data-ttu-id="8e267-120">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="8e267-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="8e267-121">パラメーター</span><span class="sxs-lookup"><span data-stu-id="8e267-121">Parameter</span></span> | <span data-ttu-id="8e267-122">型</span><span class="sxs-lookup"><span data-stu-id="8e267-122">Type</span></span>   | <span data-ttu-id="8e267-123">説明</span><span class="sxs-lookup"><span data-stu-id="8e267-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="8e267-124">period</span><span class="sxs-lookup"><span data-stu-id="8e267-124">period</span></span>    | <span data-ttu-id="8e267-125">文字列</span><span class="sxs-lookup"><span data-stu-id="8e267-125">string</span></span> | <span data-ttu-id="8e267-126">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="8e267-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="8e267-127">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="8e267-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="8e267-128">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="8e267-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="8e267-129">必須。</span><span class="sxs-lookup"><span data-stu-id="8e267-129">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="8e267-130">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8e267-130">Request headers</span></span>

| <span data-ttu-id="8e267-131">名前</span><span class="sxs-lookup"><span data-stu-id="8e267-131">Name</span></span>          | <span data-ttu-id="8e267-132">説明</span><span class="sxs-lookup"><span data-stu-id="8e267-132">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="8e267-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e267-133">Authorization</span></span> | <span data-ttu-id="8e267-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8e267-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="8e267-136">応答</span><span class="sxs-lookup"><span data-stu-id="8e267-136">Response</span></span>

<span data-ttu-id="8e267-137">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="8e267-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="8e267-138">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="8e267-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="8e267-139">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="8e267-139">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="8e267-140">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="8e267-140">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="8e267-141">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="8e267-141">Report Refresh Date</span></span>
- <span data-ttu-id="8e267-142">レポート日付</span><span class="sxs-lookup"><span data-stu-id="8e267-142">Report Date</span></span>
- <span data-ttu-id="8e267-143">チーム チャット メッセージ</span><span class="sxs-lookup"><span data-stu-id="8e267-143">Team Chat Messages</span></span>
- <span data-ttu-id="8e267-144">非公開チャット メッセージ</span><span class="sxs-lookup"><span data-stu-id="8e267-144">Private Chat Messages</span></span>
- <span data-ttu-id="8e267-145">通話</span><span class="sxs-lookup"><span data-stu-id="8e267-145">Calls</span></span>
- <span data-ttu-id="8e267-146">会議</span><span class="sxs-lookup"><span data-stu-id="8e267-146">Meetings</span></span>
- <span data-ttu-id="8e267-147">その他のアクション</span><span class="sxs-lookup"><span data-stu-id="8e267-147">Other Actions</span></span>
- <span data-ttu-id="8e267-148">レポート期間</span><span class="sxs-lookup"><span data-stu-id="8e267-148">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="8e267-149">例</span><span class="sxs-lookup"><span data-stu-id="8e267-149">Example</span></span>

#### <a name="request"></a><span data-ttu-id="8e267-150">要求</span><span class="sxs-lookup"><span data-stu-id="8e267-150">Request</span></span>

<span data-ttu-id="8e267-151">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8e267-151">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8e267-152">プロトコル</span><span class="sxs-lookup"><span data-stu-id="8e267-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getTeamsUserActivityUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8e267-153">C#</span><span class="sxs-lookup"><span data-stu-id="8e267-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsuseractivityusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8e267-154">Javascript</span><span class="sxs-lookup"><span data-stu-id="8e267-154">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsuseractivityusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8e267-155">目的-C</span><span class="sxs-lookup"><span data-stu-id="8e267-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsuseractivityusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8e267-156">Java</span><span class="sxs-lookup"><span data-stu-id="8e267-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getteamsuseractivityusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8e267-157">応答</span><span class="sxs-lookup"><span data-stu-id="8e267-157">Response</span></span>

<span data-ttu-id="8e267-158">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8e267-158">The following is an example of the response.</span></span>

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

<span data-ttu-id="8e267-159">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="8e267-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Team Chat Messages,Private Chat Messages,Calls,Meetings,Other Actions,Report Period
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
