---
title: registeredUsers を一覧表示する
description: デバイスの登録ユーザーの一覧を取得します。
ms.openlocfilehash: 370990b5b9c61b071620fe0df04fd38e98892bd1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023444"
---
# <a name="list-registeredusers"></a><span data-ttu-id="a5b67-103">registeredUsers を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="a5b67-103">List registeredUsers</span></span>

<span data-ttu-id="a5b67-104">デバイスの登録ユーザーの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="a5b67-104">Retrieve a list of users that are registered users of the device.</span></span>

<span data-ttu-id="a5b67-105">クラウドに参加済みのデバイスと登録済みの個人用デバイスの場合、登録済みのユーザーは、登録時に登録済み所有者と同じ値に設定されます。</span><span class="sxs-lookup"><span data-stu-id="a5b67-105">For cloud joined devices and registered personal devices, registered users are set to the same value as registered owners at the time of registration.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5b67-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a5b67-106">Permissions</span></span>
<span data-ttu-id="a5b67-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a5b67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a5b67-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a5b67-109">Permission type</span></span>      | <span data-ttu-id="a5b67-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a5b67-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5b67-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a5b67-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a5b67-112">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a5b67-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a5b67-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a5b67-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5b67-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a5b67-114">Not supported.</span></span>    |
|<span data-ttu-id="a5b67-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a5b67-115">Application</span></span> | <span data-ttu-id="a5b67-116">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5b67-116">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5b67-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a5b67-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredUsers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a5b67-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="a5b67-118">Optional query parameters</span></span>
<span data-ttu-id="a5b67-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="a5b67-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a5b67-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a5b67-120">Request headers</span></span>
| <span data-ttu-id="a5b67-121">名前</span><span class="sxs-lookup"><span data-stu-id="a5b67-121">Name</span></span>       | <span data-ttu-id="a5b67-122">型</span><span class="sxs-lookup"><span data-stu-id="a5b67-122">Type</span></span> | <span data-ttu-id="a5b67-123">説明</span><span class="sxs-lookup"><span data-stu-id="a5b67-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a5b67-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5b67-124">Authorization</span></span>  | <span data-ttu-id="a5b67-125">string</span><span class="sxs-lookup"><span data-stu-id="a5b67-125">string</span></span>  | <span data-ttu-id="a5b67-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a5b67-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a5b67-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="a5b67-128">Request body</span></span>
<span data-ttu-id="a5b67-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a5b67-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a5b67-130">応答</span><span class="sxs-lookup"><span data-stu-id="a5b67-130">Response</span></span>

<span data-ttu-id="a5b67-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="a5b67-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a5b67-132">例</span><span class="sxs-lookup"><span data-stu-id="a5b67-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a5b67-133">要求</span><span class="sxs-lookup"><span data-stu-id="a5b67-133">Request</span></span>
<span data-ttu-id="a5b67-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a5b67-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registeredusers"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}/registeredUsers
```
##### <a name="response"></a><span data-ttu-id="a5b67-135">応答</span><span class="sxs-lookup"><span data-stu-id="a5b67-135">Response</span></span>
<span data-ttu-id="a5b67-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a5b67-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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