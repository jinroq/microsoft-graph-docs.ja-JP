---
title: リスト oauth2PermissionGrants
description: Oauth2PermissionGrant オブジェクトのリストを取得します。
ms.openlocfilehash: 947041262ddac7ef0aab43ee455979ee0cf9bbf8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071118"
---
# <a name="list-oauth2permissiongrants"></a><span data-ttu-id="1ad19-103">リスト oauth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="1ad19-103">List oauth2PermissionGrants</span></span>

> <span data-ttu-id="1ad19-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1ad19-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1ad19-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1ad19-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1ad19-106">Oauth2PermissionGrant オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="1ad19-106">Retrieve a list of oauth2PermissionGrant objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="1ad19-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1ad19-107">Permissions</span></span>

<span data-ttu-id="1ad19-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1ad19-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1ad19-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1ad19-110">Permission type</span></span>      | <span data-ttu-id="1ad19-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1ad19-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1ad19-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1ad19-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1ad19-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1ad19-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1ad19-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1ad19-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ad19-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1ad19-115">Not supported.</span></span>    |
|<span data-ttu-id="1ad19-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1ad19-116">Application</span></span> | <span data-ttu-id="1ad19-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ad19-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1ad19-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1ad19-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /oauth2PermissionGrants
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1ad19-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="1ad19-119">Optional query parameters</span></span>
<span data-ttu-id="1ad19-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="1ad19-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1ad19-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1ad19-121">Request headers</span></span>
| <span data-ttu-id="1ad19-122">名前</span><span class="sxs-lookup"><span data-stu-id="1ad19-122">Name</span></span> | <span data-ttu-id="1ad19-123">説明</span><span class="sxs-lookup"><span data-stu-id="1ad19-123">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="1ad19-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ad19-124">Authorization</span></span>  | <span data-ttu-id="1ad19-125">string</span><span class="sxs-lookup"><span data-stu-id="1ad19-125">string</span></span>  | <span data-ttu-id="1ad19-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1ad19-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1ad19-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="1ad19-128">Request body</span></span>
<span data-ttu-id="1ad19-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1ad19-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1ad19-130">応答</span><span class="sxs-lookup"><span data-stu-id="1ad19-130">Response</span></span>

<span data-ttu-id="1ad19-131">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[oAuth2PermissionGrant](../resources/oauth2permissiongrant.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="1ad19-131">If successful, this method returns a `200 OK` response code and collection of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1ad19-132">例</span><span class="sxs-lookup"><span data-stu-id="1ad19-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="1ad19-133">要求</span><span class="sxs-lookup"><span data-stu-id="1ad19-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_oauth2permissiongrants"
}-->
```http
GET https://graph.microsoft.com/beta/oauth2PermissionGrants
```
##### <a name="response"></a><span data-ttu-id="1ad19-134">応答</span><span class="sxs-lookup"><span data-stu-id="1ad19-134">Response</span></span>

<span data-ttu-id="1ad19-p104">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1ad19-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2Permissiongrant",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 259

{
  "value": [
    {
      "clientId": "clientId-value",
      "consentType": "consentType-value",
      "expiryTime": "datetime-value",
      "id": "id-value",
      "principalId": "principalId-value",
      "resourceId": "resourceId-value",
      "scope": "scope-value",
      "startTime": "datetime-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List oauth2PermissionGrants",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->