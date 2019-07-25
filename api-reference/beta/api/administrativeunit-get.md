---
title: AdministrativeUnit を取得する
description: AdministrativeUnit オブジェクトのプロパティとリレーションシップを取得します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a583e7d826e1fb57a11c0a11fc899360ea64252d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855790"
---
# <a name="get-administrativeunit"></a><span data-ttu-id="20890-103">AdministrativeUnit を取得する</span><span class="sxs-lookup"><span data-stu-id="20890-103">Get administrativeUnit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20890-104">[AdministrativeUnit](../resources/administrativeunit.md)オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="20890-104">Retrieve the properties and relationships of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>

<span data-ttu-id="20890-105">**AdministrativeUnit**リソースは[拡張機能](/graph/extensibility-overview)をサポートしているため、 `GET`この操作を使用して、 **administrativeUnit**インスタンスでカスタムプロパティと拡張機能データを取得することもできます。</span><span class="sxs-lookup"><span data-stu-id="20890-105">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **administrativeUnit** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="20890-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="20890-106">Permissions</span></span>
<span data-ttu-id="20890-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="20890-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="20890-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="20890-109">Permission type</span></span>      | <span data-ttu-id="20890-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="20890-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="20890-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="20890-111">Delegated (work or school account)</span></span> | <span data-ttu-id="20890-112">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="20890-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="20890-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="20890-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20890-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="20890-114">Not supported.</span></span>    |
|<span data-ttu-id="20890-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="20890-115">Application</span></span> | <span data-ttu-id="20890-116">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20890-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="20890-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="20890-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="20890-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="20890-118">Optional query parameters</span></span>
<span data-ttu-id="20890-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="20890-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="20890-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="20890-120">Request headers</span></span>
| <span data-ttu-id="20890-121">名前</span><span class="sxs-lookup"><span data-stu-id="20890-121">Name</span></span>      |<span data-ttu-id="20890-122">説明</span><span class="sxs-lookup"><span data-stu-id="20890-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="20890-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="20890-123">Authorization</span></span>  | <span data-ttu-id="20890-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="20890-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="20890-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="20890-126">Request body</span></span>
<span data-ttu-id="20890-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="20890-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="20890-128">応答</span><span class="sxs-lookup"><span data-stu-id="20890-128">Response</span></span>

<span data-ttu-id="20890-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[administrativeUnit](../resources/administrativeunit.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="20890-129">If successful, this method returns a `200 OK` response code and [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="20890-130">例</span><span class="sxs-lookup"><span data-stu-id="20890-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="20890-131">要求</span><span class="sxs-lookup"><span data-stu-id="20890-131">Request</span></span>
<span data-ttu-id="20890-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="20890-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="20890-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="20890-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_administrativeunit"
}-->
```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="20890-134">C#</span><span class="sxs-lookup"><span data-stu-id="20890-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="20890-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="20890-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="20890-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="20890-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="20890-137">Java</span><span class="sxs-lookup"><span data-stu-id="20890-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-administrativeunit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="20890-138">応答</span><span class="sxs-lookup"><span data-stu-id="20890-138">Response</span></span>
<span data-ttu-id="20890-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="20890-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="20890-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="20890-142">See also</span></span>

- [<span data-ttu-id="20890-143">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="20890-143">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="20890-144">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="20890-144">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
  ]
}
-->
