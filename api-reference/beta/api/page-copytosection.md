---
title: 'page: copyToSection'
description: ページを特定のセクションにコピーします。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 842647b52902aba153967109f83eec14e1b7d219
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35877251"
---
# <a name="page-copytosection"></a><span data-ttu-id="ff80b-103">page: copyToSection</span><span class="sxs-lookup"><span data-stu-id="ff80b-103">page: copyToSection</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff80b-104">ページを特定のセクションにコピーします。</span><span class="sxs-lookup"><span data-stu-id="ff80b-104">Copies a page to a specific section.</span></span>

<span data-ttu-id="ff80b-105">コピー操作では、非同期呼び出しパターンに従います。最初に Copy アクションを呼び出してから、結果の操作エンドポイントをポーリングします。</span><span class="sxs-lookup"><span data-stu-id="ff80b-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="ff80b-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ff80b-106">Permissions</span></span>
<span data-ttu-id="ff80b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ff80b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff80b-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ff80b-109">Permission type</span></span>      | <span data-ttu-id="ff80b-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ff80b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ff80b-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ff80b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ff80b-112">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff80b-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="ff80b-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ff80b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff80b-114">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ff80b-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="ff80b-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ff80b-115">Application</span></span> | <span data-ttu-id="ff80b-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff80b-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff80b-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ff80b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/pages/{id}/copyToSection
POST /users/{id | userPrincipalName}/onenote/pages/{id}/copyToSection
POST /groups/{id}/onenote/pages/{id}/copyToSection
POST /sites/{id}/onenote/pages/{id}/copyToSection
```
## <a name="request-headers"></a><span data-ttu-id="ff80b-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ff80b-118">Request headers</span></span>
| <span data-ttu-id="ff80b-119">名前</span><span class="sxs-lookup"><span data-stu-id="ff80b-119">Name</span></span>       | <span data-ttu-id="ff80b-120">型</span><span class="sxs-lookup"><span data-stu-id="ff80b-120">Type</span></span> | <span data-ttu-id="ff80b-121">説明</span><span class="sxs-lookup"><span data-stu-id="ff80b-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ff80b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff80b-122">Authorization</span></span>  | <span data-ttu-id="ff80b-123">string</span><span class="sxs-lookup"><span data-stu-id="ff80b-123">string</span></span>  | <span data-ttu-id="ff80b-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ff80b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ff80b-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ff80b-126">Content-Type</span></span> | <span data-ttu-id="ff80b-127">string</span><span class="sxs-lookup"><span data-stu-id="ff80b-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="ff80b-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="ff80b-128">Request body</span></span>
<span data-ttu-id="ff80b-129">要求本文で、操作に必要なパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="ff80b-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="ff80b-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="ff80b-130">Parameter</span></span>    | <span data-ttu-id="ff80b-131">型</span><span class="sxs-lookup"><span data-stu-id="ff80b-131">Type</span></span>   |<span data-ttu-id="ff80b-132">説明</span><span class="sxs-lookup"><span data-stu-id="ff80b-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ff80b-133">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="ff80b-133">siteCollectionId</span></span>|<span data-ttu-id="ff80b-134">String</span><span class="sxs-lookup"><span data-stu-id="ff80b-134">String</span></span>|<span data-ttu-id="ff80b-135">コピー先の SharePoint サイトの id。</span><span class="sxs-lookup"><span data-stu-id="ff80b-135">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="ff80b-136">Office 365 チームサイトにコピーする場合にのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="ff80b-136">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="ff80b-137">siteId</span><span class="sxs-lookup"><span data-stu-id="ff80b-137">siteId</span></span>|<span data-ttu-id="ff80b-138">String</span><span class="sxs-lookup"><span data-stu-id="ff80b-138">String</span></span>|<span data-ttu-id="ff80b-139">コピー先の SharePoint web の id です。</span><span class="sxs-lookup"><span data-stu-id="ff80b-139">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="ff80b-140">Office 365 チームサイトにコピーする場合にのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="ff80b-140">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="ff80b-141">groupId</span><span class="sxs-lookup"><span data-stu-id="ff80b-141">groupId</span></span>|<span data-ttu-id="ff80b-142">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="ff80b-142">String</span></span>|<span data-ttu-id="ff80b-143">コピー先のグループの id。</span><span class="sxs-lookup"><span data-stu-id="ff80b-143">The id of the group to copy to.</span></span> <span data-ttu-id="ff80b-144">Office 365 グループにコピーする場合にのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="ff80b-144">Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="ff80b-145">id</span><span class="sxs-lookup"><span data-stu-id="ff80b-145">id</span></span>|<span data-ttu-id="ff80b-146">String</span><span class="sxs-lookup"><span data-stu-id="ff80b-146">String</span></span>|<span data-ttu-id="ff80b-147">必須。</span><span class="sxs-lookup"><span data-stu-id="ff80b-147">Required.</span></span> <span data-ttu-id="ff80b-148">コピー先のセクションの id。</span><span class="sxs-lookup"><span data-stu-id="ff80b-148">The id of the destination section.</span></span>|

## <a name="response"></a><span data-ttu-id="ff80b-149">応答</span><span class="sxs-lookup"><span data-stu-id="ff80b-149">Response</span></span>

<span data-ttu-id="ff80b-150">成功した場合、このメソッド`202 Accepted`は応答コードと`Operation-Location`ヘッダーを返します。</span><span class="sxs-lookup"><span data-stu-id="ff80b-150">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="ff80b-151">操作の場所のエンドポイントをポーリングして、[コピー操作の状態を取得](onenoteoperation-get.md)します。</span><span class="sxs-lookup"><span data-stu-id="ff80b-151">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="ff80b-152">例</span><span class="sxs-lookup"><span data-stu-id="ff80b-152">Example</span></span>
<span data-ttu-id="ff80b-153">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="ff80b-153">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ff80b-154">要求</span><span class="sxs-lookup"><span data-stu-id="ff80b-154">Request</span></span>
<span data-ttu-id="ff80b-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ff80b-155">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ff80b-156">プロトコル</span><span class="sxs-lookup"><span data-stu-id="ff80b-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "page_copytosection"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/pages/{id}/copyToSection
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "groupId": "groupId-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ff80b-157">C#</span><span class="sxs-lookup"><span data-stu-id="ff80b-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/page-copytosection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ff80b-158">Javascript</span><span class="sxs-lookup"><span data-stu-id="ff80b-158">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/page-copytosection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ff80b-159">目的-C</span><span class="sxs-lookup"><span data-stu-id="ff80b-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/page-copytosection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ff80b-160">Java</span><span class="sxs-lookup"><span data-stu-id="ff80b-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/page-copytosection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ff80b-161">応答</span><span class="sxs-lookup"><span data-stu-id="ff80b-161">Response</span></span>
<span data-ttu-id="ff80b-162">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="ff80b-162">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteOperation"
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "page: copyToSection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
