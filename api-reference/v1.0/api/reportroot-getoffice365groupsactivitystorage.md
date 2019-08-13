---
title: 'reportRoot: getOffice365GroupsActivityStorage'
description: すべてのグループ メールボックスとグループ サイトで使用されているストレージの合計を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: bab786c086c6ceaec2dc8edd768a55c9d2327abb
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36373620"
---
# <a name="reportroot-getoffice365groupsactivitystorage"></a><span data-ttu-id="72d10-103">reportRoot: getOffice365GroupsActivityStorage</span><span class="sxs-lookup"><span data-stu-id="72d10-103">reportRoot: getOffice365GroupsActivityStorage</span></span>

<span data-ttu-id="72d10-104">すべてのグループ メールボックスとグループ サイトで使用されているストレージの合計を取得します。</span><span class="sxs-lookup"><span data-stu-id="72d10-104">Get the total storage used across all group mailboxes and group sites.</span></span>

> <span data-ttu-id="72d10-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Office 365 グループ](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="72d10-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="72d10-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="72d10-106">Permissions</span></span>

<span data-ttu-id="72d10-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="72d10-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="72d10-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="72d10-109">Permission type</span></span>                        | <span data-ttu-id="72d10-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="72d10-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="72d10-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="72d10-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="72d10-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="72d10-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="72d10-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="72d10-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72d10-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="72d10-114">Not supported.</span></span>                           |
| <span data-ttu-id="72d10-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="72d10-115">Application</span></span>                            | <span data-ttu-id="72d10-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="72d10-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="72d10-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="72d10-117">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityStorage(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="72d10-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="72d10-118">Function parameters</span></span>

<span data-ttu-id="72d10-119">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="72d10-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="72d10-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="72d10-120">Parameter</span></span> | <span data-ttu-id="72d10-121">型</span><span class="sxs-lookup"><span data-stu-id="72d10-121">Type</span></span>   | <span data-ttu-id="72d10-122">説明</span><span class="sxs-lookup"><span data-stu-id="72d10-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="72d10-123">period</span><span class="sxs-lookup"><span data-stu-id="72d10-123">period</span></span>    | <span data-ttu-id="72d10-124">文字列</span><span class="sxs-lookup"><span data-stu-id="72d10-124">string</span></span> | <span data-ttu-id="72d10-125">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="72d10-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="72d10-126">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="72d10-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="72d10-127">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="72d10-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="72d10-128">必須。</span><span class="sxs-lookup"><span data-stu-id="72d10-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="72d10-129">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="72d10-129">Request headers</span></span>

| <span data-ttu-id="72d10-130">名前</span><span class="sxs-lookup"><span data-stu-id="72d10-130">Name</span></span>          | <span data-ttu-id="72d10-131">説明</span><span class="sxs-lookup"><span data-stu-id="72d10-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="72d10-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="72d10-132">Authorization</span></span> | <span data-ttu-id="72d10-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="72d10-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="72d10-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="72d10-135">If-None-Match</span></span> | <span data-ttu-id="72d10-136">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="72d10-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="72d10-137">省略可能。</span><span class="sxs-lookup"><span data-stu-id="72d10-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="72d10-138">応答</span><span class="sxs-lookup"><span data-stu-id="72d10-138">Response</span></span>

<span data-ttu-id="72d10-139">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="72d10-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="72d10-140">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="72d10-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="72d10-141">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="72d10-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="72d10-142">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="72d10-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="72d10-143">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="72d10-143">Report Refresh Date</span></span>
- <span data-ttu-id="72d10-144">使用済みメールボックス ストレージ (バイト)</span><span class="sxs-lookup"><span data-stu-id="72d10-144">Mailbox Storage Used (Byte)</span></span>
- <span data-ttu-id="72d10-145">使用済みサイト ストレージ (バイト)</span><span class="sxs-lookup"><span data-stu-id="72d10-145">Site Storage Used (Byte)</span></span>
- <span data-ttu-id="72d10-146">レポート日付</span><span class="sxs-lookup"><span data-stu-id="72d10-146">Report Date</span></span>
- <span data-ttu-id="72d10-147">レポート期間</span><span class="sxs-lookup"><span data-stu-id="72d10-147">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="72d10-148">例</span><span class="sxs-lookup"><span data-stu-id="72d10-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="72d10-149">要求</span><span class="sxs-lookup"><span data-stu-id="72d10-149">Request</span></span>

<span data-ttu-id="72d10-150">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="72d10-150">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="72d10-151">プロトコル</span><span class="sxs-lookup"><span data-stu-id="72d10-151">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365groupsactivitystorage"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365GroupsActivityStorage(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="72d10-152">C#</span><span class="sxs-lookup"><span data-stu-id="72d10-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365groupsactivitystorage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="72d10-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="72d10-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365groupsactivitystorage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="72d10-154">目的-C</span><span class="sxs-lookup"><span data-stu-id="72d10-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365groupsactivitystorage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="72d10-155">Java</span><span class="sxs-lookup"><span data-stu-id="72d10-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getoffice365groupsactivitystorage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="72d10-156">応答</span><span class="sxs-lookup"><span data-stu-id="72d10-156">Response</span></span>

<span data-ttu-id="72d10-157">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="72d10-157">The following is an example of the response.</span></span>

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

<span data-ttu-id="72d10-158">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="72d10-158">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Mailbox Storage Used (Byte),Site Storage Used (Byte),Report Date,Report Period
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
