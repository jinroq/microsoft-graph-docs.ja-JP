---
title: directoryRoleTemplate を取得する
description: directoryroletemplate オブジェクトのプロパティと関係を取得します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f41b0fe0e23b6b5595a789a8d03b95a5c8ce6e5b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33325923"
---
# <a name="get-directoryroletemplate"></a><span data-ttu-id="2be0b-103">directoryRoleTemplate を取得する</span><span class="sxs-lookup"><span data-stu-id="2be0b-103">Get directoryRoleTemplate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2be0b-104">directoryroletemplate オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="2be0b-104">Retrieve the properties and relationships of a directoryroletemplate object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2be0b-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2be0b-105">Permissions</span></span>
<span data-ttu-id="2be0b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2be0b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2be0b-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2be0b-108">Permission type</span></span>      | <span data-ttu-id="2be0b-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2be0b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2be0b-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2be0b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2be0b-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2be0b-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2be0b-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2be0b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2be0b-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2be0b-113">Not supported.</span></span>    |
|<span data-ttu-id="2be0b-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2be0b-114">Application</span></span> | <span data-ttu-id="2be0b-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2be0b-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2be0b-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2be0b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoleTemplates/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2be0b-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="2be0b-117">Optional query parameters</span></span>
<span data-ttu-id="2be0b-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポート**していません** (例: $filter はここではサポートされていません)。</span><span class="sxs-lookup"><span data-stu-id="2be0b-118">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="2be0b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2be0b-119">Request headers</span></span>
| <span data-ttu-id="2be0b-120">名前</span><span class="sxs-lookup"><span data-stu-id="2be0b-120">Name</span></span>       | <span data-ttu-id="2be0b-121">型</span><span class="sxs-lookup"><span data-stu-id="2be0b-121">Type</span></span> | <span data-ttu-id="2be0b-122">説明</span><span class="sxs-lookup"><span data-stu-id="2be0b-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2be0b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2be0b-123">Authorization</span></span>  | <span data-ttu-id="2be0b-124">string</span><span class="sxs-lookup"><span data-stu-id="2be0b-124">string</span></span>  | <span data-ttu-id="2be0b-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2be0b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2be0b-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="2be0b-127">Request body</span></span>
<span data-ttu-id="2be0b-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2be0b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2be0b-129">応答</span><span class="sxs-lookup"><span data-stu-id="2be0b-129">Response</span></span>

<span data-ttu-id="2be0b-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryRoleTemplate](../resources/directoryroletemplate.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2be0b-130">If successful, this method returns a `200 OK` response code and [directoryRoleTemplate](../resources/directoryroletemplate.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2be0b-131">例</span><span class="sxs-lookup"><span data-stu-id="2be0b-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2be0b-132">要求</span><span class="sxs-lookup"><span data-stu-id="2be0b-132">Request</span></span>
<span data-ttu-id="2be0b-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2be0b-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directoryroletemplate"
}-->
```http
GET https://graph.microsoft.com/beta/directoryRoleTemplates/{id}
```
##### <a name="response"></a><span data-ttu-id="2be0b-134">応答</span><span class="sxs-lookup"><span data-stu-id="2be0b-134">Response</span></span>
<span data-ttu-id="2be0b-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2be0b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRoleTemplate"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 98

{
  "description": "description-value",
  "displayName": "displayName-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get directoryRoleTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
