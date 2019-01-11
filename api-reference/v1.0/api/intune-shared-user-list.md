---
title: ユーザーを一覧表示する
description: user オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f286cd3bdb49f99fcc8db52b1fee8c204ccdee7c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856789"
---
# <a name="list-users"></a><span data-ttu-id="b4759-103">users のリスト</span><span class="sxs-lookup"><span data-stu-id="b4759-103">List users</span></span>

> <span data-ttu-id="b4759-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b4759-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b4759-105">[user](../resources/intune-shared-user.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="b4759-105">List properties and relationships of the [user](../resources/intune-shared-user.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b4759-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="b4759-106">Prerequisites</span></span>
<span data-ttu-id="b4759-107">この API を呼び出すには次のアクセス許可のいずれかが必要です。</span><span class="sxs-lookup"><span data-stu-id="b4759-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="b4759-108">アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b4759-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="b4759-109">特定のアクセス許可は、コンテキストに依存します。</span><span class="sxs-lookup"><span data-stu-id="b4759-109">The specific permission depends on the context.</span></span>

|<span data-ttu-id="b4759-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b4759-110">Permission type</span></span>|<span data-ttu-id="b4759-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b4759-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4759-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b4759-112">Delegated (work or school account)</span></span>| <span data-ttu-id="b4759-113">_コンテキストによって異なります_</span><span class="sxs-lookup"><span data-stu-id="b4759-113">_varies by context_</span></span>|
| <span data-ttu-id="b4759-114">&nbsp;&nbsp;デバイスの管理</span><span class="sxs-lookup"><span data-stu-id="b4759-114">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="b4759-115">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b4759-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="b4759-116">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="b4759-116">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="b4759-117">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b4759-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="b4759-118">&nbsp;&nbsp;契約時</span><span class="sxs-lookup"><span data-stu-id="b4759-118">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="b4759-119">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b4759-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="b4759-120">&nbsp;&nbsp;のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="b4759-120">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="b4759-121">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b4759-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="b4759-122">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b4759-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4759-123">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b4759-123">Not supported.</span></span>|
|<span data-ttu-id="b4759-124">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b4759-124">Application</span></span>|<span data-ttu-id="b4759-125">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b4759-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4759-126">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b4759-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users
```

## <a name="request-headers"></a><span data-ttu-id="b4759-127">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b4759-127">Request headers</span></span>
|<span data-ttu-id="b4759-128">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b4759-128">Header</span></span>|<span data-ttu-id="b4759-129">値</span><span class="sxs-lookup"><span data-stu-id="b4759-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4759-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4759-130">Authorization</span></span>|<span data-ttu-id="b4759-131">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b4759-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4759-132">Accept</span><span class="sxs-lookup"><span data-stu-id="b4759-132">Accept</span></span>|<span data-ttu-id="b4759-133">application/json</span><span class="sxs-lookup"><span data-stu-id="b4759-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4759-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="b4759-134">Request body</span></span>
<span data-ttu-id="b4759-135">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b4759-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b4759-136">応答</span><span class="sxs-lookup"><span data-stu-id="b4759-136">Response</span></span>
<span data-ttu-id="b4759-137">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [user](../resources/intune-shared-user.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="b4759-137">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/intune-shared-user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4759-138">例</span><span class="sxs-lookup"><span data-stu-id="b4759-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="b4759-139">要求</span><span class="sxs-lookup"><span data-stu-id="b4759-139">Request</span></span>
<span data-ttu-id="b4759-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b4759-140">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users
```

### <a name="response"></a><span data-ttu-id="b4759-141">応答</span><span class="sxs-lookup"><span data-stu-id="b4759-141">Response</span></span>
<span data-ttu-id="b4759-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b4759-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



