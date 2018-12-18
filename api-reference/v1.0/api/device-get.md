---
title: デバイスを取得する
description: デバイス オブジェクトのプロパティとリレーションシップを取得します。
author: tfitzmac
ms.openlocfilehash: 57032f29ace00a441aff7f68e9b61bd52e88e79b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310669"
---
# <a name="get-device"></a><span data-ttu-id="144e3-103">デバイスを取得する</span><span class="sxs-lookup"><span data-stu-id="144e3-103">Get device</span></span>

<span data-ttu-id="144e3-104">デバイス オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="144e3-104">Get the properties and relationships of a device object.</span></span>
## <a name="permissions"></a><span data-ttu-id="144e3-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="144e3-105">Permissions</span></span>
<span data-ttu-id="144e3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="144e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="144e3-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="144e3-108">Permission type</span></span>      | <span data-ttu-id="144e3-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="144e3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="144e3-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="144e3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="144e3-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="144e3-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="144e3-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="144e3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="144e3-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="144e3-113">Not supported.</span></span>    |
|<span data-ttu-id="144e3-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="144e3-114">Application</span></span> | <span data-ttu-id="144e3-115">Device.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="144e3-115">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="144e3-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="144e3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}
```
> <span data-ttu-id="144e3-117">注:要求内の"id"は、"deviceId"プロパティではなく、デバイスの id プロパティです。</span><span class="sxs-lookup"><span data-stu-id="144e3-117">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="144e3-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="144e3-118">Optional query parameters</span></span>
<span data-ttu-id="144e3-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="144e3-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="144e3-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="144e3-120">Request headers</span></span>
| <span data-ttu-id="144e3-121">名前</span><span class="sxs-lookup"><span data-stu-id="144e3-121">Name</span></span>       | <span data-ttu-id="144e3-122">種類</span><span class="sxs-lookup"><span data-stu-id="144e3-122">Type</span></span> | <span data-ttu-id="144e3-123">説明</span><span class="sxs-lookup"><span data-stu-id="144e3-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="144e3-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="144e3-124">Authorization</span></span>  | <span data-ttu-id="144e3-125">string</span><span class="sxs-lookup"><span data-stu-id="144e3-125">string</span></span>  | <span data-ttu-id="144e3-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="144e3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="144e3-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="144e3-128">Request body</span></span>
<span data-ttu-id="144e3-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="144e3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="144e3-130">応答</span><span class="sxs-lookup"><span data-stu-id="144e3-130">Response</span></span>

<span data-ttu-id="144e3-131">成功した場合、このメソッドは`200 OK`応答コードと、応答本文で[デバイス](../resources/device.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="144e3-131">If successful, this method returns a `200 OK` response code and [device](../resources/device.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="144e3-132">例</span><span class="sxs-lookup"><span data-stu-id="144e3-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="144e3-133">要求</span><span class="sxs-lookup"><span data-stu-id="144e3-133">Request</span></span>
<span data-ttu-id="144e3-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="144e3-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_device"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}
```
##### <a name="response"></a><span data-ttu-id="144e3-135">応答</span><span class="sxs-lookup"><span data-stu-id="144e3-135">Response</span></span>
<span data-ttu-id="144e3-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="144e3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "accountEnabled":false,
  "deviceId":"4c299165-6e8f-4b45-a5ba-c5d250a707ff",
  "displayName":"Test device",
  "id": "id-value",
  "operatingSystem":"linux",
  "operatingSystemVersion":"1"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get device",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
