---
title: リストの割り当て
description: ロールに関連付けられている privilegedRoleAssignment オブジェクトのリストを取得します。 各 privilegedRoleAssignment は、ユーザーに役割の割り当てを表します。
localization_priority: Normal
ms.openlocfilehash: f7dd2b94c5d3ac49a6a8c9183373801f76e27964
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508273"
---
# <a name="list-assignments"></a><span data-ttu-id="04ed2-104">リストの割り当て</span><span class="sxs-lookup"><span data-stu-id="04ed2-104">List assignments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04ed2-105">ロールに関連付けられている[privilegedRoleAssignment](../resources/privilegedroleassignment.md)オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="04ed2-105">Retrieve a list of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects that are associated with the role.</span></span> <span data-ttu-id="04ed2-106">各[privilegedRoleAssignment](../resources/privilegedroleassignment.md)は、ユーザーに役割の割り当てを表します。</span><span class="sxs-lookup"><span data-stu-id="04ed2-106">Each [privilegedRoleAssignment](../resources/privilegedroleassignment.md) represents a role assignment to a user.</span></span>
## <a name="permissions"></a><span data-ttu-id="04ed2-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="04ed2-107">Permissions</span></span>
<span data-ttu-id="04ed2-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="04ed2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="04ed2-110">リクエスターは、次のロールのいずれかを持つ必要があります:_ロールの権限を持つ管理者_、_グローバル管理者_、_セキュリティ管理者_、または_セキュリティのリーダー_です。</span><span class="sxs-lookup"><span data-stu-id="04ed2-110">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span>
 

|<span data-ttu-id="04ed2-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="04ed2-111">Permission type</span></span>      | <span data-ttu-id="04ed2-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="04ed2-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="04ed2-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="04ed2-113">Delegated (work or school account)</span></span> | <span data-ttu-id="04ed2-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="04ed2-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="04ed2-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="04ed2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04ed2-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="04ed2-116">Not supported.</span></span>    |
|<span data-ttu-id="04ed2-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="04ed2-117">Application</span></span> | <span data-ttu-id="04ed2-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="04ed2-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="04ed2-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="04ed2-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}/assignments
```

<span data-ttu-id="04ed2-120">注意してください``<id>``は、ターゲットのロールの id。</span><span class="sxs-lookup"><span data-stu-id="04ed2-120">Note that ``<id>`` is the target role id.</span></span>
## <a name="optional-query-parameters"></a><span data-ttu-id="04ed2-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="04ed2-121">Optional query parameters</span></span>
<span data-ttu-id="04ed2-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="04ed2-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="04ed2-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="04ed2-123">Request headers</span></span>
| <span data-ttu-id="04ed2-124">名前</span><span class="sxs-lookup"><span data-stu-id="04ed2-124">Name</span></span>      |<span data-ttu-id="04ed2-125">説明</span><span class="sxs-lookup"><span data-stu-id="04ed2-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="04ed2-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="04ed2-126">Authorization</span></span>  | <span data-ttu-id="04ed2-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="04ed2-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="04ed2-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="04ed2-129">Request body</span></span>
<span data-ttu-id="04ed2-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="04ed2-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="04ed2-131">応答</span><span class="sxs-lookup"><span data-stu-id="04ed2-131">Response</span></span>

<span data-ttu-id="04ed2-132">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[privilegedRoleAssignment](../resources/privilegedroleassignment.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="04ed2-132">If successful, this method returns a `200 OK` response code and collection of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects in the response body.</span></span>

<span data-ttu-id="04ed2-133">テナントの PIM を登録する必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="04ed2-133">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="04ed2-134">それ以外の場合、HTTP 403 アクセス不可の状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="04ed2-134">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="04ed2-135">例</span><span class="sxs-lookup"><span data-stu-id="04ed2-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="04ed2-136">要求</span><span class="sxs-lookup"><span data-stu-id="04ed2-136">Request</span></span>
<span data-ttu-id="04ed2-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="04ed2-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_assignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/assignments
```
##### <a name="response"></a><span data-ttu-id="04ed2-138">応答</span><span class="sxs-lookup"><span data-stu-id="04ed2-138">Response</span></span>
<span data-ttu-id="04ed2-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="04ed2-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List assignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedrole-list-assignments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
