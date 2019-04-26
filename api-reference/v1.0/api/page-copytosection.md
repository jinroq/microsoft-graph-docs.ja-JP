---
title: 'page: copytosection'
description: ページを特定のセクションにコピーします。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: b09c47ab7dbaec7b7dd63d134cdefae1260d9e8d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32556663"
---
# <a name="page-copytosection"></a><span data-ttu-id="fbb8a-103">page: copytosection</span><span class="sxs-lookup"><span data-stu-id="fbb8a-103">page: copyToSection</span></span>
<span data-ttu-id="fbb8a-104">ページを特定のセクションにコピーします。</span><span class="sxs-lookup"><span data-stu-id="fbb8a-104">Copies a page to a specific section.</span></span>

<span data-ttu-id="fbb8a-105">コピー操作では、非同期呼び出しパターンに従います。最初に copy アクションを呼び出してから、結果の操作エンドポイントをポーリングします。</span><span class="sxs-lookup"><span data-stu-id="fbb8a-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="fbb8a-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fbb8a-106">Permissions</span></span>
<span data-ttu-id="fbb8a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fbb8a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbb8a-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fbb8a-109">Permission type</span></span>      | <span data-ttu-id="fbb8a-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fbb8a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fbb8a-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fbb8a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fbb8a-112">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbb8a-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="fbb8a-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fbb8a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fbb8a-114">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fbb8a-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="fbb8a-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fbb8a-115">Application</span></span> | <span data-ttu-id="fbb8a-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbb8a-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fbb8a-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fbb8a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/pages/{id}/copyToSection
POST /users/{id | userPrincipalName}/onenote/pages/{id}/copyToSection
POST /groups/{id}/onenote/pages/{id}/copyToSection
```
## <a name="request-headers"></a><span data-ttu-id="fbb8a-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fbb8a-118">Request headers</span></span>
| <span data-ttu-id="fbb8a-119">名前</span><span class="sxs-lookup"><span data-stu-id="fbb8a-119">Name</span></span>       | <span data-ttu-id="fbb8a-120">型</span><span class="sxs-lookup"><span data-stu-id="fbb8a-120">Type</span></span> | <span data-ttu-id="fbb8a-121">説明</span><span class="sxs-lookup"><span data-stu-id="fbb8a-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fbb8a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fbb8a-122">Authorization</span></span>  | <span data-ttu-id="fbb8a-123">string</span><span class="sxs-lookup"><span data-stu-id="fbb8a-123">string</span></span>  | <span data-ttu-id="fbb8a-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="fbb8a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fbb8a-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fbb8a-126">Content-Type</span></span> | <span data-ttu-id="fbb8a-127">string</span><span class="sxs-lookup"><span data-stu-id="fbb8a-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="fbb8a-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="fbb8a-128">Request body</span></span>
<span data-ttu-id="fbb8a-129">要求本文で、操作に必要なパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="fbb8a-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="fbb8a-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="fbb8a-130">Parameter</span></span>    | <span data-ttu-id="fbb8a-131">型</span><span class="sxs-lookup"><span data-stu-id="fbb8a-131">Type</span></span>   |<span data-ttu-id="fbb8a-132">説明</span><span class="sxs-lookup"><span data-stu-id="fbb8a-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fbb8a-133">groupId</span><span class="sxs-lookup"><span data-stu-id="fbb8a-133">groupId</span></span>|<span data-ttu-id="fbb8a-134">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="fbb8a-134">String</span></span>|<span data-ttu-id="fbb8a-135">コピー先のグループの id。</span><span class="sxs-lookup"><span data-stu-id="fbb8a-135">The id of the group to copy to.</span></span> <span data-ttu-id="fbb8a-136">Office 365 グループにコピーする場合にのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="fbb8a-136">Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="fbb8a-137">id</span><span class="sxs-lookup"><span data-stu-id="fbb8a-137">id</span></span>|<span data-ttu-id="fbb8a-138">String</span><span class="sxs-lookup"><span data-stu-id="fbb8a-138">String</span></span>|<span data-ttu-id="fbb8a-139">必須。</span><span class="sxs-lookup"><span data-stu-id="fbb8a-139">Required.</span></span> <span data-ttu-id="fbb8a-140">コピー先のセクションの id。</span><span class="sxs-lookup"><span data-stu-id="fbb8a-140">The id of the destination section.</span></span>|

## <a name="response"></a><span data-ttu-id="fbb8a-141">応答</span><span class="sxs-lookup"><span data-stu-id="fbb8a-141">Response</span></span>

<span data-ttu-id="fbb8a-142">成功した場合、このメソッド`202 Accepted`は応答コードと`Operation-Location`ヘッダーを返します。</span><span class="sxs-lookup"><span data-stu-id="fbb8a-142">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="fbb8a-143">操作の場所のエンドポイントをポーリングして、[コピー操作の状態を取得](onenoteoperation-get.md)します。</span><span class="sxs-lookup"><span data-stu-id="fbb8a-143">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="fbb8a-144">例</span><span class="sxs-lookup"><span data-stu-id="fbb8a-144">Example</span></span>
<span data-ttu-id="fbb8a-145">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="fbb8a-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fbb8a-146">要求</span><span class="sxs-lookup"><span data-stu-id="fbb8a-146">Request</span></span>
<span data-ttu-id="fbb8a-147">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fbb8a-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "page_copytosection"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/pages/{id}/copyToSection
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "groupId": "groupId-value"
}
```

##### <a name="response"></a><span data-ttu-id="fbb8a-148">応答</span><span class="sxs-lookup"><span data-stu-id="fbb8a-148">Response</span></span>
<span data-ttu-id="fbb8a-149">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="fbb8a-149">Here is an example of the response.</span></span>
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
  "description": "page: copyToSection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
