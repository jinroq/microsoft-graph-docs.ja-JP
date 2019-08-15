---
title: AdministrativeUnit を作成する
description: この API を使用して、新しい administrativeUnit を作成します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c8c9c5199a9c0e78aabf237a71f802e2f9fb4d73
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36408665"
---
# <a name="create-administrativeunit"></a><span data-ttu-id="7445f-103">AdministrativeUnit を作成する</span><span class="sxs-lookup"><span data-stu-id="7445f-103">Create administrativeUnit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7445f-104">この API を使用して、新しい[administrativeUnit](../resources/administrativeunit.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="7445f-104">Use this API to create a new [administrativeUnit](../resources/administrativeunit.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="7445f-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7445f-105">Permissions</span></span>
<span data-ttu-id="7445f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7445f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7445f-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7445f-108">Permission type</span></span>      | <span data-ttu-id="7445f-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7445f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7445f-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7445f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7445f-111">AdministrativeUnit。すべての Directory.accessasuser.all について</span><span class="sxs-lookup"><span data-stu-id="7445f-111">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7445f-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7445f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7445f-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7445f-113">Not supported.</span></span>    |
|<span data-ttu-id="7445f-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7445f-114">Application</span></span> | <span data-ttu-id="7445f-115">AdministrativeUnit</span><span class="sxs-lookup"><span data-stu-id="7445f-115">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7445f-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7445f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits

```
## <a name="request-headers"></a><span data-ttu-id="7445f-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7445f-117">Request headers</span></span>
| <span data-ttu-id="7445f-118">名前</span><span class="sxs-lookup"><span data-stu-id="7445f-118">Name</span></span>      |<span data-ttu-id="7445f-119">説明</span><span class="sxs-lookup"><span data-stu-id="7445f-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7445f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7445f-120">Authorization</span></span>  | <span data-ttu-id="7445f-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7445f-p102">Bearer {token}. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="7445f-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="7445f-123">Request body</span></span>
<span data-ttu-id="7445f-124">要求本文で、 [administrativeUnit](../resources/administrativeunit.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7445f-124">In the request body, supply a JSON representation of [administrativeUnit](../resources/administrativeunit.md) object.</span></span>

<span data-ttu-id="7445f-125">**AdministrativeUnit**リソースは[拡張機能](/graph/extensibility-overview)をサポートしているため`POST` 、操作を使用して、独自のデータを作成するときにカスタムプロパティを管理単位に追加することができます。</span><span class="sxs-lookup"><span data-stu-id="7445f-125">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the administrative unit while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="7445f-126">応答</span><span class="sxs-lookup"><span data-stu-id="7445f-126">Response</span></span>

<span data-ttu-id="7445f-127">成功した場合、この`201 Created`メソッドは応答コードと、応答本文で[administrativeUnit](../resources/administrativeunit.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7445f-127">If successful, this method returns `201 Created` response code and [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7445f-128">例</span><span class="sxs-lookup"><span data-stu-id="7445f-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7445f-129">要求</span><span class="sxs-lookup"><span data-stu-id="7445f-129">Request</span></span>
<span data-ttu-id="7445f-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7445f-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7445f-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="7445f-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_administrativeunit_from_administrativeunits"
}-->
```http
POST https://graph.microsoft.com/beta/administrativeUnits
Content-type: application/json
Content-length: 150

{
    "displayName": "Seattle District Technical Schools",
    "description": "Seattle district technical schools administration",
    "visibility": "true"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7445f-132">C#</span><span class="sxs-lookup"><span data-stu-id="7445f-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-administrativeunit-from-administrativeunits-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7445f-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7445f-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-administrativeunit-from-administrativeunits-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7445f-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="7445f-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-administrativeunit-from-administrativeunits-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="7445f-135">要求本文で、 [administrativeUnit](../resources/administrativeunit.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7445f-135">In the request body, supply a JSON representation of [administrativeUnit](../resources/administrativeunit.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="7445f-136">応答</span><span class="sxs-lookup"><span data-stu-id="7445f-136">Response</span></span>
<span data-ttu-id="7445f-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7445f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeUnit"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 172

{
  "administrativeUnit": {
    "displayName": "Seattle District Technical Schools",
    "description": "Seattle district technical schools administration",
    "visibility": "true",
    "id": "7a3dc8f3-b3a0-4164-9a99-ed36f3af039f"
  }
}
```

## <a name="see-also"></a><span data-ttu-id="7445f-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="7445f-140">See also</span></span>

- [<span data-ttu-id="7445f-141">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="7445f-141">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="7445f-142">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="7445f-142">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create administrativeUnit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
