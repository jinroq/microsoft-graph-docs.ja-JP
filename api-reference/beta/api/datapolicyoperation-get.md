---
title: dataPolicyOperation を取得する
description: dataPolicyOperation オブジェクトのプロパティを取得します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5fff5d25ed83c6cfdf889c364630399acdeecb9e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32455263"
---
# <a name="get-datapolicyoperation"></a><span data-ttu-id="baedf-103">dataPolicyOperation を取得する</span><span class="sxs-lookup"><span data-stu-id="baedf-103">Get dataPolicyOperation</span></span>

<span data-ttu-id="baedf-104">dataPolicyOperation オブジェクトのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="baedf-104">Retrieve the properties of the dataPolicyOperation object.</span></span>

## <a name="permissions"></a><span data-ttu-id="baedf-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="baedf-105">Permissions</span></span>
<span data-ttu-id="baedf-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="baedf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="baedf-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="baedf-108">Permission type</span></span>      | <span data-ttu-id="baedf-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="baedf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="baedf-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="baedf-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="baedf-111">すべてのユーザーとユーザーの. すべてをエクスポートします。</span><span class="sxs-lookup"><span data-stu-id="baedf-111">User.Export.All and User.Read.All</span></span>  |
|<span data-ttu-id="baedf-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="baedf-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="baedf-113">該当なし</span><span class="sxs-lookup"><span data-stu-id="baedf-113">Not applicable</span></span>  |
|<span data-ttu-id="baedf-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="baedf-114">Application</span></span> | <span data-ttu-id="baedf-115">すべてのユーザーとユーザーの. すべてをエクスポートします。</span><span class="sxs-lookup"><span data-stu-id="baedf-115">User.Export.All and User.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="baedf-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="baedf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /dataPolicyOperations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="baedf-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="baedf-117">Request headers</span></span>
| <span data-ttu-id="baedf-118">名前</span><span class="sxs-lookup"><span data-stu-id="baedf-118">Name</span></span>      |<span data-ttu-id="baedf-119">説明</span><span class="sxs-lookup"><span data-stu-id="baedf-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="baedf-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="baedf-120">Authorization</span></span>  | <span data-ttu-id="baedf-121">ベアラー {トークン}</span><span class="sxs-lookup"><span data-stu-id="baedf-121">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="baedf-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="baedf-122">Request body</span></span>
<span data-ttu-id="baedf-123">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="baedf-123">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="baedf-124">応答</span><span class="sxs-lookup"><span data-stu-id="baedf-124">Response</span></span>
<span data-ttu-id="baedf-125">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[dataPolicyOperation](../resources/datapolicyoperation.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="baedf-125">If successful, this method returns a `200 OK` response code and [dataPolicyOperation](../resources/datapolicyoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="baedf-126">例</span><span class="sxs-lookup"><span data-stu-id="baedf-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="baedf-127">要求</span><span class="sxs-lookup"><span data-stu-id="baedf-127">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_datapolicyoperation"
}-->
```http
GET https://graph.microsoft.com/beta/dataPolicyOperations/{id}
```
##### <a name="response"></a><span data-ttu-id="baedf-128">応答</span><span class="sxs-lookup"><span data-stu-id="baedf-128">Response</span></span>
<span data-ttu-id="baedf-p102">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="baedf-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "progress": "progress-value"
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
