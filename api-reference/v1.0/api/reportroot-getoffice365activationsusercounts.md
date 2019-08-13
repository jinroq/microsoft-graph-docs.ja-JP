---
title: 'reportRoot: getOffice365ActivationsUserCounts'
description: 有効になっているユーザーの数と、デスクトップまたはデバイスまたは共有コンピューターで Office サブスクリプションをアクティブ化したユーザーの数を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: fd92cee745a9db99ebaa42cfaf00d6d63f7bd48b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327186"
---
# <a name="reportroot-getoffice365activationsusercounts"></a><span data-ttu-id="8a48e-103">reportRoot: getOffice365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="8a48e-103">reportRoot: getOffice365ActivationsUserCounts</span></span>

<span data-ttu-id="8a48e-104">有効になっているユーザーの数と、デスクトップまたはデバイスまたは共有コンピューターで Office サブスクリプションをアクティブ化したユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="8a48e-104">Get the count of users that are enabled and those that have activated the Office subscription on desktop or devices or shared computers.</span></span>

> <span data-ttu-id="8a48e-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Microsoft Office ライセンス認証](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8a48e-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="8a48e-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8a48e-106">Permissions</span></span>

<span data-ttu-id="8a48e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8a48e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8a48e-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8a48e-109">Permission type</span></span>                        | <span data-ttu-id="8a48e-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8a48e-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="8a48e-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="8a48e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8a48e-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8a48e-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="8a48e-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8a48e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a48e-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8a48e-114">Not supported.</span></span>                           |
| <span data-ttu-id="8a48e-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8a48e-115">Application</span></span>                            | <span data-ttu-id="8a48e-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8a48e-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="8a48e-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8a48e-117">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserCounts
```

## <a name="request-headers"></a><span data-ttu-id="8a48e-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8a48e-118">Request headers</span></span>

| <span data-ttu-id="8a48e-119">名前</span><span class="sxs-lookup"><span data-stu-id="8a48e-119">Name</span></span>          | <span data-ttu-id="8a48e-120">説明</span><span class="sxs-lookup"><span data-stu-id="8a48e-120">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="8a48e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a48e-121">Authorization</span></span> | <span data-ttu-id="8a48e-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8a48e-p102">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="8a48e-124">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="8a48e-124">If-None-Match</span></span> | <span data-ttu-id="8a48e-125">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="8a48e-125">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="8a48e-126">省略可能。</span><span class="sxs-lookup"><span data-stu-id="8a48e-126">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="8a48e-127">応答</span><span class="sxs-lookup"><span data-stu-id="8a48e-127">Response</span></span>

<span data-ttu-id="8a48e-128">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="8a48e-128">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="8a48e-129">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="8a48e-129">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="8a48e-130">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="8a48e-130">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="8a48e-131">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="8a48e-131">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="8a48e-132">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="8a48e-132">Report Refresh Date</span></span>
- <span data-ttu-id="8a48e-133">製品の種類</span><span class="sxs-lookup"><span data-stu-id="8a48e-133">Product Type</span></span>
- <span data-ttu-id="8a48e-134">割り当て済み</span><span class="sxs-lookup"><span data-stu-id="8a48e-134">Assigned</span></span>
- <span data-ttu-id="8a48e-135">アクティブ</span><span class="sxs-lookup"><span data-stu-id="8a48e-135">Activated</span></span>
- <span data-ttu-id="8a48e-136">共有コンピューターのライセンス認証</span><span class="sxs-lookup"><span data-stu-id="8a48e-136">Shared Computer Activation</span></span>

## <a name="example"></a><span data-ttu-id="8a48e-137">例</span><span class="sxs-lookup"><span data-stu-id="8a48e-137">Example</span></span>

#### <a name="request"></a><span data-ttu-id="8a48e-138">要求</span><span class="sxs-lookup"><span data-stu-id="8a48e-138">Request</span></span>

<span data-ttu-id="8a48e-139">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8a48e-139">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8a48e-140">プロトコル</span><span class="sxs-lookup"><span data-stu-id="8a48e-140">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activationsusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationsUserCounts
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8a48e-141">C#</span><span class="sxs-lookup"><span data-stu-id="8a48e-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activationsusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8a48e-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8a48e-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activationsusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8a48e-143">目的-C</span><span class="sxs-lookup"><span data-stu-id="8a48e-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activationsusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8a48e-144">Java</span><span class="sxs-lookup"><span data-stu-id="8a48e-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getoffice365activationsusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8a48e-145">応答</span><span class="sxs-lookup"><span data-stu-id="8a48e-145">Response</span></span>

<span data-ttu-id="8a48e-146">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8a48e-146">The following is an example of the response.</span></span>

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

<span data-ttu-id="8a48e-147">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="8a48e-147">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Product Type,Assigned,Activated,Shared Computer Activation
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
