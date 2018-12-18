---
title: ユーザーを取得する
description: user オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
ms.openlocfilehash: cf0ee7b2c6d9cf13176f65c174ee4b6ac986984b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359690"
---
# <a name="get-user"></a><span data-ttu-id="7cd87-103">ユーザーを取得する</span><span class="sxs-lookup"><span data-stu-id="7cd87-103">Get user</span></span>

> <span data-ttu-id="7cd87-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7cd87-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7cd87-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7cd87-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7cd87-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7cd87-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7cd87-107">[user](../resources/intune-shared-user.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="7cd87-107">Read properties and relationships of the [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7cd87-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="7cd87-108">Prerequisites</span></span>

<span data-ttu-id="7cd87-109">この API を呼び出すには次のアクセス許可のいずれかが必要です。</span><span class="sxs-lookup"><span data-stu-id="7cd87-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="7cd87-110">アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7cd87-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="7cd87-111">特定のアクセス許可は、コンテキストに依存します。</span><span class="sxs-lookup"><span data-stu-id="7cd87-111">The specific permission depends on the context.</span></span>

|<span data-ttu-id="7cd87-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7cd87-112">Permission type</span></span>|<span data-ttu-id="7cd87-113">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7cd87-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7cd87-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7cd87-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="7cd87-115">&nbsp; &nbsp; **デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="7cd87-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="7cd87-116">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="7cd87-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="7cd87-117">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="7cd87-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="7cd87-118">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7cd87-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="7cd87-119">&nbsp;&nbsp; **契約時**</span><span class="sxs-lookup"><span data-stu-id="7cd87-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="7cd87-120">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="7cd87-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="7cd87-121">&nbsp; &nbsp; **トラブルシューティング**</span><span class="sxs-lookup"><span data-stu-id="7cd87-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="7cd87-122">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="7cd87-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="7cd87-123">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7cd87-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7cd87-124">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7cd87-124">Not supported.</span></span>|
|<span data-ttu-id="7cd87-125">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7cd87-125">Application</span></span>|<span data-ttu-id="7cd87-126">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7cd87-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7cd87-127">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7cd87-127">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7cd87-128">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="7cd87-128">Optional query parameters</span></span>

<span data-ttu-id="7cd87-129">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="7cd87-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7cd87-130">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7cd87-130">Request headers</span></span>

|<span data-ttu-id="7cd87-131">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7cd87-131">Header</span></span>|<span data-ttu-id="7cd87-132">値</span><span class="sxs-lookup"><span data-stu-id="7cd87-132">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7cd87-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="7cd87-133">Authorization</span></span>|<span data-ttu-id="7cd87-134">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="7cd87-134">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7cd87-135">Accept</span><span class="sxs-lookup"><span data-stu-id="7cd87-135">Accept</span></span>|<span data-ttu-id="7cd87-136">application/json</span><span class="sxs-lookup"><span data-stu-id="7cd87-136">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7cd87-137">要求本文</span><span class="sxs-lookup"><span data-stu-id="7cd87-137">Request body</span></span>

<span data-ttu-id="7cd87-138">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7cd87-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7cd87-139">応答</span><span class="sxs-lookup"><span data-stu-id="7cd87-139">Response</span></span>

<span data-ttu-id="7cd87-140">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[ユーザー](../resources/intune-shared-user.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7cd87-140">If successful, this method returns a `200 OK` response code and [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7cd87-141">例</span><span class="sxs-lookup"><span data-stu-id="7cd87-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="7cd87-142">要求</span><span class="sxs-lookup"><span data-stu-id="7cd87-142">Request</span></span>

<span data-ttu-id="7cd87-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7cd87-143">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="7cd87-144">応答</span><span class="sxs-lookup"><span data-stu-id="7cd87-144">Response</span></span>

<span data-ttu-id="7cd87-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7cd87-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 118

{
  "value": {
    "@odata.type": "#microsoft.graph.user",
    "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
  }
}
```



