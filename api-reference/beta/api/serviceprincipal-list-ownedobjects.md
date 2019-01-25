---
title: 'servicePrincipals: ownedObjects を一覧表示'
description: ServicePrincipal が所有するオブジェクトの一覧を取得します。  これには、アプリケーションまたはグループが含まれます。
localization_priority: Normal
ms.openlocfilehash: 788ee23010825a657e8eb5664f11de1d2cf1b34a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514237"
---
# <a name="serviceprincipals-list-ownedobjects"></a><span data-ttu-id="ba487-104">servicePrincipals: ownedObjects を一覧表示</span><span class="sxs-lookup"><span data-stu-id="ba487-104">servicePrincipals: List ownedObjects</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba487-105">ServicePrincipal が所有するオブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="ba487-105">Retrieve a list of objects owned by the servicePrincipal.</span></span>  <span data-ttu-id="ba487-106">これには、アプリケーションまたはグループが含まれます。</span><span class="sxs-lookup"><span data-stu-id="ba487-106">This could include applications or groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="ba487-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ba487-107">Permissions</span></span>
<span data-ttu-id="ba487-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ba487-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba487-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ba487-110">Permission type</span></span>      | <span data-ttu-id="ba487-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ba487-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ba487-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ba487-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ba487-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ba487-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ba487-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ba487-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba487-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ba487-115">Not supported.</span></span>    |
|<span data-ttu-id="ba487-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ba487-116">Application</span></span> | <span data-ttu-id="ba487-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba487-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba487-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ba487-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/ownedObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ba487-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ba487-119">Optional query parameters</span></span>
<span data-ttu-id="ba487-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ba487-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ba487-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ba487-121">Request headers</span></span>
| <span data-ttu-id="ba487-122">名前</span><span class="sxs-lookup"><span data-stu-id="ba487-122">Name</span></span>       | <span data-ttu-id="ba487-123">型</span><span class="sxs-lookup"><span data-stu-id="ba487-123">Type</span></span> | <span data-ttu-id="ba487-124">説明</span><span class="sxs-lookup"><span data-stu-id="ba487-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ba487-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba487-125">Authorization</span></span>  | <span data-ttu-id="ba487-126">string</span><span class="sxs-lookup"><span data-stu-id="ba487-126">string</span></span>  | <span data-ttu-id="ba487-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ba487-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ba487-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="ba487-129">Request body</span></span>
<span data-ttu-id="ba487-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ba487-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba487-131">応答</span><span class="sxs-lookup"><span data-stu-id="ba487-131">Response</span></span>

<span data-ttu-id="ba487-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="ba487-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ba487-133">例</span><span class="sxs-lookup"><span data-stu-id="ba487-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ba487-134">要求</span><span class="sxs-lookup"><span data-stu-id="ba487-134">Request</span></span>
<span data-ttu-id="ba487-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ba487-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_ownedobjects"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/ownedObjects
```
##### <a name="response"></a><span data-ttu-id="ba487-136">応答</span><span class="sxs-lookup"><span data-stu-id="ba487-136">Response</span></span>
<span data-ttu-id="ba487-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ba487-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List ownedObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/serviceprincipal-list-ownedobjects.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
