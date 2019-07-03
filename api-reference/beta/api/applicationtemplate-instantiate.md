---
title: 'applicationTemplate: インスタンス化'
description: この API を使用して新しい applicationTemplate を作成する
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4dc67599c6db8db2d0465d08e164fef10948e910
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35439526"
---
# <a name="applicationtemplate-instantiate"></a><span data-ttu-id="9b547-103">applicationTemplate: インスタンス化</span><span class="sxs-lookup"><span data-stu-id="9b547-103">applicationTemplate: instantiate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b547-104">Azure AD アプリケーションギャラリーからディレクトリにアプリケーションのインスタンスを追加します。</span><span class="sxs-lookup"><span data-stu-id="9b547-104">Add an instance of an application from the Azure AD application gallery into your directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="9b547-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9b547-105">Permissions</span></span>

<span data-ttu-id="9b547-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9b547-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9b547-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9b547-108">Permission type</span></span>                        | <span data-ttu-id="9b547-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9b547-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9b547-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9b547-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9b547-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b547-111">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="9b547-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9b547-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b547-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9b547-113">Not supported.</span></span> |
| <span data-ttu-id="9b547-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9b547-114">Application</span></span>                            | <span data-ttu-id="9b547-115">Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b547-115">Application.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b547-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9b547-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applicationTemplates/{id}/instantiate
```

## <a name="request-headers"></a><span data-ttu-id="9b547-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9b547-117">Request headers</span></span>

| <span data-ttu-id="9b547-118">名前</span><span class="sxs-lookup"><span data-stu-id="9b547-118">Name</span></span>          | <span data-ttu-id="9b547-119">説明</span><span class="sxs-lookup"><span data-stu-id="9b547-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="9b547-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b547-120">Authorization</span></span> | <span data-ttu-id="9b547-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="9b547-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="9b547-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="9b547-122">Request body</span></span>

<span data-ttu-id="9b547-123">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="9b547-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9b547-124">パラメーター</span><span class="sxs-lookup"><span data-stu-id="9b547-124">Parameter</span></span>    | <span data-ttu-id="9b547-125">型</span><span class="sxs-lookup"><span data-stu-id="9b547-125">Type</span></span>        | <span data-ttu-id="9b547-126">説明</span><span class="sxs-lookup"><span data-stu-id="9b547-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9b547-127">displayName</span><span class="sxs-lookup"><span data-stu-id="9b547-127">displayName</span></span>|<span data-ttu-id="9b547-128">String</span><span class="sxs-lookup"><span data-stu-id="9b547-128">String</span></span>|<span data-ttu-id="9b547-129">アプリケーションのカスタム名</span><span class="sxs-lookup"><span data-stu-id="9b547-129">Custom name of the application</span></span>|

## <a name="response"></a><span data-ttu-id="9b547-130">応答</span><span class="sxs-lookup"><span data-stu-id="9b547-130">Response</span></span>

<span data-ttu-id="9b547-131">成功した場合、このメソッド`201 OK`は応答コードと、応答本文で新しい[applicationserviceprincipal](../resources/applicationserviceprincipal.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9b547-131">If successful, this method returns a `201 OK` response code and a new [applicationServicePrincipal](../resources/applicationserviceprincipal.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9b547-132">例</span><span class="sxs-lookup"><span data-stu-id="9b547-132">Examples</span></span>

<span data-ttu-id="9b547-133">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="9b547-133">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="9b547-134">要求</span><span class="sxs-lookup"><span data-stu-id="9b547-134">Request</span></span>

<span data-ttu-id="9b547-135">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9b547-135">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9b547-136">プロトコル</span><span class="sxs-lookup"><span data-stu-id="9b547-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "applicationtemplate_instantiate"
}-->

```http
POST https://graph.microsoft.com/beta/applicationTemplates/{id}/instantiate
Content-type: application/json

{
  "displayName": "My custom name"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9b547-137">C#</span><span class="sxs-lookup"><span data-stu-id="9b547-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/applicationtemplate-instantiate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9b547-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="9b547-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/applicationtemplate-instantiate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9b547-139">目的-C</span><span class="sxs-lookup"><span data-stu-id="9b547-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/applicationtemplate-instantiate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9b547-140">応答</span><span class="sxs-lookup"><span data-stu-id="9b547-140">Response</span></span>

<span data-ttu-id="9b547-141">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9b547-141">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="9b547-142">ここに示す response オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="9b547-142">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9b547-143">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="9b547-143">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationServicePrincipal"
} -->

```http
HTTP/1.1 201 OK
Content-type: application/json

{
   "servicePrincipal": {
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
   },
   "application": {
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
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applicationTemplate: instantiate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
