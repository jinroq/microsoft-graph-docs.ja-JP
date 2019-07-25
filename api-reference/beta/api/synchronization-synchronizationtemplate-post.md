---
title: 同期テンプレートの作成
description: 指定したアプリケーションの新しい同期テンプレートを作成します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b5e9a3a9e90ef803f1c7a970edcb2c624b5196bc
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869083"
---
# <a name="create-synchronizationtemplate"></a><span data-ttu-id="74b6d-103">同期テンプレートの作成</span><span class="sxs-lookup"><span data-stu-id="74b6d-103">Create synchronizationTemplate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74b6d-104">指定したアプリケーションの新しい同期テンプレートを作成します。</span><span class="sxs-lookup"><span data-stu-id="74b6d-104">Create a new synchronization template for a given application.</span></span>

## <a name="permissions"></a><span data-ttu-id="74b6d-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="74b6d-105">Permissions</span></span>
<span data-ttu-id="74b6d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="74b6d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74b6d-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="74b6d-108">Permission type</span></span>                        | <span data-ttu-id="74b6d-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="74b6d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="74b6d-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="74b6d-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="74b6d-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74b6d-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="74b6d-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="74b6d-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="74b6d-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="74b6d-113">Not supported.</span></span>|
|<span data-ttu-id="74b6d-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="74b6d-114">Application</span></span>                            |<span data-ttu-id="74b6d-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="74b6d-115">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="74b6d-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="74b6d-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/synchronization/templates/
```

## <a name="request-headers"></a><span data-ttu-id="74b6d-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="74b6d-117">Request headers</span></span>

| <span data-ttu-id="74b6d-118">名前</span><span class="sxs-lookup"><span data-stu-id="74b6d-118">Name</span></span>           | <span data-ttu-id="74b6d-119">型</span><span class="sxs-lookup"><span data-stu-id="74b6d-119">Type</span></span>    | <span data-ttu-id="74b6d-120">説明</span><span class="sxs-lookup"><span data-stu-id="74b6d-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="74b6d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="74b6d-121">Authorization</span></span>  | <span data-ttu-id="74b6d-122">string</span><span class="sxs-lookup"><span data-stu-id="74b6d-122">string</span></span>  | <span data-ttu-id="74b6d-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="74b6d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="74b6d-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="74b6d-125">Request body</span></span>

<span data-ttu-id="74b6d-126">要求本文で、作成する[同期テンプレート](../resources/synchronization-synchronizationtemplate.md)オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="74b6d-126">In the request body, supply the [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object to be created.</span></span> <span data-ttu-id="74b6d-127">`id`、 `applicationId`および`factoryTag`プロパティは必須です。</span><span class="sxs-lookup"><span data-stu-id="74b6d-127">The `id`, `applicationId` and `factoryTag` properties are required.</span></span> <span data-ttu-id="74b6d-128">テンプレートに`schema`何も指定されていない場合は、 `factoryTag`プロパティに関連付けられている既定のスキーマが使用されます。</span><span class="sxs-lookup"><span data-stu-id="74b6d-128">When no `schema` is provided with the template, the default schema associated with the `factoryTag` property will be used.</span></span>

### <a name="response"></a><span data-ttu-id="74b6d-129">応答</span><span class="sxs-lookup"><span data-stu-id="74b6d-129">Response</span></span>

<span data-ttu-id="74b6d-130">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[同期テンプレート](../resources/synchronization-synchronizationtemplate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="74b6d-130">If successful, this method returns a `201 Created` response code and a [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="74b6d-131">例</span><span class="sxs-lookup"><span data-stu-id="74b6d-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="74b6d-132">要求</span><span class="sxs-lookup"><span data-stu-id="74b6d-132">Request</span></span>
<span data-ttu-id="74b6d-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="74b6d-133">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="74b6d-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="74b6d-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_synchronizationtemplate_from_synchronization"
}-->
```http
POST https://graph.microsoft.com/beta/applications/{id}/synchronization/templates
Content-type: application/json

{ 
    "id": "SCIM-Test1",
    "applicationId": "{id}",
    "factoryTag": "CustomSCIM"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="74b6d-135">C#</span><span class="sxs-lookup"><span data-stu-id="74b6d-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-synchronizationtemplate-from-synchronization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="74b6d-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="74b6d-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-synchronizationtemplate-from-synchronization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="74b6d-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="74b6d-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-synchronizationtemplate-from-synchronization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="74b6d-138">Java</span><span class="sxs-lookup"><span data-stu-id="74b6d-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-synchronizationtemplate-from-synchronization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="74b6d-139">応答</span><span class="sxs-lookup"><span data-stu-id="74b6d-139">Response</span></span>
<span data-ttu-id="74b6d-140">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="74b6d-140">The following is an example of a response.</span></span>
><span data-ttu-id="74b6d-141">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="74b6d-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="74b6d-142">実際の呼び出しでは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="74b6d-142">All the properties will be returned in an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationTemplate"
} -->
```http
HTTP/1.1 201 Created

{
    "id": "SCIM-Test1",
    "applicationId": "{id}",
    "factoryTag": "CustomSCIM",
    "schema": {
        "directories": [],
        "synchronizationRules": []
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create synchronizationTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
