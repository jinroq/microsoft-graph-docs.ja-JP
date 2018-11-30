---
title: リスト privilegedApproval
description: Privilegedapproval オブジェクトのリストを取得します。
ms.openlocfilehash: 69e558a734f86dd72b35e61d9f8ceab52b9f981e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072919"
---
# <a name="list-privilegedapproval"></a><span data-ttu-id="51eac-103">リスト privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="51eac-103">List privilegedApproval</span></span>

> <span data-ttu-id="51eac-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="51eac-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="51eac-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="51eac-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="51eac-106">Privilegedapproval オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="51eac-106">Retrieve a list of privilegedapproval objects.</span></span>

<span data-ttu-id="51eac-107">クエリの結果をフィルターするには、標準の OData を使用して、 ``$filter`` 、Uri で表現します。</span><span class="sxs-lookup"><span data-stu-id="51eac-107">To filter the results from the query, use the standard OData ``$filter`` expressions in the URIs.</span></span>
## <a name="permissions"></a><span data-ttu-id="51eac-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="51eac-108">Permissions</span></span>
<span data-ttu-id="51eac-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="51eac-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="51eac-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="51eac-111">Permission type</span></span>      | <span data-ttu-id="51eac-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="51eac-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="51eac-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="51eac-113">Delegated (work or school account)</span></span> | <span data-ttu-id="51eac-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="51eac-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="51eac-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="51eac-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51eac-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="51eac-116">Not supported.</span></span>    |
|<span data-ttu-id="51eac-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="51eac-117">Application</span></span> | <span data-ttu-id="51eac-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="51eac-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="51eac-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="51eac-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval
```
## <a name="optional-query-parameters"></a><span data-ttu-id="51eac-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="51eac-120">Optional query parameters</span></span>
<span data-ttu-id="51eac-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="51eac-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="51eac-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="51eac-122">Request headers</span></span>
| <span data-ttu-id="51eac-123">名前</span><span class="sxs-lookup"><span data-stu-id="51eac-123">Name</span></span>      |<span data-ttu-id="51eac-124">説明</span><span class="sxs-lookup"><span data-stu-id="51eac-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="51eac-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="51eac-125">Authorization</span></span>  | <span data-ttu-id="51eac-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="51eac-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="51eac-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="51eac-128">Request body</span></span>
<span data-ttu-id="51eac-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="51eac-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51eac-130">応答</span><span class="sxs-lookup"><span data-stu-id="51eac-130">Response</span></span>

<span data-ttu-id="51eac-131">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[privilegedApproval](../resources/privilegedapproval.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="51eac-131">If successful, this method returns a `200 OK` response code and collection of [privilegedApproval](../resources/privilegedapproval.md) objects in the response body.</span></span>

<span data-ttu-id="51eac-132">テナントの PIM を登録する必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="51eac-132">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="51eac-133">それ以外の場合、HTTP 403 アクセス不可の状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="51eac-133">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="51eac-134">例</span><span class="sxs-lookup"><span data-stu-id="51eac-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="51eac-135">要求</span><span class="sxs-lookup"><span data-stu-id="51eac-135">Request</span></span>
<span data-ttu-id="51eac-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="51eac-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedapproval"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedApproval
```
##### <a name="response"></a><span data-ttu-id="51eac-137">応答</span><span class="sxs-lookup"><span data-stu-id="51eac-137">Response</span></span>
<span data-ttu-id="51eac-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="51eac-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 246

{
  "value": [
    {
      "id": "id-value",
      "userId": "userId-value",
      "roleId": "roleId-value",
      "approvalType": "approvalType-value",
      "approvalState": "approvalState-value",
      "approvalDuration": "datetime-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List privilegedApproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
