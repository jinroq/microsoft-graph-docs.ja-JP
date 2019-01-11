---
title: PrivilegedRoleAssignment を作成します。
description: この API を使用すると、新しい privilegedRoleAssignment を作成します。
localization_priority: Normal
ms.openlocfilehash: 7957aa964361890572de11c375753a49a3a9e9e6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852214"
---
# <a name="create-privilegedroleassignment"></a><span data-ttu-id="67e5b-103">PrivilegedRoleAssignment を作成します。</span><span class="sxs-lookup"><span data-stu-id="67e5b-103">Create privilegedRoleAssignment</span></span>

> <span data-ttu-id="67e5b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="67e5b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="67e5b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="67e5b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="67e5b-106">この API を使用すると、新しい[privilegedRoleAssignment](../resources/privilegedroleassignment.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="67e5b-106">Use this API to create a new  [privilegedRoleAssignment](../resources/privilegedroleassignment.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="67e5b-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="67e5b-107">Permissions</span></span>
<span data-ttu-id="67e5b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="67e5b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="67e5b-110">リクエスターでは、_ロールの権限を持つ管理者_のロールを持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="67e5b-110">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="67e5b-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="67e5b-111">Permission type</span></span>      | <span data-ttu-id="67e5b-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="67e5b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="67e5b-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="67e5b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="67e5b-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="67e5b-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="67e5b-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="67e5b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67e5b-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="67e5b-116">Not supported.</span></span>    |
|<span data-ttu-id="67e5b-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="67e5b-117">Application</span></span> | <span data-ttu-id="67e5b-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="67e5b-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="67e5b-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="67e5b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments
```
## <a name="request-headers"></a><span data-ttu-id="67e5b-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="67e5b-120">Request headers</span></span>
| <span data-ttu-id="67e5b-121">名前</span><span class="sxs-lookup"><span data-stu-id="67e5b-121">Name</span></span>       | <span data-ttu-id="67e5b-122">説明</span><span class="sxs-lookup"><span data-stu-id="67e5b-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="67e5b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="67e5b-123">Authorization</span></span>  | <span data-ttu-id="67e5b-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="67e5b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="67e5b-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="67e5b-126">Request body</span></span>
<span data-ttu-id="67e5b-127">要求の本文には、 [privilegedRoleAssignment](../resources/privilegedroleassignment.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="67e5b-127">In the request body, supply a JSON representation of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="67e5b-128">応答</span><span class="sxs-lookup"><span data-stu-id="67e5b-128">Response</span></span>

<span data-ttu-id="67e5b-129">かどうかは成功すると、このメソッドを返します`201 Created`、応答の本体で応答コードと[privilegedRoleAssignment](../resources/privilegedroleassignment.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="67e5b-129">If successful, this method returns `201 Created` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="67e5b-130">テナントの PIM を登録する必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="67e5b-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="67e5b-131">それ以外の場合、HTTP 403 アクセス不可の状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="67e5b-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="67e5b-132">例</span><span class="sxs-lookup"><span data-stu-id="67e5b-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="67e5b-133">要求</span><span class="sxs-lookup"><span data-stu-id="67e5b-133">Request</span></span>
<span data-ttu-id="67e5b-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="67e5b-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_privilegedroleassignment_from_privilegedroleassignments"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignments
Content-type: application/json
Content-length: 164

{
  "userId": "userId-value",
  "roleId": "roleId-value"
}
```
<span data-ttu-id="67e5b-135">要求の本文には、 [privilegedRoleAssignment](../resources/privilegedroleassignment.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="67e5b-135">In the request body, supply a JSON representation of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="67e5b-136">応答</span><span class="sxs-lookup"><span data-stu-id="67e5b-136">Response</span></span>
<span data-ttu-id="67e5b-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="67e5b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
} -->
```http
HTTP/1.1 201 Created
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
  "description": "Create privilegedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
