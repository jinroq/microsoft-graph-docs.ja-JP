---
title: リスト scopedRoleMembers
description: ScopedRoleMembership リソースのリストを取得します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 83eb193d46b6ee206beb3c86404e35fb8ed10cad
ms.sourcegitcommit: 27e8ddb53b699f70b676c9648db8f06bb8d831a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/27/2019
ms.locfileid: "35917959"
---
# <a name="list-scopedrolemembers"></a><span data-ttu-id="4a5c5-103">リスト scopedRoleMembers</span><span class="sxs-lookup"><span data-stu-id="4a5c5-103">List scopedRoleMembers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a5c5-104">[ScopedRoleMembership](../resources/scopedrolemembership.md)リソースのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="4a5c5-104">Retrieve a list of [scopedRoleMembership](../resources/scopedrolemembership.md) resources.</span></span>
## <a name="permissions"></a><span data-ttu-id="4a5c5-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4a5c5-105">Permissions</span></span>
<span data-ttu-id="4a5c5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4a5c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4a5c5-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4a5c5-108">Permission type</span></span>      | <span data-ttu-id="4a5c5-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4a5c5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a5c5-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4a5c5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4a5c5-111">AdministrativeUnit、AdministrativeUnit、Directory.accessasuser.all のいずれかの値を取得します。</span><span class="sxs-lookup"><span data-stu-id="4a5c5-111">AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4a5c5-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4a5c5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a5c5-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4a5c5-113">Not supported.</span></span>    |
|<span data-ttu-id="4a5c5-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4a5c5-114">Application</span></span> | <span data-ttu-id="4a5c5-115">AdministrativeUnit、AdministrativeUnit のいずれかを取得します。</span><span class="sxs-lookup"><span data-stu-id="4a5c5-115">AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4a5c5-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4a5c5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits/{id}/scopedRoleMembers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4a5c5-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="4a5c5-117">Optional query parameters</span></span>
<span data-ttu-id="4a5c5-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="4a5c5-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4a5c5-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4a5c5-119">Request headers</span></span>
| <span data-ttu-id="4a5c5-120">名前</span><span class="sxs-lookup"><span data-stu-id="4a5c5-120">Name</span></span>      |<span data-ttu-id="4a5c5-121">説明</span><span class="sxs-lookup"><span data-stu-id="4a5c5-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4a5c5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a5c5-122">Authorization</span></span>  | <span data-ttu-id="4a5c5-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4a5c5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4a5c5-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="4a5c5-125">Request body</span></span>
<span data-ttu-id="4a5c5-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="4a5c5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4a5c5-127">応答</span><span class="sxs-lookup"><span data-stu-id="4a5c5-127">Response</span></span>

<span data-ttu-id="4a5c5-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[scopedRoleMembership](../resources/scopedrolemembership.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="4a5c5-128">If successful, this method returns a `200 OK` response code and collection of [scopedRoleMembership](../resources/scopedrolemembership.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4a5c5-129">例</span><span class="sxs-lookup"><span data-stu-id="4a5c5-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4a5c5-130">要求</span><span class="sxs-lookup"><span data-stu-id="4a5c5-130">Request</span></span>
<span data-ttu-id="4a5c5-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4a5c5-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4a5c5-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="4a5c5-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_scopedrolemember"
}-->
```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/scopedRoleMembers
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4a5c5-133">C#</span><span class="sxs-lookup"><span data-stu-id="4a5c5-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-scopedrolemember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4a5c5-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="4a5c5-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-scopedrolemember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4a5c5-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="4a5c5-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-scopedrolemember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4a5c5-136">Java</span><span class="sxs-lookup"><span data-stu-id="4a5c5-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-scopedrolemember-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4a5c5-137">応答</span><span class="sxs-lookup"><span data-stu-id="4a5c5-137">Response</span></span>
<span data-ttu-id="4a5c5-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4a5c5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
