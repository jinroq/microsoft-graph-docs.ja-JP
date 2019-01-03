---
title: registeredDevices を一覧表示する　
description: ユーザーの登録済みデバイスの一覧を取得します。
ms.openlocfilehash: be157572183b165dfb3bd6e23fd7b7a46f29e94a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022394"
---
# <a name="list-registereddevices"></a><span data-ttu-id="5a0b1-103">registeredDevices を一覧表示する　</span><span class="sxs-lookup"><span data-stu-id="5a0b1-103">List registeredDevices</span></span>

<span data-ttu-id="5a0b1-104">ユーザーの登録済みデバイスの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="5a0b1-104">Get the list of user's registered devices.</span></span>
## <a name="permissions"></a><span data-ttu-id="5a0b1-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5a0b1-105">Permissions</span></span>
<span data-ttu-id="5a0b1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5a0b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a0b1-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5a0b1-108">Permission type</span></span>      | <span data-ttu-id="5a0b1-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5a0b1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5a0b1-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5a0b1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5a0b1-111">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5a0b1-111">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5a0b1-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5a0b1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a0b1-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5a0b1-113">Not supported.</span></span>    |
|<span data-ttu-id="5a0b1-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5a0b1-114">Application</span></span> | <span data-ttu-id="5a0b1-115">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a0b1-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5a0b1-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5a0b1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/registeredDevices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5a0b1-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="5a0b1-117">Optional query parameters</span></span>
<span data-ttu-id="5a0b1-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="5a0b1-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5a0b1-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5a0b1-119">Request headers</span></span>
| <span data-ttu-id="5a0b1-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5a0b1-120">Header</span></span>       | <span data-ttu-id="5a0b1-121">値</span><span class="sxs-lookup"><span data-stu-id="5a0b1-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5a0b1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a0b1-122">Authorization</span></span>  | <span data-ttu-id="5a0b1-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5a0b1-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5a0b1-125">承諾</span><span class="sxs-lookup"><span data-stu-id="5a0b1-125">Accept</span></span>  | <span data-ttu-id="5a0b1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5a0b1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a0b1-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="5a0b1-127">Request body</span></span>
<span data-ttu-id="5a0b1-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5a0b1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5a0b1-129">応答</span><span class="sxs-lookup"><span data-stu-id="5a0b1-129">Response</span></span>

<span data-ttu-id="5a0b1-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="5a0b1-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5a0b1-131">例</span><span class="sxs-lookup"><span data-stu-id="5a0b1-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5a0b1-132">要求</span><span class="sxs-lookup"><span data-stu-id="5a0b1-132">Request</span></span>
<span data-ttu-id="5a0b1-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5a0b1-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registereddevices"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/registeredDevices
```
##### <a name="response"></a><span data-ttu-id="5a0b1-134">応答</span><span class="sxs-lookup"><span data-stu-id="5a0b1-134">Response</span></span>
<span data-ttu-id="5a0b1-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5a0b1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List registeredDevices",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->