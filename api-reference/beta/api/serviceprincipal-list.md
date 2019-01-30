---
title: servicePrincipals を一覧表示する
description: servicePrincipal オブジェクトの一覧を取得します。
localization_priority: Normal
ms.openlocfilehash: cd61b69e330ac376d15bfaf99c1147b8f9402d7f
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643630"
---
# <a name="list-serviceprincipals"></a><span data-ttu-id="340f2-103">servicePrincipals を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="340f2-103">List servicePrincipals</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="340f2-104">servicePrincipal オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="340f2-104">Retrieve a list of servicePrincipal objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="340f2-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="340f2-105">Permissions</span></span>

<span data-ttu-id="340f2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="340f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="340f2-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="340f2-108">Permission type</span></span>      | <span data-ttu-id="340f2-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="340f2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="340f2-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="340f2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="340f2-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="340f2-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="340f2-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="340f2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="340f2-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="340f2-113">Not supported.</span></span>    |
|<span data-ttu-id="340f2-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="340f2-114">Application</span></span> | <span data-ttu-id="340f2-115">Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="340f2-115">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="340f2-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="340f2-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals
```
## <a name="optional-query-parameters"></a><span data-ttu-id="340f2-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="340f2-117">Optional query parameters</span></span>

<span data-ttu-id="340f2-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="340f2-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="340f2-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="340f2-119">Request headers</span></span>
| <span data-ttu-id="340f2-120">名前</span><span class="sxs-lookup"><span data-stu-id="340f2-120">Name</span></span> | <span data-ttu-id="340f2-121">説明</span><span class="sxs-lookup"><span data-stu-id="340f2-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="340f2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="340f2-122">Authorization</span></span>  | <span data-ttu-id="340f2-123">string</span><span class="sxs-lookup"><span data-stu-id="340f2-123">string</span></span>  | <span data-ttu-id="340f2-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="340f2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="340f2-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="340f2-126">Request body</span></span>

<span data-ttu-id="340f2-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="340f2-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="340f2-128">応答</span><span class="sxs-lookup"><span data-stu-id="340f2-128">Response</span></span>

<span data-ttu-id="340f2-129">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[servicePrincipal](../resources/serviceprincipal.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="340f2-129">If successful, this method returns a `200 OK` response code and collection of [servicePrincipal](../resources/serviceprincipal.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="340f2-130">例</span><span class="sxs-lookup"><span data-stu-id="340f2-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="340f2-131">要求</span><span class="sxs-lookup"><span data-stu-id="340f2-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_serviceprincipals"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals
```
##### <a name="response"></a><span data-ttu-id="340f2-132">応答</span><span class="sxs-lookup"><span data-stu-id="340f2-132">Response</span></span>

<span data-ttu-id="340f2-p103">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="340f2-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.serviceprincipal",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 488

{
  "value": [
    {
      "accountEnabled": true,
      "addIns": [
        {
          "id": "id-value",
          "type": "type-value",
          "properties": [
            {
              "key": "key-value",
              "value": "value-value"
            }
          ]
        }
      ],
      "appDisplayName": "appDisplayName-value",
      "appId": "appId-value",
      "appOwnerOrganizationId": "appOwnerOrganizationId-value",
      "appRoleAssignmentRequired": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List servicePrincipals",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/serviceprincipal-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
