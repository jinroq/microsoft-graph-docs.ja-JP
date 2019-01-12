---
title: DataPolicyOperation を取得します。
description: DataPolicyOperation オブジェクトのプロパティを取得します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2f9c4608aaa8d951b5a5fed6b499643e5a4d63d0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956340"
---
# <a name="get-datapolicyoperation"></a><span data-ttu-id="87028-103">DataPolicyOperation を取得します。</span><span class="sxs-lookup"><span data-stu-id="87028-103">Get dataPolicyOperation</span></span>

<span data-ttu-id="87028-104">**DataPolicyOperation**オブジェクトのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="87028-104">Retrieve the properties of a **dataPolicyOperation** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="87028-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="87028-105">Permissions</span></span>
<span data-ttu-id="87028-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="87028-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87028-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="87028-108">Permission type</span></span>      | <span data-ttu-id="87028-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="87028-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87028-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="87028-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="87028-111">User.Export.All、User.Read.All</span><span class="sxs-lookup"><span data-stu-id="87028-111">User.Export.All, User.Read.All</span></span>  |
|<span data-ttu-id="87028-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="87028-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="87028-113">該当なし</span><span class="sxs-lookup"><span data-stu-id="87028-113">Not applicable</span></span>  |
|<span data-ttu-id="87028-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="87028-114">Application</span></span> | <span data-ttu-id="87028-115">User.Export.All、User.Read.All</span><span class="sxs-lookup"><span data-stu-id="87028-115">User.Export.All, User.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="87028-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="87028-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /dataPolicyOperations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="87028-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="87028-117">Request headers</span></span>
| <span data-ttu-id="87028-118">名前</span><span class="sxs-lookup"><span data-stu-id="87028-118">Name</span></span>      |<span data-ttu-id="87028-119">説明</span><span class="sxs-lookup"><span data-stu-id="87028-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="87028-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="87028-120">Authorization</span></span>  | <span data-ttu-id="87028-121">ベアラー {トークン}</span><span class="sxs-lookup"><span data-stu-id="87028-121">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="87028-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="87028-122">Request body</span></span>
<span data-ttu-id="87028-123">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="87028-123">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="87028-124">応答</span><span class="sxs-lookup"><span data-stu-id="87028-124">Response</span></span>
<span data-ttu-id="87028-125">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[dataPolicyOperation](../resources/datapolicyoperation.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="87028-125">If successful, this method returns a `200 OK` response code and a [dataPolicyOperation](../resources/datapolicyoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="87028-126">例</span><span class="sxs-lookup"><span data-stu-id="87028-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="87028-127">要求</span><span class="sxs-lookup"><span data-stu-id="87028-127">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_datapolicyoperation"
}-->
```http
GET https://graph.microsoft.com/v1.0/dataPolicyOperations/{id}
```
##### <a name="response"></a><span data-ttu-id="87028-128">応答</span><span class="sxs-lookup"><span data-stu-id="87028-128">Response</span></span>
><span data-ttu-id="87028-p102">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="87028-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.dataPolicyOperation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 212

{
  "completedDateTime": "datetime-value",
  "id": "id-value",
  "status": "status-value",
  "storageLocation": "storageLocation-value",
  "userId": "userId-value",
  "submittedDateTime": "datetime-value", 
  "progress": "double-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get dataPolicyOperation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
