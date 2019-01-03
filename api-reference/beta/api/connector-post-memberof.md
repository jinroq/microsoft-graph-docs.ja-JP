---
title: コネクタを connectorGroup に追加します。
description: 新しい connectorGroup にコネクタを追加するのにには、この API を使用します。
ms.openlocfilehash: 6dfc681f997953420811fbd7223a8c121934949e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070271"
---
# <a name="add-connector-to-connectorgroup"></a><span data-ttu-id="90e94-103">コネクタを connectorGroup に追加します。</span><span class="sxs-lookup"><span data-stu-id="90e94-103">Add Connector to connectorGroup</span></span>

> <span data-ttu-id="90e94-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="90e94-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="90e94-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="90e94-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="90e94-106">新しい connectorGroup にコネクタを追加するのにには、この API を使用します。</span><span class="sxs-lookup"><span data-stu-id="90e94-106">Use this API to add a connector to a new connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="90e94-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="90e94-107">Permissions</span></span>
<span data-ttu-id="90e94-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="90e94-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90e94-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="90e94-110">Permission type</span></span>      | <span data-ttu-id="90e94-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="90e94-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="90e94-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="90e94-112">Delegated (work or school account)</span></span> | <span data-ttu-id="90e94-113">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="90e94-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="90e94-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="90e94-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90e94-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="90e94-115">Not supported.</span></span>    |
|<span data-ttu-id="90e94-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="90e94-116">Application</span></span> | <span data-ttu-id="90e94-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90e94-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="90e94-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="90e94-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /connectors/{id}/memberOf

```
## <a name="request-headers"></a><span data-ttu-id="90e94-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="90e94-119">Request headers</span></span>
| <span data-ttu-id="90e94-120">名前</span><span class="sxs-lookup"><span data-stu-id="90e94-120">Name</span></span>       | <span data-ttu-id="90e94-121">説明</span><span class="sxs-lookup"><span data-stu-id="90e94-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="90e94-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="90e94-122">Authorization</span></span>  | <span data-ttu-id="90e94-123">ベアラーです。</span><span class="sxs-lookup"><span data-stu-id="90e94-123">Bearer.</span></span> <span data-ttu-id="90e94-124">必須</span><span class="sxs-lookup"><span data-stu-id="90e94-124">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="90e94-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="90e94-125">Request body</span></span>
<span data-ttu-id="90e94-126">要求の本文には、 [connectorGroup](../resources/connectorgroup.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="90e94-126">In the request body, supply a JSON representation of [connectorGroup](../resources/connectorgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="90e94-127">応答</span><span class="sxs-lookup"><span data-stu-id="90e94-127">Response</span></span>

<span data-ttu-id="90e94-128">かどうかは成功すると、このメソッドを返します`201 Created`、応答の本体で応答コードと[connectorGroup](../resources/connectorgroup.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="90e94-128">If successful, this method returns `201 Created` response code and [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90e94-129">例</span><span class="sxs-lookup"><span data-stu-id="90e94-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="90e94-130">要求</span><span class="sxs-lookup"><span data-stu-id="90e94-130">Request</span></span>
<span data-ttu-id="90e94-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="90e94-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_connectorgroup_from_connector"
}-->
```http
POST https://graph.microsoft.com/{ver}/connectors/{id}/memberOf
Content-type: application/json
Content-length: 99

{
  "@odata.id": "https://graph.microsoft.com/{ver}/connectorGroups/{id}"
}
```
<span data-ttu-id="90e94-132">要求の本文には、 [connectorGroup](../resources/connectorgroup.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="90e94-132">In the request body, supply a JSON representation of [connectorGroup](../resources/connectorgroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="90e94-133">応答</span><span class="sxs-lookup"><span data-stu-id="90e94-133">Response</span></span>
<span data-ttu-id="90e94-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="90e94-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectorGroup"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 119

{
  "id": "id-value",
  "name": "name-value",
  "connectorGroupType": "connectorGroupType-value",
  "isDefault": false
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create connectorGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->