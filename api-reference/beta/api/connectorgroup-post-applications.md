---
title: アプリケーションを作成します。
description: 新しいアプリケーションを作成するのにには、この API を使用します。
localization_priority: Normal
ms.openlocfilehash: e9d1c76f153c27ab3df24a93b44a570c2c1d836a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824669"
---
# <a name="create-application"></a><span data-ttu-id="222d9-103">アプリケーションを作成します。</span><span class="sxs-lookup"><span data-stu-id="222d9-103">Create application</span></span>

> <span data-ttu-id="222d9-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="222d9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="222d9-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="222d9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="222d9-106">新しいアプリケーションを作成するのにには、この API を使用します。</span><span class="sxs-lookup"><span data-stu-id="222d9-106">Use this API to create a new application.</span></span>
## <a name="permissions"></a><span data-ttu-id="222d9-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="222d9-107">Permissions</span></span>
<span data-ttu-id="222d9-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="222d9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="222d9-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="222d9-110">Permission type</span></span>      | <span data-ttu-id="222d9-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="222d9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="222d9-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="222d9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="222d9-113">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="222d9-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="222d9-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="222d9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="222d9-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="222d9-115">Not supported.</span></span>    |
|<span data-ttu-id="222d9-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="222d9-116">Application</span></span> | <span data-ttu-id="222d9-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="222d9-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="222d9-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="222d9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /connectorGroups/{id}/applications

```
## <a name="request-headers"></a><span data-ttu-id="222d9-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="222d9-119">Request headers</span></span>
| <span data-ttu-id="222d9-120">名前</span><span class="sxs-lookup"><span data-stu-id="222d9-120">Name</span></span>       | <span data-ttu-id="222d9-121">説明</span><span class="sxs-lookup"><span data-stu-id="222d9-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="222d9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="222d9-122">Authorization</span></span>  | <span data-ttu-id="222d9-123">ベアラーです。</span><span class="sxs-lookup"><span data-stu-id="222d9-123">Bearer.</span></span> <span data-ttu-id="222d9-124">必須</span><span class="sxs-lookup"><span data-stu-id="222d9-124">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="222d9-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="222d9-125">Request body</span></span>
<span data-ttu-id="222d9-126">要求の本文には、[アプリケーション](../resources/application.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="222d9-126">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="222d9-127">応答</span><span class="sxs-lookup"><span data-stu-id="222d9-127">Response</span></span>

<span data-ttu-id="222d9-128">かどうかは成功すると、このメソッドを返します`201 Created`、応答の本体で応答コードと[アプリケーション](../resources/application.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="222d9-128">If successful, this method returns `201 Created` response code and [application](../resources/application.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="222d9-129">例</span><span class="sxs-lookup"><span data-stu-id="222d9-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="222d9-130">要求</span><span class="sxs-lookup"><span data-stu-id="222d9-130">Request</span></span>
<span data-ttu-id="222d9-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="222d9-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_application_from_connectorgroup"
}-->
```http
POST https://graph.microsoft.com/{ver}/connectorGroups/{id}/applications
Content-type: application/json
Content-length: 329

{
  "@odata.id": "https://graph.microsoft.com/{ver}/applications/{id}"
}
```
<span data-ttu-id="222d9-132">要求の本文には、[アプリケーション](../resources/application.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="222d9-132">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="222d9-133">応答</span><span class="sxs-lookup"><span data-stu-id="222d9-133">Response</span></span>
<span data-ttu-id="222d9-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="222d9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 355

{
  "appId": "appId-value",
  "onPremisesPublishing": {
    "externalUrl": "externalUrl-value",
    "internalUrl": "internalUrl-value",
    "externalAuthenticationType": "externalAuthenticationType-value",
    "customDomainCertificate": "customDomainCertificate-value",
    "isTranslateHostHeaderEnabled": true,
    "isOnPremPublishingEnabled": true
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create application",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
