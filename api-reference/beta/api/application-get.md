---
title: アプリケーションを取得します。
description: プロパティとアプリケーションのオブジェクトの関係を取得します。
author: lleonard-msft
ms.openlocfilehash: a041cbc4e97a59500106542b88e754b9c495f985
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303494"
---
# <a name="get-application"></a><span data-ttu-id="44bcf-103">アプリケーションを取得します。</span><span class="sxs-lookup"><span data-stu-id="44bcf-103">Get application</span></span>

> <span data-ttu-id="44bcf-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="44bcf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="44bcf-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="44bcf-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="44bcf-106">プロパティとアプリケーションのオブジェクトの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="44bcf-106">Retrieve the properties and relationships of application object.</span></span>

## <a name="permissions"></a><span data-ttu-id="44bcf-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="44bcf-107">Permissions</span></span>
<span data-ttu-id="44bcf-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="44bcf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44bcf-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="44bcf-110">Permission type</span></span>      | <span data-ttu-id="44bcf-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="44bcf-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="44bcf-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="44bcf-112">Delegated (work or school account)</span></span> | <span data-ttu-id="44bcf-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="44bcf-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="44bcf-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="44bcf-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44bcf-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="44bcf-115">Not supported.</span></span>    |
|<span data-ttu-id="44bcf-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="44bcf-116">Application</span></span> | <span data-ttu-id="44bcf-117">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="44bcf-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="44bcf-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="44bcf-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="44bcf-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="44bcf-119">Optional query parameters</span></span>
<span data-ttu-id="44bcf-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="44bcf-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="44bcf-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="44bcf-121">Request headers</span></span>
| <span data-ttu-id="44bcf-122">名前</span><span class="sxs-lookup"><span data-stu-id="44bcf-122">Name</span></span>       | <span data-ttu-id="44bcf-123">種類</span><span class="sxs-lookup"><span data-stu-id="44bcf-123">Type</span></span> | <span data-ttu-id="44bcf-124">説明</span><span class="sxs-lookup"><span data-stu-id="44bcf-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="44bcf-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="44bcf-125">Authorization</span></span>  | <span data-ttu-id="44bcf-126">string</span><span class="sxs-lookup"><span data-stu-id="44bcf-126">string</span></span>  | <span data-ttu-id="44bcf-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="44bcf-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="44bcf-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="44bcf-129">Request body</span></span>
<span data-ttu-id="44bcf-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="44bcf-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="44bcf-131">応答</span><span class="sxs-lookup"><span data-stu-id="44bcf-131">Response</span></span>

<span data-ttu-id="44bcf-132">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[アプリケーション](../resources/application.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="44bcf-132">If successful, this method returns a `200 OK` response code and [application](../resources/application.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="44bcf-133">例</span><span class="sxs-lookup"><span data-stu-id="44bcf-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="44bcf-134">要求</span><span class="sxs-lookup"><span data-stu-id="44bcf-134">Request</span></span>
<span data-ttu-id="44bcf-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="44bcf-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_application"
}-->
```http
GET https://graph.microsoft.com/beta/applications/{id}
```
##### <a name="response"></a><span data-ttu-id="44bcf-136">応答</span><span class="sxs-lookup"><span data-stu-id="44bcf-136">Response</span></span>
<span data-ttu-id="44bcf-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="44bcf-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1044

{
  "api": {
    "acceptedAccessTokenVersion": 1,
    "publishedPermissionScopes": [
      {
        "adminConsentDescription": "adminConsentDescription-value",
        "adminConsentDisplayName": "adminConsentDisplayName-value",
        "id": "id-value",
        "isEnabled": true,
        "type": "type-value",
        "userConsentDescription": "userConsentDescription-value",
        "userConsentDisplayName": "userConsentDisplayName-value",
        "value": "value-value"
      }
    ]
  },
  "allowPublicClient": true,
  "applicationAliases": [
    "applicationAliases-value"
  ],
  "createdDateTime": "datetime-value",
  "installedClients": {
    "redirectUrls": [
      "redirectUrls-value"
    ]
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get application",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->