---
title: 'ノートブック: コピーノートブック'
description: ノートブックを移動先ドキュメントライブラリのノートブックフォルダーにコピーします。 フォルダーが存在しない場合は作成されます。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 01e5f0ec7edd898c53447eafe930cc72cc9561ad
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35274586"
---
# <a name="notebook-copynotebook"></a><span data-ttu-id="9053c-104">ノートブック: コピーノートブック</span><span class="sxs-lookup"><span data-stu-id="9053c-104">notebook: copyNotebook</span></span>
<span data-ttu-id="9053c-105">ノートブックを移動先ドキュメントライブラリのノートブックフォルダーにコピーします。</span><span class="sxs-lookup"><span data-stu-id="9053c-105">Copies a notebook to the Notebooks folder in the destination Documents library.</span></span> <span data-ttu-id="9053c-106">フォルダーが存在しない場合は作成されます。</span><span class="sxs-lookup"><span data-stu-id="9053c-106">The folder is created if it doesn't exist.</span></span>

<span data-ttu-id="9053c-107">コピー操作では、非同期呼び出しパターンに従います。最初に Copy アクションを呼び出してから、結果の操作エンドポイントをポーリングします。</span><span class="sxs-lookup"><span data-stu-id="9053c-107">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="9053c-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9053c-108">Permissions</span></span>
<span data-ttu-id="9053c-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9053c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9053c-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9053c-111">Permission type</span></span>      | <span data-ttu-id="9053c-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9053c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9053c-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9053c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="9053c-114">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9053c-114">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="9053c-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9053c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9053c-116">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9053c-116">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="9053c-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9053c-117">Application</span></span> | <span data-ttu-id="9053c-118">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9053c-118">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9053c-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9053c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/copyNotebook
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/copyNotebook
POST /groups/{id}/onenote/notebooks/{id}/copyNotebook
```
## <a name="request-headers"></a><span data-ttu-id="9053c-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9053c-120">Request headers</span></span>
| <span data-ttu-id="9053c-121">名前</span><span class="sxs-lookup"><span data-stu-id="9053c-121">Name</span></span>       | <span data-ttu-id="9053c-122">型</span><span class="sxs-lookup"><span data-stu-id="9053c-122">Type</span></span> | <span data-ttu-id="9053c-123">説明</span><span class="sxs-lookup"><span data-stu-id="9053c-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9053c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9053c-124">Authorization</span></span>  | <span data-ttu-id="9053c-125">string</span><span class="sxs-lookup"><span data-stu-id="9053c-125">string</span></span>  | <span data-ttu-id="9053c-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9053c-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9053c-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9053c-128">Content-Type</span></span> | <span data-ttu-id="9053c-129">string</span><span class="sxs-lookup"><span data-stu-id="9053c-129">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="9053c-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="9053c-130">Request body</span></span>
<span data-ttu-id="9053c-131">要求本文で、操作に必要なパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="9053c-131">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span> <span data-ttu-id="9053c-132">必要なものがない場合は、空の本文を送信してもかまいません。</span><span class="sxs-lookup"><span data-stu-id="9053c-132">It's okay to send an empty body if none are needed.</span></span>

| <span data-ttu-id="9053c-133">パラメーター</span><span class="sxs-lookup"><span data-stu-id="9053c-133">Parameter</span></span>    | <span data-ttu-id="9053c-134">型</span><span class="sxs-lookup"><span data-stu-id="9053c-134">Type</span></span>   |<span data-ttu-id="9053c-135">説明</span><span class="sxs-lookup"><span data-stu-id="9053c-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9053c-136">groupId</span><span class="sxs-lookup"><span data-stu-id="9053c-136">groupId</span></span>|<span data-ttu-id="9053c-137">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="9053c-137">String</span></span>|<span data-ttu-id="9053c-138">コピー先のグループの id。</span><span class="sxs-lookup"><span data-stu-id="9053c-138">The id of the group to copy to.</span></span> <span data-ttu-id="9053c-139">Office 365 グループにコピーする場合にのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="9053c-139">Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="9053c-140">renameAs</span><span class="sxs-lookup"><span data-stu-id="9053c-140">renameAs</span></span>|<span data-ttu-id="9053c-141">String</span><span class="sxs-lookup"><span data-stu-id="9053c-141">String</span></span>|<span data-ttu-id="9053c-142">コピーするフィルターの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="9053c-142">The name of the copy.</span></span> <span data-ttu-id="9053c-143">Defaults to the name of the existing item.</span><span class="sxs-lookup"><span data-stu-id="9053c-143">Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="9053c-144">応答</span><span class="sxs-lookup"><span data-stu-id="9053c-144">Response</span></span>

<span data-ttu-id="9053c-145">成功した場合、このメソッド`202 Accepted`は応答コードと`Operation-Location`ヘッダーを返します。</span><span class="sxs-lookup"><span data-stu-id="9053c-145">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="9053c-146">操作の場所のエンドポイントをポーリングして、[コピー操作の状態を取得](onenoteoperation-get.md)します。</span><span class="sxs-lookup"><span data-stu-id="9053c-146">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="9053c-147">例</span><span class="sxs-lookup"><span data-stu-id="9053c-147">Example</span></span>
<span data-ttu-id="9053c-148">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="9053c-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9053c-149">要求</span><span class="sxs-lookup"><span data-stu-id="9053c-149">Request</span></span>
<span data-ttu-id="9053c-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9053c-150">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="9053c-151">応答</span><span class="sxs-lookup"><span data-stu-id="9053c-151">Response</span></span>
<span data-ttu-id="9053c-152">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="9053c-152">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteOperation"
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="9053c-153">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="9053c-153">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="9053c-154">C#</span><span class="sxs-lookup"><span data-stu-id="9053c-154">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/notebook_copynotebook-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9053c-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="9053c-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/notebook_copynotebook-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="9053c-156">目的-C</span><span class="sxs-lookup"><span data-stu-id="9053c-156">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/notebook_copynotebook-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebook: copyNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/notebook-copynotebook.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/notebook-copynotebook.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/notebook-copynotebook.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
