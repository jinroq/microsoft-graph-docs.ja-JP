---
title: licenseDetails を一覧表示する
description: licensedetails オブジェクトの一覧を取得します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 44402c4e673af2d1cce04e02ee7663f152d352e0
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33329932"
---
# <a name="list-licensedetails"></a><span data-ttu-id="05760-103">licenseDetails を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="05760-103">List licenseDetails</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05760-104">licensedetails オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="05760-104">Retrieve a list of licenseDetails objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="05760-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="05760-105">Permissions</span></span>
<span data-ttu-id="05760-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="05760-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05760-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="05760-108">Permission type</span></span>      | <span data-ttu-id="05760-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="05760-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="05760-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="05760-110">Delegated (work or school account)</span></span> | <span data-ttu-id="05760-111">directory.accessasuser.all、すべてのユーザーが読み取り、すべてのディレクトリを取得します。すべてのユーザーが参照します。すべてのディレクトリ。</span><span class="sxs-lookup"><span data-stu-id="05760-111">User.Read, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="05760-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="05760-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05760-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="05760-113">User.Read</span></span>    |
|<span data-ttu-id="05760-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="05760-114">Application</span></span> | <span data-ttu-id="05760-115">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05760-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="05760-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="05760-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/licenseDetails
GET /users/{id}/licenseDetails
```
## <a name="optional-query-parameters"></a><span data-ttu-id="05760-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="05760-117">Optional query parameters</span></span>
<span data-ttu-id="05760-118">このメソッドは、 [OData クエリパラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートし**ていません**。</span><span class="sxs-lookup"><span data-stu-id="05760-118">This method does **not** support [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="05760-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="05760-119">Request headers</span></span>
| <span data-ttu-id="05760-120">名前</span><span class="sxs-lookup"><span data-stu-id="05760-120">Name</span></span>      |<span data-ttu-id="05760-121">説明</span><span class="sxs-lookup"><span data-stu-id="05760-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="05760-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="05760-122">Authorization</span></span>  | <span data-ttu-id="05760-123">ベアラー &lt;コード&gt;</span><span class="sxs-lookup"><span data-stu-id="05760-123">Bearer &lt;code&gt;</span></span>|

## <a name="request-body"></a><span data-ttu-id="05760-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="05760-124">Request body</span></span>
<span data-ttu-id="05760-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="05760-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="05760-126">応答</span><span class="sxs-lookup"><span data-stu-id="05760-126">Response</span></span>

<span data-ttu-id="05760-127">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[licensedetails](../resources/licensedetails.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="05760-127">If successful, this method returns a `200 OK` response code and collection of [licenseDetails](../resources/licensedetails.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="05760-128">例</span><span class="sxs-lookup"><span data-stu-id="05760-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="05760-129">要求</span><span class="sxs-lookup"><span data-stu-id="05760-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_licensedetails"
}-->
```http
GET https://graph.microsoft.com/beta/me/licenseDetails
```
##### <a name="response"></a><span data-ttu-id="05760-130">応答</span><span class="sxs-lookup"><span data-stu-id="05760-130">Response</span></span>
<span data-ttu-id="05760-p102">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="05760-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.licenseDetails",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 389

{
  "value": [
    {
      "servicePlans": [
        {
          "servicePlanId": "servicePlanId-value",
          "servicePlanName": "servicePlanName-value",
          "provisioningStatus": "provisioningStatus-value",
          "appliesTo": "appliesTo-value"
        }
      ],
      "skuId": "skuId-value",
      "skuPartNumber": "skuPartNumber-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List licenseDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
