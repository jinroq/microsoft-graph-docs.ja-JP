---
title: デバイスを作成する
description: 新しいデバイスを作成します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 60a3e3bf2e44d975e1c3dc8383e0320a9906eda7
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33326070"
---
# <a name="create-device"></a><span data-ttu-id="c74b9-103">デバイスを作成する</span><span class="sxs-lookup"><span data-stu-id="c74b9-103">Create device</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c74b9-104">新しいデバイスを作成します。</span><span class="sxs-lookup"><span data-stu-id="c74b9-104">Create a new device.</span></span>
## <a name="permissions"></a><span data-ttu-id="c74b9-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c74b9-105">Permissions</span></span>
<span data-ttu-id="c74b9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c74b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c74b9-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c74b9-108">Permission type</span></span>      | <span data-ttu-id="c74b9-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c74b9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c74b9-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c74b9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c74b9-111">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c74b9-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c74b9-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c74b9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c74b9-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c74b9-113">Not supported.</span></span>    |
|<span data-ttu-id="c74b9-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c74b9-114">Application</span></span> | <span data-ttu-id="c74b9-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c74b9-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c74b9-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c74b9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices

```
## <a name="request-headers"></a><span data-ttu-id="c74b9-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c74b9-117">Request headers</span></span>
| <span data-ttu-id="c74b9-118">名前</span><span class="sxs-lookup"><span data-stu-id="c74b9-118">Name</span></span>       | <span data-ttu-id="c74b9-119">型</span><span class="sxs-lookup"><span data-stu-id="c74b9-119">Type</span></span> | <span data-ttu-id="c74b9-120">説明</span><span class="sxs-lookup"><span data-stu-id="c74b9-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c74b9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c74b9-121">Authorization</span></span>  | <span data-ttu-id="c74b9-122">string</span><span class="sxs-lookup"><span data-stu-id="c74b9-122">string</span></span>  | <span data-ttu-id="c74b9-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c74b9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c74b9-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="c74b9-125">Request body</span></span>
<span data-ttu-id="c74b9-126">要求本文で、[デバイス](../resources/device.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c74b9-126">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>

<span data-ttu-id="c74b9-127">**デバイス**リソースは[拡張機能](/graph/extensibility-overview)をサポートしているため`POST` 、操作を使用して、作成中に独自のデータを持つカスタムプロパティをデバイスインスタンスに追加することができます。</span><span class="sxs-lookup"><span data-stu-id="c74b9-127">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the device instance while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="c74b9-128">応答</span><span class="sxs-lookup"><span data-stu-id="c74b9-128">Response</span></span>

<span data-ttu-id="c74b9-129">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で[デバイス](../resources/device.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c74b9-129">If successful, this method returns `201 Created` response code and [device](../resources/device.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c74b9-130">例</span><span class="sxs-lookup"><span data-stu-id="c74b9-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c74b9-131">要求</span><span class="sxs-lookup"><span data-stu-id="c74b9-131">Request</span></span>
<span data-ttu-id="c74b9-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c74b9-132">Here is an example of the request.</span></span>
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
      "key": "base64Y3YxN2E1MWFlYw=="
    }
  ],
  "approximateLastSignInDateTime": "2016-10-19T10:37:00Z",
  "deviceId": "deviceId-value",
  "deviceMetadata": "deviceMetadata-value",
  "deviceVersion": 99
}
```
<span data-ttu-id="c74b9-133">要求本文で、[デバイス](../resources/device.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c74b9-133">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="c74b9-134">応答</span><span class="sxs-lookup"><span data-stu-id="c74b9-134">Response</span></span>
<span data-ttu-id="c74b9-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c74b9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "key": "base64Y3YxN2E1MWFlYw=="
    }
  ],
  "approximateLastSignInDateTime": "2016-10-19T10:37:00Z",
  "deviceId": "deviceId-value",
  "deviceMetadata": "deviceMetadata-value",
  "deviceVersion": 99
}
```

## <a name="see-also"></a><span data-ttu-id="c74b9-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="c74b9-138">See also</span></span>

- [<span data-ttu-id="c74b9-139">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="c74b9-139">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="c74b9-140">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="c74b9-140">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="c74b9-141">スキーマ拡張機能を使用したグループへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="c74b9-141">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create device",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
