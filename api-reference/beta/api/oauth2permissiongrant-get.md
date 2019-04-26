---
title: oAuth2Permissiongrant を取得する
description: oAuth2Permissiongrant オブジェクトのプロパティとリレーションシップを取得します。
localization_priority: Normal
ms.openlocfilehash: 482d1f310b6eadcfe7df9e961af4ee4c229e9c12
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33338220"
---
# <a name="get-oauth2permissiongrant"></a><span data-ttu-id="f8c60-103">oAuth2Permissiongrant を取得する</span><span class="sxs-lookup"><span data-stu-id="f8c60-103">Get oAuth2Permissiongrant</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8c60-104">oAuth2Permissiongrant オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="f8c60-104">Retrieve the properties and relationships of oAuth2Permissiongrant object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f8c60-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f8c60-105">Permissions</span></span>
<span data-ttu-id="f8c60-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f8c60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f8c60-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f8c60-108">Permission type</span></span>      | <span data-ttu-id="f8c60-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f8c60-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f8c60-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f8c60-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f8c60-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f8c60-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f8c60-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f8c60-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8c60-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f8c60-113">Not supported.</span></span>    |
|<span data-ttu-id="f8c60-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f8c60-114">Application</span></span> | <span data-ttu-id="f8c60-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8c60-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f8c60-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f8c60-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /oAuth2Permissiongrants/{id}
GET /users/{id | userPrincipalName}/oAuth2Permissiongrants/{id}
GET /drive/root/createdByUser/oAuth2Permissiongrants/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f8c60-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f8c60-117">Optional query parameters</span></span>
<span data-ttu-id="f8c60-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="f8c60-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f8c60-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f8c60-119">Request headers</span></span>
| <span data-ttu-id="f8c60-120">名前</span><span class="sxs-lookup"><span data-stu-id="f8c60-120">Name</span></span>       | <span data-ttu-id="f8c60-121">型</span><span class="sxs-lookup"><span data-stu-id="f8c60-121">Type</span></span> | <span data-ttu-id="f8c60-122">説明</span><span class="sxs-lookup"><span data-stu-id="f8c60-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f8c60-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8c60-123">Authorization</span></span>  | <span data-ttu-id="f8c60-124">string</span><span class="sxs-lookup"><span data-stu-id="f8c60-124">string</span></span>  | <span data-ttu-id="f8c60-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f8c60-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f8c60-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="f8c60-127">Request body</span></span>
<span data-ttu-id="f8c60-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f8c60-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8c60-129">応答</span><span class="sxs-lookup"><span data-stu-id="f8c60-129">Response</span></span>

<span data-ttu-id="f8c60-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[oAuth2Permissiongrant](../resources/oauth2permissiongrant.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f8c60-130">If successful, this method returns a `200 OK` response code and [oAuth2Permissiongrant](../resources/oauth2permissiongrant.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f8c60-131">例</span><span class="sxs-lookup"><span data-stu-id="f8c60-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f8c60-132">要求</span><span class="sxs-lookup"><span data-stu-id="f8c60-132">Request</span></span>
<span data-ttu-id="f8c60-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f8c60-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_oAuth2Permissiongrant"
}-->
```http
GET https://graph.microsoft.com/beta/oAuth2Permissiongrants/{id}
```
##### <a name="response"></a><span data-ttu-id="f8c60-134">応答</span><span class="sxs-lookup"><span data-stu-id="f8c60-134">Response</span></span>
<span data-ttu-id="f8c60-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f8c60-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 200

{
  "clientId": "clientId-value",
  "consentType": "consentType-value",
  "expiryTime": "2016-10-19T10:37:00Z",
  "id": "id-value",
  "principalId": "principalId-value",
  "resourceId": "resourceId-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get oAuth2Permissiongrant",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
