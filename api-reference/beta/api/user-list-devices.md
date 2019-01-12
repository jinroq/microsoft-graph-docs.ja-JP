---
title: ユーザー デバイスの一覧表示
description: プロジェクト ローマの機能をサポートしているユーザーのデバイスの一覧を取得します。 または、アプリケーションを起動またはアプリケーションにデータを送信する機能が含まれます。 した後に GET 呼び出しを行うし、デバイスが、デバイスにコマンドを送信するデバイスの ID を渡します。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 04b67b770eec38d9e70a2263cd54212077335c85
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983542"
---
# <a name="list-user-devices"></a><span data-ttu-id="e7110-105">ユーザー デバイスの一覧表示</span><span class="sxs-lookup"><span data-stu-id="e7110-105">List user devices</span></span>

> <span data-ttu-id="e7110-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e7110-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e7110-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e7110-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e7110-108">プロジェクト ローマの機能をサポートしているユーザーのデバイスの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="e7110-108">Get a list of user devices that support Project Rome capabilities.</span></span> <span data-ttu-id="e7110-109">または、アプリケーションを起動またはアプリケーションにデータを送信する機能が含まれます。</span><span class="sxs-lookup"><span data-stu-id="e7110-109">This includes the ability to launch an app, or message or send data to an application.</span></span> <span data-ttu-id="e7110-110">した後に GET 呼び出しを行うし、デバイスがデバイスに[コマンドを送信](send-device-command.md)するデバイスの ID を渡します。</span><span class="sxs-lookup"><span data-stu-id="e7110-110">After you do a GET call on me/devices, pass in the ID of the device to [send a command](send-device-command.md) to your device.</span></span>

## <a name="permissions"></a><span data-ttu-id="e7110-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e7110-111">Permissions</span></span>

<span data-ttu-id="e7110-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e7110-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e7110-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e7110-114">Permission type</span></span>      | <span data-ttu-id="e7110-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e7110-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e7110-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e7110-116">Delegated (work or school account)</span></span> | <span data-ttu-id="e7110-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e7110-117">Not supported.</span></span>    |
|<span data-ttu-id="e7110-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e7110-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7110-119">Device.Read</span><span class="sxs-lookup"><span data-stu-id="e7110-119">Device.Read</span></span>    |
|<span data-ttu-id="e7110-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e7110-120">Application</span></span> | <span data-ttu-id="e7110-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e7110-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e7110-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e7110-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices
```

## <a name="request-headers"></a><span data-ttu-id="e7110-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e7110-123">Request headers</span></span>

| <span data-ttu-id="e7110-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e7110-124">Header</span></span> |<span data-ttu-id="e7110-125">値</span><span class="sxs-lookup"><span data-stu-id="e7110-125">Value</span></span>
|:----|:------|
|<span data-ttu-id="e7110-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7110-126">Authorization</span></span>| <span data-ttu-id="e7110-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e7110-p105">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="e7110-129">承諾</span><span class="sxs-lookup"><span data-stu-id="e7110-129">Accept</span></span> | <span data-ttu-id="e7110-130">application/json</span><span class="sxs-lookup"><span data-stu-id="e7110-130">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e7110-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="e7110-131">Request body</span></span>
<span data-ttu-id="e7110-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e7110-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e7110-133">応答</span><span class="sxs-lookup"><span data-stu-id="e7110-133">Response</span></span>

<span data-ttu-id="e7110-134">成功した場合に、このメソッドは、応答本体に 200 応答コードとユーザーのデバイスのプロパティを返します。</span><span class="sxs-lookup"><span data-stu-id="e7110-134">If successful, this method returns a 200 response code and the user device properties in the response body.</span></span>

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

## <a name="example"></a><span data-ttu-id="e7110-135">例</span><span class="sxs-lookup"><span data-stu-id="e7110-135">Example</span></span>
<span data-ttu-id="e7110-136">この例では、ユーザーのデバイスの一覧を返します。</span><span class="sxs-lookup"><span data-stu-id="e7110-136">This example will return the list of devices for a user.</span></span> <span data-ttu-id="e7110-137">コマンドを使用してをデバイスに`me/devices/{id}/command`、返されたデバイスの ID を取得する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e7110-137">To command a device using `me/devices/{id}/command`, you will need to get the ID of the device that is returned.</span></span>

#### <a name="request"></a><span data-ttu-id="e7110-138">要求</span><span class="sxs-lookup"><span data-stu-id="e7110-138">Request</span></span>

<span data-ttu-id="e7110-139">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e7110-139">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "list_devices"
}-->

```http
GET me/devices
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="e7110-140">応答</span><span class="sxs-lookup"><span data-stu-id="e7110-140">Response</span></span>

<span data-ttu-id="e7110-141">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e7110-141">The following is an example of the response.</span></span> <span data-ttu-id="e7110-142">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="e7110-142">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="e7110-143">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="e7110-143">All of the properties will be returned from an actual call.</span></span>

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
