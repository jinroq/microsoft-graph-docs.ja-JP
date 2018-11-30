---
title: PrivilegedApproval を取得します。
description: プロパティと privilegedapproval オブジェクトの関係を取得します。
ms.openlocfilehash: 77db18f46bbdfec6a5a9a62e4e481facaab6cb8c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072477"
---
# <a name="get-privilegedapproval"></a><span data-ttu-id="ffa11-103">PrivilegedApproval を取得します。</span><span class="sxs-lookup"><span data-stu-id="ffa11-103">Get privilegedApproval</span></span>

> <span data-ttu-id="ffa11-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ffa11-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ffa11-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ffa11-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ffa11-106">プロパティと privilegedapproval オブジェクトの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="ffa11-106">Retrieve the properties and relationships of privilegedapproval object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ffa11-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ffa11-107">Permissions</span></span>
<span data-ttu-id="ffa11-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ffa11-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ffa11-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ffa11-110">Permission type</span></span>      | <span data-ttu-id="ffa11-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ffa11-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ffa11-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ffa11-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ffa11-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ffa11-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ffa11-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ffa11-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ffa11-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ffa11-115">Not supported.</span></span>    |
|<span data-ttu-id="ffa11-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ffa11-116">Application</span></span> | <span data-ttu-id="ffa11-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ffa11-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ffa11-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ffa11-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval/<id>
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ffa11-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ffa11-119">Optional query parameters</span></span>
<span data-ttu-id="ffa11-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ffa11-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ffa11-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ffa11-121">Request headers</span></span>
| <span data-ttu-id="ffa11-122">名前</span><span class="sxs-lookup"><span data-stu-id="ffa11-122">Name</span></span>      |<span data-ttu-id="ffa11-123">説明</span><span class="sxs-lookup"><span data-stu-id="ffa11-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ffa11-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ffa11-124">Authorization</span></span>  | <span data-ttu-id="ffa11-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ffa11-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ffa11-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="ffa11-127">Request body</span></span>
<span data-ttu-id="ffa11-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ffa11-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ffa11-129">応答</span><span class="sxs-lookup"><span data-stu-id="ffa11-129">Response</span></span>

<span data-ttu-id="ffa11-130">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[privilegedApproval](../resources/privilegedapproval.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="ffa11-130">If successful, this method returns a `200 OK` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="ffa11-131">テナントの PIM を登録する必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="ffa11-131">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="ffa11-132">それ以外の場合、HTTP 403 アクセス不可の状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="ffa11-132">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="ffa11-133">例</span><span class="sxs-lookup"><span data-stu-id="ffa11-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ffa11-134">要求</span><span class="sxs-lookup"><span data-stu-id="ffa11-134">Request</span></span>
<span data-ttu-id="ffa11-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ffa11-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedapproval"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedApproval/<id>
```
##### <a name="response"></a><span data-ttu-id="ffa11-136">応答</span><span class="sxs-lookup"><span data-stu-id="ffa11-136">Response</span></span>
<span data-ttu-id="ffa11-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ffa11-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 193

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "approvalType": "approvalType-value",
  "approvalState": "approvalState-value",
  "approvalDuration": "datetime-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get privilegedApproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
