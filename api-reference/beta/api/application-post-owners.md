---
title: 所有者を作成する
description: この API を使用して、新しい所有者を作成します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fbf78bb61c57ef447da07663b5032ab213e3b46e
ms.sourcegitcommit: 82b73552fff79a4ef7a2ee57fc2d1b3286b5bd4c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/26/2019
ms.locfileid: "35908314"
---
# <a name="create-owner"></a><span data-ttu-id="ae5b5-103">所有者を作成する</span><span class="sxs-lookup"><span data-stu-id="ae5b5-103">Create owner</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae5b5-104">この API を使用して、新しい所有者を作成します。</span><span class="sxs-lookup"><span data-stu-id="ae5b5-104">Use this API to create a new owner.</span></span>

## <a name="permissions"></a><span data-ttu-id="ae5b5-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ae5b5-105">Permissions</span></span>
<span data-ttu-id="ae5b5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ae5b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae5b5-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ae5b5-108">Permission type</span></span>      | <span data-ttu-id="ae5b5-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ae5b5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae5b5-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ae5b5-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="ae5b5-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ae5b5-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ae5b5-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ae5b5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae5b5-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae5b5-113">Not supported.</span></span>    |
|<span data-ttu-id="ae5b5-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ae5b5-114">Application</span></span> | <span data-ttu-id="ae5b5-115">Application.readwrite.ownedby とディレクトリ。すべての、およびすべてのディレクトリを取得します。すべてのアプリケーション</span><span class="sxs-lookup"><span data-stu-id="ae5b5-115">Application.ReadWrite.OwnedBy and Directory.Read.All, Application.ReadWrite.All and Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae5b5-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ae5b5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/owners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="ae5b5-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ae5b5-117">Request headers</span></span>
| <span data-ttu-id="ae5b5-118">名前</span><span class="sxs-lookup"><span data-stu-id="ae5b5-118">Name</span></span> | <span data-ttu-id="ae5b5-119">説明</span><span class="sxs-lookup"><span data-stu-id="ae5b5-119">Description</span></span>|
|:---- |:---------- |
| <span data-ttu-id="ae5b5-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae5b5-120">Authorization</span></span> | <span data-ttu-id="ae5b5-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ae5b5-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ae5b5-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="ae5b5-123">Request body</span></span>
<span data-ttu-id="ae5b5-124">要求本文で、owner として割り当てられるディレクトリオブジェクトの識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="ae5b5-124">In the request body, supply the identifier of the directory object to be assigned as owner.</span></span>

## <a name="response"></a><span data-ttu-id="ae5b5-125">応答</span><span class="sxs-lookup"><span data-stu-id="ae5b5-125">Response</span></span>

<span data-ttu-id="ae5b5-126">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="ae5b5-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ae5b5-127">例</span><span class="sxs-lookup"><span data-stu-id="ae5b5-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="ae5b5-128">要求</span><span class="sxs-lookup"><span data-stu-id="ae5b5-128">Request</span></span>
<span data-ttu-id="ae5b5-129">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="ae5b5-129">The following example shows the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ae5b5-130">プロトコル</span><span class="sxs-lookup"><span data-stu-id="ae5b5-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_application"
}-->
```http
POST https://graph.microsoft.com/beta/applications/{id}/owners/$ref
Content-type: application/json
Content-length: 30

{
"@odata.id": "https://graph.microsoft.com/beta/directoryObjects/{id}"
}

```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ae5b5-131">Javascript</span><span class="sxs-lookup"><span data-stu-id="ae5b5-131">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="ae5b5-132">応答</span><span class="sxs-lookup"><span data-stu-id="ae5b5-132">Response</span></span>

<span data-ttu-id="ae5b5-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ae5b5-133">The following is an example of the response.</span></span>

><span data-ttu-id="ae5b5-134">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="ae5b5-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ae5b5-135">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="ae5b5-135">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
