---
title: 'reportRoot: getOffice365ActivationsUserDetail'
description: Office 365 がアクティブ化されているユーザーに関する詳細情報を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 4f16e070f2ac39e83b70185192bf19d09eab1038
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35460610"
---
# <a name="reportroot-getoffice365activationsuserdetail"></a><span data-ttu-id="bf945-103">reportRoot: getOffice365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="bf945-103">reportRoot: getOffice365ActivationsUserDetail</span></span>

<span data-ttu-id="bf945-104">Office 365 がアクティブ化されているユーザーに関する詳細情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="bf945-104">Get details about users who have activated Office 365.</span></span>

> <span data-ttu-id="bf945-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Microsoft Office ライセンス認証](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bf945-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="bf945-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bf945-106">Permissions</span></span>

<span data-ttu-id="bf945-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bf945-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bf945-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bf945-109">Permission type</span></span>                        | <span data-ttu-id="bf945-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bf945-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="bf945-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="bf945-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="bf945-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf945-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="bf945-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bf945-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf945-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bf945-114">Not supported.</span></span>                           |
| <span data-ttu-id="bf945-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bf945-115">Application</span></span>                            | <span data-ttu-id="bf945-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf945-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="bf945-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bf945-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="bf945-118">プロトコル</span><span class="sxs-lookup"><span data-stu-id="bf945-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserDetail
```

## <a name="request-headers"></a><span data-ttu-id="bf945-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bf945-119">Request headers</span></span>

| <span data-ttu-id="bf945-120">名前</span><span class="sxs-lookup"><span data-stu-id="bf945-120">Name</span></span>          | <span data-ttu-id="bf945-121">説明</span><span class="sxs-lookup"><span data-stu-id="bf945-121">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="bf945-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bf945-122">Authorization</span></span> | <span data-ttu-id="bf945-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="bf945-p102">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="bf945-125">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="bf945-125">If-None-Match</span></span> | <span data-ttu-id="bf945-126">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="bf945-126">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="bf945-127">省略可能。</span><span class="sxs-lookup"><span data-stu-id="bf945-127">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="bf945-128">応答</span><span class="sxs-lookup"><span data-stu-id="bf945-128">Response</span></span>

<span data-ttu-id="bf945-129">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="bf945-129">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="bf945-130">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="bf945-130">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="bf945-131">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="bf945-131">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="bf945-132">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="bf945-132">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="bf945-133">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="bf945-133">Report Refresh Date</span></span>
- <span data-ttu-id="bf945-134">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="bf945-134">User Principal Name</span></span>
- <span data-ttu-id="bf945-135">表示名</span><span class="sxs-lookup"><span data-stu-id="bf945-135">Display Name</span></span>
- <span data-ttu-id="bf945-136">製品の種類</span><span class="sxs-lookup"><span data-stu-id="bf945-136">Product Type</span></span>
- <span data-ttu-id="bf945-137">最後のライセンス認証日</span><span class="sxs-lookup"><span data-stu-id="bf945-137">Last Activated Date</span></span>
- <span data-ttu-id="bf945-138">Windows</span><span class="sxs-lookup"><span data-stu-id="bf945-138">Windows</span></span>
- <span data-ttu-id="bf945-139">Mac</span><span class="sxs-lookup"><span data-stu-id="bf945-139">Mac</span></span>
- <span data-ttu-id="bf945-140">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="bf945-140">Windows 10 Mobile</span></span>
- <span data-ttu-id="bf945-141">iOS</span><span class="sxs-lookup"><span data-stu-id="bf945-141">iOS</span></span>
- <span data-ttu-id="bf945-142">Android</span><span class="sxs-lookup"><span data-stu-id="bf945-142">Android</span></span>
- <span data-ttu-id="bf945-143">共有コンピューターでのアクティブ化</span><span class="sxs-lookup"><span data-stu-id="bf945-143">Activated On Shared Computer</span></span>

## <a name="example"></a><span data-ttu-id="bf945-144">例</span><span class="sxs-lookup"><span data-stu-id="bf945-144">Example</span></span>

#### <a name="request"></a><span data-ttu-id="bf945-145">要求</span><span class="sxs-lookup"><span data-stu-id="bf945-145">Request</span></span>

<span data-ttu-id="bf945-146">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="bf945-146">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activationsuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationsUserDetail
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bf945-147">C#</span><span class="sxs-lookup"><span data-stu-id="bf945-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activationsuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bf945-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="bf945-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activationsuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bf945-149">目的-C</span><span class="sxs-lookup"><span data-stu-id="bf945-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activationsuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="bf945-150">応答</span><span class="sxs-lookup"><span data-stu-id="bf945-150">Response</span></span>

<span data-ttu-id="bf945-151">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="bf945-151">The following is an example of the response.</span></span>

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

<span data-ttu-id="bf945-152">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="bf945-152">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Product Type,Last Activated Date,Windows,Mac,Windows 10 Mobile,iOS,Android,Activated On Shared Computer
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
