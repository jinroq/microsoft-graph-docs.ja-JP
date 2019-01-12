---
title: registeredUsers を一覧表示する
description: デバイスの登録ユーザーの一覧を取得します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d3a5e8dbc92860ac4829f4aa4c3e509e6f4ec9b4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980602"
---
# <a name="list-registeredusers"></a><span data-ttu-id="c12e1-103">registeredUsers を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="c12e1-103">List registeredUsers</span></span>

> <span data-ttu-id="c12e1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c12e1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c12e1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c12e1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c12e1-106">デバイスの登録ユーザーの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="c12e1-106">Retrieve a list of users that are registered users of the device.</span></span>

<span data-ttu-id="c12e1-107">クラウドに参加済みのデバイスと登録済みの個人用デバイスの場合、登録済みのユーザーは、登録時に登録済み所有者と同じ値に設定されます。</span><span class="sxs-lookup"><span data-stu-id="c12e1-107">For cloud joined devices and registered personal devices, registered users are set to the same value as registered owners at the time of registration.</span></span>

## <a name="permissions"></a><span data-ttu-id="c12e1-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c12e1-108">Permissions</span></span>
<span data-ttu-id="c12e1-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c12e1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c12e1-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c12e1-111">Permission type</span></span>      | <span data-ttu-id="c12e1-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c12e1-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c12e1-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c12e1-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c12e1-114">Directory.Read.All または Directory.ReadWrite.All または Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c12e1-114">Directory.Read.All or Directory.ReadWrite.All or Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c12e1-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c12e1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c12e1-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c12e1-116">Not supported.</span></span> |
|<span data-ttu-id="c12e1-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c12e1-117">Application</span></span> | <span data-ttu-id="c12e1-118">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c12e1-118">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c12e1-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c12e1-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredUsers
```

> <span data-ttu-id="c12e1-120">注:要求内の"id"は、"deviceId"プロパティではなく、デバイスの id プロパティです。</span><span class="sxs-lookup"><span data-stu-id="c12e1-120">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="c12e1-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c12e1-121">Optional query parameters</span></span>
<span data-ttu-id="c12e1-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c12e1-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c12e1-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c12e1-123">Request headers</span></span>
| <span data-ttu-id="c12e1-124">名前</span><span class="sxs-lookup"><span data-stu-id="c12e1-124">Name</span></span>       | <span data-ttu-id="c12e1-125">種類</span><span class="sxs-lookup"><span data-stu-id="c12e1-125">Type</span></span> | <span data-ttu-id="c12e1-126">説明</span><span class="sxs-lookup"><span data-stu-id="c12e1-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c12e1-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="c12e1-127">Authorization</span></span>  | <span data-ttu-id="c12e1-128">string</span><span class="sxs-lookup"><span data-stu-id="c12e1-128">string</span></span>  | <span data-ttu-id="c12e1-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c12e1-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c12e1-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="c12e1-131">Request body</span></span>
<span data-ttu-id="c12e1-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c12e1-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c12e1-133">応答</span><span class="sxs-lookup"><span data-stu-id="c12e1-133">Response</span></span>

<span data-ttu-id="c12e1-134">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="c12e1-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c12e1-135">例</span><span class="sxs-lookup"><span data-stu-id="c12e1-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c12e1-136">要求</span><span class="sxs-lookup"><span data-stu-id="c12e1-136">Request</span></span>
<span data-ttu-id="c12e1-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c12e1-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registeredusers"
}-->
```http
GET https://graph.microsoft.com/beta/devices/{id}/registeredUsers
```
##### <a name="response"></a><span data-ttu-id="c12e1-138">応答</span><span class="sxs-lookup"><span data-stu-id="c12e1-138">Response</span></span>
<span data-ttu-id="c12e1-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c12e1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List registeredUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
