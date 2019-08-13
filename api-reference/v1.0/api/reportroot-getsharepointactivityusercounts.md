---
title: 'reportRoot: getSharePointActivityUserCounts'
description: アクティブ ユーザーの数の傾向を取得します。 ユーザーが一定期間中にファイル アクティビティ (保存、同期、変更、共有) を実行するか、またはページにアクセスすると、そのユーザーはアクティブとみなされます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 7eabd3b86f83283005918670981839c04098318b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36321845"
---
# <a name="reportroot-getsharepointactivityusercounts"></a><span data-ttu-id="f194a-104">reportRoot: getSharePointActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="f194a-104">reportRoot: getSharePointActivityUserCounts</span></span>

<span data-ttu-id="f194a-105">アクティブ ユーザーの数の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="f194a-105">Get the trend in the number of active users.</span></span> <span data-ttu-id="f194a-106">ユーザーが一定期間中にファイル アクティビティ (保存、同期、変更、共有) を実行するか、またはページにアクセスすると、そのユーザーはアクティブとみなされます。</span><span class="sxs-lookup"><span data-stu-id="f194a-106">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span>

> <span data-ttu-id="f194a-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: SharePoint アクティビティ](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f194a-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="f194a-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f194a-108">Permissions</span></span>

<span data-ttu-id="f194a-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f194a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f194a-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f194a-111">Permission type</span></span>                        | <span data-ttu-id="f194a-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f194a-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="f194a-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="f194a-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="f194a-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f194a-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="f194a-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f194a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f194a-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f194a-116">Not supported.</span></span>                           |
| <span data-ttu-id="f194a-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f194a-117">Application</span></span>                            | <span data-ttu-id="f194a-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f194a-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="f194a-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f194a-119">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="f194a-120">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="f194a-120">Function parameters</span></span>

<span data-ttu-id="f194a-121">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="f194a-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="f194a-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="f194a-122">Parameter</span></span> | <span data-ttu-id="f194a-123">型</span><span class="sxs-lookup"><span data-stu-id="f194a-123">Type</span></span>   | <span data-ttu-id="f194a-124">説明</span><span class="sxs-lookup"><span data-stu-id="f194a-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="f194a-125">period</span><span class="sxs-lookup"><span data-stu-id="f194a-125">period</span></span>    | <span data-ttu-id="f194a-126">文字列</span><span class="sxs-lookup"><span data-stu-id="f194a-126">string</span></span> | <span data-ttu-id="f194a-127">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="f194a-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="f194a-128">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="f194a-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="f194a-129">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="f194a-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="f194a-130">必須。</span><span class="sxs-lookup"><span data-stu-id="f194a-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="f194a-131">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f194a-131">Request headers</span></span>

| <span data-ttu-id="f194a-132">名前</span><span class="sxs-lookup"><span data-stu-id="f194a-132">Name</span></span>          | <span data-ttu-id="f194a-133">説明</span><span class="sxs-lookup"><span data-stu-id="f194a-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="f194a-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="f194a-134">Authorization</span></span> | <span data-ttu-id="f194a-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f194a-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="f194a-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="f194a-137">If-None-Match</span></span> | <span data-ttu-id="f194a-138">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="f194a-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="f194a-139">省略可能。</span><span class="sxs-lookup"><span data-stu-id="f194a-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="f194a-140">応答</span><span class="sxs-lookup"><span data-stu-id="f194a-140">Response</span></span>

<span data-ttu-id="f194a-141">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="f194a-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="f194a-142">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="f194a-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="f194a-143">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="f194a-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="f194a-144">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="f194a-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="f194a-145">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="f194a-145">Report Refresh Date</span></span>
- <span data-ttu-id="f194a-146">アクセスしたページ</span><span class="sxs-lookup"><span data-stu-id="f194a-146">Visited Page</span></span>
- <span data-ttu-id="f194a-147">表示済みまたは編集済み</span><span class="sxs-lookup"><span data-stu-id="f194a-147">Viewed Or Edited</span></span>
- <span data-ttu-id="f194a-148">同期済み</span><span class="sxs-lookup"><span data-stu-id="f194a-148">Synced</span></span>
- <span data-ttu-id="f194a-149">社内で共有済み</span><span class="sxs-lookup"><span data-stu-id="f194a-149">Shared Internally</span></span>
- <span data-ttu-id="f194a-150">外部で共有済み</span><span class="sxs-lookup"><span data-stu-id="f194a-150">Shared Externally</span></span>
- <span data-ttu-id="f194a-151">レポート日付</span><span class="sxs-lookup"><span data-stu-id="f194a-151">Report Date</span></span>
- <span data-ttu-id="f194a-152">レポート期間</span><span class="sxs-lookup"><span data-stu-id="f194a-152">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="f194a-153">例</span><span class="sxs-lookup"><span data-stu-id="f194a-153">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f194a-154">要求</span><span class="sxs-lookup"><span data-stu-id="f194a-154">Request</span></span>

<span data-ttu-id="f194a-155">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f194a-155">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f194a-156">プロトコル</span><span class="sxs-lookup"><span data-stu-id="f194a-156">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getsharepointactivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointActivityUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f194a-157">C#</span><span class="sxs-lookup"><span data-stu-id="f194a-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointactivityusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f194a-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f194a-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointactivityusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f194a-159">目的-C</span><span class="sxs-lookup"><span data-stu-id="f194a-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointactivityusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f194a-160">Java</span><span class="sxs-lookup"><span data-stu-id="f194a-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getsharepointactivityusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f194a-161">応答</span><span class="sxs-lookup"><span data-stu-id="f194a-161">Response</span></span>

<span data-ttu-id="f194a-162">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f194a-162">The following is an example of the response.</span></span>

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

<span data-ttu-id="f194a-163">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="f194a-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Visited Page,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
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
