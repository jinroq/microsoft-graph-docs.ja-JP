---
title: リスト windowsManagementAppHealthStates
description: windowsmanagementapphealthstate オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f417b29a8699d8b1ade4195992cf5ec431c8a67f
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31779700"
---
# <a name="list-windowsmanagementapphealthstates"></a><span data-ttu-id="e8599-103">リスト windowsManagementAppHealthStates</span><span class="sxs-lookup"><span data-stu-id="e8599-103">List windowsManagementAppHealthStates</span></span>

> <span data-ttu-id="e8599-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e8599-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8599-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e8599-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8599-106">[windowsmanagementapphealthstate](../resources/intune-devices-windowsmanagementapphealthstate.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="e8599-106">List properties and relationships of the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e8599-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="e8599-107">Prerequisites</span></span>
<span data-ttu-id="e8599-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e8599-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8599-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e8599-110">Permission type</span></span>|<span data-ttu-id="e8599-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e8599-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8599-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e8599-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e8599-113">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e8599-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="e8599-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e8599-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8599-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e8599-115">Not supported.</span></span>|
|<span data-ttu-id="e8599-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e8599-116">Application</span></span>|<span data-ttu-id="e8599-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e8599-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8599-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e8599-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsManagementApp/healthStates
```

## <a name="request-headers"></a><span data-ttu-id="e8599-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e8599-119">Request headers</span></span>
|<span data-ttu-id="e8599-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e8599-120">Header</span></span>|<span data-ttu-id="e8599-121">値</span><span class="sxs-lookup"><span data-stu-id="e8599-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8599-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8599-122">Authorization</span></span>|<span data-ttu-id="e8599-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="e8599-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8599-124">承諾</span><span class="sxs-lookup"><span data-stu-id="e8599-124">Accept</span></span>|<span data-ttu-id="e8599-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e8599-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8599-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="e8599-126">Request body</span></span>
<span data-ttu-id="e8599-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e8599-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8599-128">応答</span><span class="sxs-lookup"><span data-stu-id="e8599-128">Response</span></span>
<span data-ttu-id="e8599-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[windowsmanagementapphealthstate](../resources/intune-devices-windowsmanagementapphealthstate.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="e8599-129">If successful, this method returns a `200 OK` response code and a collection of [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8599-130">例</span><span class="sxs-lookup"><span data-stu-id="e8599-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8599-131">要求</span><span class="sxs-lookup"><span data-stu-id="e8599-131">Request</span></span>
<span data-ttu-id="e8599-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e8599-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp/healthStates
```

### <a name="response"></a><span data-ttu-id="e8599-133">応答</span><span class="sxs-lookup"><span data-stu-id="e8599-133">Response</span></span>
<span data-ttu-id="e8599-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e8599-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 410

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsManagementAppHealthState",
      "id": "5c7e50fb-50fb-5c7e-fb50-7e5cfb507e5c",
      "healthState": "healthy",
      "installedVersion": "Installed Version value",
      "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00",
      "deviceName": "Device Name value",
      "deviceOSVersion": "Device OSVersion value"
    }
  ]
}
```





