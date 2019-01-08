---
title: リスト privilegedApproval
description: Privilegedapproval オブジェクトのリストを取得します。
ms.openlocfilehash: 35b3e2cf6b4034731c8ddf9d1af41e129acbfe3f
ms.sourcegitcommit: 37591c2299c80e7675cd2b5f781e1eeeba628a60
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/08/2019
ms.locfileid: "27748172"
---
# <a name="list-privilegedapproval"></a><span data-ttu-id="5eea3-103">リスト privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="5eea3-103">List privilegedApproval</span></span>

> <span data-ttu-id="5eea3-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5eea3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5eea3-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5eea3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5eea3-106">Privilegedapproval オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="5eea3-106">Retrieve a list of privilegedapproval objects.</span></span>

<span data-ttu-id="5eea3-107">クエリの結果をフィルターするには、標準の OData を使用して、 ``$filter`` 、Uri で表現します。</span><span class="sxs-lookup"><span data-stu-id="5eea3-107">To filter the results from the query, use the standard OData ``$filter`` expressions in the URIs.</span></span>
## <a name="permissions"></a><span data-ttu-id="5eea3-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5eea3-108">Permissions</span></span>
<span data-ttu-id="5eea3-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5eea3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5eea3-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5eea3-111">Permission type</span></span>      | <span data-ttu-id="5eea3-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5eea3-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5eea3-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5eea3-113">Delegated (work or school account)</span></span> | <span data-ttu-id="5eea3-114">PrivilegedAccess.ReadWrite.AzureAD、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5eea3-114">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5eea3-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5eea3-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5eea3-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5eea3-116">Not supported.</span></span>    |
|<span data-ttu-id="5eea3-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5eea3-117">Application</span></span> | <span data-ttu-id="5eea3-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5eea3-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5eea3-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5eea3-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5eea3-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="5eea3-120">Optional query parameters</span></span>
<span data-ttu-id="5eea3-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="5eea3-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5eea3-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5eea3-122">Request headers</span></span>
| <span data-ttu-id="5eea3-123">名前</span><span class="sxs-lookup"><span data-stu-id="5eea3-123">Name</span></span>      |<span data-ttu-id="5eea3-124">説明</span><span class="sxs-lookup"><span data-stu-id="5eea3-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5eea3-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="5eea3-125">Authorization</span></span>  | <span data-ttu-id="5eea3-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5eea3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5eea3-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="5eea3-128">Request body</span></span>
<span data-ttu-id="5eea3-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5eea3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5eea3-130">応答</span><span class="sxs-lookup"><span data-stu-id="5eea3-130">Response</span></span>

<span data-ttu-id="5eea3-131">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[privilegedApproval](../resources/privilegedapproval.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="5eea3-131">If successful, this method returns a `200 OK` response code and collection of [privilegedApproval](../resources/privilegedapproval.md) objects in the response body.</span></span>

<span data-ttu-id="5eea3-132">テナントの PIM を登録する必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="5eea3-132">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="5eea3-133">それ以外の場合、HTTP 403 アクセス不可の状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="5eea3-133">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="5eea3-134">例</span><span class="sxs-lookup"><span data-stu-id="5eea3-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5eea3-135">要求</span><span class="sxs-lookup"><span data-stu-id="5eea3-135">Request</span></span>
<span data-ttu-id="5eea3-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5eea3-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedapproval"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedApproval
```
##### <a name="response"></a><span data-ttu-id="5eea3-137">応答</span><span class="sxs-lookup"><span data-stu-id="5eea3-137">Response</span></span>
<span data-ttu-id="5eea3-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5eea3-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
