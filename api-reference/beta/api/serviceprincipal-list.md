---
title: リスト servicePrincipals
description: ServicePrincipal オブジェクトのリストを取得します。
localization_priority: Normal
ms.openlocfilehash: d7e0a9a34ac0ab7a166c40336671ec4d0a89ddd6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837612"
---
# <a name="list-serviceprincipals"></a><span data-ttu-id="fc25a-103">リスト servicePrincipals</span><span class="sxs-lookup"><span data-stu-id="fc25a-103">List servicePrincipals</span></span>

> <span data-ttu-id="fc25a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fc25a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fc25a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fc25a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fc25a-106">ServicePrincipal オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="fc25a-106">Retrieve a list of servicePrincipal objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="fc25a-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fc25a-107">Permissions</span></span>

<span data-ttu-id="fc25a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fc25a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="fc25a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fc25a-110">Permission type</span></span>      | <span data-ttu-id="fc25a-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fc25a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc25a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fc25a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fc25a-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fc25a-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fc25a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fc25a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc25a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fc25a-115">Not supported.</span></span>    |
|<span data-ttu-id="fc25a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fc25a-116">Application</span></span> | <span data-ttu-id="fc25a-117">Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="fc25a-117">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc25a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fc25a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fc25a-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="fc25a-119">Optional query parameters</span></span>

<span data-ttu-id="fc25a-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="fc25a-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fc25a-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fc25a-121">Request headers</span></span>
| <span data-ttu-id="fc25a-122">名前</span><span class="sxs-lookup"><span data-stu-id="fc25a-122">Name</span></span> | <span data-ttu-id="fc25a-123">説明</span><span class="sxs-lookup"><span data-stu-id="fc25a-123">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="fc25a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc25a-124">Authorization</span></span>  | <span data-ttu-id="fc25a-125">string</span><span class="sxs-lookup"><span data-stu-id="fc25a-125">string</span></span>  | <span data-ttu-id="fc25a-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="fc25a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fc25a-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="fc25a-128">Request body</span></span>

<span data-ttu-id="fc25a-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="fc25a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fc25a-130">応答</span><span class="sxs-lookup"><span data-stu-id="fc25a-130">Response</span></span>

<span data-ttu-id="fc25a-131">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[servicePrincipal](../resources/serviceprincipal.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="fc25a-131">If successful, this method returns a `200 OK` response code and collection of [servicePrincipal](../resources/serviceprincipal.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc25a-132">例</span><span class="sxs-lookup"><span data-stu-id="fc25a-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="fc25a-133">要求</span><span class="sxs-lookup"><span data-stu-id="fc25a-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_serviceprincipals"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals
```
##### <a name="response"></a><span data-ttu-id="fc25a-134">応答</span><span class="sxs-lookup"><span data-stu-id="fc25a-134">Response</span></span>

<span data-ttu-id="fc25a-p104">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fc25a-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List servicePrincipals",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
