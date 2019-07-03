---
title: 上司を割り当てる
description: この API を使用して、ユーザーの上司を割り当てます。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9f4c9da1913a255c875585378f10a4c3c6d9a7e1
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35456765"
---
# <a name="assign-a-manager"></a><span data-ttu-id="7a963-103">上司を割り当てる</span><span class="sxs-lookup"><span data-stu-id="7a963-103">Assign a manager</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a963-104">この API を使用して、ユーザーの上司を割り当てます。</span><span class="sxs-lookup"><span data-stu-id="7a963-104">Use this API to assign a user's manager.</span></span>
> <span data-ttu-id="7a963-105">注:直属の部下を割り当てることはできません。代わりにこの API を使用します。</span><span class="sxs-lookup"><span data-stu-id="7a963-105">Note: You cannot assign direct reports - instead use this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="7a963-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7a963-106">Permissions</span></span>
<span data-ttu-id="7a963-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7a963-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a963-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7a963-109">Permission type</span></span>      | <span data-ttu-id="7a963-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7a963-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7a963-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7a963-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7a963-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7a963-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7a963-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7a963-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7a963-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7a963-114">Not supported.</span></span>    |
|<span data-ttu-id="7a963-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7a963-115">Application</span></span> | <span data-ttu-id="7a963-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a963-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7a963-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7a963-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /users/{id}/manager/$ref
```
## <a name="request-headers"></a><span data-ttu-id="7a963-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7a963-118">Request headers</span></span>
| <span data-ttu-id="7a963-119">名前</span><span class="sxs-lookup"><span data-stu-id="7a963-119">Name</span></span>       | <span data-ttu-id="7a963-120">型</span><span class="sxs-lookup"><span data-stu-id="7a963-120">Type</span></span> | <span data-ttu-id="7a963-121">説明</span><span class="sxs-lookup"><span data-stu-id="7a963-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7a963-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a963-122">Authorization</span></span>  | <span data-ttu-id="7a963-123">string</span><span class="sxs-lookup"><span data-stu-id="7a963-123">string</span></span>  | <span data-ttu-id="7a963-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7a963-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7a963-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="7a963-126">Request body</span></span>
<span data-ttu-id="7a963-127">要求本文で、追加する [directoryObject](../resources/directoryobject.md) または[ユーザー](../resources/user.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7a963-127">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="7a963-128">応答</span><span class="sxs-lookup"><span data-stu-id="7a963-128">Response</span></span>

<span data-ttu-id="7a963-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="7a963-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a963-131">例</span><span class="sxs-lookup"><span data-stu-id="7a963-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7a963-132">要求</span><span class="sxs-lookup"><span data-stu-id="7a963-132">Request</span></span>
<span data-ttu-id="7a963-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7a963-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7a963-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="7a963-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
PUT https://graph.microsoft.com/v1.0/users/{id}/manager/$ref
Content-type: application/json
Content-length: xxx

{
  "@odata.id": "https://graph.microsoft.com/v1.0/users/{id}"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7a963-135">C#</span><span class="sxs-lookup"><span data-stu-id="7a963-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7a963-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="7a963-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7a963-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="7a963-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="7a963-138">要求本文で、追加する[ユーザー](../resources/user.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7a963-138">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>
##### <a name="response"></a><span data-ttu-id="7a963-139">応答</span><span class="sxs-lookup"><span data-stu-id="7a963-139">Response</span></span>
<span data-ttu-id="7a963-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7a963-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
