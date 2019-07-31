---
title: 'ノートブック: コピーノートブック'
description: ノートブックを移動先ドキュメントライブラリのノートブックフォルダーにコピーします。 フォルダーが存在しない場合は作成されます。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 38c8bc918b49ee6e4da5ed7ff921d1f661a0c4a3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35983764"
---
# <a name="notebook-copynotebook"></a><span data-ttu-id="37cad-104">ノートブック: コピーノートブック</span><span class="sxs-lookup"><span data-stu-id="37cad-104">notebook: copyNotebook</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37cad-105">ノートブックを移動先ドキュメントライブラリのノートブックフォルダーにコピーします。</span><span class="sxs-lookup"><span data-stu-id="37cad-105">Copies a notebook to the Notebooks folder in the destination Documents library.</span></span> <span data-ttu-id="37cad-106">フォルダーが存在しない場合は作成されます。</span><span class="sxs-lookup"><span data-stu-id="37cad-106">The folder is created if it doesn't exist.</span></span>

<span data-ttu-id="37cad-107">コピー操作では、非同期呼び出しパターンに従います。最初に Copy アクションを呼び出してから、結果の操作エンドポイントをポーリングします。</span><span class="sxs-lookup"><span data-stu-id="37cad-107">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="37cad-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="37cad-108">Permissions</span></span>
<span data-ttu-id="37cad-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="37cad-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37cad-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="37cad-111">Permission type</span></span>      | <span data-ttu-id="37cad-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="37cad-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="37cad-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="37cad-113">Delegated (work or school account)</span></span> | <span data-ttu-id="37cad-114">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37cad-114">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="37cad-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="37cad-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37cad-116">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="37cad-116">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="37cad-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="37cad-117">Application</span></span> | <span data-ttu-id="37cad-118">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37cad-118">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="37cad-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="37cad-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/copyNotebook
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/copyNotebook
POST /groups/{id}/onenote/notebooks/{id}/copyNotebook
POST /sites/{id}/onenote/notebooks/{id}/copyNotebook
```
## <a name="request-headers"></a><span data-ttu-id="37cad-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="37cad-120">Request headers</span></span>
| <span data-ttu-id="37cad-121">名前</span><span class="sxs-lookup"><span data-stu-id="37cad-121">Name</span></span>       | <span data-ttu-id="37cad-122">型</span><span class="sxs-lookup"><span data-stu-id="37cad-122">Type</span></span> | <span data-ttu-id="37cad-123">説明</span><span class="sxs-lookup"><span data-stu-id="37cad-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="37cad-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="37cad-124">Authorization</span></span>  | <span data-ttu-id="37cad-125">string</span><span class="sxs-lookup"><span data-stu-id="37cad-125">string</span></span>  | <span data-ttu-id="37cad-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="37cad-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="37cad-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="37cad-128">Content-Type</span></span> | <span data-ttu-id="37cad-129">string</span><span class="sxs-lookup"><span data-stu-id="37cad-129">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="37cad-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="37cad-130">Request body</span></span>
<span data-ttu-id="37cad-131">要求本文で、操作に必要なパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="37cad-131">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span> <span data-ttu-id="37cad-132">必要なものがない場合は、空の本文を送信してもかまいません。</span><span class="sxs-lookup"><span data-stu-id="37cad-132">It's okay to send an empty body if none are needed.</span></span>

| <span data-ttu-id="37cad-133">パラメーター</span><span class="sxs-lookup"><span data-stu-id="37cad-133">Parameter</span></span>    | <span data-ttu-id="37cad-134">型</span><span class="sxs-lookup"><span data-stu-id="37cad-134">Type</span></span>   |<span data-ttu-id="37cad-135">説明</span><span class="sxs-lookup"><span data-stu-id="37cad-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="37cad-136">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="37cad-136">siteCollectionId</span></span>|<span data-ttu-id="37cad-137">String</span><span class="sxs-lookup"><span data-stu-id="37cad-137">String</span></span>|<span data-ttu-id="37cad-138">コピー先の SharePoint サイトの id。</span><span class="sxs-lookup"><span data-stu-id="37cad-138">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="37cad-139">Office 365 チームサイトにコピーする場合にのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="37cad-139">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="37cad-140">siteId</span><span class="sxs-lookup"><span data-stu-id="37cad-140">siteId</span></span>|<span data-ttu-id="37cad-141">String</span><span class="sxs-lookup"><span data-stu-id="37cad-141">String</span></span>|<span data-ttu-id="37cad-142">コピー先の SharePoint web の id です。</span><span class="sxs-lookup"><span data-stu-id="37cad-142">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="37cad-143">Office 365 チームサイトにコピーする場合にのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="37cad-143">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="37cad-144">groupId</span><span class="sxs-lookup"><span data-stu-id="37cad-144">groupId</span></span>|<span data-ttu-id="37cad-145">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="37cad-145">String</span></span>|<span data-ttu-id="37cad-146">コピー先のグループの id。</span><span class="sxs-lookup"><span data-stu-id="37cad-146">The id of the group to copy to.</span></span> <span data-ttu-id="37cad-147">Office 365 グループにコピーする場合にのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="37cad-147">Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="37cad-148">renameAs</span><span class="sxs-lookup"><span data-stu-id="37cad-148">renameAs</span></span>|<span data-ttu-id="37cad-149">String</span><span class="sxs-lookup"><span data-stu-id="37cad-149">String</span></span>|<span data-ttu-id="37cad-150">コピーするフィルターの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="37cad-150">The name of the copy.</span></span> <span data-ttu-id="37cad-151">Defaults to the name of the existing item.</span><span class="sxs-lookup"><span data-stu-id="37cad-151">Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="37cad-152">応答</span><span class="sxs-lookup"><span data-stu-id="37cad-152">Response</span></span>

<span data-ttu-id="37cad-153">成功した場合、このメソッド`202 Accepted`は応答コードと`Operation-Location`ヘッダーを返します。</span><span class="sxs-lookup"><span data-stu-id="37cad-153">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="37cad-154">操作の場所のエンドポイントをポーリングして、[コピー操作の状態を取得](onenoteoperation-get.md)します。</span><span class="sxs-lookup"><span data-stu-id="37cad-154">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="37cad-155">例</span><span class="sxs-lookup"><span data-stu-id="37cad-155">Example</span></span>
<span data-ttu-id="37cad-156">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="37cad-156">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="37cad-157">要求</span><span class="sxs-lookup"><span data-stu-id="37cad-157">Request</span></span>
<span data-ttu-id="37cad-158">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="37cad-158">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="37cad-159">プロトコル</span><span class="sxs-lookup"><span data-stu-id="37cad-159">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="37cad-160">C#</span><span class="sxs-lookup"><span data-stu-id="37cad-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/notebook-copynotebook-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="37cad-161">Javascript</span><span class="sxs-lookup"><span data-stu-id="37cad-161">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/notebook-copynotebook-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="37cad-162">目的-C</span><span class="sxs-lookup"><span data-stu-id="37cad-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/notebook-copynotebook-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="37cad-163">Java</span><span class="sxs-lookup"><span data-stu-id="37cad-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/notebook-copynotebook-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="37cad-164">応答</span><span class="sxs-lookup"><span data-stu-id="37cad-164">Response</span></span>
<span data-ttu-id="37cad-165">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="37cad-165">Here is an example of the response.</span></span>
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
