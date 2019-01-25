---
title: SynchronizationTemplate を作成します。
description: 特定のアプリケーション用の新しい同期テンプレートを作成します。
localization_priority: Normal
ms.openlocfilehash: ce519b57766956b10d05b6b3745ca16f609b597c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509890"
---
# <a name="create-synchronizationtemplate"></a><span data-ttu-id="b452f-103">SynchronizationTemplate を作成します。</span><span class="sxs-lookup"><span data-stu-id="b452f-103">Create synchronizationTemplate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b452f-104">特定のアプリケーション用の新しい同期テンプレートを作成します。</span><span class="sxs-lookup"><span data-stu-id="b452f-104">Create a new synchronization template for a given application.</span></span>

## <a name="permissions"></a><span data-ttu-id="b452f-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b452f-105">Permissions</span></span>
<span data-ttu-id="b452f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b452f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b452f-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b452f-108">Permission type</span></span>                        | <span data-ttu-id="b452f-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b452f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b452f-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b452f-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="b452f-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b452f-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="b452f-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b452f-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="b452f-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b452f-113">Not supported.</span></span>|
|<span data-ttu-id="b452f-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b452f-114">Application</span></span>                            |<span data-ttu-id="b452f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b452f-115">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="b452f-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b452f-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/synchronization/templates/
```

## <a name="request-headers"></a><span data-ttu-id="b452f-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b452f-117">Request headers</span></span>

| <span data-ttu-id="b452f-118">名前</span><span class="sxs-lookup"><span data-stu-id="b452f-118">Name</span></span>           | <span data-ttu-id="b452f-119">型</span><span class="sxs-lookup"><span data-stu-id="b452f-119">Type</span></span>    | <span data-ttu-id="b452f-120">説明</span><span class="sxs-lookup"><span data-stu-id="b452f-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="b452f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b452f-121">Authorization</span></span>  | <span data-ttu-id="b452f-122">string</span><span class="sxs-lookup"><span data-stu-id="b452f-122">string</span></span>  | <span data-ttu-id="b452f-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b452f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b452f-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="b452f-125">Request body</span></span>

<span data-ttu-id="b452f-126">要求の本文には、 [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md)オブジェクトを作成するを指定します。</span><span class="sxs-lookup"><span data-stu-id="b452f-126">In the request body, supply the [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object to be created.</span></span> <span data-ttu-id="b452f-127">`id`、`applicationId`と`factoryTag`のプロパティが必要です。</span><span class="sxs-lookup"><span data-stu-id="b452f-127">The `id`, `applicationId` and `factoryTag` properties are required.</span></span> <span data-ttu-id="b452f-128">いいえ`schema`に、テンプレートを使用して既定のスキーマが関連付けられているが、`factoryTag`プロパティが使われます。</span><span class="sxs-lookup"><span data-stu-id="b452f-128">When no `schema` is provided with the template, the default schema associated with the `factoryTag` property will be used.</span></span>

### <a name="response"></a><span data-ttu-id="b452f-129">応答</span><span class="sxs-lookup"><span data-stu-id="b452f-129">Response</span></span>

<span data-ttu-id="b452f-130">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="b452f-130">If successful, this method returns a `201 Created` response code and a [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="b452f-131">例</span><span class="sxs-lookup"><span data-stu-id="b452f-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b452f-132">要求</span><span class="sxs-lookup"><span data-stu-id="b452f-132">Request</span></span>
<span data-ttu-id="b452f-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b452f-133">The following is an example of a request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="b452f-134">応答</span><span class="sxs-lookup"><span data-stu-id="b452f-134">Response</span></span>
<span data-ttu-id="b452f-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b452f-135">The following is an example of a response.</span></span>
><span data-ttu-id="b452f-136">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="b452f-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b452f-137">すべてのプロパティは、実際の呼び出しで返されます。</span><span class="sxs-lookup"><span data-stu-id="b452f-137">All the properties will be returned in an actual call.</span></span>
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
    "Error: /api-reference/beta/api/synchronization-synchronizationtemplate-post.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
