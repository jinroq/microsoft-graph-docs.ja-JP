---
title: 'privilegedRole: selfDeactivate'
description: リクエスターに割り当てられているロールを非アクティブ化します。
ms.openlocfilehash: f9f72a4f61dfd154829406eb535b394f8f137069
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067008"
---
# <a name="privilegedrole-selfdeactivate"></a><span data-ttu-id="ac9d0-103">privilegedRole: selfDeactivate</span><span class="sxs-lookup"><span data-stu-id="ac9d0-103">privilegedRole: selfDeactivate</span></span>

> <span data-ttu-id="ac9d0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ac9d0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ac9d0-106">リクエスターに割り当てられているロールを非アクティブ化します。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-106">Deactivate the role that is assigned to the requestor.</span></span>
## <a name="permissions"></a><span data-ttu-id="ac9d0-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ac9d0-107">Permissions</span></span>
<span data-ttu-id="ac9d0-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="ac9d0-110">リクエスターは呼び出すことができますのみ```selfDeactivate```彼に割り当てられているロールです。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-110">The requestor can only call ```selfDeactivate``` for the role that is assigned to him.</span></span> 

|<span data-ttu-id="ac9d0-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ac9d0-111">Permission type</span></span>      | <span data-ttu-id="ac9d0-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ac9d0-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ac9d0-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ac9d0-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ac9d0-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ac9d0-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ac9d0-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ac9d0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac9d0-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-116">Not supported.</span></span>    |
|<span data-ttu-id="ac9d0-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ac9d0-117">Application</span></span> | <span data-ttu-id="ac9d0-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ac9d0-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ac9d0-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoles/{id}/selfDeactivate
```

<span data-ttu-id="ac9d0-120">注意してください``<id>``は、ターゲットのロールの id。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-120">Note that ``<id>`` is the target role id.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ac9d0-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ac9d0-121">Request headers</span></span>
| <span data-ttu-id="ac9d0-122">名前</span><span class="sxs-lookup"><span data-stu-id="ac9d0-122">Name</span></span>       | <span data-ttu-id="ac9d0-123">説明</span><span class="sxs-lookup"><span data-stu-id="ac9d0-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ac9d0-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac9d0-124">Authorization</span></span>  | <span data-ttu-id="ac9d0-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ac9d0-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="ac9d0-127">Request body</span></span>
<span data-ttu-id="ac9d0-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ac9d0-129">応答</span><span class="sxs-lookup"><span data-stu-id="ac9d0-129">Response</span></span>

<span data-ttu-id="ac9d0-130">かどうかは成功すると、このメソッドを返します`200 OK`、応答の本体で応答コードと[privilegedRoleAssignment](../resources/privilegedroleassignment.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-130">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="ac9d0-131">テナントの PIM を登録する必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-131">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="ac9d0-132">それ以外の場合、HTTP 403 アクセス不可の状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-132">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="ac9d0-133">例</span><span class="sxs-lookup"><span data-stu-id="ac9d0-133">Example</span></span>
<span data-ttu-id="ac9d0-134">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-134">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ac9d0-135">要求</span><span class="sxs-lookup"><span data-stu-id="ac9d0-135">Request</span></span>
<span data-ttu-id="ac9d0-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedrole_selfdeactivate"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoles/{id}/selfDeactivate
```

##### <a name="response"></a><span data-ttu-id="ac9d0-137">応答</span><span class="sxs-lookup"><span data-stu-id="ac9d0-137">Response</span></span>
<span data-ttu-id="ac9d0-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "privilegedRole: selfDeactivate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->