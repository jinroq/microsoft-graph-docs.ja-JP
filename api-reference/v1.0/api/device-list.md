---
title: デバイスを一覧表示する
description: 組織に登録されているデバイス オブジェクトの一覧を取得します。
author: tfitzmac
ms.openlocfilehash: a17dcdd3fc15a04276095b2f356cc780ae6a8fee
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314379"
---
# <a name="list-devices"></a><span data-ttu-id="a189f-103">デバイスを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="a189f-103">List devices</span></span>

<span data-ttu-id="a189f-104">組織に登録されているデバイス オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="a189f-104">Retrieve a list of device objects registered in the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="a189f-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a189f-105">Permissions</span></span>
<span data-ttu-id="a189f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a189f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a189f-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a189f-108">Permission type</span></span>      | <span data-ttu-id="a189f-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a189f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a189f-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a189f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a189f-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a189f-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a189f-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a189f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a189f-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a189f-113">Not supported.</span></span>    |
|<span data-ttu-id="a189f-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a189f-114">Application</span></span> | <span data-ttu-id="a189f-115">Device.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a189f-115">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a189f-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a189f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a189f-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="a189f-117">Optional query parameters</span></span>
<span data-ttu-id="a189f-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="a189f-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a189f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a189f-119">Request headers</span></span>
| <span data-ttu-id="a189f-120">名前</span><span class="sxs-lookup"><span data-stu-id="a189f-120">Name</span></span>       | <span data-ttu-id="a189f-121">種類</span><span class="sxs-lookup"><span data-stu-id="a189f-121">Type</span></span> | <span data-ttu-id="a189f-122">説明</span><span class="sxs-lookup"><span data-stu-id="a189f-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a189f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a189f-123">Authorization</span></span>  | <span data-ttu-id="a189f-124">string</span><span class="sxs-lookup"><span data-stu-id="a189f-124">string</span></span>  | <span data-ttu-id="a189f-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a189f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a189f-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="a189f-127">Request body</span></span>
<span data-ttu-id="a189f-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a189f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a189f-129">応答</span><span class="sxs-lookup"><span data-stu-id="a189f-129">Response</span></span>

<span data-ttu-id="a189f-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [device](../resources/device.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="a189f-130">If successful, this method returns a `200 OK` response code and collection of [device](../resources/device.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a189f-131">例</span><span class="sxs-lookup"><span data-stu-id="a189f-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a189f-132">要求</span><span class="sxs-lookup"><span data-stu-id="a189f-132">Request</span></span>
<span data-ttu-id="a189f-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a189f-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_devices"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices
```

##### <a name="response"></a><span data-ttu-id="a189f-134">応答</span><span class="sxs-lookup"><span data-stu-id="a189f-134">Response</span></span>
<span data-ttu-id="a189f-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a189f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "accountEnabled":false,
      "deviceId":"4c299165-6e8f-4b45-a5ba-c5d250a707ff",
      "displayName":"Test device",
      "id": "id-value",
      "operatingSystem":"linux",
      "operatingSystemVersion":"1"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List devices",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->