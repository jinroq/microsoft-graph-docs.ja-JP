---
title: 'page: copyToSection'
description: 特定のセクションにページをコピーします。
ms.openlocfilehash: d725c72eb78613845e808a3ec3694513730bb01f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072030"
---
# <a name="page-copytosection"></a><span data-ttu-id="d2c1e-103">page: copyToSection</span><span class="sxs-lookup"><span data-stu-id="d2c1e-103">page: copyToSection</span></span>

> <span data-ttu-id="d2c1e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d2c1e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d2c1e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d2c1e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d2c1e-106">特定のセクションにページをコピーします。</span><span class="sxs-lookup"><span data-stu-id="d2c1e-106">Copies a page to a specific section.</span></span>

<span data-ttu-id="d2c1e-107">Copy 操作では、非同期の呼び出しパターンに従います。まず Copy 操作を呼び出し、次に結果の操作エンドポイントをポーリングします。</span><span class="sxs-lookup"><span data-stu-id="d2c1e-107">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2c1e-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d2c1e-108">Permissions</span></span>
<span data-ttu-id="d2c1e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d2c1e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2c1e-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d2c1e-111">Permission type</span></span>      | <span data-ttu-id="d2c1e-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d2c1e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2c1e-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d2c1e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d2c1e-114">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2c1e-114">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="d2c1e-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d2c1e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2c1e-116">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d2c1e-116">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="d2c1e-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d2c1e-117">Application</span></span> | <span data-ttu-id="d2c1e-118">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2c1e-118">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d2c1e-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d2c1e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/pages/{id}/copyToSection
POST /users/{id | userPrincipalName}/onenote/pages/{id}/copyToSection
POST /groups/{id}/onenote/pages/{id}/copyToSection
POST /sites/{id}/onenote/pages/{id}/copyToSection
```
## <a name="request-headers"></a><span data-ttu-id="d2c1e-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d2c1e-120">Request headers</span></span>
| <span data-ttu-id="d2c1e-121">名前</span><span class="sxs-lookup"><span data-stu-id="d2c1e-121">Name</span></span>       | <span data-ttu-id="d2c1e-122">型</span><span class="sxs-lookup"><span data-stu-id="d2c1e-122">Type</span></span> | <span data-ttu-id="d2c1e-123">説明</span><span class="sxs-lookup"><span data-stu-id="d2c1e-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d2c1e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2c1e-124">Authorization</span></span>  | <span data-ttu-id="d2c1e-125">string</span><span class="sxs-lookup"><span data-stu-id="d2c1e-125">string</span></span>  | <span data-ttu-id="d2c1e-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d2c1e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d2c1e-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d2c1e-128">Content-Type</span></span> | <span data-ttu-id="d2c1e-129">string</span><span class="sxs-lookup"><span data-stu-id="d2c1e-129">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="d2c1e-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="d2c1e-130">Request body</span></span>
<span data-ttu-id="d2c1e-131">要求本文では、操作に必要なパラメーターを格納する JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="d2c1e-131">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="d2c1e-132">パラメーター</span><span class="sxs-lookup"><span data-stu-id="d2c1e-132">Parameter</span></span>    | <span data-ttu-id="d2c1e-133">型</span><span class="sxs-lookup"><span data-stu-id="d2c1e-133">Type</span></span>   |<span data-ttu-id="d2c1e-134">説明</span><span class="sxs-lookup"><span data-stu-id="d2c1e-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d2c1e-135">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="d2c1e-135">siteCollectionId</span></span>|<span data-ttu-id="d2c1e-136">String</span><span class="sxs-lookup"><span data-stu-id="d2c1e-136">String</span></span>|<span data-ttu-id="d2c1e-137">コピーする SharePoint サイトの id です。</span><span class="sxs-lookup"><span data-stu-id="d2c1e-137">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="d2c1e-138">Office 365 チーム サイトにコピーするときにのみを使用します。</span><span class="sxs-lookup"><span data-stu-id="d2c1e-138">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="d2c1e-139">siteId</span><span class="sxs-lookup"><span data-stu-id="d2c1e-139">siteId</span></span>|<span data-ttu-id="d2c1e-140">String</span><span class="sxs-lookup"><span data-stu-id="d2c1e-140">String</span></span>|<span data-ttu-id="d2c1e-141">コピーする SharePoint web の id です。</span><span class="sxs-lookup"><span data-stu-id="d2c1e-141">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="d2c1e-142">Office 365 チーム サイトにコピーするときにのみを使用します。</span><span class="sxs-lookup"><span data-stu-id="d2c1e-142">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="d2c1e-143">グループ Id</span><span class="sxs-lookup"><span data-stu-id="d2c1e-143">groupId</span></span>|<span data-ttu-id="d2c1e-144">String</span><span class="sxs-lookup"><span data-stu-id="d2c1e-144">String</span></span>|<span data-ttu-id="d2c1e-p106">コピー先グループの ID。Office 365 グループにコピーする場合にのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="d2c1e-p106">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="d2c1e-147">id</span><span class="sxs-lookup"><span data-stu-id="d2c1e-147">id</span></span>|<span data-ttu-id="d2c1e-148">String</span><span class="sxs-lookup"><span data-stu-id="d2c1e-148">String</span></span>|<span data-ttu-id="d2c1e-p107">必須。コピー先セクションの ID です。</span><span class="sxs-lookup"><span data-stu-id="d2c1e-p107">Required. The id of the destination section.</span></span>|

## <a name="response"></a><span data-ttu-id="d2c1e-151">応答</span><span class="sxs-lookup"><span data-stu-id="d2c1e-151">Response</span></span>

<span data-ttu-id="d2c1e-p108">成功した場合、このメソッドは `202 Accepted` 応答コードと `Operation-Location` ヘッダーを返します。Operation-Location エンドポイントをポーリングして、[コピー操作の状態を取得します](onenoteoperation-get.md)。</span><span class="sxs-lookup"><span data-stu-id="d2c1e-p108">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="d2c1e-154">例</span><span class="sxs-lookup"><span data-stu-id="d2c1e-154">Example</span></span>
<span data-ttu-id="d2c1e-155">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="d2c1e-155">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d2c1e-156">要求</span><span class="sxs-lookup"><span data-stu-id="d2c1e-156">Request</span></span>
<span data-ttu-id="d2c1e-157">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d2c1e-157">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="d2c1e-158">応答</span><span class="sxs-lookup"><span data-stu-id="d2c1e-158">Response</span></span>
<span data-ttu-id="d2c1e-159">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="d2c1e-159">Here is an example of the response.</span></span>
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