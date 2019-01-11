---
title: DataPolicyOperation を取得します。
description: DataPolicyOperation オブジェクトのプロパティを取得します。
localization_priority: Normal
ms.openlocfilehash: a06b2b119683a75516b0d51f955565276249be41
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860362"
---
# <a name="get-datapolicyoperation"></a><span data-ttu-id="79ee0-103">DataPolicyOperation を取得します。</span><span class="sxs-lookup"><span data-stu-id="79ee0-103">Get dataPolicyOperation</span></span>

<span data-ttu-id="79ee0-104">**DataPolicyOperation**オブジェクトのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="79ee0-104">Retrieve the properties of a **dataPolicyOperation** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="79ee0-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="79ee0-105">Permissions</span></span>
<span data-ttu-id="79ee0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="79ee0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79ee0-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="79ee0-108">Permission type</span></span>      | <span data-ttu-id="79ee0-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="79ee0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="79ee0-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="79ee0-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="79ee0-111">User.Export.All、User.Read.All</span><span class="sxs-lookup"><span data-stu-id="79ee0-111">User.Export.All, User.Read.All</span></span>  |
|<span data-ttu-id="79ee0-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="79ee0-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="79ee0-113">該当なし</span><span class="sxs-lookup"><span data-stu-id="79ee0-113">Not applicable</span></span>  |
|<span data-ttu-id="79ee0-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="79ee0-114">Application</span></span> | <span data-ttu-id="79ee0-115">User.Export.All、User.Read.All</span><span class="sxs-lookup"><span data-stu-id="79ee0-115">User.Export.All, User.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="79ee0-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="79ee0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /dataPolicyOperations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="79ee0-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="79ee0-117">Request headers</span></span>
| <span data-ttu-id="79ee0-118">名前</span><span class="sxs-lookup"><span data-stu-id="79ee0-118">Name</span></span>      |<span data-ttu-id="79ee0-119">説明</span><span class="sxs-lookup"><span data-stu-id="79ee0-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="79ee0-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="79ee0-120">Authorization</span></span>  | <span data-ttu-id="79ee0-121">ベアラー {トークン}</span><span class="sxs-lookup"><span data-stu-id="79ee0-121">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="79ee0-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="79ee0-122">Request body</span></span>
<span data-ttu-id="79ee0-123">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="79ee0-123">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="79ee0-124">応答</span><span class="sxs-lookup"><span data-stu-id="79ee0-124">Response</span></span>
<span data-ttu-id="79ee0-125">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[dataPolicyOperation](../resources/datapolicyoperation.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="79ee0-125">If successful, this method returns a `200 OK` response code and a [dataPolicyOperation](../resources/datapolicyoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="79ee0-126">例</span><span class="sxs-lookup"><span data-stu-id="79ee0-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="79ee0-127">要求</span><span class="sxs-lookup"><span data-stu-id="79ee0-127">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_datapolicyoperation"
}-->
```http
GET https://graph.microsoft.com/v1.0/dataPolicyOperations/{id}
```
##### <a name="response"></a><span data-ttu-id="79ee0-128">応答</span><span class="sxs-lookup"><span data-stu-id="79ee0-128">Response</span></span>
><span data-ttu-id="79ee0-p102">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="79ee0-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
