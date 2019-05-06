---
title: ディレクトリ ロールのメンバーを追加する
description: この API を使用して、新しいディレクトリ ロールのメンバーを作成します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8037ee8945b7f8bc25e2daf39dd23a2142b81045
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33590298"
---
# <a name="add-directory-role-member"></a><span data-ttu-id="b6fd8-103">ディレクトリ ロールのメンバーを追加する</span><span class="sxs-lookup"><span data-stu-id="b6fd8-103">Add directory role member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6fd8-104">この API を使用して、新しいディレクトリ ロールのメンバーを作成します。</span><span class="sxs-lookup"><span data-stu-id="b6fd8-104">Use this API to create a new directory role member.</span></span>
## <a name="permissions"></a><span data-ttu-id="b6fd8-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b6fd8-105">Permissions</span></span>
<span data-ttu-id="b6fd8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b6fd8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6fd8-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b6fd8-108">Permission type</span></span>      | <span data-ttu-id="b6fd8-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b6fd8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b6fd8-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b6fd8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b6fd8-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b6fd8-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b6fd8-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b6fd8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6fd8-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b6fd8-113">Not supported.</span></span>    |
|<span data-ttu-id="b6fd8-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b6fd8-114">Application</span></span> | <span data-ttu-id="b6fd8-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b6fd8-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b6fd8-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b6fd8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles/{id}/members/$ref

```
## <a name="request-headers"></a><span data-ttu-id="b6fd8-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b6fd8-117">Request headers</span></span>
| <span data-ttu-id="b6fd8-118">名前</span><span class="sxs-lookup"><span data-stu-id="b6fd8-118">Name</span></span>       | <span data-ttu-id="b6fd8-119">型</span><span class="sxs-lookup"><span data-stu-id="b6fd8-119">Type</span></span> | <span data-ttu-id="b6fd8-120">説明</span><span class="sxs-lookup"><span data-stu-id="b6fd8-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b6fd8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6fd8-121">Authorization</span></span>  | <span data-ttu-id="b6fd8-122">string</span><span class="sxs-lookup"><span data-stu-id="b6fd8-122">string</span></span>  | <span data-ttu-id="b6fd8-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b6fd8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b6fd8-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="b6fd8-125">Request body</span></span>
<span data-ttu-id="b6fd8-126">要求本文で、[directoryObject](../resources/directoryobject.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b6fd8-126">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b6fd8-127">応答</span><span class="sxs-lookup"><span data-stu-id="b6fd8-127">Response</span></span>

<span data-ttu-id="b6fd8-128">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b6fd8-128">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6fd8-129">例</span><span class="sxs-lookup"><span data-stu-id="b6fd8-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b6fd8-130">要求</span><span class="sxs-lookup"><span data-stu-id="b6fd8-130">Request</span></span>
<span data-ttu-id="b6fd8-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b6fd8-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryrole"
}-->
```http
POST https://graph.microsoft.com/beta/directoryRoles/{id}/members/$ref
Content-type: application/json
Content-length: 30

{
  "directoryObject": {
  }
}
```
<span data-ttu-id="b6fd8-132">要求本文に、[directoryObject](../resources/directoryobject.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b6fd8-132">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="b6fd8-133">応答</span><span class="sxs-lookup"><span data-stu-id="b6fd8-133">Response</span></span>
<span data-ttu-id="b6fd8-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b6fd8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 51

{
  "directoryObject": {
    "id": "id-value"
  }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="b6fd8-137">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="b6fd8-137">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b6fd8-138">Java</span><span class="sxs-lookup"><span data-stu-id="b6fd8-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_directoryrole-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directoryrole-post-members.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
