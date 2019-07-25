---
title: ディレクトリ ロールのメンバーを追加する
description: この API を使用して、新しいディレクトリ ロールのメンバーを作成します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 06338f2dfbed00f3150a9278cbc9f4a21a59b5c1
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35891069"
---
# <a name="add-directory-role-member"></a><span data-ttu-id="d0676-103">ディレクトリ ロールのメンバーを追加する</span><span class="sxs-lookup"><span data-stu-id="d0676-103">Add directory role member</span></span>

<span data-ttu-id="d0676-104">この API を使用して、新しいディレクトリ ロールのメンバーを作成します。</span><span class="sxs-lookup"><span data-stu-id="d0676-104">Use this API to create a new directory role member.</span></span>

## <a name="permissions"></a><span data-ttu-id="d0676-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d0676-105">Permissions</span></span>
<span data-ttu-id="d0676-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d0676-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0676-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d0676-108">Permission type</span></span>      | <span data-ttu-id="d0676-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d0676-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0676-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d0676-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d0676-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d0676-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d0676-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d0676-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0676-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d0676-113">Not supported.</span></span>    |
|<span data-ttu-id="d0676-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d0676-114">Application</span></span> | <span data-ttu-id="d0676-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d0676-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d0676-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d0676-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles/{id}/members/$ref

```
## <a name="request-headers"></a><span data-ttu-id="d0676-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d0676-117">Request headers</span></span>
| <span data-ttu-id="d0676-118">名前</span><span class="sxs-lookup"><span data-stu-id="d0676-118">Name</span></span>       | <span data-ttu-id="d0676-119">型</span><span class="sxs-lookup"><span data-stu-id="d0676-119">Type</span></span> | <span data-ttu-id="d0676-120">説明</span><span class="sxs-lookup"><span data-stu-id="d0676-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d0676-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0676-121">Authorization</span></span>  | <span data-ttu-id="d0676-122">string</span><span class="sxs-lookup"><span data-stu-id="d0676-122">string</span></span>  | <span data-ttu-id="d0676-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d0676-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d0676-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d0676-125">Content-Type</span></span>  | <span data-ttu-id="d0676-126">string</span><span class="sxs-lookup"><span data-stu-id="d0676-126">string</span></span>  | <span data-ttu-id="d0676-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d0676-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d0676-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="d0676-128">Request body</span></span>
<span data-ttu-id="d0676-129">要求本文で、追加する [directoryObject](../resources/directoryobject.md) または[ユーザー](../resources/user.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d0676-129">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="d0676-130">応答</span><span class="sxs-lookup"><span data-stu-id="d0676-130">Response</span></span>

<span data-ttu-id="d0676-131">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="d0676-131">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d0676-132">例</span><span class="sxs-lookup"><span data-stu-id="d0676-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d0676-133">要求</span><span class="sxs-lookup"><span data-stu-id="d0676-133">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d0676-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="d0676-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryrole"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryRoles/{id}/members/$ref
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d0676-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="d0676-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d0676-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="d0676-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-directoryrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="ctabcsharp"></a>[<span data-ttu-id="d0676-137">C#</span><span class="sxs-lookup"><span data-stu-id="d0676-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-directoryrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d0676-138">Java</span><span class="sxs-lookup"><span data-stu-id="d0676-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-directoryrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d0676-139">応答</span><span class="sxs-lookup"><span data-stu-id="d0676-139">Response</span></span>
<span data-ttu-id="d0676-140">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="d0676-140">Note: The response object shown here may be truncated for brevity.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
Content-type: text/plain

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
