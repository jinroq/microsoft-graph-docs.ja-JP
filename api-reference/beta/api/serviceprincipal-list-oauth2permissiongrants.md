---
title: 'servicePrincipal: List oAuth2Permissiongrants'
description: OAuth2Permissiongrant オブジェクトのリストを取得します。
localization_priority: Normal
ms.openlocfilehash: 104d197d843acfb1ac7c20330dd4c7e3af58ee60
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638789"
---
# <a name="serviceprincipal-list-oauth2permissiongrants"></a><span data-ttu-id="18061-103">servicePrincipal: List oAuth2Permissiongrants</span><span class="sxs-lookup"><span data-stu-id="18061-103">servicePrincipal: List oAuth2Permissiongrants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18061-104">OAuth2Permissiongrant オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="18061-104">Retrieve a list of oAuth2Permissiongrant objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="18061-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="18061-105">Permissions</span></span>
<span data-ttu-id="18061-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="18061-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18061-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="18061-108">Permission type</span></span>      | <span data-ttu-id="18061-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="18061-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18061-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="18061-110">Delegated (work or school account)</span></span> | <span data-ttu-id="18061-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="18061-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="18061-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="18061-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18061-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="18061-113">Not supported.</span></span>    |
|<span data-ttu-id="18061-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="18061-114">Application</span></span> | <span data-ttu-id="18061-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18061-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="18061-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="18061-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/oAuth2Permissiongrants
```
## <a name="optional-query-parameters"></a><span data-ttu-id="18061-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="18061-117">Optional query parameters</span></span>
<span data-ttu-id="18061-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="18061-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="18061-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="18061-119">Request headers</span></span>
| <span data-ttu-id="18061-120">名前</span><span class="sxs-lookup"><span data-stu-id="18061-120">Name</span></span>       | <span data-ttu-id="18061-121">型</span><span class="sxs-lookup"><span data-stu-id="18061-121">Type</span></span> | <span data-ttu-id="18061-122">説明</span><span class="sxs-lookup"><span data-stu-id="18061-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="18061-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="18061-123">Authorization</span></span>  | <span data-ttu-id="18061-124">string</span><span class="sxs-lookup"><span data-stu-id="18061-124">string</span></span>  | <span data-ttu-id="18061-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="18061-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="18061-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="18061-127">Request body</span></span>
<span data-ttu-id="18061-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="18061-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18061-129">応答</span><span class="sxs-lookup"><span data-stu-id="18061-129">Response</span></span>

<span data-ttu-id="18061-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[oAuth2Permissiongrant](../resources/oauth2permissiongrant.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="18061-130">If successful, this method returns a `200 OK` response code and collection of [oAuth2Permissiongrant](../resources/oauth2permissiongrant.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="18061-131">例</span><span class="sxs-lookup"><span data-stu-id="18061-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="18061-132">要求</span><span class="sxs-lookup"><span data-stu-id="18061-132">Request</span></span>
<span data-ttu-id="18061-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="18061-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_oAuth2Permissiongrants"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/oAuth2Permissiongrants
```
##### <a name="response"></a><span data-ttu-id="18061-134">応答</span><span class="sxs-lookup"><span data-stu-id="18061-134">Response</span></span>
<span data-ttu-id="18061-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="18061-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 253

{
  "value": [
    {
      "clientId": "clientId-value",
      "consentType": "consentType-value",
      "expiryTime": "2016-10-19T10:37:00Z",
      "id": "id-value",
      "principalId": "principalId-value",
      "resourceId": "resourceId-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="18061-138">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="18061-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="18061-139">Visual</span><span class="sxs-lookup"><span data-stu-id="18061-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_oAuth2Permissiongrants-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="18061-140">Java</span><span class="sxs-lookup"><span data-stu-id="18061-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_oAuth2Permissiongrants-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List oAuth2Permissiongrants",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/serviceprincipal-list-oauth2permissiongrants.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/serviceprincipal-list-oauth2permissiongrants.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
