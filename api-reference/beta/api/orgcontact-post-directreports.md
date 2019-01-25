---
title: DirectReport を作成します。
description: この API を使用すると、新しい directReport を作成します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 44a31857619100646536eb7e4ad68d51bade851a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526852"
---
# <a name="create-directreport"></a><span data-ttu-id="429eb-103">DirectReport を作成します。</span><span class="sxs-lookup"><span data-stu-id="429eb-103">Create directReport</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="429eb-104">この API を使用すると、新しい directReport を作成します。</span><span class="sxs-lookup"><span data-stu-id="429eb-104">Use this API to create a new directReport.</span></span>
## <a name="permissions"></a><span data-ttu-id="429eb-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="429eb-105">Permissions</span></span>
<span data-ttu-id="429eb-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="429eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="429eb-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="429eb-108">Permission type</span></span>      | <span data-ttu-id="429eb-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="429eb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="429eb-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="429eb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="429eb-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="429eb-111">Not supported.</span></span>    |
|<span data-ttu-id="429eb-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="429eb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="429eb-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="429eb-113">Not supported.</span></span>    |
|<span data-ttu-id="429eb-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="429eb-114">Application</span></span> | <span data-ttu-id="429eb-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="429eb-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="429eb-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="429eb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/directReports

```
## <a name="request-headers"></a><span data-ttu-id="429eb-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="429eb-117">Request headers</span></span>
| <span data-ttu-id="429eb-118">名前</span><span class="sxs-lookup"><span data-stu-id="429eb-118">Name</span></span>       | <span data-ttu-id="429eb-119">型</span><span class="sxs-lookup"><span data-stu-id="429eb-119">Type</span></span> | <span data-ttu-id="429eb-120">説明</span><span class="sxs-lookup"><span data-stu-id="429eb-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="429eb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="429eb-121">Authorization</span></span>  | <span data-ttu-id="429eb-122">string</span><span class="sxs-lookup"><span data-stu-id="429eb-122">string</span></span>  | <span data-ttu-id="429eb-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="429eb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="429eb-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="429eb-125">Request body</span></span>
<span data-ttu-id="429eb-126">要求本文で、[directoryObject](../resources/directoryobject.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="429eb-126">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="429eb-127">応答</span><span class="sxs-lookup"><span data-stu-id="429eb-127">Response</span></span>

<span data-ttu-id="429eb-128">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="429eb-128">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="429eb-129">例</span><span class="sxs-lookup"><span data-stu-id="429eb-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="429eb-130">要求</span><span class="sxs-lookup"><span data-stu-id="429eb-130">Request</span></span>
<span data-ttu-id="429eb-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="429eb-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_orgcontact"
}-->
```http
POST https://graph.microsoft.com/beta/contacts/{id}/directReports
Content-type: application/json
Content-length: 30

{
  "directoryObject": {
  }
}
```
<span data-ttu-id="429eb-132">要求本文で、[directoryObject](../resources/directoryobject.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="429eb-132">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="429eb-133">応答</span><span class="sxs-lookup"><span data-stu-id="429eb-133">Response</span></span>
<span data-ttu-id="429eb-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="429eb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create directReport",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/orgcontact-post-directreports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
