---
title: ScopedRoleMember を取得します。
description: ScopedRoleMembership の特定のリソースを取得します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 79c669554d60ffd5e4445290166779b98701f9aa
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573558"
---
# <a name="get-a-scopedrolemember"></a><span data-ttu-id="ea134-103">ScopedRoleMember を取得します。</span><span class="sxs-lookup"><span data-stu-id="ea134-103">Get a scopedRoleMember</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea134-104">[ScopedRoleMembership](../resources/scopedrolemembership.md)特定のリソースを取得します。</span><span class="sxs-lookup"><span data-stu-id="ea134-104">Retrieve a specific [scopedRoleMembership](../resources/scopedrolemembership.md) resource.</span></span>
## <a name="permissions"></a><span data-ttu-id="ea134-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ea134-105">Permissions</span></span>
<span data-ttu-id="ea134-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ea134-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ea134-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ea134-108">Permission type</span></span>      | <span data-ttu-id="ea134-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ea134-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ea134-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ea134-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ea134-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ea134-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ea134-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ea134-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea134-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ea134-113">Not supported.</span></span>    |
|<span data-ttu-id="ea134-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ea134-114">Application</span></span> | <span data-ttu-id="ea134-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea134-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ea134-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ea134-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits/{id}/scopedRoleMembers/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ea134-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ea134-117">Optional query parameters</span></span>
<span data-ttu-id="ea134-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ea134-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ea134-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ea134-119">Request headers</span></span>
| <span data-ttu-id="ea134-120">名前</span><span class="sxs-lookup"><span data-stu-id="ea134-120">Name</span></span>      |<span data-ttu-id="ea134-121">説明</span><span class="sxs-lookup"><span data-stu-id="ea134-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ea134-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea134-122">Authorization</span></span>  | <span data-ttu-id="ea134-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ea134-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ea134-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="ea134-125">Request body</span></span>
<span data-ttu-id="ea134-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ea134-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea134-127">応答</span><span class="sxs-lookup"><span data-stu-id="ea134-127">Response</span></span>

<span data-ttu-id="ea134-128">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に要求された[scopedRoleMembership](../resources/scopedrolemembership.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="ea134-128">If successful, this method returns a `200 OK` response code and the requested [scopedRoleMembership](../resources/scopedrolemembership.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ea134-129">例</span><span class="sxs-lookup"><span data-stu-id="ea134-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ea134-130">要求</span><span class="sxs-lookup"><span data-stu-id="ea134-130">Request</span></span>
<span data-ttu-id="ea134-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ea134-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_scopedrolemember"
}-->
```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/scopedRoleMembers/{id}
```
##### <a name="response"></a><span data-ttu-id="ea134-132">応答</span><span class="sxs-lookup"><span data-stu-id="ea134-132">Response</span></span>
<span data-ttu-id="ea134-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ea134-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedRoleMembership"
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
<!--
{
  "type": "#page.annotation",
  "description": "List scopedRoleMembers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/administrativeunit-get-scopedrolemembers.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
