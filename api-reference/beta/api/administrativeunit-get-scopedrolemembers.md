---
title: ScopedRoleMember を取得します。
description: ScopedRoleMembership の特定のリソースを取得します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bf707c4bca33302286ab686cf74d9faba63fac7a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971705"
---
# <a name="get-a-scopedrolemember"></a><span data-ttu-id="1d873-103">ScopedRoleMember を取得します。</span><span class="sxs-lookup"><span data-stu-id="1d873-103">Get a scopedRoleMember</span></span>

> <span data-ttu-id="1d873-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1d873-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1d873-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1d873-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1d873-106">[ScopedRoleMembership](../resources/scopedrolemembership.md)特定のリソースを取得します。</span><span class="sxs-lookup"><span data-stu-id="1d873-106">Retrieve a specific [scopedRoleMembership](../resources/scopedrolemembership.md) resource.</span></span>
## <a name="permissions"></a><span data-ttu-id="1d873-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1d873-107">Permissions</span></span>
<span data-ttu-id="1d873-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1d873-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1d873-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1d873-110">Permission type</span></span>      | <span data-ttu-id="1d873-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1d873-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d873-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1d873-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1d873-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1d873-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1d873-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1d873-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d873-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1d873-115">Not supported.</span></span>    |
|<span data-ttu-id="1d873-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1d873-116">Application</span></span> | <span data-ttu-id="1d873-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d873-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1d873-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1d873-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits/{id}/scopedRoleMembers/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1d873-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="1d873-119">Optional query parameters</span></span>
<span data-ttu-id="1d873-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="1d873-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1d873-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1d873-121">Request headers</span></span>
| <span data-ttu-id="1d873-122">名前</span><span class="sxs-lookup"><span data-stu-id="1d873-122">Name</span></span>      |<span data-ttu-id="1d873-123">説明</span><span class="sxs-lookup"><span data-stu-id="1d873-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1d873-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d873-124">Authorization</span></span>  | <span data-ttu-id="1d873-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1d873-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1d873-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="1d873-127">Request body</span></span>
<span data-ttu-id="1d873-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1d873-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1d873-129">応答</span><span class="sxs-lookup"><span data-stu-id="1d873-129">Response</span></span>

<span data-ttu-id="1d873-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に要求された[scopedRoleMembership](../resources/scopedrolemembership.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="1d873-130">If successful, this method returns a `200 OK` response code and the requested [scopedRoleMembership](../resources/scopedrolemembership.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1d873-131">例</span><span class="sxs-lookup"><span data-stu-id="1d873-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1d873-132">要求</span><span class="sxs-lookup"><span data-stu-id="1d873-132">Request</span></span>
<span data-ttu-id="1d873-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1d873-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_scopedrolemember"
}-->
```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/scopedRoleMembers/{id}
```
##### <a name="response"></a><span data-ttu-id="1d873-134">応答</span><span class="sxs-lookup"><span data-stu-id="1d873-134">Response</span></span>
<span data-ttu-id="1d873-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1d873-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedrolemembership"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 307

{
  "id": "id-value",
  "roleId": "roleId-value",
  "administrativeUnitId": "administrativeUnitId-value",
  "roleMemberInfo": {
      "id": "id-value",
      "displayName": "displayName-value",
      "userPrincipalName": "userPrincipalName-value"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List scopedRoleMembers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
