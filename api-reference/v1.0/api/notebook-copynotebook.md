---
title: 'notebook: copyNotebook'
description: コピー先ドキュメント ライブラリの [ノートブック] フォルダーにノートブックをコピーします。フォルダーが存在しない場合は、そのフォルダーが作成されます。
localization_priority: Normal
ms.openlocfilehash: 927cdd95a1cf39b27ac18faeeae11ccc56cfff6f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812769"
---
# <a name="notebook-copynotebook"></a><span data-ttu-id="9cde1-104">notebook: copyNotebook</span><span class="sxs-lookup"><span data-stu-id="9cde1-104">notebook: copyNotebook</span></span>
<span data-ttu-id="9cde1-p102">コピー先ドキュメント ライブラリの [ノートブック] フォルダーにノートブックをコピーします。フォルダーが存在しない場合は、そのフォルダーが作成されます。</span><span class="sxs-lookup"><span data-stu-id="9cde1-p102">Copies a notebook to the Notebooks folder in the destination Documents library. The folder is created if it doesn't exist.</span></span>

<span data-ttu-id="9cde1-107">Copy 操作では、非同期の呼び出しパターンに従います。まず Copy 操作を呼び出し、次に結果の操作エンドポイントをポーリングします。</span><span class="sxs-lookup"><span data-stu-id="9cde1-107">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="9cde1-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9cde1-108">Permissions</span></span>
<span data-ttu-id="9cde1-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9cde1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9cde1-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9cde1-111">Permission type</span></span>      | <span data-ttu-id="9cde1-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9cde1-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9cde1-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9cde1-113">Delegated (work or school account)</span></span> | <span data-ttu-id="9cde1-114">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cde1-114">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="9cde1-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9cde1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9cde1-116">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9cde1-116">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="9cde1-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9cde1-117">Application</span></span> | <span data-ttu-id="9cde1-118">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cde1-118">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9cde1-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9cde1-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/copyNotebook
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/copyNotebook
POST /groups/{id}/onenote/notebooks/{id}/copyNotebook
```
## <a name="request-headers"></a><span data-ttu-id="9cde1-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9cde1-120">Request headers</span></span>
| <span data-ttu-id="9cde1-121">名前</span><span class="sxs-lookup"><span data-stu-id="9cde1-121">Name</span></span>       | <span data-ttu-id="9cde1-122">種類</span><span class="sxs-lookup"><span data-stu-id="9cde1-122">Type</span></span> | <span data-ttu-id="9cde1-123">説明</span><span class="sxs-lookup"><span data-stu-id="9cde1-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9cde1-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9cde1-124">Authorization</span></span>  | <span data-ttu-id="9cde1-125">string</span><span class="sxs-lookup"><span data-stu-id="9cde1-125">string</span></span>  | <span data-ttu-id="9cde1-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9cde1-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9cde1-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9cde1-128">Content-Type</span></span> | <span data-ttu-id="9cde1-129">string</span><span class="sxs-lookup"><span data-stu-id="9cde1-129">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="9cde1-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="9cde1-130">Request body</span></span>
<span data-ttu-id="9cde1-p105">要求本文では、操作に必要なパラメーターを格納する JSON オブジェクトを指定します。パラメーターが必要ない場合は、空の要求本文を送信してもかまいません。</span><span class="sxs-lookup"><span data-stu-id="9cde1-p105">In the request body, provide a JSON object that contains the parameters that your operation needs. It's okay to send an empty body if none are needed.</span></span>

| <span data-ttu-id="9cde1-133">パラメーター</span><span class="sxs-lookup"><span data-stu-id="9cde1-133">Parameter</span></span>    | <span data-ttu-id="9cde1-134">Type</span><span class="sxs-lookup"><span data-stu-id="9cde1-134">Type</span></span>   |<span data-ttu-id="9cde1-135">説明</span><span class="sxs-lookup"><span data-stu-id="9cde1-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9cde1-136">groupId</span><span class="sxs-lookup"><span data-stu-id="9cde1-136">groupId</span></span>|<span data-ttu-id="9cde1-137">String</span><span class="sxs-lookup"><span data-stu-id="9cde1-137">String</span></span>|<span data-ttu-id="9cde1-p106">コピー先グループの ID。Office 365 グループにコピーする場合にのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="9cde1-p106">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="9cde1-140">renameAs</span><span class="sxs-lookup"><span data-stu-id="9cde1-140">renameAs</span></span>|<span data-ttu-id="9cde1-141">String</span><span class="sxs-lookup"><span data-stu-id="9cde1-141">String</span></span>|<span data-ttu-id="9cde1-p107">コピーの名前。既定値は、既存のアイテムの名前になります。</span><span class="sxs-lookup"><span data-stu-id="9cde1-p107">The name of the copy. Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="9cde1-144">応答</span><span class="sxs-lookup"><span data-stu-id="9cde1-144">Response</span></span>

<span data-ttu-id="9cde1-p108">成功した場合、このメソッドは `202 Accepted` 応答コードと `Operation-Location` ヘッダーを返します。Operation-Location エンドポイントをポーリングして、[コピー操作の状態を取得します](onenoteoperation-get.md)。</span><span class="sxs-lookup"><span data-stu-id="9cde1-p108">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="9cde1-147">例</span><span class="sxs-lookup"><span data-stu-id="9cde1-147">Example</span></span>
<span data-ttu-id="9cde1-148">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="9cde1-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9cde1-149">要求</span><span class="sxs-lookup"><span data-stu-id="9cde1-149">Request</span></span>
<span data-ttu-id="9cde1-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9cde1-150">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="9cde1-151">応答</span><span class="sxs-lookup"><span data-stu-id="9cde1-151">Response</span></span>
<span data-ttu-id="9cde1-152">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="9cde1-152">Here is an example of the response.</span></span>
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
