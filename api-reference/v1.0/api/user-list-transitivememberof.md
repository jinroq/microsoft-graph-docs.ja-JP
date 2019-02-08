---
title: ボックスの一覧ユーザーの推移的な memberOf
description: グループ、ユーザーがのメンバーであるディレクトリの役割を取得します。 この API 要求は、推移的なもすべてのグループの入れ子にされたメンバーを返します。
author: anchanda
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 824e037d5f1e02051d315860ad3faa1254c25967
ms.sourcegitcommit: d6209114cbbe8072e3ecf7eba23819ae5ace7db5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/01/2019
ms.locfileid: "29694483"
---
# <a name="list-user-transitive-memberof"></a><span data-ttu-id="a1a27-104">ボックスの一覧ユーザーの推移的な memberOf</span><span class="sxs-lookup"><span data-stu-id="a1a27-104">List user transitive memberOf</span></span>

<span data-ttu-id="a1a27-105">グループ、ユーザーがのメンバーであるディレクトリの役割を取得します。</span><span class="sxs-lookup"><span data-stu-id="a1a27-105">Get groups, directory roles that the user is a member of.</span></span> <span data-ttu-id="a1a27-106">この API 要求は、推移的なもすべてのグループの入れ子にされたメンバーを返します。</span><span class="sxs-lookup"><span data-stu-id="a1a27-106">This API request is transitive, and will also return all groups the user is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="a1a27-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a1a27-107">Permissions</span></span>

<span data-ttu-id="a1a27-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a1a27-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1a27-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a1a27-110">Permission type</span></span>      | <span data-ttu-id="a1a27-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a1a27-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a1a27-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a1a27-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a1a27-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a1a27-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a1a27-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a1a27-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1a27-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a1a27-115">Not supported.</span></span>    |
|<span data-ttu-id="a1a27-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a1a27-116">Application</span></span> | <span data-ttu-id="a1a27-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1a27-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a1a27-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a1a27-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id | userPrincipalName}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a1a27-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="a1a27-119">Optional query parameters</span></span>

<span data-ttu-id="a1a27-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="a1a27-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a1a27-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a1a27-121">Request headers</span></span>

| <span data-ttu-id="a1a27-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a1a27-122">Header</span></span>       | <span data-ttu-id="a1a27-123">値</span><span class="sxs-lookup"><span data-stu-id="a1a27-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a1a27-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1a27-124">Authorization</span></span>  | <span data-ttu-id="a1a27-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a1a27-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a1a27-127">承諾</span><span class="sxs-lookup"><span data-stu-id="a1a27-127">Accept</span></span>  | <span data-ttu-id="a1a27-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a1a27-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1a27-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="a1a27-129">Request body</span></span>

<span data-ttu-id="a1a27-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a1a27-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1a27-131">応答</span><span class="sxs-lookup"><span data-stu-id="a1a27-131">Response</span></span>

<span data-ttu-id="a1a27-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="a1a27-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1a27-133">例</span><span class="sxs-lookup"><span data-stu-id="a1a27-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1a27-134">要求</span><span class="sxs-lookup"><span data-stu-id="a1a27-134">Request</span></span>

<span data-ttu-id="a1a27-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a1a27-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_transitivememberof"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/transitiveMemberOf
```

### <a name="response"></a><span data-ttu-id="a1a27-136">応答</span><span class="sxs-lookup"><span data-stu-id="a1a27-136">Response</span></span>

<span data-ttu-id="a1a27-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a1a27-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List transitiveMsemberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->