---
title: デバイスを作成する
description: 新しいデバイスを作成し、組織に登録します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f7781e83aaa90127308ec0eae1cc11e3b5c4a843
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35449135"
---
# <a name="create-device"></a><span data-ttu-id="44e08-103">デバイスを作成する</span><span class="sxs-lookup"><span data-stu-id="44e08-103">Create device</span></span>

<span data-ttu-id="44e08-104">新しいデバイスを作成し、組織に登録します。</span><span class="sxs-lookup"><span data-stu-id="44e08-104">Create and register a new device in the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="44e08-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="44e08-105">Permissions</span></span>
<span data-ttu-id="44e08-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="44e08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="44e08-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="44e08-108">Permission type</span></span>      | <span data-ttu-id="44e08-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="44e08-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="44e08-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="44e08-110">Delegated (work or school account)</span></span> | <span data-ttu-id="44e08-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="44e08-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="44e08-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="44e08-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44e08-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="44e08-113">Not supported.</span></span>    |
|<span data-ttu-id="44e08-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="44e08-114">Application</span></span> | <span data-ttu-id="44e08-115">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44e08-115">Device.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="44e08-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="44e08-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices

```
## <a name="request-headers"></a><span data-ttu-id="44e08-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="44e08-117">Request headers</span></span>
| <span data-ttu-id="44e08-118">名前</span><span class="sxs-lookup"><span data-stu-id="44e08-118">Name</span></span>       | <span data-ttu-id="44e08-119">型</span><span class="sxs-lookup"><span data-stu-id="44e08-119">Type</span></span> | <span data-ttu-id="44e08-120">説明</span><span class="sxs-lookup"><span data-stu-id="44e08-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="44e08-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="44e08-121">Authorization</span></span>  | <span data-ttu-id="44e08-122">string</span><span class="sxs-lookup"><span data-stu-id="44e08-122">string</span></span>  | <span data-ttu-id="44e08-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="44e08-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="44e08-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="44e08-125">Content-type</span></span> | <span data-ttu-id="44e08-126">string</span><span class="sxs-lookup"><span data-stu-id="44e08-126">string</span></span> | <span data-ttu-id="44e08-127">application/json</span><span class="sxs-lookup"><span data-stu-id="44e08-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="44e08-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="44e08-128">Request body</span></span>
<span data-ttu-id="44e08-129">要求本文で、[デバイス](../resources/device.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="44e08-129">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="44e08-130">応答</span><span class="sxs-lookup"><span data-stu-id="44e08-130">Response</span></span>

<span data-ttu-id="44e08-131">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で[デバイス](../resources/device.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="44e08-131">If successful, this method returns `201 Created` response code and [device](../resources/device.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44e08-132">例</span><span class="sxs-lookup"><span data-stu-id="44e08-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="44e08-133">要求</span><span class="sxs-lookup"><span data-stu-id="44e08-133">Request</span></span>
<span data-ttu-id="44e08-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="44e08-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="44e08-135">プロトコル</span><span class="sxs-lookup"><span data-stu-id="44e08-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_device_from_devices"
}-->
```http
POST https://graph.microsoft.com/v1.0/devices
Content-type: application/json

{
  "accountEnabled":false,
  "alternativeSecurityIds":
  [
    {
      "type":2,
      "key":"base64Y3YxN2E1MWFlYw=="
    }
  ],
  "deviceId":"4c299165-6e8f-4b45-a5ba-c5d250a707ff",
  "displayName":"Test device",
  "operatingSystem":"linux",
  "operatingSystemVersion":"1"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="44e08-136">C#</span><span class="sxs-lookup"><span data-stu-id="44e08-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-device-from-devices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="44e08-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="44e08-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-device-from-devices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="44e08-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="44e08-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-device-from-devices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="44e08-139">要求本文で、[デバイス](../resources/device.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="44e08-139">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="44e08-140">応答</span><span class="sxs-lookup"><span data-stu-id="44e08-140">Response</span></span>
<span data-ttu-id="44e08-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="44e08-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "accountEnabled":false,
  "alternativeSecurityIds":
  [
    {
      "type":2,
      "key":"base64Y3YxN2E1MWFlYw=="
    }
  ],
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
  "description": "Create device",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
