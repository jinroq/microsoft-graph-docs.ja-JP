---
title: 'セクション: copyToNotebook'
description: 特定のノートブックにセクションをコピーします。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: ed7285f601d0509404ecab73a2029e9f55212971
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33603580"
---
# <a name="section-copytonotebook"></a><span data-ttu-id="18e96-103">セクション: copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="18e96-103">section: copyToNotebook</span></span>
<span data-ttu-id="18e96-104">特定のノートブックにセクションをコピーします。</span><span class="sxs-lookup"><span data-stu-id="18e96-104">Copies a section to a specific notebook.</span></span>

<span data-ttu-id="18e96-105">コピー操作では、非同期呼び出しパターンに従います。最初に Copy アクションを呼び出してから、結果の操作エンドポイントをポーリングします。</span><span class="sxs-lookup"><span data-stu-id="18e96-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>
## <a name="permissions"></a><span data-ttu-id="18e96-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="18e96-106">Permissions</span></span>
<span data-ttu-id="18e96-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="18e96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18e96-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="18e96-109">Permission type</span></span>      | <span data-ttu-id="18e96-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="18e96-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18e96-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="18e96-111">Delegated (work or school account)</span></span> | <span data-ttu-id="18e96-112">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18e96-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="18e96-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="18e96-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18e96-114">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18e96-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="18e96-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="18e96-115">Application</span></span> | <span data-ttu-id="18e96-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18e96-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="18e96-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="18e96-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToNotebook
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToNotebook
POST /groups/{id}/onenote/sections/{id}/copyToNotebook
```
## <a name="request-headers"></a><span data-ttu-id="18e96-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="18e96-118">Request headers</span></span>
| <span data-ttu-id="18e96-119">名前</span><span class="sxs-lookup"><span data-stu-id="18e96-119">Name</span></span>       | <span data-ttu-id="18e96-120">型</span><span class="sxs-lookup"><span data-stu-id="18e96-120">Type</span></span> | <span data-ttu-id="18e96-121">説明</span><span class="sxs-lookup"><span data-stu-id="18e96-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="18e96-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="18e96-122">Authorization</span></span>  | <span data-ttu-id="18e96-123">string</span><span class="sxs-lookup"><span data-stu-id="18e96-123">string</span></span>  | <span data-ttu-id="18e96-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="18e96-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="18e96-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="18e96-126">Content-Type</span></span> | <span data-ttu-id="18e96-127">string</span><span class="sxs-lookup"><span data-stu-id="18e96-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="18e96-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="18e96-128">Request body</span></span>
<span data-ttu-id="18e96-129">要求本文で、操作に必要なパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="18e96-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="18e96-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="18e96-130">Parameter</span></span>    | <span data-ttu-id="18e96-131">型</span><span class="sxs-lookup"><span data-stu-id="18e96-131">Type</span></span>   |<span data-ttu-id="18e96-132">説明</span><span class="sxs-lookup"><span data-stu-id="18e96-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="18e96-133">groupId</span><span class="sxs-lookup"><span data-stu-id="18e96-133">groupId</span></span>|<span data-ttu-id="18e96-134">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="18e96-134">String</span></span>|<span data-ttu-id="18e96-135">コピー先のグループの id。</span><span class="sxs-lookup"><span data-stu-id="18e96-135">The id of the group to copy to.</span></span> <span data-ttu-id="18e96-136">Office 365 グループにコピーする場合にのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="18e96-136">Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="18e96-137">id</span><span class="sxs-lookup"><span data-stu-id="18e96-137">id</span></span>|<span data-ttu-id="18e96-138">String</span><span class="sxs-lookup"><span data-stu-id="18e96-138">String</span></span>|<span data-ttu-id="18e96-139">必須。</span><span class="sxs-lookup"><span data-stu-id="18e96-139">Required.</span></span> <span data-ttu-id="18e96-140">コピー先のノートブックの id を指定します。</span><span class="sxs-lookup"><span data-stu-id="18e96-140">The id of the destination notebook.</span></span> |
|<span data-ttu-id="18e96-141">renameAs</span><span class="sxs-lookup"><span data-stu-id="18e96-141">renameAs</span></span>|<span data-ttu-id="18e96-142">String</span><span class="sxs-lookup"><span data-stu-id="18e96-142">String</span></span>|<span data-ttu-id="18e96-143">コピーするフィルターの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="18e96-143">The name of the copy.</span></span> <span data-ttu-id="18e96-144">Defaults to the name of the existing item.</span><span class="sxs-lookup"><span data-stu-id="18e96-144">Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="18e96-145">応答</span><span class="sxs-lookup"><span data-stu-id="18e96-145">Response</span></span>

<span data-ttu-id="18e96-146">成功した場合、このメソッド`202 Accepted`は応答コードと`Operation-Location`ヘッダーを返します。</span><span class="sxs-lookup"><span data-stu-id="18e96-146">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="18e96-147">操作の場所のエンドポイントをポーリングして、[コピー操作の状態を取得](onenoteoperation-get.md)します。</span><span class="sxs-lookup"><span data-stu-id="18e96-147">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="18e96-148">例</span><span class="sxs-lookup"><span data-stu-id="18e96-148">Example</span></span>
<span data-ttu-id="18e96-149">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="18e96-149">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="18e96-150">要求</span><span class="sxs-lookup"><span data-stu-id="18e96-150">Request</span></span>
<span data-ttu-id="18e96-151">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="18e96-151">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "section_copytonotebook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/sections/{id}/copyToNotebook
Content-type: application/json
Content-length: 84

{
  "id": "id-value",
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```

##### <a name="response"></a><span data-ttu-id="18e96-152">応答</span><span class="sxs-lookup"><span data-stu-id="18e96-152">Response</span></span>
<span data-ttu-id="18e96-153">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="18e96-153">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteOperation"
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="18e96-154">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="18e96-154">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="18e96-155">Visual</span><span class="sxs-lookup"><span data-stu-id="18e96-155">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/section_copytonotebook-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="18e96-156">Java</span><span class="sxs-lookup"><span data-stu-id="18e96-156">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/section_copytonotebook-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "section: copyToNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/section-copytonotebook.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/section-copytonotebook.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
