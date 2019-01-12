---
title: Get administrativeUnit
description: プロパティと administrativeUnit オブジェクトの関係を取得します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d91db6fa5365d9e0db7f655ecab75fa594b4ea8b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931945"
---
# <a name="get-administrativeunit"></a><span data-ttu-id="22067-103">Get administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="22067-103">Get administrativeUnit</span></span>

> <span data-ttu-id="22067-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="22067-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="22067-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="22067-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="22067-106">プロパティと[administrativeUnit](../resources/administrativeunit.md)オブジェクトの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="22067-106">Retrieve the properties and relationships of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>

<span data-ttu-id="22067-107">**AdministrativeUnit**リソースでは、[拡張機能](/graph/extensibility-overview)をサポートするため使用することも、 `GET` **administrativeUnit**インスタンスのカスタム プロパティと拡張機能のデータを取得する操作です。</span><span class="sxs-lookup"><span data-stu-id="22067-107">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **administrativeUnit** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="22067-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="22067-108">Permissions</span></span>
<span data-ttu-id="22067-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="22067-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="22067-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="22067-111">Permission type</span></span>      | <span data-ttu-id="22067-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="22067-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="22067-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="22067-113">Delegated (work or school account)</span></span> | <span data-ttu-id="22067-114">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="22067-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="22067-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="22067-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22067-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="22067-116">Not supported.</span></span>    |
|<span data-ttu-id="22067-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="22067-117">Application</span></span> | <span data-ttu-id="22067-118">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22067-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="22067-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="22067-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="22067-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="22067-120">Optional query parameters</span></span>
<span data-ttu-id="22067-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="22067-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="22067-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="22067-122">Request headers</span></span>
| <span data-ttu-id="22067-123">名前</span><span class="sxs-lookup"><span data-stu-id="22067-123">Name</span></span>      |<span data-ttu-id="22067-124">説明</span><span class="sxs-lookup"><span data-stu-id="22067-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="22067-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="22067-125">Authorization</span></span>  | <span data-ttu-id="22067-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="22067-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="22067-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="22067-128">Request body</span></span>
<span data-ttu-id="22067-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="22067-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22067-130">応答</span><span class="sxs-lookup"><span data-stu-id="22067-130">Response</span></span>

<span data-ttu-id="22067-131">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[administrativeUnit](../resources/administrativeunit.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="22067-131">If successful, this method returns a `200 OK` response code and [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="22067-132">例</span><span class="sxs-lookup"><span data-stu-id="22067-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="22067-133">要求</span><span class="sxs-lookup"><span data-stu-id="22067-133">Request</span></span>
<span data-ttu-id="22067-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="22067-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_administrativeunit"
}-->
```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}
```
##### <a name="response"></a><span data-ttu-id="22067-135">応答</span><span class="sxs-lookup"><span data-stu-id="22067-135">Response</span></span>
<span data-ttu-id="22067-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="22067-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="22067-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="22067-139">See also</span></span>

- [<span data-ttu-id="22067-140">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="22067-140">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="22067-141">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="22067-141">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get administrativeUnit",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
