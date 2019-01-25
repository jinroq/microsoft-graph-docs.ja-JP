---
title: AdministrativeUnit を作成します。
description: この API を使用すると、新しい administrativeUnit を作成します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 999f65db5c50ae012cf10242100523b2f6d0c4ce
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509687"
---
# <a name="create-administrativeunit"></a><span data-ttu-id="a9953-103">AdministrativeUnit を作成します。</span><span class="sxs-lookup"><span data-stu-id="a9953-103">Create administrativeUnit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9953-104">この API を使用すると、新しい[administrativeUnit](../resources/administrativeunit.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="a9953-104">Use this API to create a new [administrativeUnit](../resources/administrativeunit.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="a9953-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a9953-105">Permissions</span></span>
<span data-ttu-id="a9953-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a9953-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a9953-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a9953-108">Permission type</span></span>      | <span data-ttu-id="a9953-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a9953-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a9953-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a9953-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a9953-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a9953-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a9953-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a9953-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9953-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a9953-113">Not supported.</span></span>    |
|<span data-ttu-id="a9953-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a9953-114">Application</span></span> | <span data-ttu-id="a9953-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a9953-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a9953-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a9953-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits

```
## <a name="request-headers"></a><span data-ttu-id="a9953-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a9953-117">Request headers</span></span>
| <span data-ttu-id="a9953-118">名前</span><span class="sxs-lookup"><span data-stu-id="a9953-118">Name</span></span>      |<span data-ttu-id="a9953-119">説明</span><span class="sxs-lookup"><span data-stu-id="a9953-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a9953-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9953-120">Authorization</span></span>  | <span data-ttu-id="a9953-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a9953-p102">Bearer {token}. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="a9953-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="a9953-123">Request body</span></span>
<span data-ttu-id="a9953-124">要求の本文には、 [administrativeUnit](../resources/administrativeunit.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="a9953-124">In the request body, supply a JSON representation of [administrativeUnit](../resources/administrativeunit.md) object.</span></span>

<span data-ttu-id="a9953-125">使用することができます**administrativeUnit**リソースでは、[拡張機能](/graph/extensibility-overview)をサポートするため、`POST`操作管理単位に作成時に実際のデータにカスタム プロパティを追加するとします。</span><span class="sxs-lookup"><span data-stu-id="a9953-125">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the administrative unit while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="a9953-126">応答</span><span class="sxs-lookup"><span data-stu-id="a9953-126">Response</span></span>

<span data-ttu-id="a9953-127">かどうかは成功すると、このメソッドを返します`201 Created`、応答の本体で応答コードと[administrativeUnit](../resources/administrativeunit.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="a9953-127">If successful, this method returns `201 Created` response code and [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9953-128">例</span><span class="sxs-lookup"><span data-stu-id="a9953-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a9953-129">要求</span><span class="sxs-lookup"><span data-stu-id="a9953-129">Request</span></span>
<span data-ttu-id="a9953-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a9953-130">Here is an example of the request.</span></span>
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
<span data-ttu-id="a9953-131">要求の本文には、 [administrativeUnit](../resources/administrativeunit.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="a9953-131">In the request body, supply a JSON representation of [administrativeUnit](../resources/administrativeunit.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="a9953-132">応答</span><span class="sxs-lookup"><span data-stu-id="a9953-132">Response</span></span>
<span data-ttu-id="a9953-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a9953-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="a9953-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="a9953-136">See also</span></span>

- [<span data-ttu-id="a9953-137">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="a9953-137">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="a9953-138">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="a9953-138">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
    "Error: /api-reference/beta/api/administrativeunit-post-administrativeunits.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
