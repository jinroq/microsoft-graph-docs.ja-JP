---
title: 'page: copytosection'
description: ページを特定のセクションにコピーします。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: dd7abb016345195bd5a32e20a5623d6fca9fd6ff
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32539400"
---
# <a name="page-copytosection"></a><span data-ttu-id="c580c-103">page: copytosection</span><span class="sxs-lookup"><span data-stu-id="c580c-103">page: copyToSection</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c580c-104">ページを特定のセクションにコピーします。</span><span class="sxs-lookup"><span data-stu-id="c580c-104">Copies a page to a specific section.</span></span>

<span data-ttu-id="c580c-105">コピー操作では、非同期呼び出しパターンに従います。最初に copy アクションを呼び出してから、結果の操作エンドポイントをポーリングします。</span><span class="sxs-lookup"><span data-stu-id="c580c-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="c580c-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c580c-106">Permissions</span></span>
<span data-ttu-id="c580c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c580c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c580c-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c580c-109">Permission type</span></span>      | <span data-ttu-id="c580c-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c580c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c580c-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c580c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c580c-112">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c580c-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="c580c-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c580c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c580c-114">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c580c-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="c580c-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c580c-115">Application</span></span> | <span data-ttu-id="c580c-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c580c-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c580c-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c580c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/pages/{id}/copyToSection
POST /users/{id | userPrincipalName}/onenote/pages/{id}/copyToSection
POST /groups/{id}/onenote/pages/{id}/copyToSection
POST /sites/{id}/onenote/pages/{id}/copyToSection
```
## <a name="request-headers"></a><span data-ttu-id="c580c-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c580c-118">Request headers</span></span>
| <span data-ttu-id="c580c-119">名前</span><span class="sxs-lookup"><span data-stu-id="c580c-119">Name</span></span>       | <span data-ttu-id="c580c-120">型</span><span class="sxs-lookup"><span data-stu-id="c580c-120">Type</span></span> | <span data-ttu-id="c580c-121">説明</span><span class="sxs-lookup"><span data-stu-id="c580c-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c580c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c580c-122">Authorization</span></span>  | <span data-ttu-id="c580c-123">string</span><span class="sxs-lookup"><span data-stu-id="c580c-123">string</span></span>  | <span data-ttu-id="c580c-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c580c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c580c-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c580c-126">Content-Type</span></span> | <span data-ttu-id="c580c-127">string</span><span class="sxs-lookup"><span data-stu-id="c580c-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="c580c-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="c580c-128">Request body</span></span>
<span data-ttu-id="c580c-129">要求本文で、操作に必要なパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="c580c-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="c580c-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="c580c-130">Parameter</span></span>    | <span data-ttu-id="c580c-131">型</span><span class="sxs-lookup"><span data-stu-id="c580c-131">Type</span></span>   |<span data-ttu-id="c580c-132">説明</span><span class="sxs-lookup"><span data-stu-id="c580c-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c580c-133">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="c580c-133">siteCollectionId</span></span>|<span data-ttu-id="c580c-134">String</span><span class="sxs-lookup"><span data-stu-id="c580c-134">String</span></span>|<span data-ttu-id="c580c-135">コピー先の SharePoint サイトの id。</span><span class="sxs-lookup"><span data-stu-id="c580c-135">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="c580c-136">Office 365 チームサイトにコピーする場合にのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="c580c-136">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="c580c-137">siteId</span><span class="sxs-lookup"><span data-stu-id="c580c-137">siteId</span></span>|<span data-ttu-id="c580c-138">String</span><span class="sxs-lookup"><span data-stu-id="c580c-138">String</span></span>|<span data-ttu-id="c580c-139">コピー先の SharePoint web の id です。</span><span class="sxs-lookup"><span data-stu-id="c580c-139">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="c580c-140">Office 365 チームサイトにコピーする場合にのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="c580c-140">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="c580c-141">groupId</span><span class="sxs-lookup"><span data-stu-id="c580c-141">groupId</span></span>|<span data-ttu-id="c580c-142">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="c580c-142">String</span></span>|<span data-ttu-id="c580c-143">コピー先のグループの id。</span><span class="sxs-lookup"><span data-stu-id="c580c-143">The id of the group to copy to.</span></span> <span data-ttu-id="c580c-144">Office 365 グループにコピーする場合にのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="c580c-144">Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="c580c-145">id</span><span class="sxs-lookup"><span data-stu-id="c580c-145">id</span></span>|<span data-ttu-id="c580c-146">String</span><span class="sxs-lookup"><span data-stu-id="c580c-146">String</span></span>|<span data-ttu-id="c580c-147">必須。</span><span class="sxs-lookup"><span data-stu-id="c580c-147">Required.</span></span> <span data-ttu-id="c580c-148">コピー先のセクションの id。</span><span class="sxs-lookup"><span data-stu-id="c580c-148">The id of the destination section.</span></span>|

## <a name="response"></a><span data-ttu-id="c580c-149">応答</span><span class="sxs-lookup"><span data-stu-id="c580c-149">Response</span></span>

<span data-ttu-id="c580c-150">成功した場合、このメソッド`202 Accepted`は応答コードと`Operation-Location`ヘッダーを返します。</span><span class="sxs-lookup"><span data-stu-id="c580c-150">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="c580c-151">操作の場所のエンドポイントをポーリングして、[コピー操作の状態を取得](onenoteoperation-get.md)します。</span><span class="sxs-lookup"><span data-stu-id="c580c-151">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="c580c-152">例</span><span class="sxs-lookup"><span data-stu-id="c580c-152">Example</span></span>
<span data-ttu-id="c580c-153">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="c580c-153">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c580c-154">要求</span><span class="sxs-lookup"><span data-stu-id="c580c-154">Request</span></span>
<span data-ttu-id="c580c-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c580c-155">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="c580c-156">応答</span><span class="sxs-lookup"><span data-stu-id="c580c-156">Response</span></span>
<span data-ttu-id="c580c-157">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="c580c-157">Here is an example of the response.</span></span>
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
    "Error: /api-reference/beta/api/page-copytosection.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
