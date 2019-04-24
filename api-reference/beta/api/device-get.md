---
title: デバイスを取得する
description: デバイス オブジェクトのプロパティとリレーションシップを取得します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b6b0bc325620a27d9383b4a12d5f3da970c0c267
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32455283"
---
# <a name="get-device"></a><span data-ttu-id="d95fe-103">デバイスを取得する</span><span class="sxs-lookup"><span data-stu-id="d95fe-103">Get device</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d95fe-104">デバイス オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="d95fe-104">Get the properties and relationships of a device object.</span></span>

<span data-ttu-id="d95fe-105">**デバイス**リソースは[拡張機能](/graph/extensibility-overview)をサポートしているため、 `GET`操作を使用して、**デバイス**インスタンスでカスタムプロパティと拡張機能データを取得することもできます。</span><span class="sxs-lookup"><span data-stu-id="d95fe-105">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **device** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="d95fe-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d95fe-106">Permissions</span></span>
<span data-ttu-id="d95fe-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d95fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d95fe-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d95fe-109">Permission type</span></span>      | <span data-ttu-id="d95fe-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d95fe-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d95fe-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d95fe-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d95fe-112">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d95fe-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d95fe-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d95fe-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d95fe-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d95fe-114">Not supported.</span></span>    |
|<span data-ttu-id="d95fe-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d95fe-115">Application</span></span> | <span data-ttu-id="d95fe-116">Device.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d95fe-116">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d95fe-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d95fe-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d95fe-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="d95fe-118">Optional query parameters</span></span>
<span data-ttu-id="d95fe-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d95fe-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d95fe-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d95fe-120">Request headers</span></span>
| <span data-ttu-id="d95fe-121">名前</span><span class="sxs-lookup"><span data-stu-id="d95fe-121">Name</span></span>       | <span data-ttu-id="d95fe-122">型</span><span class="sxs-lookup"><span data-stu-id="d95fe-122">Type</span></span> | <span data-ttu-id="d95fe-123">説明</span><span class="sxs-lookup"><span data-stu-id="d95fe-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d95fe-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d95fe-124">Authorization</span></span>  | <span data-ttu-id="d95fe-125">string</span><span class="sxs-lookup"><span data-stu-id="d95fe-125">string</span></span>  | <span data-ttu-id="d95fe-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d95fe-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d95fe-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="d95fe-128">Request body</span></span>
<span data-ttu-id="d95fe-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d95fe-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d95fe-130">応答</span><span class="sxs-lookup"><span data-stu-id="d95fe-130">Response</span></span>

<span data-ttu-id="d95fe-131">成功した場合、このメソッドは`200 OK`応答コードと、応答本文で[デバイス](../resources/device.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d95fe-131">If successful, this method returns a `200 OK` response code and [device](../resources/device.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d95fe-132">例</span><span class="sxs-lookup"><span data-stu-id="d95fe-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d95fe-133">要求</span><span class="sxs-lookup"><span data-stu-id="d95fe-133">Request</span></span>
<span data-ttu-id="d95fe-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d95fe-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_device"
}-->
```http
GET https://graph.microsoft.com/beta/devices/{id}
```

> <span data-ttu-id="d95fe-135">注:要求内の"id"は、"deviceId"プロパティではなく、デバイスの id プロパティです。</span><span class="sxs-lookup"><span data-stu-id="d95fe-135">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

##### <a name="response"></a><span data-ttu-id="d95fe-136">応答</span><span class="sxs-lookup"><span data-stu-id="d95fe-136">Response</span></span>
<span data-ttu-id="d95fe-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d95fe-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="d95fe-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="d95fe-140">See also</span></span>

- [<span data-ttu-id="d95fe-141">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="d95fe-141">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="d95fe-142">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="d95fe-142">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="d95fe-143">スキーマ拡張機能を使用したグループへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="d95fe-143">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get device",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/device-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
