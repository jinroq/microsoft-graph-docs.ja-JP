---
title: directoryObject を取得する
description: directoryObject オブジェクトのプロパティとリレーションシップを取得します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6ab9543469d5ad9618c4cf2f476c33ba866ed08e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514412"
---
# <a name="get-directoryobject"></a><span data-ttu-id="1dc8f-103">directoryObject を取得する</span><span class="sxs-lookup"><span data-stu-id="1dc8f-103">Get directoryObject</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1dc8f-104">プロパティと directoryobject オブジェクトの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="1dc8f-104">Retrieve the properties and relationships of directoryobject object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1dc8f-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1dc8f-105">Permissions</span></span>
<span data-ttu-id="1dc8f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1dc8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1dc8f-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1dc8f-108">Permission type</span></span>      | <span data-ttu-id="1dc8f-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1dc8f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1dc8f-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1dc8f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1dc8f-111">Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1dc8f-111">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1dc8f-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1dc8f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1dc8f-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1dc8f-113">Not supported.</span></span>    |
|<span data-ttu-id="1dc8f-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1dc8f-114">Application</span></span> | <span data-ttu-id="1dc8f-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="1dc8f-115">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1dc8f-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1dc8f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryObjects/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1dc8f-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="1dc8f-117">Optional query parameters</span></span>
<span data-ttu-id="1dc8f-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="1dc8f-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1dc8f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1dc8f-119">Request headers</span></span>
| <span data-ttu-id="1dc8f-120">名前</span><span class="sxs-lookup"><span data-stu-id="1dc8f-120">Name</span></span>       | <span data-ttu-id="1dc8f-121">型</span><span class="sxs-lookup"><span data-stu-id="1dc8f-121">Type</span></span> | <span data-ttu-id="1dc8f-122">説明</span><span class="sxs-lookup"><span data-stu-id="1dc8f-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1dc8f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1dc8f-123">Authorization</span></span>  | <span data-ttu-id="1dc8f-124">string</span><span class="sxs-lookup"><span data-stu-id="1dc8f-124">string</span></span>  | <span data-ttu-id="1dc8f-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1dc8f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1dc8f-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="1dc8f-127">Request body</span></span>
<span data-ttu-id="1dc8f-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1dc8f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1dc8f-129">応答</span><span class="sxs-lookup"><span data-stu-id="1dc8f-129">Response</span></span>

<span data-ttu-id="1dc8f-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1dc8f-130">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1dc8f-131">例</span><span class="sxs-lookup"><span data-stu-id="1dc8f-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1dc8f-132">要求</span><span class="sxs-lookup"><span data-stu-id="1dc8f-132">Request</span></span>
<span data-ttu-id="1dc8f-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1dc8f-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directoryobject"
}-->
```http
GET https://graph.microsoft.com/beta/directoryObjects/{id}
```
##### <a name="response"></a><span data-ttu-id="1dc8f-134">応答</span><span class="sxs-lookup"><span data-stu-id="1dc8f-134">Response</span></span>
<span data-ttu-id="1dc8f-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1dc8f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 22

{
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get directoryObject",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directoryobject-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
