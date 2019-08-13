---
title: 'セクション: copyToNotebook'
description: 特定のノートブックにセクションをコピーします。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: b149654a1f909291320ea86f6e6a84055549a9ba
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36364396"
---
# <a name="section-copytonotebook"></a><span data-ttu-id="40042-103">セクション: copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="40042-103">section: copyToNotebook</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40042-104">特定のノートブックにセクションをコピーします。</span><span class="sxs-lookup"><span data-stu-id="40042-104">Copies a section to a specific notebook.</span></span>

<span data-ttu-id="40042-105">コピー操作では、非同期呼び出しパターンに従います。最初に Copy アクションを呼び出してから、結果の操作エンドポイントをポーリングします。</span><span class="sxs-lookup"><span data-stu-id="40042-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>
## <a name="permissions"></a><span data-ttu-id="40042-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="40042-106">Permissions</span></span>
<span data-ttu-id="40042-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="40042-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40042-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="40042-109">Permission type</span></span>      | <span data-ttu-id="40042-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="40042-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="40042-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="40042-111">Delegated (work or school account)</span></span> | <span data-ttu-id="40042-112">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40042-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="40042-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="40042-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40042-114">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="40042-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="40042-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="40042-115">Application</span></span> | <span data-ttu-id="40042-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40042-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="40042-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="40042-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToNotebook
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToNotebook
POST /groups/{id}/onenote/sections/{id}/copyToNotebook
POST /sites/{id}/onenote/sections/{id}/copyToNotebook
```
## <a name="request-headers"></a><span data-ttu-id="40042-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="40042-118">Request headers</span></span>
| <span data-ttu-id="40042-119">名前</span><span class="sxs-lookup"><span data-stu-id="40042-119">Name</span></span>       | <span data-ttu-id="40042-120">型</span><span class="sxs-lookup"><span data-stu-id="40042-120">Type</span></span> | <span data-ttu-id="40042-121">説明</span><span class="sxs-lookup"><span data-stu-id="40042-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="40042-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="40042-122">Authorization</span></span>  | <span data-ttu-id="40042-123">string</span><span class="sxs-lookup"><span data-stu-id="40042-123">string</span></span>  | <span data-ttu-id="40042-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="40042-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="40042-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="40042-126">Content-Type</span></span> | <span data-ttu-id="40042-127">string</span><span class="sxs-lookup"><span data-stu-id="40042-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="40042-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="40042-128">Request body</span></span>
<span data-ttu-id="40042-129">要求本文で、操作に必要なパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="40042-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="40042-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="40042-130">Parameter</span></span>    | <span data-ttu-id="40042-131">型</span><span class="sxs-lookup"><span data-stu-id="40042-131">Type</span></span>   |<span data-ttu-id="40042-132">説明</span><span class="sxs-lookup"><span data-stu-id="40042-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="40042-133">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="40042-133">siteCollectionId</span></span>|<span data-ttu-id="40042-134">String</span><span class="sxs-lookup"><span data-stu-id="40042-134">String</span></span>|<span data-ttu-id="40042-135">コピー先の SharePoint サイトの id。</span><span class="sxs-lookup"><span data-stu-id="40042-135">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="40042-136">Office 365 チームサイトにコピーする場合にのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="40042-136">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="40042-137">siteId</span><span class="sxs-lookup"><span data-stu-id="40042-137">siteId</span></span>|<span data-ttu-id="40042-138">String</span><span class="sxs-lookup"><span data-stu-id="40042-138">String</span></span>|<span data-ttu-id="40042-139">コピー先の SharePoint web の id です。</span><span class="sxs-lookup"><span data-stu-id="40042-139">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="40042-140">Office 365 チームサイトにコピーする場合にのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="40042-140">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="40042-141">groupId</span><span class="sxs-lookup"><span data-stu-id="40042-141">groupId</span></span>|<span data-ttu-id="40042-142">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="40042-142">String</span></span>|<span data-ttu-id="40042-143">コピー先のグループの id。</span><span class="sxs-lookup"><span data-stu-id="40042-143">The id of the group to copy to.</span></span> <span data-ttu-id="40042-144">Office 365 グループにコピーする場合にのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="40042-144">Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="40042-145">id</span><span class="sxs-lookup"><span data-stu-id="40042-145">id</span></span>|<span data-ttu-id="40042-146">String</span><span class="sxs-lookup"><span data-stu-id="40042-146">String</span></span>|<span data-ttu-id="40042-147">必須。</span><span class="sxs-lookup"><span data-stu-id="40042-147">Required.</span></span> <span data-ttu-id="40042-148">コピー先のノートブックの id を指定します。</span><span class="sxs-lookup"><span data-stu-id="40042-148">The id of the destination notebook.</span></span> |
|<span data-ttu-id="40042-149">renameAs</span><span class="sxs-lookup"><span data-stu-id="40042-149">renameAs</span></span>|<span data-ttu-id="40042-150">String</span><span class="sxs-lookup"><span data-stu-id="40042-150">String</span></span>|<span data-ttu-id="40042-151">コピーするフィルターの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="40042-151">The name of the copy.</span></span> <span data-ttu-id="40042-152">Defaults to the name of the existing item.</span><span class="sxs-lookup"><span data-stu-id="40042-152">Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="40042-153">応答</span><span class="sxs-lookup"><span data-stu-id="40042-153">Response</span></span>

<span data-ttu-id="40042-154">成功した場合、このメソッド`202 Accepted`は応答コードと`Operation-Location`ヘッダーを返します。</span><span class="sxs-lookup"><span data-stu-id="40042-154">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="40042-155">操作の場所のエンドポイントをポーリングして、[コピー操作の状態を取得](onenoteoperation-get.md)します。</span><span class="sxs-lookup"><span data-stu-id="40042-155">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="40042-156">例</span><span class="sxs-lookup"><span data-stu-id="40042-156">Example</span></span>
<span data-ttu-id="40042-157">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="40042-157">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="40042-158">要求</span><span class="sxs-lookup"><span data-stu-id="40042-158">Request</span></span>
<span data-ttu-id="40042-159">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="40042-159">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="40042-160">プロトコル</span><span class="sxs-lookup"><span data-stu-id="40042-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "section_copytonotebook"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/sections/{id}/copyToNotebook
Content-type: application/json
Content-length: 84

{
  "id": "id-value",
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="40042-161">C#</span><span class="sxs-lookup"><span data-stu-id="40042-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/section-copytonotebook-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="40042-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="40042-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/section-copytonotebook-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="40042-163">目的-C</span><span class="sxs-lookup"><span data-stu-id="40042-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/section-copytonotebook-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="40042-164">Java</span><span class="sxs-lookup"><span data-stu-id="40042-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/section-copytonotebook-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="40042-165">応答</span><span class="sxs-lookup"><span data-stu-id="40042-165">Response</span></span>
<span data-ttu-id="40042-166">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="40042-166">Here is an example of the response.</span></span>
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
  "description": "section: copyToNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
