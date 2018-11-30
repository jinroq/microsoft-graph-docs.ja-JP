---
title: リスト privilegedRoles
description: PrivilegedRole オブジェクトのリストを取得します。
ms.openlocfilehash: 6800096f36e1fb8237216cf9ea708b3b20ff21ae
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069268"
---
# <a name="list-privilegedroles"></a><span data-ttu-id="c8387-103">リスト privilegedRoles</span><span class="sxs-lookup"><span data-stu-id="c8387-103">List privilegedRoles</span></span>

> <span data-ttu-id="c8387-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c8387-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c8387-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8387-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c8387-106">[PrivilegedRole](../resources/privilegedrole.md)オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="c8387-106">Retrieve a list of [privilegedRole](../resources/privilegedrole.md) objects.</span></span>

<span data-ttu-id="c8387-107">クエリの結果をフィルターするには、標準の OData を使用して、 ``$filter`` 、Uri で表現します。</span><span class="sxs-lookup"><span data-stu-id="c8387-107">To filter the results from the query, use the standard OData ``$filter`` expressions in the URIs.</span></span>
## <a name="permissions"></a><span data-ttu-id="c8387-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c8387-108">Permissions</span></span>
<span data-ttu-id="c8387-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c8387-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="c8387-111">リクエスターは、次のロールのいずれかを持つ必要があります:_ロールの権限を持つ管理者_、_グローバル管理者_、_セキュリティ管理者_、または_セキュリティのリーダー_です。</span><span class="sxs-lookup"><span data-stu-id="c8387-111">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span>
 

|<span data-ttu-id="c8387-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c8387-112">Permission type</span></span>      | <span data-ttu-id="c8387-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c8387-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c8387-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c8387-114">Delegated (work or school account)</span></span> | <span data-ttu-id="c8387-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c8387-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c8387-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c8387-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8387-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8387-117">Not supported.</span></span>    |
|<span data-ttu-id="c8387-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c8387-118">Application</span></span> | <span data-ttu-id="c8387-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8387-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c8387-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c8387-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c8387-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c8387-121">Optional query parameters</span></span>
<span data-ttu-id="c8387-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c8387-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c8387-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c8387-123">Request headers</span></span>
| <span data-ttu-id="c8387-124">名前</span><span class="sxs-lookup"><span data-stu-id="c8387-124">Name</span></span>      |<span data-ttu-id="c8387-125">説明</span><span class="sxs-lookup"><span data-stu-id="c8387-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c8387-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8387-126">Authorization</span></span>  | <span data-ttu-id="c8387-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c8387-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c8387-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="c8387-129">Request body</span></span>
<span data-ttu-id="c8387-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c8387-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8387-131">応答</span><span class="sxs-lookup"><span data-stu-id="c8387-131">Response</span></span>

<span data-ttu-id="c8387-132">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[privilegedRole](../resources/privilegedrole.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="c8387-132">If successful, this method returns a `200 OK` response code and collection of [privilegedRole](../resources/privilegedrole.md) objects in the response body.</span></span>

<span data-ttu-id="c8387-133">テナントの PIM を登録する必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="c8387-133">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="c8387-134">それ以外の場合、HTTP 403 アクセス不可の状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="c8387-134">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="c8387-135">例</span><span class="sxs-lookup"><span data-stu-id="c8387-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c8387-136">要求</span><span class="sxs-lookup"><span data-stu-id="c8387-136">Request</span></span>
<span data-ttu-id="c8387-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c8387-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroles"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles
```
##### <a name="response"></a><span data-ttu-id="c8387-138">応答</span><span class="sxs-lookup"><span data-stu-id="c8387-138">Response</span></span>
<span data-ttu-id="c8387-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c8387-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRole",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 83

{
  "value": [
    {
      "id": "id-value",
      "name": "name-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List privilegedRoles",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->