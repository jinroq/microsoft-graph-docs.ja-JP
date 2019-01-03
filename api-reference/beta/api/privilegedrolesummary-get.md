---
title: PrivilegedRoleSummary を取得します。
description: プロパティと privilegedRoleSummary オブジェクトの関係を取得します。
ms.openlocfilehash: 8be8fd91cbe3601953cfc0a760e31ca49ae1cf56
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072027"
---
# <a name="get-privilegedrolesummary"></a><span data-ttu-id="02a10-103">PrivilegedRoleSummary を取得します。</span><span class="sxs-lookup"><span data-stu-id="02a10-103">Get privilegedRoleSummary</span></span>

> <span data-ttu-id="02a10-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="02a10-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="02a10-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="02a10-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="02a10-106">プロパティと[privilegedRoleSummary](../resources/privilegedrolesummary.md)オブジェクトの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="02a10-106">Retrieve the properties and relationships of [privilegedRoleSummary](../resources/privilegedrolesummary.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="02a10-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="02a10-107">Permissions</span></span>
<span data-ttu-id="02a10-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="02a10-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="02a10-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="02a10-110">Permission type</span></span>      | <span data-ttu-id="02a10-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="02a10-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02a10-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="02a10-112">Delegated (work or school account)</span></span> | <span data-ttu-id="02a10-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="02a10-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="02a10-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="02a10-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02a10-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="02a10-115">Not supported.</span></span>    |
|<span data-ttu-id="02a10-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="02a10-116">Application</span></span> | <span data-ttu-id="02a10-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="02a10-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="02a10-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="02a10-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}?$expand=summary
```
## <a name="optional-query-parameters"></a><span data-ttu-id="02a10-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="02a10-119">Optional query parameters</span></span>
<span data-ttu-id="02a10-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="02a10-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="02a10-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="02a10-121">Request headers</span></span>
| <span data-ttu-id="02a10-122">名前</span><span class="sxs-lookup"><span data-stu-id="02a10-122">Name</span></span>      |<span data-ttu-id="02a10-123">説明</span><span class="sxs-lookup"><span data-stu-id="02a10-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="02a10-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="02a10-124">Authorization</span></span>  | <span data-ttu-id="02a10-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="02a10-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="02a10-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="02a10-127">Request body</span></span>
<span data-ttu-id="02a10-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="02a10-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="02a10-129">応答</span><span class="sxs-lookup"><span data-stu-id="02a10-129">Response</span></span>

<span data-ttu-id="02a10-130">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[privilegedRoleSummary](../resources/privilegedrolesummary.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="02a10-130">If successful, this method returns a `200 OK` response code and [privilegedRoleSummary](../resources/privilegedrolesummary.md) object in the response body.</span></span>

<span data-ttu-id="02a10-131">テナントの PIM を登録する必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="02a10-131">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="02a10-132">それ以外の場合、HTTP 403 アクセス不可の状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="02a10-132">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="02a10-133">例</span><span class="sxs-lookup"><span data-stu-id="02a10-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="02a10-134">要求</span><span class="sxs-lookup"><span data-stu-id="02a10-134">Request</span></span>
<span data-ttu-id="02a10-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="02a10-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedrolesummary"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/summary
```
##### <a name="response"></a><span data-ttu-id="02a10-136">応答</span><span class="sxs-lookup"><span data-stu-id="02a10-136">Response</span></span>
<span data-ttu-id="02a10-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="02a10-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleSummary"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 137

{
  "id": "id-value",
  "status": "status-value",
  "usersCount": 99,
  "managedCount": 99,
  "elevatedCount": 99,
  "mfaEnabled": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get privilegedRoleSummary",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->