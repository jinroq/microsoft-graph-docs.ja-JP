---
title: 'ノートブック: コピーノートブック'
description: ノートブックを移動先ドキュメントライブラリのノートブックフォルダーにコピーします。 フォルダーが存在しない場合は作成されます。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: c91731a522cf26edd96eec34f0c0a9c762721fcd
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36342727"
---
# <a name="notebook-copynotebook"></a><span data-ttu-id="9b6a4-104">ノートブック: コピーノートブック</span><span class="sxs-lookup"><span data-stu-id="9b6a4-104">notebook: copyNotebook</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b6a4-105">ノートブックを移動先ドキュメントライブラリのノートブックフォルダーにコピーします。</span><span class="sxs-lookup"><span data-stu-id="9b6a4-105">Copies a notebook to the Notebooks folder in the destination Documents library.</span></span> <span data-ttu-id="9b6a4-106">フォルダーが存在しない場合は作成されます。</span><span class="sxs-lookup"><span data-stu-id="9b6a4-106">The folder is created if it doesn't exist.</span></span>

<span data-ttu-id="9b6a4-107">コピー操作では、非同期呼び出しパターンに従います。最初に Copy アクションを呼び出してから、結果の操作エンドポイントをポーリングします。</span><span class="sxs-lookup"><span data-stu-id="9b6a4-107">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="9b6a4-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9b6a4-108">Permissions</span></span>
<span data-ttu-id="9b6a4-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9b6a4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b6a4-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9b6a4-111">Permission type</span></span>      | <span data-ttu-id="9b6a4-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9b6a4-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9b6a4-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9b6a4-113">Delegated (work or school account)</span></span> | <span data-ttu-id="9b6a4-114">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b6a4-114">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="9b6a4-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9b6a4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b6a4-116">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9b6a4-116">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="9b6a4-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9b6a4-117">Application</span></span> | <span data-ttu-id="9b6a4-118">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b6a4-118">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9b6a4-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9b6a4-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/copyNotebook
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/copyNotebook
POST /groups/{id}/onenote/notebooks/{id}/copyNotebook
POST /sites/{id}/onenote/notebooks/{id}/copyNotebook
```
## <a name="request-headers"></a><span data-ttu-id="9b6a4-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9b6a4-120">Request headers</span></span>
| <span data-ttu-id="9b6a4-121">名前</span><span class="sxs-lookup"><span data-stu-id="9b6a4-121">Name</span></span>       | <span data-ttu-id="9b6a4-122">型</span><span class="sxs-lookup"><span data-stu-id="9b6a4-122">Type</span></span> | <span data-ttu-id="9b6a4-123">説明</span><span class="sxs-lookup"><span data-stu-id="9b6a4-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9b6a4-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b6a4-124">Authorization</span></span>  | <span data-ttu-id="9b6a4-125">string</span><span class="sxs-lookup"><span data-stu-id="9b6a4-125">string</span></span>  | <span data-ttu-id="9b6a4-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9b6a4-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9b6a4-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9b6a4-128">Content-Type</span></span> | <span data-ttu-id="9b6a4-129">string</span><span class="sxs-lookup"><span data-stu-id="9b6a4-129">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="9b6a4-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="9b6a4-130">Request body</span></span>
<span data-ttu-id="9b6a4-131">要求本文で、操作に必要なパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="9b6a4-131">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span> <span data-ttu-id="9b6a4-132">必要なものがない場合は、空の本文を送信してもかまいません。</span><span class="sxs-lookup"><span data-stu-id="9b6a4-132">It's okay to send an empty body if none are needed.</span></span>

| <span data-ttu-id="9b6a4-133">パラメーター</span><span class="sxs-lookup"><span data-stu-id="9b6a4-133">Parameter</span></span>    | <span data-ttu-id="9b6a4-134">型</span><span class="sxs-lookup"><span data-stu-id="9b6a4-134">Type</span></span>   |<span data-ttu-id="9b6a4-135">説明</span><span class="sxs-lookup"><span data-stu-id="9b6a4-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9b6a4-136">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="9b6a4-136">siteCollectionId</span></span>|<span data-ttu-id="9b6a4-137">String</span><span class="sxs-lookup"><span data-stu-id="9b6a4-137">String</span></span>|<span data-ttu-id="9b6a4-138">コピー先の SharePoint サイトの id。</span><span class="sxs-lookup"><span data-stu-id="9b6a4-138">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="9b6a4-139">Office 365 チームサイトにコピーする場合にのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="9b6a4-139">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="9b6a4-140">siteId</span><span class="sxs-lookup"><span data-stu-id="9b6a4-140">siteId</span></span>|<span data-ttu-id="9b6a4-141">String</span><span class="sxs-lookup"><span data-stu-id="9b6a4-141">String</span></span>|<span data-ttu-id="9b6a4-142">コピー先の SharePoint web の id です。</span><span class="sxs-lookup"><span data-stu-id="9b6a4-142">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="9b6a4-143">Office 365 チームサイトにコピーする場合にのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="9b6a4-143">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="9b6a4-144">groupId</span><span class="sxs-lookup"><span data-stu-id="9b6a4-144">groupId</span></span>|<span data-ttu-id="9b6a4-145">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="9b6a4-145">String</span></span>|<span data-ttu-id="9b6a4-146">コピー先のグループの id。</span><span class="sxs-lookup"><span data-stu-id="9b6a4-146">The id of the group to copy to.</span></span> <span data-ttu-id="9b6a4-147">Office 365 グループにコピーする場合にのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="9b6a4-147">Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="9b6a4-148">renameAs</span><span class="sxs-lookup"><span data-stu-id="9b6a4-148">renameAs</span></span>|<span data-ttu-id="9b6a4-149">String</span><span class="sxs-lookup"><span data-stu-id="9b6a4-149">String</span></span>|<span data-ttu-id="9b6a4-150">コピーするフィルターの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="9b6a4-150">The name of the copy.</span></span> <span data-ttu-id="9b6a4-151">Defaults to the name of the existing item.</span><span class="sxs-lookup"><span data-stu-id="9b6a4-151">Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="9b6a4-152">応答</span><span class="sxs-lookup"><span data-stu-id="9b6a4-152">Response</span></span>

<span data-ttu-id="9b6a4-153">成功した場合、このメソッド`202 Accepted`は応答コードと`Operation-Location`ヘッダーを返します。</span><span class="sxs-lookup"><span data-stu-id="9b6a4-153">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="9b6a4-154">操作の場所のエンドポイントをポーリングして、[コピー操作の状態を取得](onenoteoperation-get.md)します。</span><span class="sxs-lookup"><span data-stu-id="9b6a4-154">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="9b6a4-155">例</span><span class="sxs-lookup"><span data-stu-id="9b6a4-155">Example</span></span>
<span data-ttu-id="9b6a4-156">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="9b6a4-156">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9b6a4-157">要求</span><span class="sxs-lookup"><span data-stu-id="9b6a4-157">Request</span></span>
<span data-ttu-id="9b6a4-158">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9b6a4-158">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9b6a4-159">プロトコル</span><span class="sxs-lookup"><span data-stu-id="9b6a4-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "notebook_copynotebook"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/notebooks/{id}/copyNotebook
Content-type: application/json
Content-length: 108

{
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9b6a4-160">C#</span><span class="sxs-lookup"><span data-stu-id="9b6a4-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/notebook-copynotebook-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9b6a4-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9b6a4-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/notebook-copynotebook-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9b6a4-162">目的-C</span><span class="sxs-lookup"><span data-stu-id="9b6a4-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/notebook-copynotebook-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9b6a4-163">Java</span><span class="sxs-lookup"><span data-stu-id="9b6a4-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/notebook-copynotebook-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9b6a4-164">応答</span><span class="sxs-lookup"><span data-stu-id="9b6a4-164">Response</span></span>
<span data-ttu-id="9b6a4-165">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="9b6a4-165">Here is an example of the response.</span></span>
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
  "description": "notebook: copyNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
