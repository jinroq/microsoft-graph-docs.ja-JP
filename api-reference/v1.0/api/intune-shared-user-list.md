---
title: ユーザーを一覧表示する
description: user オブジェクトのプロパティとリレーションシップをリストします。
ms.openlocfilehash: 06044d50bf21e52f61a66a7e54b11c69c9e5f700
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023296"
---
# <a name="list-users"></a><span data-ttu-id="9d6b1-103">users のリスト</span><span class="sxs-lookup"><span data-stu-id="9d6b1-103">List users</span></span>

> <span data-ttu-id="9d6b1-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9d6b1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9d6b1-105">[user](../resources/intune-shared-user.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="9d6b1-105">List properties and relationships of the [user](../resources/intune-shared-user.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9d6b1-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="9d6b1-106">Prerequisites</span></span>
<span data-ttu-id="9d6b1-107">この API を呼び出すには次のアクセス許可のいずれかが必要です。</span><span class="sxs-lookup"><span data-stu-id="9d6b1-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="9d6b1-108">アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9d6b1-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="9d6b1-109">特定のアクセス許可は、コンテキストに依存します。</span><span class="sxs-lookup"><span data-stu-id="9d6b1-109">The specific permission depends on the context.</span></span>

|<span data-ttu-id="9d6b1-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9d6b1-110">Permission type</span></span>|<span data-ttu-id="9d6b1-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9d6b1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9d6b1-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9d6b1-112">Delegated (work or school account)</span></span>| <span data-ttu-id="9d6b1-113">_コンテキストによって異なります_</span><span class="sxs-lookup"><span data-stu-id="9d6b1-113">_varies by context_</span></span>|
| <span data-ttu-id="9d6b1-114">&nbsp;&nbsp;デバイスの管理</span><span class="sxs-lookup"><span data-stu-id="9d6b1-114">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="9d6b1-115">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="9d6b1-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="9d6b1-116">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="9d6b1-116">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="9d6b1-117">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="9d6b1-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="9d6b1-118">&nbsp;&nbsp;契約時</span><span class="sxs-lookup"><span data-stu-id="9d6b1-118">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="9d6b1-119">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="9d6b1-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="9d6b1-120">&nbsp;&nbsp;のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="9d6b1-120">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="9d6b1-121">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="9d6b1-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="9d6b1-122">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9d6b1-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9d6b1-123">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9d6b1-123">Not supported.</span></span>|
|<span data-ttu-id="9d6b1-124">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9d6b1-124">Application</span></span>|<span data-ttu-id="9d6b1-125">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9d6b1-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9d6b1-126">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9d6b1-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users
```

## <a name="request-headers"></a><span data-ttu-id="9d6b1-127">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9d6b1-127">Request headers</span></span>
|<span data-ttu-id="9d6b1-128">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9d6b1-128">Header</span></span>|<span data-ttu-id="9d6b1-129">値</span><span class="sxs-lookup"><span data-stu-id="9d6b1-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9d6b1-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d6b1-130">Authorization</span></span>|<span data-ttu-id="9d6b1-131">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="9d6b1-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9d6b1-132">Accept</span><span class="sxs-lookup"><span data-stu-id="9d6b1-132">Accept</span></span>|<span data-ttu-id="9d6b1-133">application/json</span><span class="sxs-lookup"><span data-stu-id="9d6b1-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d6b1-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="9d6b1-134">Request body</span></span>
<span data-ttu-id="9d6b1-135">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="9d6b1-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9d6b1-136">応答</span><span class="sxs-lookup"><span data-stu-id="9d6b1-136">Response</span></span>
<span data-ttu-id="9d6b1-137">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [user](../resources/intune-shared-user.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="9d6b1-137">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/intune-shared-user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d6b1-138">例</span><span class="sxs-lookup"><span data-stu-id="9d6b1-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="9d6b1-139">要求</span><span class="sxs-lookup"><span data-stu-id="9d6b1-139">Request</span></span>
<span data-ttu-id="9d6b1-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9d6b1-140">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users
```

### <a name="response"></a><span data-ttu-id="9d6b1-141">応答</span><span class="sxs-lookup"><span data-stu-id="9d6b1-141">Response</span></span>
<span data-ttu-id="9d6b1-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9d6b1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 136

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
    }
  ]
}
```



