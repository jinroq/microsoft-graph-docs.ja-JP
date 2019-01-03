---
title: デバイスを作成する
description: 新しいデバイスを作成します。
author: tfitzmac
ms.openlocfilehash: e2b52c67ee34df9a609fbb53972ee8b859e6889f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336142"
---
# <a name="create-device"></a><span data-ttu-id="e6c6a-103">デバイスを作成する</span><span class="sxs-lookup"><span data-stu-id="e6c6a-103">Create device</span></span>

> <span data-ttu-id="e6c6a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e6c6a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e6c6a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e6c6a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e6c6a-106">新しいデバイスを作成します。</span><span class="sxs-lookup"><span data-stu-id="e6c6a-106">Create a new device.</span></span>
## <a name="permissions"></a><span data-ttu-id="e6c6a-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e6c6a-107">Permissions</span></span>
<span data-ttu-id="e6c6a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e6c6a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e6c6a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e6c6a-110">Permission type</span></span>      | <span data-ttu-id="e6c6a-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e6c6a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e6c6a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e6c6a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e6c6a-113">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e6c6a-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e6c6a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e6c6a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6c6a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e6c6a-115">Not supported.</span></span>    |
|<span data-ttu-id="e6c6a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e6c6a-116">Application</span></span> | <span data-ttu-id="e6c6a-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6c6a-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e6c6a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e6c6a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices

```
## <a name="request-headers"></a><span data-ttu-id="e6c6a-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e6c6a-119">Request headers</span></span>
| <span data-ttu-id="e6c6a-120">名前</span><span class="sxs-lookup"><span data-stu-id="e6c6a-120">Name</span></span>       | <span data-ttu-id="e6c6a-121">種類</span><span class="sxs-lookup"><span data-stu-id="e6c6a-121">Type</span></span> | <span data-ttu-id="e6c6a-122">説明</span><span class="sxs-lookup"><span data-stu-id="e6c6a-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e6c6a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6c6a-123">Authorization</span></span>  | <span data-ttu-id="e6c6a-124">string</span><span class="sxs-lookup"><span data-stu-id="e6c6a-124">string</span></span>  | <span data-ttu-id="e6c6a-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e6c6a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e6c6a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="e6c6a-127">Request body</span></span>
<span data-ttu-id="e6c6a-128">要求本文で、[デバイス](../resources/device.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e6c6a-128">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>

<span data-ttu-id="e6c6a-129">**デバイス**・ リソースは、[拡張機能](/graph/extensibility-overview)をサポートするため使用すること、`POST`操作し、作成時にデバイス インスタンスに独自のデータを持つカスタム プロパティを追加します。</span><span class="sxs-lookup"><span data-stu-id="e6c6a-129">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the device instance while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="e6c6a-130">応答</span><span class="sxs-lookup"><span data-stu-id="e6c6a-130">Response</span></span>

<span data-ttu-id="e6c6a-131">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で[デバイス](../resources/device.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e6c6a-131">If successful, this method returns `201 Created` response code and [device](../resources/device.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6c6a-132">例</span><span class="sxs-lookup"><span data-stu-id="e6c6a-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e6c6a-133">要求</span><span class="sxs-lookup"><span data-stu-id="e6c6a-133">Request</span></span>
<span data-ttu-id="e6c6a-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e6c6a-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_device_from_devices"
}-->
```http
POST https://graph.microsoft.com/beta/devices
Content-type: application/json
Content-length: 364

{
  "accountEnabled": true,
  "alternativeSecurityIds": [
    {
      "type": 99,
      "identityProvider": "identityProvider-value",
      "key": "key-value"
    }
  ],
  "approximateLastSignInDateTime": "2016-10-19T10:37:00Z",
  "deviceId": "deviceId-value",
  "deviceMetadata": "deviceMetadata-value",
  "deviceVersion": 99
}
```
<span data-ttu-id="e6c6a-135">要求本文で、[デバイス](../resources/device.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e6c6a-135">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="e6c6a-136">応答</span><span class="sxs-lookup"><span data-stu-id="e6c6a-136">Response</span></span>
<span data-ttu-id="e6c6a-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e6c6a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 364

{
  "accountEnabled": true,
  "alternativeSecurityIds": [
    {
      "type": 99,
      "identityProvider": "identityProvider-value",
      "key": "key-value"
    }
  ],
  "approximateLastSignInDateTime": "2016-10-19T10:37:00Z",
  "deviceId": "deviceId-value",
  "deviceMetadata": "deviceMetadata-value",
  "deviceVersion": 99
}
```

## <a name="see-also"></a><span data-ttu-id="e6c6a-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="e6c6a-140">See also</span></span>

- [<span data-ttu-id="e6c6a-141">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="e6c6a-141">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="e6c6a-142">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="e6c6a-142">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="e6c6a-143">スキーマ拡張機能を使用したグループへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="e6c6a-143">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create device",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->