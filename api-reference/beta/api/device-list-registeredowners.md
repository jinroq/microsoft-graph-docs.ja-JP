---
title: registeredOwners を一覧表示する
description: デバイスの登録済み所有者の一覧を取得します。 登録済み所有者は、デバイスがクラウドに参加済みか、または個人用デバイスが登録済みのユーザーです。 登録済み所有者は、登録時に設定されます。 現在、所有者は 1 人しかいることができません。
ms.openlocfilehash: 9b2acee14598c631c7f782391cb22a7917685e02
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071128"
---
# <a name="list-registeredowners"></a><span data-ttu-id="2852c-106">registeredOwners を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="2852c-106">List registeredOwners</span></span>

> <span data-ttu-id="2852c-107">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2852c-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2852c-108">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2852c-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2852c-109">デバイスの登録済み所有者の一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="2852c-109">Retrieve a list of users that are registered owners of the device.</span></span> <span data-ttu-id="2852c-110">登録済み所有者は、デバイスがクラウドに参加済みか、または個人用デバイスが登録済みのユーザーです。</span><span class="sxs-lookup"><span data-stu-id="2852c-110">A registered owner is the user that cloud joined the device or registered their personal device.</span></span> <span data-ttu-id="2852c-111">登録済み所有者は、登録時に設定されます。</span><span class="sxs-lookup"><span data-stu-id="2852c-111">The registered owner is set at the time of registration.</span></span> <span data-ttu-id="2852c-112">現在、所有者は 1 人しかいることができません。</span><span class="sxs-lookup"><span data-stu-id="2852c-112">Currently, there can be only one owner.</span></span>

## <a name="permissions"></a><span data-ttu-id="2852c-113">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2852c-113">Permissions</span></span>

<span data-ttu-id="2852c-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2852c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2852c-116">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2852c-116">Permission type</span></span>      | <span data-ttu-id="2852c-117">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2852c-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2852c-118">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2852c-118">Delegated (work or school account)</span></span> | <span data-ttu-id="2852c-119">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2852c-119">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2852c-120">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2852c-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2852c-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2852c-121">Not supported.</span></span>    |
|<span data-ttu-id="2852c-122">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2852c-122">Application</span></span> | <span data-ttu-id="2852c-123">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2852c-123">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2852c-124">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2852c-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredOwners
```

> <span data-ttu-id="2852c-125">注:要求内の"id"は、"deviceId"プロパティではなく、デバイスの id プロパティです。</span><span class="sxs-lookup"><span data-stu-id="2852c-125">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="2852c-126">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="2852c-126">Optional query parameters</span></span>
<span data-ttu-id="2852c-127">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="2852c-127">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="2852c-128">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2852c-128">Request headers</span></span>
| <span data-ttu-id="2852c-129">名前</span><span class="sxs-lookup"><span data-stu-id="2852c-129">Name</span></span>       | <span data-ttu-id="2852c-130">型</span><span class="sxs-lookup"><span data-stu-id="2852c-130">Type</span></span> | <span data-ttu-id="2852c-131">説明</span><span class="sxs-lookup"><span data-stu-id="2852c-131">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2852c-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="2852c-132">Authorization</span></span>  | <span data-ttu-id="2852c-133">string</span><span class="sxs-lookup"><span data-stu-id="2852c-133">string</span></span>  | <span data-ttu-id="2852c-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2852c-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2852c-136">要求本文</span><span class="sxs-lookup"><span data-stu-id="2852c-136">Request body</span></span>
<span data-ttu-id="2852c-137">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2852c-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2852c-138">応答</span><span class="sxs-lookup"><span data-stu-id="2852c-138">Response</span></span>

<span data-ttu-id="2852c-139">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="2852c-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2852c-140">例</span><span class="sxs-lookup"><span data-stu-id="2852c-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2852c-141">要求</span><span class="sxs-lookup"><span data-stu-id="2852c-141">Request</span></span>
<span data-ttu-id="2852c-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2852c-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registeredowners"
}-->
```http
GET https://graph.microsoft.com/beta/devices/{id}/registeredOwners
```
##### <a name="response"></a><span data-ttu-id="2852c-143">応答</span><span class="sxs-lookup"><span data-stu-id="2852c-143">Response</span></span>
<span data-ttu-id="2852c-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2852c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List registeredOwners",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->