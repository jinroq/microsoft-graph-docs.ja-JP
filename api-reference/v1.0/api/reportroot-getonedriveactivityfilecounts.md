---
title: 'reportRoot: getOneDriveActivityFileCounts'
description: いずれかの OneDrive アカウントに対してファイル操作を実行した、一意のライセンス ユーザーの数を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 1de9937f2c54bedbb43b2d33d7cbe7ee09d510f3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36025058"
---
# <a name="reportroot-getonedriveactivityfilecounts"></a><span data-ttu-id="33188-103">reportRoot: getOneDriveActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="33188-103">reportRoot: getOneDriveActivityFileCounts</span></span>

<span data-ttu-id="33188-104">いずれかの OneDrive アカウントに対してファイル操作を実行した、一意のライセンス ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="33188-104">Get the number of unique, licensed users that performed file interactions against any OneDrive account.</span></span>

> <span data-ttu-id="33188-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: OneDrive for Business のアクティビティ](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="33188-105">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="permissions"></a><span data-ttu-id="33188-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="33188-106">Permissions</span></span>

<span data-ttu-id="33188-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="33188-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="33188-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="33188-109">Permission type</span></span>                        | <span data-ttu-id="33188-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="33188-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="33188-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="33188-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="33188-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="33188-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="33188-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="33188-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33188-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="33188-114">Not supported.</span></span>                           |
| <span data-ttu-id="33188-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="33188-115">Application</span></span>                            | <span data-ttu-id="33188-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="33188-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="33188-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="33188-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="33188-118">プロトコル</span><span class="sxs-lookup"><span data-stu-id="33188-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveActivityFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="33188-119">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="33188-119">Function parameters</span></span>

<span data-ttu-id="33188-120">要求 URL に、次のパラメーターと有効な値を指定します。</span><span class="sxs-lookup"><span data-stu-id="33188-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="33188-121">パラメーター</span><span class="sxs-lookup"><span data-stu-id="33188-121">Parameter</span></span> | <span data-ttu-id="33188-122">型</span><span class="sxs-lookup"><span data-stu-id="33188-122">Type</span></span>   | <span data-ttu-id="33188-123">説明</span><span class="sxs-lookup"><span data-stu-id="33188-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="33188-124">period</span><span class="sxs-lookup"><span data-stu-id="33188-124">period</span></span>    | <span data-ttu-id="33188-125">文字列</span><span class="sxs-lookup"><span data-stu-id="33188-125">string</span></span> | <span data-ttu-id="33188-126">レポートを集計する期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="33188-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="33188-127">{period_value} でサポートされている値は D7、D30、D90、D180 です。</span><span class="sxs-lookup"><span data-stu-id="33188-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="33188-128">これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。</span><span class="sxs-lookup"><span data-stu-id="33188-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="33188-129">必須。</span><span class="sxs-lookup"><span data-stu-id="33188-129">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="33188-130">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="33188-130">Request headers</span></span>

| <span data-ttu-id="33188-131">名前</span><span class="sxs-lookup"><span data-stu-id="33188-131">Name</span></span>          | <span data-ttu-id="33188-132">説明</span><span class="sxs-lookup"><span data-stu-id="33188-132">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="33188-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="33188-133">Authorization</span></span> | <span data-ttu-id="33188-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="33188-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="33188-136">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="33188-136">If-None-Match</span></span> | <span data-ttu-id="33188-137">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="33188-137">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="33188-138">省略可能。</span><span class="sxs-lookup"><span data-stu-id="33188-138">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="33188-139">応答</span><span class="sxs-lookup"><span data-stu-id="33188-139">Response</span></span>

<span data-ttu-id="33188-140">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="33188-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="33188-141">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="33188-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="33188-142">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="33188-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="33188-143">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="33188-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="33188-144">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="33188-144">Report Refresh Date</span></span>
- <span data-ttu-id="33188-145">表示済みまたは編集済み</span><span class="sxs-lookup"><span data-stu-id="33188-145">Viewed Or Edited</span></span>
- <span data-ttu-id="33188-146">同期済み</span><span class="sxs-lookup"><span data-stu-id="33188-146">Synced</span></span>
- <span data-ttu-id="33188-147">社内で共有済み</span><span class="sxs-lookup"><span data-stu-id="33188-147">Shared Internally</span></span>
- <span data-ttu-id="33188-148">外部で共有済み</span><span class="sxs-lookup"><span data-stu-id="33188-148">Shared Externally</span></span>
- <span data-ttu-id="33188-149">レポート日付</span><span class="sxs-lookup"><span data-stu-id="33188-149">Report Date</span></span>
- <span data-ttu-id="33188-150">レポート期間</span><span class="sxs-lookup"><span data-stu-id="33188-150">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="33188-151">例</span><span class="sxs-lookup"><span data-stu-id="33188-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="33188-152">要求</span><span class="sxs-lookup"><span data-stu-id="33188-152">Request</span></span>

<span data-ttu-id="33188-153">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="33188-153">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getonedriveactivityfilecounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOneDriveActivityFileCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="33188-154">C#</span><span class="sxs-lookup"><span data-stu-id="33188-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveactivityfilecounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="33188-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="33188-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveactivityfilecounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="33188-156">目的-C</span><span class="sxs-lookup"><span data-stu-id="33188-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveactivityfilecounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="33188-157">Java</span><span class="sxs-lookup"><span data-stu-id="33188-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getonedriveactivityfilecounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="33188-158">応答</span><span class="sxs-lookup"><span data-stu-id="33188-158">Response</span></span>

<span data-ttu-id="33188-159">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="33188-159">The following is an example of the response.</span></span>

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

<span data-ttu-id="33188-160">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="33188-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
