---
title: SynchronizationTemplate を作成します。
description: 特定のアプリケーション用の新しい同期テンプレートを作成します。
ms.openlocfilehash: 1c7bc08eee4088796123d3c7fa2cac5c83becac2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068424"
---
# <a name="create-synchronizationtemplate"></a><span data-ttu-id="cadf5-103">SynchronizationTemplate を作成します。</span><span class="sxs-lookup"><span data-stu-id="cadf5-103">Create synchronizationTemplate</span></span>

> <span data-ttu-id="cadf5-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cadf5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cadf5-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cadf5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cadf5-106">特定のアプリケーション用の新しい同期テンプレートを作成します。</span><span class="sxs-lookup"><span data-stu-id="cadf5-106">Create a new synchronization template for a given application.</span></span>

## <a name="permissions"></a><span data-ttu-id="cadf5-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cadf5-107">Permissions</span></span>
<span data-ttu-id="cadf5-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cadf5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cadf5-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cadf5-110">Permission type</span></span>                        | <span data-ttu-id="cadf5-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cadf5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="cadf5-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cadf5-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="cadf5-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cadf5-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="cadf5-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cadf5-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="cadf5-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cadf5-115">Not supported.</span></span>|
|<span data-ttu-id="cadf5-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cadf5-116">Application</span></span>                            |<span data-ttu-id="cadf5-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cadf5-117">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="cadf5-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cadf5-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/synchronization/templates/
```

## <a name="request-headers"></a><span data-ttu-id="cadf5-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cadf5-119">Request headers</span></span>

| <span data-ttu-id="cadf5-120">名前</span><span class="sxs-lookup"><span data-stu-id="cadf5-120">Name</span></span>           | <span data-ttu-id="cadf5-121">型</span><span class="sxs-lookup"><span data-stu-id="cadf5-121">Type</span></span>    | <span data-ttu-id="cadf5-122">説明</span><span class="sxs-lookup"><span data-stu-id="cadf5-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="cadf5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cadf5-123">Authorization</span></span>  | <span data-ttu-id="cadf5-124">string</span><span class="sxs-lookup"><span data-stu-id="cadf5-124">string</span></span>  | <span data-ttu-id="cadf5-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="cadf5-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cadf5-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="cadf5-127">Request body</span></span>

<span data-ttu-id="cadf5-128">要求の本文には、 [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md)オブジェクトを作成するを指定します。</span><span class="sxs-lookup"><span data-stu-id="cadf5-128">In the request body, supply the [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object to be created.</span></span> <span data-ttu-id="cadf5-129">`id`、`applicationId`と`factoryTag`のプロパティが必要です。</span><span class="sxs-lookup"><span data-stu-id="cadf5-129">The `id`, `applicationId` and `factoryTag` properties are required.</span></span> <span data-ttu-id="cadf5-130">いいえ`schema`に、テンプレートを使用して既定のスキーマが関連付けられているが、`factoryTag`プロパティが使われます。</span><span class="sxs-lookup"><span data-stu-id="cadf5-130">When no `schema` is provided with the template, the default schema associated with the `factoryTag` property will be used.</span></span>

### <a name="response"></a><span data-ttu-id="cadf5-131">応答</span><span class="sxs-lookup"><span data-stu-id="cadf5-131">Response</span></span>

<span data-ttu-id="cadf5-132">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="cadf5-132">If successful, this method returns a `201 Created` response code and a [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="cadf5-133">例</span><span class="sxs-lookup"><span data-stu-id="cadf5-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="cadf5-134">要求</span><span class="sxs-lookup"><span data-stu-id="cadf5-134">Request</span></span>
<span data-ttu-id="cadf5-135">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cadf5-135">The following is an example of a request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="cadf5-136">応答</span><span class="sxs-lookup"><span data-stu-id="cadf5-136">Response</span></span>
<span data-ttu-id="cadf5-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cadf5-137">The following is an example of a response.</span></span>
><span data-ttu-id="cadf5-138">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="cadf5-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="cadf5-139">すべてのプロパティは、実際の呼び出しで返されます。</span><span class="sxs-lookup"><span data-stu-id="cadf5-139">All the properties will be returned in an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create synchronizationTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->