---
title: リスト scopedRoleMembers
description: ScopedRoleMembership リソースのリストを取得します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7c2210b459ac832926012ebb2194528df85a71cf
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36408714"
---
# <a name="list-scopedrolemembers"></a><span data-ttu-id="c35cc-103">リスト scopedRoleMembers</span><span class="sxs-lookup"><span data-stu-id="c35cc-103">List scopedRoleMembers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c35cc-104">[ScopedRoleMembership](../resources/scopedrolemembership.md)リソースのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="c35cc-104">Retrieve a list of [scopedRoleMembership](../resources/scopedrolemembership.md) resources.</span></span>
## <a name="permissions"></a><span data-ttu-id="c35cc-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c35cc-105">Permissions</span></span>
<span data-ttu-id="c35cc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c35cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c35cc-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c35cc-108">Permission type</span></span>      | <span data-ttu-id="c35cc-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c35cc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c35cc-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c35cc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c35cc-111">RoleManagement、RoleManagement、Directory.accessasuser.all、および all のいずれかを取得します。すべてのディレクトリについては。</span><span class="sxs-lookup"><span data-stu-id="c35cc-111">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c35cc-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c35cc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c35cc-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c35cc-113">Not supported.</span></span>    |
|<span data-ttu-id="c35cc-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c35cc-114">Application</span></span> | <span data-ttu-id="c35cc-115">RoleManagement、RoleManagement、および All のいずれかのディレクトリを参照しています。</span><span class="sxs-lookup"><span data-stu-id="c35cc-115">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c35cc-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c35cc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits/{id}/scopedRoleMembers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c35cc-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c35cc-117">Optional query parameters</span></span>
<span data-ttu-id="c35cc-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c35cc-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c35cc-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c35cc-119">Request headers</span></span>
| <span data-ttu-id="c35cc-120">名前</span><span class="sxs-lookup"><span data-stu-id="c35cc-120">Name</span></span>      |<span data-ttu-id="c35cc-121">説明</span><span class="sxs-lookup"><span data-stu-id="c35cc-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c35cc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c35cc-122">Authorization</span></span>  | <span data-ttu-id="c35cc-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c35cc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c35cc-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="c35cc-125">Request body</span></span>
<span data-ttu-id="c35cc-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c35cc-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c35cc-127">応答</span><span class="sxs-lookup"><span data-stu-id="c35cc-127">Response</span></span>

<span data-ttu-id="c35cc-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[scopedRoleMembership](../resources/scopedrolemembership.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="c35cc-128">If successful, this method returns a `200 OK` response code and collection of [scopedRoleMembership](../resources/scopedrolemembership.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c35cc-129">例</span><span class="sxs-lookup"><span data-stu-id="c35cc-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c35cc-130">要求</span><span class="sxs-lookup"><span data-stu-id="c35cc-130">Request</span></span>
<span data-ttu-id="c35cc-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c35cc-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c35cc-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="c35cc-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_scopedrolemember"
}-->
```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/scopedRoleMembers
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c35cc-133">C#</span><span class="sxs-lookup"><span data-stu-id="c35cc-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-scopedrolemember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c35cc-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c35cc-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-scopedrolemember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c35cc-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="c35cc-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-scopedrolemember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c35cc-136">応答</span><span class="sxs-lookup"><span data-stu-id="c35cc-136">Response</span></span>
<span data-ttu-id="c35cc-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c35cc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedRoleMembership",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 307

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List scopedRoleMembers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
