---
title: ユーザー デバイスの一覧表示
description: プロジェクト ローマの機能をサポートしているユーザーのデバイスの一覧を取得します。 または、アプリケーションを起動またはアプリケーションにデータを送信する機能が含まれます。 した後に GET 呼び出しを行うし、デバイスが、デバイスにコマンドを送信するデバイスの ID を渡します。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 891f66691149106d4ff5a2951170524203eb2ea7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509526"
---
# <a name="list-user-devices"></a><span data-ttu-id="d80e4-105">ユーザー デバイスの一覧表示</span><span class="sxs-lookup"><span data-stu-id="d80e4-105">List user devices</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d80e4-106">プロジェクト ローマの機能をサポートしているユーザーのデバイスの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="d80e4-106">Get a list of user devices that support Project Rome capabilities.</span></span> <span data-ttu-id="d80e4-107">または、アプリケーションを起動またはアプリケーションにデータを送信する機能が含まれます。</span><span class="sxs-lookup"><span data-stu-id="d80e4-107">This includes the ability to launch an app, or message or send data to an application.</span></span> <span data-ttu-id="d80e4-108">した後に GET 呼び出しを行うし、デバイスがデバイスに[コマンドを送信](send-device-command.md)するデバイスの ID を渡します。</span><span class="sxs-lookup"><span data-stu-id="d80e4-108">After you do a GET call on me/devices, pass in the ID of the device to [send a command](send-device-command.md) to your device.</span></span>

## <a name="permissions"></a><span data-ttu-id="d80e4-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d80e4-109">Permissions</span></span>

<span data-ttu-id="d80e4-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d80e4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d80e4-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d80e4-112">Permission type</span></span>      | <span data-ttu-id="d80e4-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d80e4-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d80e4-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d80e4-114">Delegated (work or school account)</span></span> | <span data-ttu-id="d80e4-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d80e4-115">Not supported.</span></span>    |
|<span data-ttu-id="d80e4-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d80e4-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d80e4-117">Device.Read</span><span class="sxs-lookup"><span data-stu-id="d80e4-117">Device.Read</span></span>    |
|<span data-ttu-id="d80e4-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d80e4-118">Application</span></span> | <span data-ttu-id="d80e4-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d80e4-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d80e4-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d80e4-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices
```

## <a name="request-headers"></a><span data-ttu-id="d80e4-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d80e4-121">Request headers</span></span>

| <span data-ttu-id="d80e4-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d80e4-122">Header</span></span> |<span data-ttu-id="d80e4-123">値</span><span class="sxs-lookup"><span data-stu-id="d80e4-123">Value</span></span>
|:----|:------|
|<span data-ttu-id="d80e4-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d80e4-124">Authorization</span></span>| <span data-ttu-id="d80e4-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d80e4-p104">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="d80e4-127">承諾</span><span class="sxs-lookup"><span data-stu-id="d80e4-127">Accept</span></span> | <span data-ttu-id="d80e4-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d80e4-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d80e4-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="d80e4-129">Request body</span></span>
<span data-ttu-id="d80e4-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d80e4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d80e4-131">応答</span><span class="sxs-lookup"><span data-stu-id="d80e4-131">Response</span></span>

<span data-ttu-id="d80e4-132">成功した場合に、このメソッドは、応答本体に 200 応答コードとユーザーのデバイスのプロパティを返します。</span><span class="sxs-lookup"><span data-stu-id="d80e4-132">If successful, this method returns a 200 response code and the user device properties in the response body.</span></span>

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

## <a name="example"></a><span data-ttu-id="d80e4-133">例</span><span class="sxs-lookup"><span data-stu-id="d80e4-133">Example</span></span>
<span data-ttu-id="d80e4-134">この例では、ユーザーのデバイスの一覧を返します。</span><span class="sxs-lookup"><span data-stu-id="d80e4-134">This example will return the list of devices for a user.</span></span> <span data-ttu-id="d80e4-135">コマンドを使用してをデバイスに`me/devices/{id}/command`、返されたデバイスの ID を取得する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d80e4-135">To command a device using `me/devices/{id}/command`, you will need to get the ID of the device that is returned.</span></span>

#### <a name="request"></a><span data-ttu-id="d80e4-136">要求</span><span class="sxs-lookup"><span data-stu-id="d80e4-136">Request</span></span>

<span data-ttu-id="d80e4-137">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d80e4-137">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "list_devices"
}-->

```http
GET me/devices
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="d80e4-138">応答</span><span class="sxs-lookup"><span data-stu-id="d80e4-138">Response</span></span>

<span data-ttu-id="d80e4-139">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d80e4-139">The following is an example of the response.</span></span> <span data-ttu-id="d80e4-140">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="d80e4-140">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d80e4-141">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="d80e4-141">All of the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-devices.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
