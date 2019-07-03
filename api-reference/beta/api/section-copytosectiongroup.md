---
title: 'セクション: copyToSectionGroup'
description: 指定したセクショングループにセクションをコピーします。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: c96f332611cdc9d1f3e19772f33c09ee5648dc18
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35457444"
---
# <a name="section-copytosectiongroup"></a><span data-ttu-id="2fcaa-103">セクション: copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="2fcaa-103">section: copyToSectionGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2fcaa-104">指定したセクショングループにセクションをコピーします。</span><span class="sxs-lookup"><span data-stu-id="2fcaa-104">Copies a section to a specific section group.</span></span>

<span data-ttu-id="2fcaa-105">コピー操作では、非同期呼び出しパターンに従います。最初に Copy アクションを呼び出してから、結果の操作エンドポイントをポーリングします。</span><span class="sxs-lookup"><span data-stu-id="2fcaa-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="2fcaa-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2fcaa-106">Permissions</span></span>
<span data-ttu-id="2fcaa-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2fcaa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2fcaa-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2fcaa-109">Permission type</span></span>      | <span data-ttu-id="2fcaa-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2fcaa-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2fcaa-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2fcaa-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2fcaa-112">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2fcaa-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="2fcaa-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2fcaa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2fcaa-114">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2fcaa-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="2fcaa-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2fcaa-115">Application</span></span> | <span data-ttu-id="2fcaa-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2fcaa-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2fcaa-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2fcaa-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToSectionGroup
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToSectionGroup
POST /groups/{id}/onenote/sections/{id}/copyToSectionGroup
POST /sites/{id}/onenote/sections/{id}/copyToSectionGroup
```
## <a name="request-headers"></a><span data-ttu-id="2fcaa-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2fcaa-118">Request headers</span></span>
| <span data-ttu-id="2fcaa-119">名前</span><span class="sxs-lookup"><span data-stu-id="2fcaa-119">Name</span></span>       | <span data-ttu-id="2fcaa-120">型</span><span class="sxs-lookup"><span data-stu-id="2fcaa-120">Type</span></span> | <span data-ttu-id="2fcaa-121">説明</span><span class="sxs-lookup"><span data-stu-id="2fcaa-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2fcaa-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2fcaa-122">Authorization</span></span>  | <span data-ttu-id="2fcaa-123">string</span><span class="sxs-lookup"><span data-stu-id="2fcaa-123">string</span></span>  | <span data-ttu-id="2fcaa-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2fcaa-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2fcaa-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2fcaa-126">Content-Type</span></span> | <span data-ttu-id="2fcaa-127">string</span><span class="sxs-lookup"><span data-stu-id="2fcaa-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="2fcaa-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="2fcaa-128">Request body</span></span>
<span data-ttu-id="2fcaa-129">要求本文で、操作に必要なパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="2fcaa-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="2fcaa-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="2fcaa-130">Parameter</span></span>    | <span data-ttu-id="2fcaa-131">型</span><span class="sxs-lookup"><span data-stu-id="2fcaa-131">Type</span></span>   |<span data-ttu-id="2fcaa-132">説明</span><span class="sxs-lookup"><span data-stu-id="2fcaa-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2fcaa-133">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="2fcaa-133">siteCollectionId</span></span>|<span data-ttu-id="2fcaa-134">String</span><span class="sxs-lookup"><span data-stu-id="2fcaa-134">String</span></span>|<span data-ttu-id="2fcaa-135">コピー先の SharePoint サイトの id。</span><span class="sxs-lookup"><span data-stu-id="2fcaa-135">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="2fcaa-136">Office 365 チームサイトにコピーする場合にのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="2fcaa-136">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="2fcaa-137">siteId</span><span class="sxs-lookup"><span data-stu-id="2fcaa-137">siteId</span></span>|<span data-ttu-id="2fcaa-138">String</span><span class="sxs-lookup"><span data-stu-id="2fcaa-138">String</span></span>|<span data-ttu-id="2fcaa-139">コピー先の SharePoint web の id です。</span><span class="sxs-lookup"><span data-stu-id="2fcaa-139">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="2fcaa-140">Office 365 チームサイトにコピーする場合にのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="2fcaa-140">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="2fcaa-141">groupId</span><span class="sxs-lookup"><span data-stu-id="2fcaa-141">groupId</span></span>|<span data-ttu-id="2fcaa-142">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="2fcaa-142">String</span></span>|<span data-ttu-id="2fcaa-143">コピー先のグループの id。</span><span class="sxs-lookup"><span data-stu-id="2fcaa-143">The id of the group to copy to.</span></span> <span data-ttu-id="2fcaa-144">Office 365 グループにコピーする場合にのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="2fcaa-144">Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="2fcaa-145">id</span><span class="sxs-lookup"><span data-stu-id="2fcaa-145">id</span></span>|<span data-ttu-id="2fcaa-146">String</span><span class="sxs-lookup"><span data-stu-id="2fcaa-146">String</span></span>|<span data-ttu-id="2fcaa-147">必須。</span><span class="sxs-lookup"><span data-stu-id="2fcaa-147">Required.</span></span> <span data-ttu-id="2fcaa-148">コピー先のセクショングループの id を指定します。</span><span class="sxs-lookup"><span data-stu-id="2fcaa-148">The id of the destination section group.</span></span> |
|<span data-ttu-id="2fcaa-149">renameAs</span><span class="sxs-lookup"><span data-stu-id="2fcaa-149">renameAs</span></span>|<span data-ttu-id="2fcaa-150">String</span><span class="sxs-lookup"><span data-stu-id="2fcaa-150">String</span></span>|<span data-ttu-id="2fcaa-151">コピーするフィルターの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="2fcaa-151">The name of the copy.</span></span> <span data-ttu-id="2fcaa-152">Defaults to the name of the existing item.</span><span class="sxs-lookup"><span data-stu-id="2fcaa-152">Defaults to the name of the existing item.</span></span> |

<!--groupId missing-->
<!--|siteCollectionId|String||
|siteId|String||-->

## <a name="response"></a><span data-ttu-id="2fcaa-153">応答</span><span class="sxs-lookup"><span data-stu-id="2fcaa-153">Response</span></span>

<span data-ttu-id="2fcaa-154">成功した場合、このメソッド`202 Accepted`は応答コードと`Operation-Location`ヘッダーを返します。</span><span class="sxs-lookup"><span data-stu-id="2fcaa-154">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="2fcaa-155">操作の場所のエンドポイントをポーリングして、[コピー操作の状態を取得](onenoteoperation-get.md)します。</span><span class="sxs-lookup"><span data-stu-id="2fcaa-155">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="2fcaa-156">例</span><span class="sxs-lookup"><span data-stu-id="2fcaa-156">Example</span></span>
<span data-ttu-id="2fcaa-157">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="2fcaa-157">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2fcaa-158">要求</span><span class="sxs-lookup"><span data-stu-id="2fcaa-158">Request</span></span>
<span data-ttu-id="2fcaa-159">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2fcaa-159">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2fcaa-160">プロトコル</span><span class="sxs-lookup"><span data-stu-id="2fcaa-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "section_copytosectiongroup"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/sections/{id}/copyToSectionGroup
Content-type: application/json
Content-length: 84

{
  "id": "id-value",
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2fcaa-161">C#</span><span class="sxs-lookup"><span data-stu-id="2fcaa-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/section-copytosectiongroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2fcaa-162">Javascript</span><span class="sxs-lookup"><span data-stu-id="2fcaa-162">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/section-copytosectiongroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2fcaa-163">目的-C</span><span class="sxs-lookup"><span data-stu-id="2fcaa-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/section-copytosectiongroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2fcaa-164">応答</span><span class="sxs-lookup"><span data-stu-id="2fcaa-164">Response</span></span>
<span data-ttu-id="2fcaa-165">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="2fcaa-165">Here is an example of the response.</span></span>
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
  "description": "section: copyToSectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
