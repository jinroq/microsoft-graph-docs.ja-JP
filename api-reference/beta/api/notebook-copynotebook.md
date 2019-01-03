---
title: 'notebook: copyNotebook'
description: コピー先ドキュメント ライブラリの [ノートブック] フォルダーにノートブックをコピーします。フォルダーが存在しない場合は、そのフォルダーが作成されます。
ms.openlocfilehash: 4d22c6904f14d0ccc5d4f3de35cdf46fbd3afd6a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070336"
---
# <a name="notebook-copynotebook"></a><span data-ttu-id="e755c-104">notebook: copyNotebook</span><span class="sxs-lookup"><span data-stu-id="e755c-104">notebook: copyNotebook</span></span>

> <span data-ttu-id="e755c-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e755c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e755c-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e755c-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e755c-p103">コピー先ドキュメント ライブラリの [ノートブック] フォルダーにノートブックをコピーします。フォルダーが存在しない場合は、そのフォルダーが作成されます。</span><span class="sxs-lookup"><span data-stu-id="e755c-p103">Copies a notebook to the Notebooks folder in the destination Documents library. The folder is created if it doesn't exist.</span></span>

<span data-ttu-id="e755c-109">Copy 操作では、非同期の呼び出しパターンに従います。まず Copy 操作を呼び出し、次に結果の操作エンドポイントをポーリングします。</span><span class="sxs-lookup"><span data-stu-id="e755c-109">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="e755c-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e755c-110">Permissions</span></span>
<span data-ttu-id="e755c-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e755c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e755c-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e755c-113">Permission type</span></span>      | <span data-ttu-id="e755c-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e755c-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e755c-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e755c-115">Delegated (work or school account)</span></span> | <span data-ttu-id="e755c-116">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e755c-116">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="e755c-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e755c-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e755c-118">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e755c-118">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="e755c-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e755c-119">Application</span></span> | <span data-ttu-id="e755c-120">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e755c-120">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e755c-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e755c-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/copyNotebook
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/copyNotebook
POST /groups/{id}/onenote/notebooks/{id}/copyNotebook
POST /sites/{id}/onenote/notebooks/{id}/copyNotebook
```
## <a name="request-headers"></a><span data-ttu-id="e755c-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e755c-122">Request headers</span></span>
| <span data-ttu-id="e755c-123">名前</span><span class="sxs-lookup"><span data-stu-id="e755c-123">Name</span></span>       | <span data-ttu-id="e755c-124">型</span><span class="sxs-lookup"><span data-stu-id="e755c-124">Type</span></span> | <span data-ttu-id="e755c-125">説明</span><span class="sxs-lookup"><span data-stu-id="e755c-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e755c-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="e755c-126">Authorization</span></span>  | <span data-ttu-id="e755c-127">string</span><span class="sxs-lookup"><span data-stu-id="e755c-127">string</span></span>  | <span data-ttu-id="e755c-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e755c-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e755c-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e755c-130">Content-Type</span></span> | <span data-ttu-id="e755c-131">string</span><span class="sxs-lookup"><span data-stu-id="e755c-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="e755c-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="e755c-132">Request body</span></span>
<span data-ttu-id="e755c-p106">要求本文では、操作に必要なパラメーターを格納する JSON オブジェクトを指定します。パラメーターが必要ない場合は、空の要求本文を送信してもかまいません。</span><span class="sxs-lookup"><span data-stu-id="e755c-p106">In the request body, provide a JSON object that contains the parameters that your operation needs. It's okay to send an empty body if none are needed.</span></span>

| <span data-ttu-id="e755c-135">パラメーター</span><span class="sxs-lookup"><span data-stu-id="e755c-135">Parameter</span></span>    | <span data-ttu-id="e755c-136">型</span><span class="sxs-lookup"><span data-stu-id="e755c-136">Type</span></span>   |<span data-ttu-id="e755c-137">説明</span><span class="sxs-lookup"><span data-stu-id="e755c-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e755c-138">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="e755c-138">siteCollectionId</span></span>|<span data-ttu-id="e755c-139">String</span><span class="sxs-lookup"><span data-stu-id="e755c-139">String</span></span>|<span data-ttu-id="e755c-140">コピーする SharePoint サイトの id です。</span><span class="sxs-lookup"><span data-stu-id="e755c-140">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="e755c-141">Office 365 チーム サイトにコピーするときにのみを使用します。</span><span class="sxs-lookup"><span data-stu-id="e755c-141">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="e755c-142">siteId</span><span class="sxs-lookup"><span data-stu-id="e755c-142">siteId</span></span>|<span data-ttu-id="e755c-143">String</span><span class="sxs-lookup"><span data-stu-id="e755c-143">String</span></span>|<span data-ttu-id="e755c-144">コピーする SharePoint web の id です。</span><span class="sxs-lookup"><span data-stu-id="e755c-144">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="e755c-145">Office 365 チーム サイトにコピーするときにのみを使用します。</span><span class="sxs-lookup"><span data-stu-id="e755c-145">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="e755c-146">グループ Id</span><span class="sxs-lookup"><span data-stu-id="e755c-146">groupId</span></span>|<span data-ttu-id="e755c-147">String</span><span class="sxs-lookup"><span data-stu-id="e755c-147">String</span></span>|<span data-ttu-id="e755c-p109">コピー先グループの ID。Office 365 グループにコピーする場合にのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="e755c-p109">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="e755c-150">renameAs</span><span class="sxs-lookup"><span data-stu-id="e755c-150">renameAs</span></span>|<span data-ttu-id="e755c-151">String</span><span class="sxs-lookup"><span data-stu-id="e755c-151">String</span></span>|<span data-ttu-id="e755c-p110">コピーの名前。既定値は、既存のアイテムの名前になります。</span><span class="sxs-lookup"><span data-stu-id="e755c-p110">The name of the copy. Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="e755c-154">応答</span><span class="sxs-lookup"><span data-stu-id="e755c-154">Response</span></span>

<span data-ttu-id="e755c-p111">成功した場合、このメソッドは `202 Accepted` 応答コードと `Operation-Location` ヘッダーを返します。Operation-Location エンドポイントをポーリングして、[コピー操作の状態を取得します](onenoteoperation-get.md)。</span><span class="sxs-lookup"><span data-stu-id="e755c-p111">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="e755c-157">例</span><span class="sxs-lookup"><span data-stu-id="e755c-157">Example</span></span>
<span data-ttu-id="e755c-158">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="e755c-158">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e755c-159">要求</span><span class="sxs-lookup"><span data-stu-id="e755c-159">Request</span></span>
<span data-ttu-id="e755c-160">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e755c-160">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="e755c-161">応答</span><span class="sxs-lookup"><span data-stu-id="e755c-161">Response</span></span>
<span data-ttu-id="e755c-162">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="e755c-162">Here is an example of the response.</span></span>
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
  "tocPath": ""
}-->