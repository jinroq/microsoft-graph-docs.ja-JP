---
title: 'section: copyToNotebook'
description: 特定のノートブックにセクションをコピーします。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 4ec5292aa7b11b268b73514af8aee42260e3d6a9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523324"
---
# <a name="section-copytonotebook"></a><span data-ttu-id="78c82-103">section: copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="78c82-103">section: copyToNotebook</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78c82-104">特定のノートブックにセクションをコピーします。</span><span class="sxs-lookup"><span data-stu-id="78c82-104">Copies a section to a specific notebook.</span></span>

<span data-ttu-id="78c82-105">Copy 操作では、非同期の呼び出しパターンに従います。まず Copy 操作を呼び出し、次に結果の操作エンドポイントをポーリングします。</span><span class="sxs-lookup"><span data-stu-id="78c82-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>
## <a name="permissions"></a><span data-ttu-id="78c82-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="78c82-106">Permissions</span></span>
<span data-ttu-id="78c82-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="78c82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78c82-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="78c82-109">Permission type</span></span>      | <span data-ttu-id="78c82-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="78c82-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="78c82-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="78c82-111">Delegated (work or school account)</span></span> | <span data-ttu-id="78c82-112">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78c82-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="78c82-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="78c82-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78c82-114">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="78c82-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="78c82-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="78c82-115">Application</span></span> | <span data-ttu-id="78c82-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78c82-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="78c82-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="78c82-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToNotebook
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToNotebook
POST /groups/{id}/onenote/sections/{id}/copyToNotebook
POST /sites/{id}/onenote/sections/{id}/copyToNotebook
```
## <a name="request-headers"></a><span data-ttu-id="78c82-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="78c82-118">Request headers</span></span>
| <span data-ttu-id="78c82-119">名前</span><span class="sxs-lookup"><span data-stu-id="78c82-119">Name</span></span>       | <span data-ttu-id="78c82-120">型</span><span class="sxs-lookup"><span data-stu-id="78c82-120">Type</span></span> | <span data-ttu-id="78c82-121">説明</span><span class="sxs-lookup"><span data-stu-id="78c82-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="78c82-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="78c82-122">Authorization</span></span>  | <span data-ttu-id="78c82-123">string</span><span class="sxs-lookup"><span data-stu-id="78c82-123">string</span></span>  | <span data-ttu-id="78c82-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="78c82-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="78c82-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="78c82-126">Content-Type</span></span> | <span data-ttu-id="78c82-127">string</span><span class="sxs-lookup"><span data-stu-id="78c82-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="78c82-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="78c82-128">Request body</span></span>
<span data-ttu-id="78c82-129">要求本文では、操作に必要なパラメーターを格納する JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="78c82-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="78c82-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="78c82-130">Parameter</span></span>    | <span data-ttu-id="78c82-131">型</span><span class="sxs-lookup"><span data-stu-id="78c82-131">Type</span></span>   |<span data-ttu-id="78c82-132">説明</span><span class="sxs-lookup"><span data-stu-id="78c82-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="78c82-133">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="78c82-133">siteCollectionId</span></span>|<span data-ttu-id="78c82-134">String</span><span class="sxs-lookup"><span data-stu-id="78c82-134">String</span></span>|<span data-ttu-id="78c82-135">コピーする SharePoint サイトの id です。</span><span class="sxs-lookup"><span data-stu-id="78c82-135">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="78c82-136">Office 365 チーム サイトにコピーするときにのみを使用します。</span><span class="sxs-lookup"><span data-stu-id="78c82-136">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="78c82-137">siteId</span><span class="sxs-lookup"><span data-stu-id="78c82-137">siteId</span></span>|<span data-ttu-id="78c82-138">String</span><span class="sxs-lookup"><span data-stu-id="78c82-138">String</span></span>|<span data-ttu-id="78c82-139">コピーする SharePoint web の id です。</span><span class="sxs-lookup"><span data-stu-id="78c82-139">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="78c82-140">Office 365 チーム サイトにコピーするときにのみを使用します。</span><span class="sxs-lookup"><span data-stu-id="78c82-140">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="78c82-141">groupId</span><span class="sxs-lookup"><span data-stu-id="78c82-141">groupId</span></span>|<span data-ttu-id="78c82-142">文字列</span><span class="sxs-lookup"><span data-stu-id="78c82-142">String</span></span>|<span data-ttu-id="78c82-p105">コピー先グループの ID。Office 365 グループにコピーする場合にのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="78c82-p105">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="78c82-145">id</span><span class="sxs-lookup"><span data-stu-id="78c82-145">id</span></span>|<span data-ttu-id="78c82-146">String</span><span class="sxs-lookup"><span data-stu-id="78c82-146">String</span></span>|<span data-ttu-id="78c82-p106">必須。コピー先ノートブックの ID。</span><span class="sxs-lookup"><span data-stu-id="78c82-p106">Required. The id of the destination notebook.</span></span> |
|<span data-ttu-id="78c82-149">renameAs</span><span class="sxs-lookup"><span data-stu-id="78c82-149">renameAs</span></span>|<span data-ttu-id="78c82-150">String</span><span class="sxs-lookup"><span data-stu-id="78c82-150">String</span></span>|<span data-ttu-id="78c82-p107">コピーの名前。既定値は、既存のアイテムの名前になります。</span><span class="sxs-lookup"><span data-stu-id="78c82-p107">The name of the copy. Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="78c82-153">応答</span><span class="sxs-lookup"><span data-stu-id="78c82-153">Response</span></span>

<span data-ttu-id="78c82-p108">成功した場合、このメソッドは `202 Accepted` 応答コードと `Operation-Location` ヘッダーを返します。Operation-Location エンドポイントをポーリングして、[コピー操作の状態を取得します](onenoteoperation-get.md)。</span><span class="sxs-lookup"><span data-stu-id="78c82-p108">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="78c82-156">例</span><span class="sxs-lookup"><span data-stu-id="78c82-156">Example</span></span>
<span data-ttu-id="78c82-157">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="78c82-157">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="78c82-158">要求</span><span class="sxs-lookup"><span data-stu-id="78c82-158">Request</span></span>
<span data-ttu-id="78c82-159">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="78c82-159">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "section_copytonotebook"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/sections/{id}/copyToNotebook
Content-type: application/json
Content-length: 84

{
  "id": "id-value",
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```

##### <a name="response"></a><span data-ttu-id="78c82-160">応答</span><span class="sxs-lookup"><span data-stu-id="78c82-160">Response</span></span>
<span data-ttu-id="78c82-161">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="78c82-161">Here is an example of the response.</span></span>
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
  "description": "section: copyToNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/section-copytonotebook.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
