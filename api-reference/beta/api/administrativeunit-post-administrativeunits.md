---
title: AdministrativeUnit を作成します。
description: この API を使用すると、新しい administrativeUnit を作成します。
ms.openlocfilehash: ef69276f15cd8b8ec9d066ff707233ff1e219150
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067687"
---
# <a name="create-administrativeunit"></a><span data-ttu-id="9ba88-103">AdministrativeUnit を作成します。</span><span class="sxs-lookup"><span data-stu-id="9ba88-103">Create administrativeUnit</span></span>

> <span data-ttu-id="9ba88-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9ba88-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9ba88-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9ba88-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9ba88-106">この API を使用すると、新しい[administrativeUnit](../resources/administrativeunit.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="9ba88-106">Use this API to create a new [administrativeUnit](../resources/administrativeunit.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="9ba88-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9ba88-107">Permissions</span></span>
<span data-ttu-id="9ba88-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9ba88-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9ba88-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9ba88-110">Permission type</span></span>      | <span data-ttu-id="9ba88-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9ba88-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ba88-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9ba88-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9ba88-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9ba88-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9ba88-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9ba88-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ba88-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9ba88-115">Not supported.</span></span>    |
|<span data-ttu-id="9ba88-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9ba88-116">Application</span></span> | <span data-ttu-id="9ba88-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9ba88-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ba88-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9ba88-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits

```
## <a name="request-headers"></a><span data-ttu-id="9ba88-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9ba88-119">Request headers</span></span>
| <span data-ttu-id="9ba88-120">名前</span><span class="sxs-lookup"><span data-stu-id="9ba88-120">Name</span></span>      |<span data-ttu-id="9ba88-121">説明</span><span class="sxs-lookup"><span data-stu-id="9ba88-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9ba88-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ba88-122">Authorization</span></span>  | <span data-ttu-id="9ba88-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9ba88-p103">Bearer {token}. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="9ba88-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="9ba88-125">Request body</span></span>
<span data-ttu-id="9ba88-126">要求の本文には、 [administrativeUnit](../resources/administrativeunit.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="9ba88-126">In the request body, supply a JSON representation of [administrativeUnit](../resources/administrativeunit.md) object.</span></span>

<span data-ttu-id="9ba88-127">使用することができます**administrativeUnit**リソースでは、[拡張機能](/graph/extensibility-overview)をサポートするため、`POST`操作管理単位に作成時に実際のデータにカスタム プロパティを追加するとします。</span><span class="sxs-lookup"><span data-stu-id="9ba88-127">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the administrative unit while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="9ba88-128">応答</span><span class="sxs-lookup"><span data-stu-id="9ba88-128">Response</span></span>

<span data-ttu-id="9ba88-129">かどうかは成功すると、このメソッドを返します`201 Created`、応答の本体で応答コードと[administrativeUnit](../resources/administrativeunit.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="9ba88-129">If successful, this method returns `201 Created` response code and [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ba88-130">例</span><span class="sxs-lookup"><span data-stu-id="9ba88-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9ba88-131">要求</span><span class="sxs-lookup"><span data-stu-id="9ba88-131">Request</span></span>
<span data-ttu-id="9ba88-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9ba88-132">Here is an example of the request.</span></span>
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
<span data-ttu-id="9ba88-133">要求の本文には、 [administrativeUnit](../resources/administrativeunit.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="9ba88-133">In the request body, supply a JSON representation of [administrativeUnit](../resources/administrativeunit.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="9ba88-134">応答</span><span class="sxs-lookup"><span data-stu-id="9ba88-134">Response</span></span>
<span data-ttu-id="9ba88-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9ba88-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="9ba88-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="9ba88-138">See also</span></span>

- [<span data-ttu-id="9ba88-139">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="9ba88-139">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="9ba88-140">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="9ba88-140">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create administrativeUnit",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->