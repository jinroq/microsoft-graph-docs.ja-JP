---
title: 上司を割り当てる
description: この API を使用して、ユーザーの上司を割り当てます。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b8d545b1aa606ae1c87391138347d6d4018a5d6a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35987529"
---
# <a name="assign-a-manager"></a><span data-ttu-id="7b4b5-103">上司を割り当てる</span><span class="sxs-lookup"><span data-stu-id="7b4b5-103">Assign a manager</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b4b5-104">この API を使用して、ユーザーの上司を割り当てます。</span><span class="sxs-lookup"><span data-stu-id="7b4b5-104">Use this API to assign a user's manager.</span></span>
> <span data-ttu-id="7b4b5-105">注:直属の部下を割り当てることはできません。代わりにこの API を使用します。</span><span class="sxs-lookup"><span data-stu-id="7b4b5-105">Note: You cannot assign direct reports - instead use this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="7b4b5-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7b4b5-106">Permissions</span></span>
<span data-ttu-id="7b4b5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7b4b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b4b5-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7b4b5-109">Permission type</span></span>      | <span data-ttu-id="7b4b5-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7b4b5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7b4b5-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7b4b5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7b4b5-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7b4b5-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7b4b5-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7b4b5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b4b5-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7b4b5-114">Not supported.</span></span>    |
|<span data-ttu-id="7b4b5-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7b4b5-115">Application</span></span> | <span data-ttu-id="7b4b5-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b4b5-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7b4b5-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7b4b5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /users/{id}/manager/$ref
```
## <a name="request-headers"></a><span data-ttu-id="7b4b5-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7b4b5-118">Request headers</span></span>
| <span data-ttu-id="7b4b5-119">名前</span><span class="sxs-lookup"><span data-stu-id="7b4b5-119">Name</span></span>       | <span data-ttu-id="7b4b5-120">型</span><span class="sxs-lookup"><span data-stu-id="7b4b5-120">Type</span></span> | <span data-ttu-id="7b4b5-121">説明</span><span class="sxs-lookup"><span data-stu-id="7b4b5-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7b4b5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b4b5-122">Authorization</span></span>  | <span data-ttu-id="7b4b5-123">string</span><span class="sxs-lookup"><span data-stu-id="7b4b5-123">string</span></span>  | <span data-ttu-id="7b4b5-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7b4b5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7b4b5-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="7b4b5-126">Request body</span></span>
<span data-ttu-id="7b4b5-127">要求本文で、追加する [directoryObject](../resources/directoryobject.md) または[ユーザー](../resources/user.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7b4b5-127">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="7b4b5-128">応答</span><span class="sxs-lookup"><span data-stu-id="7b4b5-128">Response</span></span>

<span data-ttu-id="7b4b5-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="7b4b5-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b4b5-131">例</span><span class="sxs-lookup"><span data-stu-id="7b4b5-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7b4b5-132">要求</span><span class="sxs-lookup"><span data-stu-id="7b4b5-132">Request</span></span>
<span data-ttu-id="7b4b5-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7b4b5-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7b4b5-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="7b4b5-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_manager_for_user"
}-->
```http
PUT https://graph.microsoft.com/v1.0/users/{id}/manager/$ref
Content-type: application/json
Content-length: xxx

{
  "@odata.id": "https://graph.microsoft.com/v1.0/users/{id}"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7b4b5-135">C#</span><span class="sxs-lookup"><span data-stu-id="7b4b5-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-manager-for-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7b4b5-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="7b4b5-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-manager-for-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7b4b5-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="7b4b5-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-manager-for-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7b4b5-138">Java</span><span class="sxs-lookup"><span data-stu-id="7b4b5-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-manager-for-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="7b4b5-139">要求本文で、追加する[ユーザー](../resources/user.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7b4b5-139">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>
##### <a name="response"></a><span data-ttu-id="7b4b5-140">応答</span><span class="sxs-lookup"><span data-stu-id="7b4b5-140">Response</span></span>
<span data-ttu-id="7b4b5-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7b4b5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
