---
title: 'ノートブック: コピーノートブック'
description: ノートブックを移動先ドキュメントライブラリのノートブックフォルダーにコピーします。 フォルダーが存在しない場合は作成されます。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 473d2904c2b5ea5b44aaa85cc5a535cda6318535
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36374520"
---
# <a name="notebook-copynotebook"></a><span data-ttu-id="b5604-104">ノートブック: コピーノートブック</span><span class="sxs-lookup"><span data-stu-id="b5604-104">notebook: copyNotebook</span></span>
<span data-ttu-id="b5604-105">ノートブックを移動先ドキュメントライブラリのノートブックフォルダーにコピーします。</span><span class="sxs-lookup"><span data-stu-id="b5604-105">Copies a notebook to the Notebooks folder in the destination Documents library.</span></span> <span data-ttu-id="b5604-106">フォルダーが存在しない場合は作成されます。</span><span class="sxs-lookup"><span data-stu-id="b5604-106">The folder is created if it doesn't exist.</span></span>

<span data-ttu-id="b5604-107">コピー操作では、非同期呼び出しパターンに従います。最初に Copy アクションを呼び出してから、結果の操作エンドポイントをポーリングします。</span><span class="sxs-lookup"><span data-stu-id="b5604-107">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="b5604-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b5604-108">Permissions</span></span>
<span data-ttu-id="b5604-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b5604-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5604-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b5604-111">Permission type</span></span>      | <span data-ttu-id="b5604-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b5604-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b5604-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b5604-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b5604-114">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5604-114">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="b5604-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b5604-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5604-116">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b5604-116">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="b5604-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b5604-117">Application</span></span> | <span data-ttu-id="b5604-118">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5604-118">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b5604-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b5604-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/copyNotebook
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/copyNotebook
POST /groups/{id}/onenote/notebooks/{id}/copyNotebook
```
## <a name="request-headers"></a><span data-ttu-id="b5604-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b5604-120">Request headers</span></span>
| <span data-ttu-id="b5604-121">名前</span><span class="sxs-lookup"><span data-stu-id="b5604-121">Name</span></span>       | <span data-ttu-id="b5604-122">型</span><span class="sxs-lookup"><span data-stu-id="b5604-122">Type</span></span> | <span data-ttu-id="b5604-123">説明</span><span class="sxs-lookup"><span data-stu-id="b5604-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b5604-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5604-124">Authorization</span></span>  | <span data-ttu-id="b5604-125">string</span><span class="sxs-lookup"><span data-stu-id="b5604-125">string</span></span>  | <span data-ttu-id="b5604-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b5604-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b5604-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b5604-128">Content-Type</span></span> | <span data-ttu-id="b5604-129">string</span><span class="sxs-lookup"><span data-stu-id="b5604-129">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="b5604-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="b5604-130">Request body</span></span>
<span data-ttu-id="b5604-131">要求本文で、操作に必要なパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="b5604-131">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span> <span data-ttu-id="b5604-132">必要なものがない場合は、空の本文を送信してもかまいません。</span><span class="sxs-lookup"><span data-stu-id="b5604-132">It's okay to send an empty body if none are needed.</span></span>

| <span data-ttu-id="b5604-133">パラメーター</span><span class="sxs-lookup"><span data-stu-id="b5604-133">Parameter</span></span>    | <span data-ttu-id="b5604-134">型</span><span class="sxs-lookup"><span data-stu-id="b5604-134">Type</span></span>   |<span data-ttu-id="b5604-135">説明</span><span class="sxs-lookup"><span data-stu-id="b5604-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b5604-136">groupId</span><span class="sxs-lookup"><span data-stu-id="b5604-136">groupId</span></span>|<span data-ttu-id="b5604-137">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="b5604-137">String</span></span>|<span data-ttu-id="b5604-138">コピー先のグループの id。</span><span class="sxs-lookup"><span data-stu-id="b5604-138">The id of the group to copy to.</span></span> <span data-ttu-id="b5604-139">Office 365 グループにコピーする場合にのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="b5604-139">Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="b5604-140">renameAs</span><span class="sxs-lookup"><span data-stu-id="b5604-140">renameAs</span></span>|<span data-ttu-id="b5604-141">String</span><span class="sxs-lookup"><span data-stu-id="b5604-141">String</span></span>|<span data-ttu-id="b5604-142">コピーするフィルターの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="b5604-142">The name of the copy.</span></span> <span data-ttu-id="b5604-143">Defaults to the name of the existing item.</span><span class="sxs-lookup"><span data-stu-id="b5604-143">Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="b5604-144">応答</span><span class="sxs-lookup"><span data-stu-id="b5604-144">Response</span></span>

<span data-ttu-id="b5604-145">成功した場合、このメソッド`202 Accepted`は応答コードと`Operation-Location`ヘッダーを返します。</span><span class="sxs-lookup"><span data-stu-id="b5604-145">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="b5604-146">操作の場所のエンドポイントをポーリングして、[コピー操作の状態を取得](onenoteoperation-get.md)します。</span><span class="sxs-lookup"><span data-stu-id="b5604-146">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="b5604-147">例</span><span class="sxs-lookup"><span data-stu-id="b5604-147">Example</span></span>
<span data-ttu-id="b5604-148">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="b5604-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b5604-149">要求</span><span class="sxs-lookup"><span data-stu-id="b5604-149">Request</span></span>
<span data-ttu-id="b5604-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b5604-150">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b5604-151">プロトコル</span><span class="sxs-lookup"><span data-stu-id="b5604-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "notebook_copynotebook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/copyNotebook
Content-type: application/json
Content-length: 108

{
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b5604-152">C#</span><span class="sxs-lookup"><span data-stu-id="b5604-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/notebook-copynotebook-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b5604-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b5604-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/notebook-copynotebook-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b5604-154">目的-C</span><span class="sxs-lookup"><span data-stu-id="b5604-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/notebook-copynotebook-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b5604-155">Java</span><span class="sxs-lookup"><span data-stu-id="b5604-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/notebook-copynotebook-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b5604-156">応答</span><span class="sxs-lookup"><span data-stu-id="b5604-156">Response</span></span>
<span data-ttu-id="b5604-157">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="b5604-157">Here is an example of the response.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "notebook: copyNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
