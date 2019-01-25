---
title: 'notebook: copyNotebook'
description: コピー先ドキュメント ライブラリの [ノートブック] フォルダーにノートブックをコピーします。フォルダーが存在しない場合は、そのフォルダーが作成されます。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 7100d768fb411aeab8ccbd0622de26aeae8a7133
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515602"
---
# <a name="notebook-copynotebook"></a><span data-ttu-id="8546c-104">notebook: copyNotebook</span><span class="sxs-lookup"><span data-stu-id="8546c-104">notebook: copyNotebook</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8546c-p102">コピー先ドキュメント ライブラリの [ノートブック] フォルダーにノートブックをコピーします。フォルダーが存在しない場合は、そのフォルダーが作成されます。</span><span class="sxs-lookup"><span data-stu-id="8546c-p102">Copies a notebook to the Notebooks folder in the destination Documents library. The folder is created if it doesn't exist.</span></span>

<span data-ttu-id="8546c-107">Copy 操作では、非同期の呼び出しパターンに従います。まず Copy 操作を呼び出し、次に結果の操作エンドポイントをポーリングします。</span><span class="sxs-lookup"><span data-stu-id="8546c-107">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="8546c-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8546c-108">Permissions</span></span>
<span data-ttu-id="8546c-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8546c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8546c-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8546c-111">Permission type</span></span>      | <span data-ttu-id="8546c-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8546c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8546c-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8546c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="8546c-114">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8546c-114">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="8546c-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8546c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8546c-116">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8546c-116">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="8546c-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8546c-117">Application</span></span> | <span data-ttu-id="8546c-118">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8546c-118">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8546c-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8546c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/copyNotebook
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/copyNotebook
POST /groups/{id}/onenote/notebooks/{id}/copyNotebook
POST /sites/{id}/onenote/notebooks/{id}/copyNotebook
```
## <a name="request-headers"></a><span data-ttu-id="8546c-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8546c-120">Request headers</span></span>
| <span data-ttu-id="8546c-121">名前</span><span class="sxs-lookup"><span data-stu-id="8546c-121">Name</span></span>       | <span data-ttu-id="8546c-122">型</span><span class="sxs-lookup"><span data-stu-id="8546c-122">Type</span></span> | <span data-ttu-id="8546c-123">説明</span><span class="sxs-lookup"><span data-stu-id="8546c-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8546c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8546c-124">Authorization</span></span>  | <span data-ttu-id="8546c-125">string</span><span class="sxs-lookup"><span data-stu-id="8546c-125">string</span></span>  | <span data-ttu-id="8546c-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8546c-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8546c-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8546c-128">Content-Type</span></span> | <span data-ttu-id="8546c-129">string</span><span class="sxs-lookup"><span data-stu-id="8546c-129">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="8546c-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="8546c-130">Request body</span></span>
<span data-ttu-id="8546c-p105">要求本文では、操作に必要なパラメーターを格納する JSON オブジェクトを指定します。パラメーターが必要ない場合は、空の要求本文を送信してもかまいません。</span><span class="sxs-lookup"><span data-stu-id="8546c-p105">In the request body, provide a JSON object that contains the parameters that your operation needs. It's okay to send an empty body if none are needed.</span></span>

| <span data-ttu-id="8546c-133">パラメーター</span><span class="sxs-lookup"><span data-stu-id="8546c-133">Parameter</span></span>    | <span data-ttu-id="8546c-134">型</span><span class="sxs-lookup"><span data-stu-id="8546c-134">Type</span></span>   |<span data-ttu-id="8546c-135">説明</span><span class="sxs-lookup"><span data-stu-id="8546c-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8546c-136">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="8546c-136">siteCollectionId</span></span>|<span data-ttu-id="8546c-137">String</span><span class="sxs-lookup"><span data-stu-id="8546c-137">String</span></span>|<span data-ttu-id="8546c-138">コピーする SharePoint サイトの id です。</span><span class="sxs-lookup"><span data-stu-id="8546c-138">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="8546c-139">Office 365 チーム サイトにコピーするときにのみを使用します。</span><span class="sxs-lookup"><span data-stu-id="8546c-139">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="8546c-140">siteId</span><span class="sxs-lookup"><span data-stu-id="8546c-140">siteId</span></span>|<span data-ttu-id="8546c-141">String</span><span class="sxs-lookup"><span data-stu-id="8546c-141">String</span></span>|<span data-ttu-id="8546c-142">コピーする SharePoint web の id です。</span><span class="sxs-lookup"><span data-stu-id="8546c-142">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="8546c-143">Office 365 チーム サイトにコピーするときにのみを使用します。</span><span class="sxs-lookup"><span data-stu-id="8546c-143">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="8546c-144">groupId</span><span class="sxs-lookup"><span data-stu-id="8546c-144">groupId</span></span>|<span data-ttu-id="8546c-145">文字列</span><span class="sxs-lookup"><span data-stu-id="8546c-145">String</span></span>|<span data-ttu-id="8546c-p108">コピー先グループの ID。Office 365 グループにコピーする場合にのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="8546c-p108">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="8546c-148">renameAs</span><span class="sxs-lookup"><span data-stu-id="8546c-148">renameAs</span></span>|<span data-ttu-id="8546c-149">String</span><span class="sxs-lookup"><span data-stu-id="8546c-149">String</span></span>|<span data-ttu-id="8546c-p109">コピーの名前。既定値は、既存のアイテムの名前になります。</span><span class="sxs-lookup"><span data-stu-id="8546c-p109">The name of the copy. Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="8546c-152">応答</span><span class="sxs-lookup"><span data-stu-id="8546c-152">Response</span></span>

<span data-ttu-id="8546c-p110">成功した場合、このメソッドは `202 Accepted` 応答コードと `Operation-Location` ヘッダーを返します。Operation-Location エンドポイントをポーリングして、[コピー操作の状態を取得します](onenoteoperation-get.md)。</span><span class="sxs-lookup"><span data-stu-id="8546c-p110">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="8546c-155">例</span><span class="sxs-lookup"><span data-stu-id="8546c-155">Example</span></span>
<span data-ttu-id="8546c-156">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="8546c-156">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8546c-157">要求</span><span class="sxs-lookup"><span data-stu-id="8546c-157">Request</span></span>
<span data-ttu-id="8546c-158">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8546c-158">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="8546c-159">応答</span><span class="sxs-lookup"><span data-stu-id="8546c-159">Response</span></span>
<span data-ttu-id="8546c-160">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="8546c-160">Here is an example of the response.</span></span>
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
    "Error: /api-reference/beta/api/notebook-copynotebook.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
