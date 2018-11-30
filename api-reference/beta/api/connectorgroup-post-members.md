---
title: コネクタを connectorGroup に追加します。
description: ConnectorGroup にコネクタを追加するのにには、この API を使用します。
ms.openlocfilehash: f5e7330dd5476daacda47a78400181ad3ebc0e2b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068941"
---
# <a name="add-connector-to-connectorgroup"></a><span data-ttu-id="d9f35-103">コネクタを connectorGroup に追加します。</span><span class="sxs-lookup"><span data-stu-id="d9f35-103">Add connector to connectorGroup</span></span>

> <span data-ttu-id="d9f35-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d9f35-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d9f35-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d9f35-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d9f35-106">ConnectorGroup にコネクタを追加するのにには、この API を使用します。</span><span class="sxs-lookup"><span data-stu-id="d9f35-106">Use this API to add a connector to a connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="d9f35-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d9f35-107">Permissions</span></span>
<span data-ttu-id="d9f35-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d9f35-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9f35-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d9f35-110">Permission type</span></span>      | <span data-ttu-id="d9f35-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d9f35-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9f35-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d9f35-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d9f35-113">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d9f35-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d9f35-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d9f35-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9f35-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d9f35-115">Not supported.</span></span>    |
|<span data-ttu-id="d9f35-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d9f35-116">Application</span></span> | <span data-ttu-id="d9f35-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9f35-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d9f35-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d9f35-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /connectorGroups/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="d9f35-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d9f35-119">Request headers</span></span>
| <span data-ttu-id="d9f35-120">名前</span><span class="sxs-lookup"><span data-stu-id="d9f35-120">Name</span></span>       | <span data-ttu-id="d9f35-121">説明</span><span class="sxs-lookup"><span data-stu-id="d9f35-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d9f35-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9f35-122">Authorization</span></span>  | <span data-ttu-id="d9f35-123">ベアラーです。</span><span class="sxs-lookup"><span data-stu-id="d9f35-123">Bearer.</span></span> <span data-ttu-id="d9f35-124">必須</span><span class="sxs-lookup"><span data-stu-id="d9f35-124">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9f35-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="d9f35-125">Request body</span></span>
<span data-ttu-id="d9f35-126">要求の本文には、[コネクタ](../resources/connector.md)オブジェクトへのリンクの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="d9f35-126">In the request body, supply a JSON representation of a link to a   [connector](../resources/connector.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d9f35-127">応答</span><span class="sxs-lookup"><span data-stu-id="d9f35-127">Response</span></span>

<span data-ttu-id="d9f35-128">かどうかは成功すると、このメソッドを返します`201 Created`、応答の本体で応答コードと[コネクタ](../resources/connector.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="d9f35-128">If successful, this method returns `201 Created` response code and [connector](../resources/connector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9f35-129">例</span><span class="sxs-lookup"><span data-stu-id="d9f35-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d9f35-130">要求</span><span class="sxs-lookup"><span data-stu-id="d9f35-130">Request</span></span>
<span data-ttu-id="d9f35-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d9f35-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_connector_from_connectorgroup"
}-->
```http
POST https://graph.microsoft.com/{ver}/connectorGroups/{id}/members/$ref
Content-type: application/json
Content-length: 104

{
  "@odata.id": "https://graph.microsoft.com/{ver}/connector/{id}"
}
```
<span data-ttu-id="d9f35-132">要求の本文には、[コネクタ](../resources/connector.md)オブジェクトへのリンクの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="d9f35-132">In the request body, supply a JSON representation of a link to a  [connector](../resources/connector.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="d9f35-133">応答</span><span class="sxs-lookup"><span data-stu-id="d9f35-133">Response</span></span>
<span data-ttu-id="d9f35-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d9f35-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connector"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 124

{
  "id": "id-value",
  "machineName": "machineName-value",
  "externalIp": "externalIp-value",
  "status": "status-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create connector",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
