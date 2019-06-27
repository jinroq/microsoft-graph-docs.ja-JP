---
title: アプリケーションを作成する
description: この API を使用して、新しいアプリケーションを作成します。
author: VinodRavichandran
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: a9cf7f8888ee8026a3a98d2816c64c82c8f45b1e
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258444"
---
# <a name="create-application"></a><span data-ttu-id="fbf0b-103">アプリケーションを作成する</span><span class="sxs-lookup"><span data-stu-id="fbf0b-103">Create Application</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fbf0b-104">この API を使用して、新しいアプリケーションを作成します。</span><span class="sxs-lookup"><span data-stu-id="fbf0b-104">Use this API to create a new application.</span></span>

## <a name="permissions"></a><span data-ttu-id="fbf0b-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fbf0b-105">Permissions</span></span>
<span data-ttu-id="fbf0b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fbf0b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="fbf0b-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fbf0b-108">Permission type</span></span>      | <span data-ttu-id="fbf0b-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fbf0b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fbf0b-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fbf0b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fbf0b-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fbf0b-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fbf0b-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fbf0b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fbf0b-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fbf0b-113">Not supported.</span></span>    |
|<span data-ttu-id="fbf0b-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fbf0b-114">Application</span></span> | <span data-ttu-id="fbf0b-115">Application.ReadWrite.OwnedBy、Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbf0b-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fbf0b-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fbf0b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications
```

## <a name="request-headers"></a><span data-ttu-id="fbf0b-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fbf0b-117">Request headers</span></span>
| <span data-ttu-id="fbf0b-118">名前</span><span class="sxs-lookup"><span data-stu-id="fbf0b-118">Name</span></span>       | <span data-ttu-id="fbf0b-119">型</span><span class="sxs-lookup"><span data-stu-id="fbf0b-119">Type</span></span> | <span data-ttu-id="fbf0b-120">説明</span><span class="sxs-lookup"><span data-stu-id="fbf0b-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fbf0b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fbf0b-121">Authorization</span></span>  | <span data-ttu-id="fbf0b-122">string</span><span class="sxs-lookup"><span data-stu-id="fbf0b-122">string</span></span>  | <span data-ttu-id="fbf0b-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="fbf0b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fbf0b-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="fbf0b-125">Request body</span></span>
<span data-ttu-id="fbf0b-126">要求本文で、[application](../resources/application.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="fbf0b-126">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="fbf0b-127">応答</span><span class="sxs-lookup"><span data-stu-id="fbf0b-127">Response</span></span>

<span data-ttu-id="fbf0b-128">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [application](../resources/application.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="fbf0b-128">If successful, this method returns `201 Created` response code and [application](../resources/application.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbf0b-129">例</span><span class="sxs-lookup"><span data-stu-id="fbf0b-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fbf0b-130">要求</span><span class="sxs-lookup"><span data-stu-id="fbf0b-130">Request</span></span>
<span data-ttu-id="fbf0b-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fbf0b-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_application_from_applications"
}-->
```http
POST https://graph.microsoft.com/beta/applications
Content-type: application/json
Content-length: 67

{
  "allowPublicClient": true,
  "displayName": "Display name"
}
```
<span data-ttu-id="fbf0b-132">要求本文で、[application](../resources/application.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="fbf0b-132">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="fbf0b-133">応答</span><span class="sxs-lookup"><span data-stu-id="fbf0b-133">Response</span></span>
<span data-ttu-id="fbf0b-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fbf0b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 1145

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#applications/$entity",
    "id": "b5b2920e-a47c-43b7-91ef-25ae96fddddd",
    "deletedDateTime": null,
    "api": {
        "acceptedAccessTokenVersion": 2,
        "publishedPermissionScopes": []
    },
    "allowPublicClient": true,
    "applicationAliases": [],
    "appRoles": [],
    "createdDateTime": "2017-05-25T16:33:04.3646617Z",
    "installedClients": {
        "redirectUrls": []
    },
    "displayName": "Display name",
    "info": {
        "termsOfServiceUrl": null,
        "supportUrl": null,
        "privacyStatementUrl": null,
        "marketingUrl": null,
        "logoUrl": null
    },
    "keyCredentials": [],
    "orgRestrictions": [],
    "passwordCredentials": [],
    "preAuthorizedApplications": [],
    "requiredResourceAccess": [],
    "tags": [],
    "web": {
        "redirectUrls": [],
        "logoutUrl": null,
        "oauth2AllowImplicitFlow": null
    }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="fbf0b-137">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="fbf0b-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="fbf0b-138">C#</span><span class="sxs-lookup"><span data-stu-id="fbf0b-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_application_from_applications-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fbf0b-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="fbf0b-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_application_from_applications-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="fbf0b-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fbf0b-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_application_from_applications-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/application-post-applications.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/application-post-applications.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/application-post-applications.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
