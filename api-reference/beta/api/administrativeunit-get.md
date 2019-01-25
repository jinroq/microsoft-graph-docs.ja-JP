---
title: Get administrativeUnit
description: プロパティと administrativeUnit オブジェクトの関係を取得します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 588d116d546503fa8db6c8ba56c5d0e328a10b8a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521608"
---
# <a name="get-administrativeunit"></a><span data-ttu-id="4af72-103">Get administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="4af72-103">Get administrativeUnit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4af72-104">プロパティと[administrativeUnit](../resources/administrativeunit.md)オブジェクトの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="4af72-104">Retrieve the properties and relationships of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>

<span data-ttu-id="4af72-105">**AdministrativeUnit**リソースでは、[拡張機能](/graph/extensibility-overview)をサポートするため使用することも、 `GET` **administrativeUnit**インスタンスのカスタム プロパティと拡張機能のデータを取得する操作です。</span><span class="sxs-lookup"><span data-stu-id="4af72-105">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **administrativeUnit** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="4af72-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4af72-106">Permissions</span></span>
<span data-ttu-id="4af72-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4af72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4af72-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4af72-109">Permission type</span></span>      | <span data-ttu-id="4af72-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4af72-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4af72-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4af72-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4af72-112">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4af72-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4af72-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4af72-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4af72-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4af72-114">Not supported.</span></span>    |
|<span data-ttu-id="4af72-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4af72-115">Application</span></span> | <span data-ttu-id="4af72-116">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4af72-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4af72-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4af72-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4af72-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="4af72-118">Optional query parameters</span></span>
<span data-ttu-id="4af72-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="4af72-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4af72-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4af72-120">Request headers</span></span>
| <span data-ttu-id="4af72-121">名前</span><span class="sxs-lookup"><span data-stu-id="4af72-121">Name</span></span>      |<span data-ttu-id="4af72-122">説明</span><span class="sxs-lookup"><span data-stu-id="4af72-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4af72-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4af72-123">Authorization</span></span>  | <span data-ttu-id="4af72-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4af72-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4af72-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="4af72-126">Request body</span></span>
<span data-ttu-id="4af72-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="4af72-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4af72-128">応答</span><span class="sxs-lookup"><span data-stu-id="4af72-128">Response</span></span>

<span data-ttu-id="4af72-129">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[administrativeUnit](../resources/administrativeunit.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="4af72-129">If successful, this method returns a `200 OK` response code and [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4af72-130">例</span><span class="sxs-lookup"><span data-stu-id="4af72-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4af72-131">要求</span><span class="sxs-lookup"><span data-stu-id="4af72-131">Request</span></span>
<span data-ttu-id="4af72-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4af72-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_administrativeunit"
}-->
```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}
```
##### <a name="response"></a><span data-ttu-id="4af72-133">応答</span><span class="sxs-lookup"><span data-stu-id="4af72-133">Response</span></span>
<span data-ttu-id="4af72-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4af72-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeUnit"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 134

{
  "displayName": "displayName-value",
  "description": "description-value",
  "visibility": "visibility-value",
  "id": "id-value"
}
```

## <a name="see-also"></a><span data-ttu-id="4af72-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="4af72-137">See also</span></span>

- [<span data-ttu-id="4af72-138">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="4af72-138">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="4af72-139">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="4af72-139">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get administrativeUnit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/administrativeunit-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
