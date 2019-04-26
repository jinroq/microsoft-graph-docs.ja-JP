---
title: コネクタをコネクタグループに追加する
description: この API を使用して、コネクタを新しいコネクタグループに追加します。
localization_priority: Normal
ms.openlocfilehash: d0357e1fc3c911111b392b783e94723e8084e44a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33327522"
---
# <a name="add-connector-to-connectorgroup"></a><span data-ttu-id="00e6d-103">コネクタをコネクタグループに追加する</span><span class="sxs-lookup"><span data-stu-id="00e6d-103">Add Connector to connectorGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00e6d-104">この API を使用して、コネクタを新しいコネクタグループに追加します。</span><span class="sxs-lookup"><span data-stu-id="00e6d-104">Use this API to add a connector to a new connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="00e6d-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="00e6d-105">Permissions</span></span>
<span data-ttu-id="00e6d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="00e6d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00e6d-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="00e6d-108">Permission type</span></span>      | <span data-ttu-id="00e6d-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="00e6d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="00e6d-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="00e6d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="00e6d-111">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="00e6d-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="00e6d-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="00e6d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00e6d-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="00e6d-113">Not supported.</span></span>    |
|<span data-ttu-id="00e6d-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="00e6d-114">Application</span></span> | <span data-ttu-id="00e6d-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00e6d-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="00e6d-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="00e6d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /connectors/{id}/memberOf

```
## <a name="request-headers"></a><span data-ttu-id="00e6d-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="00e6d-117">Request headers</span></span>
| <span data-ttu-id="00e6d-118">名前</span><span class="sxs-lookup"><span data-stu-id="00e6d-118">Name</span></span>       | <span data-ttu-id="00e6d-119">説明</span><span class="sxs-lookup"><span data-stu-id="00e6d-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="00e6d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="00e6d-120">Authorization</span></span>  | <span data-ttu-id="00e6d-121">ベアラー.</span><span class="sxs-lookup"><span data-stu-id="00e6d-121">Bearer.</span></span> <span data-ttu-id="00e6d-122">必須</span><span class="sxs-lookup"><span data-stu-id="00e6d-122">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="00e6d-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="00e6d-123">Request body</span></span>
<span data-ttu-id="00e6d-124">要求本文で、[コネクタグループ](../resources/connectorgroup.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="00e6d-124">In the request body, supply a JSON representation of [connectorGroup](../resources/connectorgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="00e6d-125">応答</span><span class="sxs-lookup"><span data-stu-id="00e6d-125">Response</span></span>

<span data-ttu-id="00e6d-126">成功した場合、この`201 Created`メソッドは応答コードと、応答本文で[コネクタグループ](../resources/connectorgroup.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="00e6d-126">If successful, this method returns `201 Created` response code and [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00e6d-127">例</span><span class="sxs-lookup"><span data-stu-id="00e6d-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="00e6d-128">要求</span><span class="sxs-lookup"><span data-stu-id="00e6d-128">Request</span></span>
<span data-ttu-id="00e6d-129">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="00e6d-129">Here is an example of the request.</span></span>
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
<span data-ttu-id="00e6d-130">要求本文で、[コネクタグループ](../resources/connectorgroup.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="00e6d-130">In the request body, supply a JSON representation of [connectorGroup](../resources/connectorgroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="00e6d-131">応答</span><span class="sxs-lookup"><span data-stu-id="00e6d-131">Response</span></span>
<span data-ttu-id="00e6d-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="00e6d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create connectorGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
