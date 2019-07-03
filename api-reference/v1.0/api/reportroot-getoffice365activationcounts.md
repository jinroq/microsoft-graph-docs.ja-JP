---
title: 'reportRoot: getOffice365ActivationCounts'
description: デスクトップとデバイスでの Office 365 のライセンス認証の数を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 122b95a09ec2135e0e9c900f4168a78a99104c0b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35445227"
---
# <a name="reportroot-getoffice365activationcounts"></a><span data-ttu-id="7f026-103">reportRoot: getOffice365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="7f026-103">reportRoot: getOffice365ActivationCounts</span></span>

<span data-ttu-id="7f026-104">デスクトップとデバイスでの Office 365 のライセンス認証の数を取得します。</span><span class="sxs-lookup"><span data-stu-id="7f026-104">Get the count of Office 365 activations on desktops and devices.</span></span>

> <span data-ttu-id="7f026-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Microsoft Office ライセンス認証](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7f026-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="7f026-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7f026-106">Permissions</span></span>

<span data-ttu-id="7f026-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7f026-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7f026-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7f026-109">Permission type</span></span>                        | <span data-ttu-id="7f026-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7f026-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="7f026-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="7f026-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7f026-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f026-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="7f026-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7f026-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f026-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f026-114">Not supported.</span></span>                           |
| <span data-ttu-id="7f026-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7f026-115">Application</span></span>                            | <span data-ttu-id="7f026-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f026-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="7f026-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7f026-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7f026-118">プロトコル</span><span class="sxs-lookup"><span data-stu-id="7f026-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationCounts
```

## <a name="request-headers"></a><span data-ttu-id="7f026-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7f026-119">Request headers</span></span>

| <span data-ttu-id="7f026-120">名前</span><span class="sxs-lookup"><span data-stu-id="7f026-120">Name</span></span>          | <span data-ttu-id="7f026-121">説明</span><span class="sxs-lookup"><span data-stu-id="7f026-121">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="7f026-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f026-122">Authorization</span></span> | <span data-ttu-id="7f026-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7f026-p102">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="7f026-125">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="7f026-125">If-None-Match</span></span> | <span data-ttu-id="7f026-126">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="7f026-126">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="7f026-127">省略可能。</span><span class="sxs-lookup"><span data-stu-id="7f026-127">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="7f026-128">応答</span><span class="sxs-lookup"><span data-stu-id="7f026-128">Response</span></span>

<span data-ttu-id="7f026-129">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="7f026-129">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="7f026-130">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="7f026-130">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="7f026-131">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="7f026-131">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="7f026-132">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="7f026-132">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="7f026-133">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="7f026-133">Report Refresh Date</span></span>
- <span data-ttu-id="7f026-134">製品の種類</span><span class="sxs-lookup"><span data-stu-id="7f026-134">Product Type</span></span>
- <span data-ttu-id="7f026-135">Windows</span><span class="sxs-lookup"><span data-stu-id="7f026-135">Windows</span></span>
- <span data-ttu-id="7f026-136">Mac</span><span class="sxs-lookup"><span data-stu-id="7f026-136">Mac</span></span>
- <span data-ttu-id="7f026-137">Android</span><span class="sxs-lookup"><span data-stu-id="7f026-137">Android</span></span>
- <span data-ttu-id="7f026-138">iOS</span><span class="sxs-lookup"><span data-stu-id="7f026-138">iOS</span></span>
- <span data-ttu-id="7f026-139">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="7f026-139">Windows 10 Mobile</span></span>

## <a name="example"></a><span data-ttu-id="7f026-140">例</span><span class="sxs-lookup"><span data-stu-id="7f026-140">Example</span></span>

#### <a name="request"></a><span data-ttu-id="7f026-141">要求</span><span class="sxs-lookup"><span data-stu-id="7f026-141">Request</span></span>

<span data-ttu-id="7f026-142">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7f026-142">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activationcounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationCounts
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7f026-143">C#</span><span class="sxs-lookup"><span data-stu-id="7f026-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activationcounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7f026-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="7f026-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activationcounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7f026-145">目的-C</span><span class="sxs-lookup"><span data-stu-id="7f026-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activationcounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7f026-146">応答</span><span class="sxs-lookup"><span data-stu-id="7f026-146">Response</span></span>

<span data-ttu-id="7f026-147">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7f026-147">The following is an example of the response.</span></span>

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

<span data-ttu-id="7f026-148">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="7f026-148">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Product Type,Windows,Mac,Android,iOS,Windows 10 Mobile
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
