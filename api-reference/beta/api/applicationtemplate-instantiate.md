---
title: 'applicationTemplate: インスタンス化'
description: この API を使用して新しい applicationTemplate を作成する
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d3874f7e015816dbc76ce99fa1fc26f65727ad97
ms.sourcegitcommit: 7c03131291113c343a98bb0234d31bd4535a4050
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/22/2019
ms.locfileid: "35147922"
---
# <a name="applicationtemplate-instantiate"></a><span data-ttu-id="0f9d1-103">applicationTemplate: インスタンス化</span><span class="sxs-lookup"><span data-stu-id="0f9d1-103">applicationTemplate: instantiate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f9d1-104">Azure AD アプリケーションギャラリーからディレクトリにアプリケーションのインスタンスを追加します。</span><span class="sxs-lookup"><span data-stu-id="0f9d1-104">Add an instance of an application from the Azure AD application gallery into your directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="0f9d1-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0f9d1-105">Permissions</span></span>

<span data-ttu-id="0f9d1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0f9d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0f9d1-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0f9d1-108">Permission type</span></span>                        | <span data-ttu-id="0f9d1-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0f9d1-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0f9d1-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0f9d1-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0f9d1-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f9d1-111">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="0f9d1-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0f9d1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f9d1-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0f9d1-113">Not supported.</span></span> |
| <span data-ttu-id="0f9d1-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0f9d1-114">Application</span></span>                            | <span data-ttu-id="0f9d1-115">Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f9d1-115">Application.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f9d1-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0f9d1-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applicationTemplates/{id}/instantiate
```

## <a name="request-headers"></a><span data-ttu-id="0f9d1-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0f9d1-117">Request headers</span></span>

| <span data-ttu-id="0f9d1-118">名前</span><span class="sxs-lookup"><span data-stu-id="0f9d1-118">Name</span></span>          | <span data-ttu-id="0f9d1-119">説明</span><span class="sxs-lookup"><span data-stu-id="0f9d1-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0f9d1-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f9d1-120">Authorization</span></span> | <span data-ttu-id="0f9d1-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="0f9d1-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="0f9d1-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="0f9d1-122">Request body</span></span>

<span data-ttu-id="0f9d1-123">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="0f9d1-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0f9d1-124">パラメーター</span><span class="sxs-lookup"><span data-stu-id="0f9d1-124">Parameter</span></span>    | <span data-ttu-id="0f9d1-125">型</span><span class="sxs-lookup"><span data-stu-id="0f9d1-125">Type</span></span>        | <span data-ttu-id="0f9d1-126">説明</span><span class="sxs-lookup"><span data-stu-id="0f9d1-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0f9d1-127">displayName</span><span class="sxs-lookup"><span data-stu-id="0f9d1-127">displayName</span></span>|<span data-ttu-id="0f9d1-128">String</span><span class="sxs-lookup"><span data-stu-id="0f9d1-128">String</span></span>|<span data-ttu-id="0f9d1-129">アプリケーションのカスタム名</span><span class="sxs-lookup"><span data-stu-id="0f9d1-129">Custom name of the application</span></span>|

## <a name="response"></a><span data-ttu-id="0f9d1-130">応答</span><span class="sxs-lookup"><span data-stu-id="0f9d1-130">Response</span></span>

<span data-ttu-id="0f9d1-131">成功した場合、このメソッド`201 OK`は応答コードと、応答本文で新しい[applicationserviceprincipal](../resources/applicationserviceprincipal.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0f9d1-131">If successful, this method returns a `201 OK` response code and a new [applicationServicePrincipal](../resources/applicationserviceprincipal.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0f9d1-132">例</span><span class="sxs-lookup"><span data-stu-id="0f9d1-132">Examples</span></span>

<span data-ttu-id="0f9d1-133">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="0f9d1-133">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="0f9d1-134">要求</span><span class="sxs-lookup"><span data-stu-id="0f9d1-134">Request</span></span>

<span data-ttu-id="0f9d1-135">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0f9d1-135">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0f9d1-136">応答</span><span class="sxs-lookup"><span data-stu-id="0f9d1-136">Response</span></span>

<span data-ttu-id="0f9d1-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0f9d1-137">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="0f9d1-138">ここに示す response オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="0f9d1-138">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0f9d1-139">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="0f9d1-139">All the properties will be returned from an actual call.</span></span>

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