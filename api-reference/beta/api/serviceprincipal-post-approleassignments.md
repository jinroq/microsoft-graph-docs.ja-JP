---
title: AppRoleAssignment を作成します。
description: この API を使用すると、新しい appRoleAssignment を作成します。
localization_priority: Normal
ms.openlocfilehash: ce498312f294ff11b97f12b136a6f48ebb4d3791
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886983"
---
# <a name="create-approleassignment"></a><span data-ttu-id="973a1-103">AppRoleAssignment を作成します。</span><span class="sxs-lookup"><span data-stu-id="973a1-103">Create appRoleAssignment</span></span>

> <span data-ttu-id="973a1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="973a1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="973a1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="973a1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="973a1-106">この API を使用すると、新しい appRoleAssignment を作成します。</span><span class="sxs-lookup"><span data-stu-id="973a1-106">Use this API to create a new appRoleAssignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="973a1-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="973a1-107">Permissions</span></span>
<span data-ttu-id="973a1-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="973a1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="973a1-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="973a1-110">Permission type</span></span>      | <span data-ttu-id="973a1-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="973a1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="973a1-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="973a1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="973a1-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="973a1-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="973a1-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="973a1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="973a1-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="973a1-115">Not supported.</span></span>    |
|<span data-ttu-id="973a1-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="973a1-116">Application</span></span> | <span data-ttu-id="973a1-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="973a1-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="973a1-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="973a1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/appRoleAssignments

```
## <a name="request-headers"></a><span data-ttu-id="973a1-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="973a1-119">Request headers</span></span>
| <span data-ttu-id="973a1-120">名前</span><span class="sxs-lookup"><span data-stu-id="973a1-120">Name</span></span>       | <span data-ttu-id="973a1-121">種類</span><span class="sxs-lookup"><span data-stu-id="973a1-121">Type</span></span> | <span data-ttu-id="973a1-122">説明</span><span class="sxs-lookup"><span data-stu-id="973a1-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="973a1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="973a1-123">Authorization</span></span>  | <span data-ttu-id="973a1-124">string</span><span class="sxs-lookup"><span data-stu-id="973a1-124">string</span></span>  | <span data-ttu-id="973a1-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="973a1-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="973a1-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="973a1-127">Request body</span></span>
<span data-ttu-id="973a1-128">要求の本文には、 [appRoleAssignment](../resources/approleassignment.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="973a1-128">In the request body, supply a JSON representation of [appRoleAssignment](../resources/approleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="973a1-129">応答</span><span class="sxs-lookup"><span data-stu-id="973a1-129">Response</span></span>

<span data-ttu-id="973a1-130">かどうかは成功すると、このメソッドを返します`201 Created`、応答の本体で応答コードと[appRoleAssignment](../resources/approleassignment.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="973a1-130">If successful, this method returns `201 Created` response code and [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="973a1-131">例</span><span class="sxs-lookup"><span data-stu-id="973a1-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="973a1-132">要求</span><span class="sxs-lookup"><span data-stu-id="973a1-132">Request</span></span>
<span data-ttu-id="973a1-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="973a1-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_approleassignment_from_serviceprincipal"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/appRoleAssignments
Content-type: application/json
Content-length: 233

{
  "creationTimestamp": "2016-10-19T10:37:00Z",
  "principalDisplayName": "principalDisplayName-value",
  "principalId": "principalId-value",
  "principalType": "principalType-value",
  "resourceDisplayName": "resourceDisplayName-value"
}
```
<span data-ttu-id="973a1-134">要求の本文には、 [appRoleAssignment](../resources/approleassignment.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="973a1-134">In the request body, supply a JSON representation of [appRoleAssignment](../resources/approleassignment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="973a1-135">応答</span><span class="sxs-lookup"><span data-stu-id="973a1-135">Response</span></span>
<span data-ttu-id="973a1-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="973a1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.approleassignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 253

{
  "creationTimestamp": "2016-10-19T10:37:00Z",
  "id": "id-value",
  "principalDisplayName": "principalDisplayName-value",
  "principalId": "principalId-value",
  "principalType": "principalType-value",
  "resourceDisplayName": "resourceDisplayName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create appRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
