---
title: 'section: copyToNotebook'
description: 特定のノートブックにセクションをコピーします。
ms.openlocfilehash: 365e4745f01c3d011cbf8cf0186a16b5eb580c5b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022734"
---
# <a name="section-copytonotebook"></a><span data-ttu-id="45622-103">section: copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="45622-103">section: copyToNotebook</span></span>
<span data-ttu-id="45622-104">特定のノートブックにセクションをコピーします。</span><span class="sxs-lookup"><span data-stu-id="45622-104">Copies a section to a specific notebook.</span></span>

<span data-ttu-id="45622-105">Copy 操作では、非同期の呼び出しパターンに従います。まず Copy 操作を呼び出し、次に結果の操作エンドポイントをポーリングします。</span><span class="sxs-lookup"><span data-stu-id="45622-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>
## <a name="permissions"></a><span data-ttu-id="45622-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="45622-106">Permissions</span></span>
<span data-ttu-id="45622-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="45622-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45622-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="45622-109">Permission type</span></span>      | <span data-ttu-id="45622-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="45622-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="45622-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="45622-111">Delegated (work or school account)</span></span> | <span data-ttu-id="45622-112">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45622-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="45622-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="45622-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45622-114">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="45622-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="45622-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="45622-115">Application</span></span> | <span data-ttu-id="45622-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45622-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="45622-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="45622-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToNotebook
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToNotebook
POST /groups/{id}/onenote/sections/{id}/copyToNotebook
```
## <a name="request-headers"></a><span data-ttu-id="45622-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="45622-118">Request headers</span></span>
| <span data-ttu-id="45622-119">名前</span><span class="sxs-lookup"><span data-stu-id="45622-119">Name</span></span>       | <span data-ttu-id="45622-120">型</span><span class="sxs-lookup"><span data-stu-id="45622-120">Type</span></span> | <span data-ttu-id="45622-121">説明</span><span class="sxs-lookup"><span data-stu-id="45622-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="45622-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="45622-122">Authorization</span></span>  | <span data-ttu-id="45622-123">string</span><span class="sxs-lookup"><span data-stu-id="45622-123">string</span></span>  | <span data-ttu-id="45622-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="45622-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="45622-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="45622-126">Content-Type</span></span> | <span data-ttu-id="45622-127">string</span><span class="sxs-lookup"><span data-stu-id="45622-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="45622-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="45622-128">Request body</span></span>
<span data-ttu-id="45622-129">要求本文では、操作に必要なパラメーターを格納する JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="45622-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="45622-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="45622-130">Parameter</span></span>    | <span data-ttu-id="45622-131">型</span><span class="sxs-lookup"><span data-stu-id="45622-131">Type</span></span>   |<span data-ttu-id="45622-132">説明</span><span class="sxs-lookup"><span data-stu-id="45622-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="45622-133">groupId</span><span class="sxs-lookup"><span data-stu-id="45622-133">groupId</span></span>|<span data-ttu-id="45622-134">String</span><span class="sxs-lookup"><span data-stu-id="45622-134">String</span></span>|<span data-ttu-id="45622-p103">コピー先グループの ID。Office 365 グループにコピーする場合にのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="45622-p103">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="45622-137">id</span><span class="sxs-lookup"><span data-stu-id="45622-137">id</span></span>|<span data-ttu-id="45622-138">String</span><span class="sxs-lookup"><span data-stu-id="45622-138">String</span></span>|<span data-ttu-id="45622-p104">必須。コピー先ノートブックの ID。</span><span class="sxs-lookup"><span data-stu-id="45622-p104">Required. The id of the destination notebook.</span></span> |
|<span data-ttu-id="45622-141">renameAs</span><span class="sxs-lookup"><span data-stu-id="45622-141">renameAs</span></span>|<span data-ttu-id="45622-142">String</span><span class="sxs-lookup"><span data-stu-id="45622-142">String</span></span>|<span data-ttu-id="45622-p105">コピーの名前。既定値は、既存のアイテムの名前になります。</span><span class="sxs-lookup"><span data-stu-id="45622-p105">The name of the copy. Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="45622-145">応答</span><span class="sxs-lookup"><span data-stu-id="45622-145">Response</span></span>

<span data-ttu-id="45622-p106">成功した場合、このメソッドは `202 Accepted` 応答コードと `Operation-Location` ヘッダーを返します。Operation-Location エンドポイントをポーリングして、[コピー操作の状態を取得します](onenoteoperation-get.md)。</span><span class="sxs-lookup"><span data-stu-id="45622-p106">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="45622-148">例</span><span class="sxs-lookup"><span data-stu-id="45622-148">Example</span></span>
<span data-ttu-id="45622-149">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="45622-149">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="45622-150">要求</span><span class="sxs-lookup"><span data-stu-id="45622-150">Request</span></span>
<span data-ttu-id="45622-151">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="45622-151">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="45622-152">応答</span><span class="sxs-lookup"><span data-stu-id="45622-152">Response</span></span>
<span data-ttu-id="45622-153">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="45622-153">Here is an example of the response.</span></span>
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
  "description": "section: copyToNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->