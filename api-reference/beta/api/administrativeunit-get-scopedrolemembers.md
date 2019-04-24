---
title: scopedRoleMember を取得する
description: 特定の scopedRoleMembership リソースを取得します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0e961097184730922aebd4348f88b8570d5c24ca
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459470"
---
# <a name="get-a-scopedrolemember"></a><span data-ttu-id="6827f-103">scopedRoleMember を取得する</span><span class="sxs-lookup"><span data-stu-id="6827f-103">Get a scopedRoleMember</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6827f-104">特定の[scopedRoleMembership](../resources/scopedrolemembership.md)リソースを取得します。</span><span class="sxs-lookup"><span data-stu-id="6827f-104">Retrieve a specific [scopedRoleMembership](../resources/scopedrolemembership.md) resource.</span></span>
## <a name="permissions"></a><span data-ttu-id="6827f-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6827f-105">Permissions</span></span>
<span data-ttu-id="6827f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6827f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6827f-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6827f-108">Permission type</span></span>      | <span data-ttu-id="6827f-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6827f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6827f-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6827f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6827f-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6827f-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6827f-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6827f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6827f-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6827f-113">Not supported.</span></span>    |
|<span data-ttu-id="6827f-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6827f-114">Application</span></span> | <span data-ttu-id="6827f-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6827f-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6827f-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6827f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits/{id}/scopedRoleMembers/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6827f-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="6827f-117">Optional query parameters</span></span>
<span data-ttu-id="6827f-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="6827f-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6827f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6827f-119">Request headers</span></span>
| <span data-ttu-id="6827f-120">名前</span><span class="sxs-lookup"><span data-stu-id="6827f-120">Name</span></span>      |<span data-ttu-id="6827f-121">説明</span><span class="sxs-lookup"><span data-stu-id="6827f-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6827f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6827f-122">Authorization</span></span>  | <span data-ttu-id="6827f-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6827f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6827f-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="6827f-125">Request body</span></span>
<span data-ttu-id="6827f-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6827f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6827f-127">応答</span><span class="sxs-lookup"><span data-stu-id="6827f-127">Response</span></span>

<span data-ttu-id="6827f-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で要求された[scopedRoleMembership](../resources/scopedrolemembership.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6827f-128">If successful, this method returns a `200 OK` response code and the requested [scopedRoleMembership](../resources/scopedrolemembership.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6827f-129">例</span><span class="sxs-lookup"><span data-stu-id="6827f-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6827f-130">要求</span><span class="sxs-lookup"><span data-stu-id="6827f-130">Request</span></span>
<span data-ttu-id="6827f-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6827f-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_scopedrolemember"
}-->
```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/scopedRoleMembers/{id}
```
##### <a name="response"></a><span data-ttu-id="6827f-132">応答</span><span class="sxs-lookup"><span data-stu-id="6827f-132">Response</span></span>
<span data-ttu-id="6827f-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6827f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
