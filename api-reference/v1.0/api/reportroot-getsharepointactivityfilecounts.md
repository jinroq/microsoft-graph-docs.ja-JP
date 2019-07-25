---
title: 'reportRoot: getSharePointActivityFileCounts'
description: SharePoint サイトに保存されているファイルを操作した、それぞれ別個のライセンス ユーザーの数を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 17e4d806f08cde191ba7757a183e452645ba8343
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893588"
---
# <a name="reportroot-getsharepointactivityfilecounts"></a><span data-ttu-id="ef1c8-103">reportRoot: getSharePointActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="ef1c8-103">reportRoot: getSharePointActivityFileCounts</span></span>

<span data-ttu-id="ef1c8-104">SharePoint サイトに保存されているファイルを操作した、それぞれ別個のライセンス ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="ef1c8-104">Get the number of unique, licensed users who interacted with files stored on SharePoint sites.</span></span>

> <span data-ttu-id="ef1c8-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: SharePoint アクティビティ](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ef1c8-105">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="ef1c8-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ef1c8-106">Permissions</span></span>

<span data-ttu-id="ef1c8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ef1c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ef1c8-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ef1c8-109">Permission type</span></span>                        | <span data-ttu-id="ef1c8-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ef1c8-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ef1c8-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="ef1c8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ef1c8-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ef1c8-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ef1c8-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ef1c8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef1c8-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ef1c8-114">Not supported.</span></span>                           |
| <span data-ttu-id="ef1c8-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ef1c8-115">Application</span></span>                            | <span data-ttu-id="ef1c8-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ef1c8-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="ef1c8-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ef1c8-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ef1c8-118">プロトコル</span><span class="sxs-lookup"><span data-stu-id="ef1c8-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="ef1c8-119">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="ef1c8-119">Function parameters</span></span>

<span data-ttu-id="ef1c8-120">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="ef1c8-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="ef1c8-121">パラメーター</span><span class="sxs-lookup"><span data-stu-id="ef1c8-121">Parameter</span></span> | <span data-ttu-id="ef1c8-122">型</span><span class="sxs-lookup"><span data-stu-id="ef1c8-122">Type</span></span>   | <span data-ttu-id="ef1c8-123">説明</span><span class="sxs-lookup"><span data-stu-id="ef1c8-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="ef1c8-124">period</span><span class="sxs-lookup"><span data-stu-id="ef1c8-124">period</span></span>    | <span data-ttu-id="ef1c8-125">文字列</span><span class="sxs-lookup"><span data-stu-id="ef1c8-125">string</span></span> | <span data-ttu-id="ef1c8-126">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="ef1c8-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="ef1c8-127">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="ef1c8-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="ef1c8-128">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="ef1c8-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="ef1c8-129">必須。</span><span class="sxs-lookup"><span data-stu-id="ef1c8-129">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="ef1c8-130">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ef1c8-130">Request headers</span></span>

| <span data-ttu-id="ef1c8-131">名前</span><span class="sxs-lookup"><span data-stu-id="ef1c8-131">Name</span></span>          | <span data-ttu-id="ef1c8-132">説明</span><span class="sxs-lookup"><span data-stu-id="ef1c8-132">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="ef1c8-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef1c8-133">Authorization</span></span> | <span data-ttu-id="ef1c8-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ef1c8-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="ef1c8-136">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="ef1c8-136">If-None-Match</span></span> | <span data-ttu-id="ef1c8-137">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="ef1c8-137">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="ef1c8-138">省略可能。</span><span class="sxs-lookup"><span data-stu-id="ef1c8-138">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="ef1c8-139">応答</span><span class="sxs-lookup"><span data-stu-id="ef1c8-139">Response</span></span>

<span data-ttu-id="ef1c8-140">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="ef1c8-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ef1c8-141">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="ef1c8-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ef1c8-142">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="ef1c8-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ef1c8-143">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="ef1c8-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="ef1c8-144">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="ef1c8-144">Report Refresh Date</span></span>
- <span data-ttu-id="ef1c8-145">表示済みまたは編集済み</span><span class="sxs-lookup"><span data-stu-id="ef1c8-145">Viewed Or Edited</span></span>
- <span data-ttu-id="ef1c8-146">同期済み</span><span class="sxs-lookup"><span data-stu-id="ef1c8-146">Synced</span></span>
- <span data-ttu-id="ef1c8-147">社内で共有済み</span><span class="sxs-lookup"><span data-stu-id="ef1c8-147">Shared Internally</span></span>
- <span data-ttu-id="ef1c8-148">外部で共有済み</span><span class="sxs-lookup"><span data-stu-id="ef1c8-148">Shared Externally</span></span>
- <span data-ttu-id="ef1c8-149">レポート日付</span><span class="sxs-lookup"><span data-stu-id="ef1c8-149">Report Date</span></span>
- <span data-ttu-id="ef1c8-150">レポート期間</span><span class="sxs-lookup"><span data-stu-id="ef1c8-150">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="ef1c8-151">例</span><span class="sxs-lookup"><span data-stu-id="ef1c8-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ef1c8-152">要求</span><span class="sxs-lookup"><span data-stu-id="ef1c8-152">Request</span></span>

<span data-ttu-id="ef1c8-153">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ef1c8-153">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getsharepointactivityfilecounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointActivityFileCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ef1c8-154">C#</span><span class="sxs-lookup"><span data-stu-id="ef1c8-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointactivityfilecounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ef1c8-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="ef1c8-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointactivityfilecounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ef1c8-156">目的-C</span><span class="sxs-lookup"><span data-stu-id="ef1c8-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointactivityfilecounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ef1c8-157">Java</span><span class="sxs-lookup"><span data-stu-id="ef1c8-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getsharepointactivityfilecounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ef1c8-158">応答</span><span class="sxs-lookup"><span data-stu-id="ef1c8-158">Response</span></span>

<span data-ttu-id="ef1c8-159">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ef1c8-159">The following is an example of the response.</span></span>

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

<span data-ttu-id="ef1c8-160">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="ef1c8-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
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
