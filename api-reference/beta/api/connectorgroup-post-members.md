---
title: コネクタをコネクタグループに追加する
description: コネクタをコネクタグループに追加するには、この API を使用します。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: c8b428ca6c724ce37116430cbae56587866c13eb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35943387"
---
# <a name="add-connector-to-connectorgroup"></a><span data-ttu-id="ed149-103">コネクタをコネクタグループに追加する</span><span class="sxs-lookup"><span data-stu-id="ed149-103">Add connector to connectorGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed149-104">コネクタをコネクタグループに追加するには、この API を使用します。</span><span class="sxs-lookup"><span data-stu-id="ed149-104">Use this API to add a connector to a connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="ed149-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ed149-105">Permissions</span></span>
<span data-ttu-id="ed149-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ed149-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed149-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ed149-108">Permission type</span></span>      | <span data-ttu-id="ed149-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ed149-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ed149-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ed149-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ed149-111">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ed149-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ed149-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ed149-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed149-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ed149-113">Not supported.</span></span>    |
|<span data-ttu-id="ed149-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ed149-114">Application</span></span> | <span data-ttu-id="ed149-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed149-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ed149-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ed149-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /connectorGroups/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="ed149-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ed149-117">Request headers</span></span>
| <span data-ttu-id="ed149-118">名前</span><span class="sxs-lookup"><span data-stu-id="ed149-118">Name</span></span>       | <span data-ttu-id="ed149-119">説明</span><span class="sxs-lookup"><span data-stu-id="ed149-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ed149-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed149-120">Authorization</span></span>  | <span data-ttu-id="ed149-121">ベアラー.</span><span class="sxs-lookup"><span data-stu-id="ed149-121">Bearer.</span></span> <span data-ttu-id="ed149-122">必須</span><span class="sxs-lookup"><span data-stu-id="ed149-122">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed149-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="ed149-123">Request body</span></span>
<span data-ttu-id="ed149-124">要求本文で、[コネクタ](../resources/connector.md)オブジェクトへのリンクの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ed149-124">In the request body, supply a JSON representation of a link to a   [connector](../resources/connector.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ed149-125">応答</span><span class="sxs-lookup"><span data-stu-id="ed149-125">Response</span></span>

<span data-ttu-id="ed149-126">成功した場合、この`201 Created`メソッドは応答コードと、応答本文で[コネクタ](../resources/connector.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ed149-126">If successful, this method returns `201 Created` response code and [connector](../resources/connector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed149-127">例</span><span class="sxs-lookup"><span data-stu-id="ed149-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ed149-128">要求</span><span class="sxs-lookup"><span data-stu-id="ed149-128">Request</span></span>
<span data-ttu-id="ed149-129">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ed149-129">Here is an example of the request.</span></span>
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
<span data-ttu-id="ed149-130">要求本文で、[コネクタ](../resources/connector.md)オブジェクトへのリンクの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ed149-130">In the request body, supply a JSON representation of a link to a  [connector](../resources/connector.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="ed149-131">応答</span><span class="sxs-lookup"><span data-stu-id="ed149-131">Response</span></span>
<span data-ttu-id="ed149-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ed149-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create connector",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
