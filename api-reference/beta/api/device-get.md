---
title: デバイスを取得する
description: デバイス オブジェクトのプロパティとリレーションシップを取得します。
ms.openlocfilehash: 69c962d6b248738fb03bb3ac39cc37f667ea88e9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066931"
---
# <a name="get-device"></a><span data-ttu-id="b1e6d-103">デバイスを取得する</span><span class="sxs-lookup"><span data-stu-id="b1e6d-103">Get device</span></span>

> <span data-ttu-id="b1e6d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b1e6d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b1e6d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b1e6d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b1e6d-106">デバイス オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="b1e6d-106">Get the properties and relationships of a device object.</span></span>

<span data-ttu-id="b1e6d-107">**デバイス**・ リソースは、[拡張機能](/graph/extensibility-overview)をサポートするため使用することも、 `GET` 、**デバイス**インスタンスのカスタム プロパティと拡張機能のデータを取得する操作です。</span><span class="sxs-lookup"><span data-stu-id="b1e6d-107">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **device** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1e6d-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b1e6d-108">Permissions</span></span>
<span data-ttu-id="b1e6d-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b1e6d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b1e6d-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b1e6d-111">Permission type</span></span>      | <span data-ttu-id="b1e6d-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b1e6d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b1e6d-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b1e6d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b1e6d-114">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b1e6d-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b1e6d-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b1e6d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1e6d-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b1e6d-116">Not supported.</span></span>    |
|<span data-ttu-id="b1e6d-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b1e6d-117">Application</span></span> | <span data-ttu-id="b1e6d-118">Device.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1e6d-118">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b1e6d-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b1e6d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b1e6d-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="b1e6d-120">Optional query parameters</span></span>
<span data-ttu-id="b1e6d-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="b1e6d-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b1e6d-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b1e6d-122">Request headers</span></span>
| <span data-ttu-id="b1e6d-123">名前</span><span class="sxs-lookup"><span data-stu-id="b1e6d-123">Name</span></span>       | <span data-ttu-id="b1e6d-124">型</span><span class="sxs-lookup"><span data-stu-id="b1e6d-124">Type</span></span> | <span data-ttu-id="b1e6d-125">説明</span><span class="sxs-lookup"><span data-stu-id="b1e6d-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b1e6d-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1e6d-126">Authorization</span></span>  | <span data-ttu-id="b1e6d-127">string</span><span class="sxs-lookup"><span data-stu-id="b1e6d-127">string</span></span>  | <span data-ttu-id="b1e6d-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b1e6d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b1e6d-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="b1e6d-130">Request body</span></span>
<span data-ttu-id="b1e6d-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b1e6d-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b1e6d-132">応答</span><span class="sxs-lookup"><span data-stu-id="b1e6d-132">Response</span></span>

<span data-ttu-id="b1e6d-133">成功した場合、このメソッドは`200 OK`応答コードと、応答本文で[デバイス](../resources/device.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b1e6d-133">If successful, this method returns a `200 OK` response code and [device](../resources/device.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b1e6d-134">例</span><span class="sxs-lookup"><span data-stu-id="b1e6d-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b1e6d-135">要求</span><span class="sxs-lookup"><span data-stu-id="b1e6d-135">Request</span></span>
<span data-ttu-id="b1e6d-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b1e6d-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_device"
}-->
```http
GET https://graph.microsoft.com/beta/devices/{id}
```

> <span data-ttu-id="b1e6d-137">注:要求内の"id"は、"deviceId"プロパティではなく、デバイスの id プロパティです。</span><span class="sxs-lookup"><span data-stu-id="b1e6d-137">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

##### <a name="response"></a><span data-ttu-id="b1e6d-138">応答</span><span class="sxs-lookup"><span data-stu-id="b1e6d-138">Response</span></span>
<span data-ttu-id="b1e6d-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b1e6d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 322

{
  "accountEnabled": true,
  "approximateLastSignInDateTime": "2016-10-19T10:37:00Z",
  "deviceId": "deviceId-value",
  "deviceMetadata": "deviceMetadata-value",
  "deviceVersion": 99
}
```

## <a name="see-also"></a><span data-ttu-id="b1e6d-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="b1e6d-142">See also</span></span>

- [<span data-ttu-id="b1e6d-143">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="b1e6d-143">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="b1e6d-144">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="b1e6d-144">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="b1e6d-145">スキーマ拡張機能を使用したグループへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="b1e6d-145">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get device",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->