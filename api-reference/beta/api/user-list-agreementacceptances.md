---
title: リスト agreementAcceptances
description: ユーザーの agreementAcceptance オブジェクトのリストを取得します。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fb92ff6c4a59b266735c09ed8e9d902813f5012f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953596"
---
# <a name="list-agreementacceptances"></a><span data-ttu-id="13a57-103">リスト agreementAcceptances</span><span class="sxs-lookup"><span data-stu-id="13a57-103">List agreementAcceptances</span></span>

> <span data-ttu-id="13a57-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="13a57-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="13a57-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="13a57-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="13a57-106">ユーザーの[agreementAcceptance](../resources/agreementacceptance.md)オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="13a57-106">Retrieve a list of a user's [agreementAcceptance](../resources/agreementacceptance.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="13a57-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="13a57-107">Permissions</span></span>
<span data-ttu-id="13a57-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="13a57-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13a57-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="13a57-110">Permission type</span></span>                        | <span data-ttu-id="13a57-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="13a57-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="13a57-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="13a57-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="13a57-113">AgreementAcceptance.Read</span><span class="sxs-lookup"><span data-stu-id="13a57-113">AgreementAcceptance.Read</span></span> |
|<span data-ttu-id="13a57-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="13a57-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13a57-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="13a57-115">Not supported.</span></span> |
|<span data-ttu-id="13a57-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="13a57-116">Application</span></span>                            | <span data-ttu-id="13a57-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="13a57-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="13a57-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="13a57-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/agreementAcceptances
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="13a57-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="13a57-119">Request headers</span></span>
| <span data-ttu-id="13a57-120">名前</span><span class="sxs-lookup"><span data-stu-id="13a57-120">Name</span></span>      |<span data-ttu-id="13a57-121">説明</span><span class="sxs-lookup"><span data-stu-id="13a57-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="13a57-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="13a57-122">Authorization</span></span> | <span data-ttu-id="13a57-123">ベアラー {トークン}</span><span class="sxs-lookup"><span data-stu-id="13a57-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="13a57-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="13a57-124">Request body</span></span>
<span data-ttu-id="13a57-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="13a57-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="13a57-126">応答</span><span class="sxs-lookup"><span data-stu-id="13a57-126">Response</span></span>
<span data-ttu-id="13a57-127">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[agreementAcceptance](../resources/agreementacceptance.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="13a57-127">If successful, this method returns a `200 OK` response code and a collection of [agreementAcceptance](../resources/agreementacceptance.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="13a57-128">例</span><span class="sxs-lookup"><span data-stu-id="13a57-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="13a57-129">要求</span><span class="sxs-lookup"><span data-stu-id="13a57-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_agreementacceptances"
}-->
```http
GET https://graph.microsoft.com/beta/me/agreementAcceptances
```
##### <a name="response"></a><span data-ttu-id="13a57-130">応答</span><span class="sxs-lookup"><span data-stu-id="13a57-130">Response</span></span>
><span data-ttu-id="13a57-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="13a57-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreementAcceptance",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 303

{
  "value": [
    {
      "agreementId": "agreementId-value",
      "userId": "userId-value",
      "agreementFileId": "agreementFileId-value",
      "recordedDateTime": "datetime-value",
      "userDisplayName": "userDisplayName-value",
      "userPrincipalName": "userPrincipalName-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List agreementAcceptances",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
