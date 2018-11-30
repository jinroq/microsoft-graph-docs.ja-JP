---
title: リストの割り当て
description: ロールに関連付けられている privilegedRoleAssignment オブジェクトのリストを取得します。 各 privilegedRoleAssignment は、ユーザーに役割の割り当てを表します。
ms.openlocfilehash: 52cc720381baa6b7c82fe3b5c88d469081da3b81
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071199"
---
# <a name="list-assignments"></a><span data-ttu-id="8cbf9-104">リストの割り当て</span><span class="sxs-lookup"><span data-stu-id="8cbf9-104">List assignments</span></span>

> <span data-ttu-id="8cbf9-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8cbf9-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8cbf9-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8cbf9-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8cbf9-107">ロールに関連付けられている[privilegedRoleAssignment](../resources/privilegedroleassignment.md)オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="8cbf9-107">Retrieve a list of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects that are associated with the role.</span></span> <span data-ttu-id="8cbf9-108">各[privilegedRoleAssignment](../resources/privilegedroleassignment.md)は、ユーザーに役割の割り当てを表します。</span><span class="sxs-lookup"><span data-stu-id="8cbf9-108">Each [privilegedRoleAssignment](../resources/privilegedroleassignment.md) represents a role assignment to a user.</span></span>
## <a name="permissions"></a><span data-ttu-id="8cbf9-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8cbf9-109">Permissions</span></span>
<span data-ttu-id="8cbf9-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8cbf9-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="8cbf9-112">リクエスターは、次のロールのいずれかを持つ必要があります:_ロールの権限を持つ管理者_、_グローバル管理者_、_セキュリティ管理者_、または_セキュリティのリーダー_です。</span><span class="sxs-lookup"><span data-stu-id="8cbf9-112">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span>
 

|<span data-ttu-id="8cbf9-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8cbf9-113">Permission type</span></span>      | <span data-ttu-id="8cbf9-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8cbf9-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8cbf9-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8cbf9-115">Delegated (work or school account)</span></span> | <span data-ttu-id="8cbf9-116">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8cbf9-116">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8cbf9-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8cbf9-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8cbf9-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8cbf9-118">Not supported.</span></span>    |
|<span data-ttu-id="8cbf9-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8cbf9-119">Application</span></span> | <span data-ttu-id="8cbf9-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8cbf9-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8cbf9-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8cbf9-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}/assignments
```

<span data-ttu-id="8cbf9-122">注意してください``<id>``は、ターゲットのロールの id。</span><span class="sxs-lookup"><span data-stu-id="8cbf9-122">Note that ``<id>`` is the target role id.</span></span>
## <a name="optional-query-parameters"></a><span data-ttu-id="8cbf9-123">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="8cbf9-123">Optional query parameters</span></span>
<span data-ttu-id="8cbf9-124">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="8cbf9-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8cbf9-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8cbf9-125">Request headers</span></span>
| <span data-ttu-id="8cbf9-126">名前</span><span class="sxs-lookup"><span data-stu-id="8cbf9-126">Name</span></span>      |<span data-ttu-id="8cbf9-127">説明</span><span class="sxs-lookup"><span data-stu-id="8cbf9-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8cbf9-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="8cbf9-128">Authorization</span></span>  | <span data-ttu-id="8cbf9-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8cbf9-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8cbf9-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="8cbf9-131">Request body</span></span>
<span data-ttu-id="8cbf9-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8cbf9-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8cbf9-133">応答</span><span class="sxs-lookup"><span data-stu-id="8cbf9-133">Response</span></span>

<span data-ttu-id="8cbf9-134">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[privilegedRoleAssignment](../resources/privilegedroleassignment.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="8cbf9-134">If successful, this method returns a `200 OK` response code and collection of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects in the response body.</span></span>

<span data-ttu-id="8cbf9-135">テナントの PIM を登録する必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="8cbf9-135">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="8cbf9-136">それ以外の場合、HTTP 403 アクセス不可の状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="8cbf9-136">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="8cbf9-137">例</span><span class="sxs-lookup"><span data-stu-id="8cbf9-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8cbf9-138">要求</span><span class="sxs-lookup"><span data-stu-id="8cbf9-138">Request</span></span>
<span data-ttu-id="8cbf9-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8cbf9-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_assignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/assignments
```
##### <a name="response"></a><span data-ttu-id="8cbf9-140">応答</span><span class="sxs-lookup"><span data-stu-id="8cbf9-140">Response</span></span>
<span data-ttu-id="8cbf9-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8cbf9-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "value": [
    {
      "id": "id-value",
      "userId": "userId-value",
      "roleId": "roleId-value",
      "isElevated": true,
      "expirationDateTime": "2016-10-19T10:37:00Z",
      "resultMessage": "resultMessage-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List assignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
