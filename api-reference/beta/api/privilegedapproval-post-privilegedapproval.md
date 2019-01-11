---
title: PrivilegedApproval を作成します。
description: この API を使用すると、新しい privilegedApproval を作成します。
localization_priority: Normal
ms.openlocfilehash: 806a48ff66ad20dfdda05b0029975913c6dde28e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872080"
---
# <a name="create-privilegedapproval"></a><span data-ttu-id="c78a4-103">PrivilegedApproval を作成します。</span><span class="sxs-lookup"><span data-stu-id="c78a4-103">Create privilegedApproval</span></span>

> <span data-ttu-id="c78a4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c78a4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c78a4-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c78a4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c78a4-106">この API を使用すると、新しい privilegedApproval を作成します。</span><span class="sxs-lookup"><span data-stu-id="c78a4-106">Use this API to create a new privilegedApproval.</span></span>
## <a name="permissions"></a><span data-ttu-id="c78a4-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c78a4-107">Permissions</span></span>
<span data-ttu-id="c78a4-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c78a4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c78a4-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c78a4-110">Permission type</span></span>      | <span data-ttu-id="c78a4-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c78a4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c78a4-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c78a4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c78a4-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c78a4-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c78a4-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c78a4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c78a4-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c78a4-115">Not supported.</span></span>    |
|<span data-ttu-id="c78a4-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c78a4-116">Application</span></span> | <span data-ttu-id="c78a4-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c78a4-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c78a4-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c78a4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedApproval

```
## <a name="request-headers"></a><span data-ttu-id="c78a4-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c78a4-119">Request headers</span></span>
| <span data-ttu-id="c78a4-120">名前</span><span class="sxs-lookup"><span data-stu-id="c78a4-120">Name</span></span>       | <span data-ttu-id="c78a4-121">説明</span><span class="sxs-lookup"><span data-stu-id="c78a4-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c78a4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c78a4-122">Authorization</span></span>  | <span data-ttu-id="c78a4-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c78a4-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c78a4-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="c78a4-125">Request body</span></span>
<span data-ttu-id="c78a4-126">要求の本文には、 [privilegedApproval](../resources/privilegedapproval.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="c78a4-126">In the request body, supply a JSON representation of [privilegedApproval](../resources/privilegedapproval.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c78a4-127">応答</span><span class="sxs-lookup"><span data-stu-id="c78a4-127">Response</span></span>

<span data-ttu-id="c78a4-128">かどうかは成功すると、このメソッドを返します`201 Created`、応答の本体で応答コードと[privilegedApproval](../resources/privilegedapproval.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="c78a4-128">If successful, this method returns `201 Created` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="c78a4-129">テナントの PIM を登録する必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="c78a4-129">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="c78a4-130">それ以外の場合、HTTP 403 アクセス不可の状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="c78a4-130">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="c78a4-131">例</span><span class="sxs-lookup"><span data-stu-id="c78a4-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c78a4-132">要求</span><span class="sxs-lookup"><span data-stu-id="c78a4-132">Request</span></span>
<span data-ttu-id="c78a4-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c78a4-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_privilegedapproval_from_privilegedapproval"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedApproval
Content-type: application/json
Content-length: 180

{
  "userId": "userId-value",
  "roleId": "roleId-value",
  "approvalType": "approvalType-value",
  "approvalState": "approvalState-value",
  "approvalDuration": "datetime-value"
}
```
<span data-ttu-id="c78a4-134">要求の本文には、 [privilegedApproval](../resources/privilegedapproval.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="c78a4-134">In the request body, supply a JSON representation of [privilegedApproval](../resources/privilegedapproval.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="c78a4-135">応答</span><span class="sxs-lookup"><span data-stu-id="c78a4-135">Response</span></span>
<span data-ttu-id="c78a4-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c78a4-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 200

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "approvalType": "approvalType-value",
  "approvalState": "approvalState-value",
  "approvalDuration": "datetime-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create privilegedApproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
