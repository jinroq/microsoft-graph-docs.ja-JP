---
title: アプリケーションを作成する
description: この API を使用して、新しいアプリケーションを作成します。
author: VinodRavichandran
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: b86030eede69b85d7b66e4ec5acdd7e2dfef0ce4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459109"
---
# <a name="create-application"></a><span data-ttu-id="98816-103">アプリケーションを作成する</span><span class="sxs-lookup"><span data-stu-id="98816-103">Create application</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98816-104">この API を使用して、新しいアプリケーションを作成します。</span><span class="sxs-lookup"><span data-stu-id="98816-104">Use this API to create a new event.</span></span>

## <a name="permissions"></a><span data-ttu-id="98816-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="98816-105">Permissions</span></span>
<span data-ttu-id="98816-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="98816-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="98816-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="98816-108">Permission type</span></span>      | <span data-ttu-id="98816-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="98816-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="98816-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="98816-110">Delegated (work or school account)</span></span> | <span data-ttu-id="98816-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="98816-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="98816-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="98816-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98816-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="98816-113">Not supported.</span></span>    |
|<span data-ttu-id="98816-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="98816-114">Application</span></span> | <span data-ttu-id="98816-115">Application.ReadWrite.OwnedBy、Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98816-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="98816-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="98816-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications
```

## <a name="request-headers"></a><span data-ttu-id="98816-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="98816-117">Request headers</span></span>
| <span data-ttu-id="98816-118">名前</span><span class="sxs-lookup"><span data-stu-id="98816-118">Name</span></span>       | <span data-ttu-id="98816-119">型</span><span class="sxs-lookup"><span data-stu-id="98816-119">Type</span></span> | <span data-ttu-id="98816-120">説明</span><span class="sxs-lookup"><span data-stu-id="98816-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="98816-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="98816-121">Authorization</span></span>  | <span data-ttu-id="98816-122">string</span><span class="sxs-lookup"><span data-stu-id="98816-122">string</span></span>  | <span data-ttu-id="98816-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="98816-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="98816-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="98816-125">Request body</span></span>
<span data-ttu-id="98816-126">要求本文で、[application](../resources/application.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="98816-126">In the request body, supply a JSON representation of [event](../resources/application.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="98816-127">応答</span><span class="sxs-lookup"><span data-stu-id="98816-127">Response</span></span>

<span data-ttu-id="98816-128">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [application](../resources/application.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="98816-128">If successful, this method returns `201 Created` response code and [event](../resources/application.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98816-129">例</span><span class="sxs-lookup"><span data-stu-id="98816-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="98816-130">要求</span><span class="sxs-lookup"><span data-stu-id="98816-130">Request</span></span>
<span data-ttu-id="98816-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="98816-131">Here is an example of the request.</span></span>
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
<span data-ttu-id="98816-132">要求本文で、[application](../resources/application.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="98816-132">In the request body, supply a JSON representation of [calendar](../resources/application.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="98816-133">応答</span><span class="sxs-lookup"><span data-stu-id="98816-133">Response</span></span>
<span data-ttu-id="98816-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="98816-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
