---
title: updateWindowsDeviceAccount アクション
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f7ca9b880a6225702b5b5f7e5b6fcd5c26f693c4
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33909513"
---
# <a name="updatewindowsdeviceaccount-action"></a><span data-ttu-id="7ff1e-103">updateWindowsDeviceAccount アクション</span><span class="sxs-lookup"><span data-stu-id="7ff1e-103">updateWindowsDeviceAccount action</span></span>

> <span data-ttu-id="7ff1e-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7ff1e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7ff1e-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7ff1e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ff1e-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="7ff1e-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7ff1e-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="7ff1e-107">Prerequisites</span></span>
<span data-ttu-id="7ff1e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7ff1e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ff1e-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7ff1e-110">Permission type</span></span>|<span data-ttu-id="7ff1e-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7ff1e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7ff1e-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7ff1e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7ff1e-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="7ff1e-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="7ff1e-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7ff1e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7ff1e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7ff1e-115">Not supported.</span></span>|
|<span data-ttu-id="7ff1e-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7ff1e-116">Application</span></span>|<span data-ttu-id="7ff1e-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7ff1e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7ff1e-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7ff1e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/updateWindowsDeviceAccount
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
```

## <a name="request-headers"></a><span data-ttu-id="7ff1e-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7ff1e-119">Request headers</span></span>
|<span data-ttu-id="7ff1e-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7ff1e-120">Header</span></span>|<span data-ttu-id="7ff1e-121">値</span><span class="sxs-lookup"><span data-stu-id="7ff1e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7ff1e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ff1e-122">Authorization</span></span>|<span data-ttu-id="7ff1e-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="7ff1e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7ff1e-124">承諾</span><span class="sxs-lookup"><span data-stu-id="7ff1e-124">Accept</span></span>|<span data-ttu-id="7ff1e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7ff1e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ff1e-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="7ff1e-126">Request body</span></span>
<span data-ttu-id="7ff1e-127">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7ff1e-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="7ff1e-128">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="7ff1e-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="7ff1e-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7ff1e-129">Property</span></span>|<span data-ttu-id="7ff1e-130">型</span><span class="sxs-lookup"><span data-stu-id="7ff1e-130">Type</span></span>|<span data-ttu-id="7ff1e-131">説明</span><span class="sxs-lookup"><span data-stu-id="7ff1e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ff1e-132">updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="7ff1e-132">updateWindowsDeviceAccountActionParameter</span></span>|[<span data-ttu-id="7ff1e-133">updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="7ff1e-133">updateWindowsDeviceAccountActionParameter</span></span>](../resources/intune-devices-updatewindowsdeviceaccountactionparameter.md)|<span data-ttu-id="7ff1e-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="7ff1e-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7ff1e-135">応答</span><span class="sxs-lookup"><span data-stu-id="7ff1e-135">Response</span></span>
<span data-ttu-id="7ff1e-136">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="7ff1e-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7ff1e-137">例</span><span class="sxs-lookup"><span data-stu-id="7ff1e-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="7ff1e-138">要求</span><span class="sxs-lookup"><span data-stu-id="7ff1e-138">Request</span></span>
<span data-ttu-id="7ff1e-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7ff1e-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount

Content-type: application/json
Content-length: 532

{
  "updateWindowsDeviceAccountActionParameter": {
    "@odata.type": "microsoft.graph.updateWindowsDeviceAccountActionParameter",
    "deviceAccount": {
      "@odata.type": "microsoft.graph.windowsDeviceAccount",
      "password": "Password value"
    },
    "passwordRotationEnabled": true,
    "calendarSyncEnabled": true,
    "deviceAccountEmail": "Device Account Email value",
    "exchangeServer": "Exchange Server value",
    "sessionInitiationProtocalAddress": "Session Initiation Protocal Address value"
  }
}
```

### <a name="response"></a><span data-ttu-id="7ff1e-140">応答</span><span class="sxs-lookup"><span data-stu-id="7ff1e-140">Response</span></span>
<span data-ttu-id="7ff1e-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7ff1e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




