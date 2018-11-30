---
title: PrivilegedRoleAssignment を取得します。
description: プロパティと privilegedRoleAssignment オブジェクトの関係を取得します。
ms.openlocfilehash: ad8815842698be0ef6a3eef37dc3e26f7dc11dbd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068703"
---
# <a name="get-privilegedroleassignment"></a><span data-ttu-id="1589b-103">PrivilegedRoleAssignment を取得します。</span><span class="sxs-lookup"><span data-stu-id="1589b-103">Get privilegedRoleAssignment</span></span>

> <span data-ttu-id="1589b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1589b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1589b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1589b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1589b-106">プロパティと privilegedRoleAssignment オブジェクトの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="1589b-106">Retrieve the properties and relationships of privilegedRoleAssignment object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1589b-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1589b-107">Permissions</span></span>
<span data-ttu-id="1589b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1589b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="1589b-110">リクエスターは、次のロールのいずれかを持つ必要があります:_ロールの権限を持つ管理者_、_グローバル管理者_、_セキュリティ管理者_、または_セキュリティのリーダー_です。</span><span class="sxs-lookup"><span data-stu-id="1589b-110">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="1589b-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1589b-111">Permission type</span></span>      | <span data-ttu-id="1589b-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1589b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1589b-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1589b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="1589b-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1589b-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1589b-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1589b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1589b-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1589b-116">Not supported.</span></span>    |
|<span data-ttu-id="1589b-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1589b-117">Application</span></span> | <span data-ttu-id="1589b-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1589b-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1589b-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1589b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1589b-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="1589b-120">Optional query parameters</span></span>
<span data-ttu-id="1589b-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="1589b-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1589b-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1589b-122">Request headers</span></span>
| <span data-ttu-id="1589b-123">名前</span><span class="sxs-lookup"><span data-stu-id="1589b-123">Name</span></span>      |<span data-ttu-id="1589b-124">説明</span><span class="sxs-lookup"><span data-stu-id="1589b-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1589b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="1589b-125">Authorization</span></span>  | <span data-ttu-id="1589b-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1589b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1589b-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="1589b-128">Request body</span></span>
<span data-ttu-id="1589b-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1589b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1589b-130">応答</span><span class="sxs-lookup"><span data-stu-id="1589b-130">Response</span></span>

<span data-ttu-id="1589b-131">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[privilegedRoleAssignment](../resources/privilegedroleassignment.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="1589b-131">If successful, this method returns a `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="1589b-132">テナントの PIM を登録する必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="1589b-132">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="1589b-133">それ以外の場合、HTTP 403 アクセス不可の状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="1589b-133">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="1589b-134">例</span><span class="sxs-lookup"><span data-stu-id="1589b-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1589b-135">要求</span><span class="sxs-lookup"><span data-stu-id="1589b-135">Request</span></span>
<span data-ttu-id="1589b-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1589b-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignment"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}
```
##### <a name="response"></a><span data-ttu-id="1589b-137">応答</span><span class="sxs-lookup"><span data-stu-id="1589b-137">Response</span></span>
<span data-ttu-id="1589b-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1589b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 184

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "isElevated": true,
  "expirationDateTime": "2016-10-19T10:37:00Z",
  "resultMessage": "resultMessage-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get privilegedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->