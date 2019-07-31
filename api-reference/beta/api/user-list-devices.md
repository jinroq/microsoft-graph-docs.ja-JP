---
title: ユーザー デバイスを一覧表示する
description: プロジェクトローマ機能をサポートするユーザーデバイスのリストを取得します。 これには、アプリを起動したり、アプリケーションに対してデータを送信したりする機能が含まれます。 [自分/デバイスで呼び出しを実行した後、デバイスにコマンドを送信するには、デバイスの ID] を渡します。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 292124babfb71ad1c86ae373f123c2f5d57df3b4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35996253"
---
# <a name="list-user-devices"></a><span data-ttu-id="16d1e-105">ユーザー デバイスを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="16d1e-105">List user devices</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16d1e-106">プロジェクトローマ機能をサポートするユーザーデバイスのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="16d1e-106">Get a list of user devices that support Project Rome capabilities.</span></span> <span data-ttu-id="16d1e-107">これには、アプリを起動したり、アプリケーションに対してデータを送信したりする機能が含まれます。</span><span class="sxs-lookup"><span data-stu-id="16d1e-107">This includes the ability to launch an app, or message or send data to an application.</span></span> <span data-ttu-id="16d1e-108">[自分/デバイスで呼び出しを実行した後、デバイスに[コマンドを送信](send-device-command.md)するには、デバイスの ID] を渡します。</span><span class="sxs-lookup"><span data-stu-id="16d1e-108">After you do a GET call on me/devices, pass in the ID of the device to [send a command](send-device-command.md) to your device.</span></span>

## <a name="permissions"></a><span data-ttu-id="16d1e-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="16d1e-109">Permissions</span></span>

<span data-ttu-id="16d1e-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="16d1e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="16d1e-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="16d1e-112">Permission type</span></span>      | <span data-ttu-id="16d1e-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="16d1e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16d1e-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="16d1e-114">Delegated (work or school account)</span></span> | <span data-ttu-id="16d1e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="16d1e-115">Not supported.</span></span>    |
|<span data-ttu-id="16d1e-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="16d1e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16d1e-117">Device.Read</span><span class="sxs-lookup"><span data-stu-id="16d1e-117">Device.Read</span></span>    |
|<span data-ttu-id="16d1e-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="16d1e-118">Application</span></span> | <span data-ttu-id="16d1e-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="16d1e-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="16d1e-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="16d1e-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices
```

## <a name="request-headers"></a><span data-ttu-id="16d1e-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="16d1e-121">Request headers</span></span>

| <span data-ttu-id="16d1e-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="16d1e-122">Header</span></span> |<span data-ttu-id="16d1e-123">値</span><span class="sxs-lookup"><span data-stu-id="16d1e-123">Value</span></span>
|:----|:------|
|<span data-ttu-id="16d1e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="16d1e-124">Authorization</span></span>| <span data-ttu-id="16d1e-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="16d1e-p104">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="16d1e-127">承諾</span><span class="sxs-lookup"><span data-stu-id="16d1e-127">Accept</span></span> | <span data-ttu-id="16d1e-128">application/json</span><span class="sxs-lookup"><span data-stu-id="16d1e-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="16d1e-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="16d1e-129">Request body</span></span>
<span data-ttu-id="16d1e-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="16d1e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16d1e-131">応答</span><span class="sxs-lookup"><span data-stu-id="16d1e-131">Response</span></span>

<span data-ttu-id="16d1e-132">成功した場合、このメソッドは応答本文で200応答コードとユーザーデバイスプロパティを返します。</span><span class="sxs-lookup"><span data-stu-id="16d1e-132">If successful, this method returns a 200 response code and the user device properties in the response body.</span></span>

<!-- { "blockType": "ignored" } -->

```http
HTTP/1.1 200 OK
```

<!-- { "blockType": "ignored" } -->

```json
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#devices",
  "value": [
    {
      "name": "name",
      "id": "id",
      "status": "status",
      "platform": "platform",
      "kind": "formFactor",
      "model": "model",
      "manufacturer": "manufacturer",
    }
  ]
}
```

## <a name="example"></a><span data-ttu-id="16d1e-133">例</span><span class="sxs-lookup"><span data-stu-id="16d1e-133">Example</span></span>
<span data-ttu-id="16d1e-134">この例では、ユーザーのデバイスの一覧を返します。</span><span class="sxs-lookup"><span data-stu-id="16d1e-134">This example will return the list of devices for a user.</span></span> <span data-ttu-id="16d1e-135">を使用して`me/devices/{id}/command`デバイスのコマンドを実行するには、返されるデバイスの ID を取得する必要があります。</span><span class="sxs-lookup"><span data-stu-id="16d1e-135">To command a device using `me/devices/{id}/command`, you will need to get the ID of the device that is returned.</span></span>

#### <a name="request"></a><span data-ttu-id="16d1e-136">要求</span><span class="sxs-lookup"><span data-stu-id="16d1e-136">Request</span></span>

<span data-ttu-id="16d1e-137">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="16d1e-137">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "list_devices"
}-->

```http
GET me/devices
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="16d1e-138">応答</span><span class="sxs-lookup"><span data-stu-id="16d1e-138">Response</span></span>

<span data-ttu-id="16d1e-139">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="16d1e-139">The following is an example of the response.</span></span> <span data-ttu-id="16d1e-140">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="16d1e-140">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="16d1e-141">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="16d1e-141">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.device",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 140

{
  "value": [
    {
      "Name": "JimSurface",
      "id": "6841b3db-2b55-467b-ad84-79a41a4ef665",
      "Manufacturer": "Microsoft Corporation",
      "Model": "Surface Book",
      "Kind": "Tablet",
      "Status": "Unknown",
      "Platform": "Windows"
    }
  ]
}
```
