---
title: アプリケーション一覧
description: ConnectorGroup に関連付けられているアプリケーション オブジェクトのリストを取得します。
ms.openlocfilehash: 11d81454677b60e2402c4d1fe32aae5c974c1afc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070270"
---
# <a name="list-applications"></a><span data-ttu-id="ddb02-103">アプリケーション一覧</span><span class="sxs-lookup"><span data-stu-id="ddb02-103">List applications</span></span>

> <span data-ttu-id="ddb02-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ddb02-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ddb02-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ddb02-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ddb02-106">ConnectorGroup に関連付けられているアプリケーション オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="ddb02-106">Retrieve a list of application objects associated with the connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="ddb02-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ddb02-107">Permissions</span></span>
<span data-ttu-id="ddb02-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ddb02-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ddb02-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ddb02-110">Permission type</span></span>      | <span data-ttu-id="ddb02-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ddb02-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ddb02-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ddb02-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ddb02-113">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ddb02-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ddb02-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ddb02-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ddb02-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ddb02-115">Not supported.</span></span>    |
|<span data-ttu-id="ddb02-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ddb02-116">Application</span></span> | <span data-ttu-id="ddb02-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddb02-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ddb02-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ddb02-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /connectorGroups/{id}/applications
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ddb02-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ddb02-119">Optional query parameters</span></span>
<span data-ttu-id="ddb02-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ddb02-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ddb02-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ddb02-121">Request headers</span></span>
| <span data-ttu-id="ddb02-122">名前</span><span class="sxs-lookup"><span data-stu-id="ddb02-122">Name</span></span>      |<span data-ttu-id="ddb02-123">説明</span><span class="sxs-lookup"><span data-stu-id="ddb02-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ddb02-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ddb02-124">Authorization</span></span>  | <span data-ttu-id="ddb02-125">ベアラーです。</span><span class="sxs-lookup"><span data-stu-id="ddb02-125">Bearer.</span></span> <span data-ttu-id="ddb02-126">必須</span><span class="sxs-lookup"><span data-stu-id="ddb02-126">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="ddb02-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="ddb02-127">Request body</span></span>
<span data-ttu-id="ddb02-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ddb02-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ddb02-129">応答</span><span class="sxs-lookup"><span data-stu-id="ddb02-129">Response</span></span>

<span data-ttu-id="ddb02-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[アプリケーション](../resources/application.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="ddb02-130">If successful, this method returns a `200 OK` response code and collection of [application](../resources/application.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ddb02-131">例</span><span class="sxs-lookup"><span data-stu-id="ddb02-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ddb02-132">要求</span><span class="sxs-lookup"><span data-stu-id="ddb02-132">Request</span></span>
<span data-ttu-id="ddb02-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ddb02-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_applications"
}-->
```http
GET https://graph.microsoft.com/{ver}/connectorGroups/{id}/applications
```
##### <a name="response"></a><span data-ttu-id="ddb02-134">応答</span><span class="sxs-lookup"><span data-stu-id="ddb02-134">Response</span></span>
<span data-ttu-id="ddb02-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ddb02-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 420

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List applications",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->