---
title: setDeviceName アクション
description: デバイスのデバイス名を設定します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a73ec88c96b80fd6d8a2cd6843cacf0ff81807bd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411856"
---
# <a name="setdevicename-action"></a><span data-ttu-id="1d6de-103">setDeviceName アクション</span><span class="sxs-lookup"><span data-stu-id="1d6de-103">setDeviceName action</span></span>

> <span data-ttu-id="1d6de-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1d6de-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1d6de-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1d6de-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1d6de-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1d6de-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d6de-107">デバイスのデバイス名を設定します。</span><span class="sxs-lookup"><span data-stu-id="1d6de-107">Set device name of the device.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1d6de-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="1d6de-108">Prerequisites</span></span>
<span data-ttu-id="1d6de-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1d6de-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1d6de-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1d6de-111">Permission type</span></span>|<span data-ttu-id="1d6de-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1d6de-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d6de-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1d6de-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1d6de-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="1d6de-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="1d6de-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1d6de-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d6de-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1d6de-116">Not supported.</span></span>|
|<span data-ttu-id="1d6de-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1d6de-117">Application</span></span>|<span data-ttu-id="1d6de-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1d6de-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d6de-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1d6de-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/setDeviceName
POST /deviceManagement/managedDevices/{managedDeviceId}/setDeviceName
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/setDeviceName
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/setDeviceName
```

## <a name="request-headers"></a><span data-ttu-id="1d6de-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1d6de-120">Request headers</span></span>
|<span data-ttu-id="1d6de-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1d6de-121">Header</span></span>|<span data-ttu-id="1d6de-122">値</span><span class="sxs-lookup"><span data-stu-id="1d6de-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1d6de-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d6de-123">Authorization</span></span>|<span data-ttu-id="1d6de-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="1d6de-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1d6de-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1d6de-125">Accept</span></span>|<span data-ttu-id="1d6de-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1d6de-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d6de-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="1d6de-127">Request body</span></span>
<span data-ttu-id="1d6de-128">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1d6de-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="1d6de-129">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="1d6de-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="1d6de-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1d6de-130">Property</span></span>|<span data-ttu-id="1d6de-131">型</span><span class="sxs-lookup"><span data-stu-id="1d6de-131">Type</span></span>|<span data-ttu-id="1d6de-132">説明</span><span class="sxs-lookup"><span data-stu-id="1d6de-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d6de-133">deviceName</span><span class="sxs-lookup"><span data-stu-id="1d6de-133">deviceName</span></span>|<span data-ttu-id="1d6de-134">String</span><span class="sxs-lookup"><span data-stu-id="1d6de-134">String</span></span>|<span data-ttu-id="1d6de-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="1d6de-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="1d6de-136">応答</span><span class="sxs-lookup"><span data-stu-id="1d6de-136">Response</span></span>
<span data-ttu-id="1d6de-137">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="1d6de-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1d6de-138">例</span><span class="sxs-lookup"><span data-stu-id="1d6de-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="1d6de-139">要求</span><span class="sxs-lookup"><span data-stu-id="1d6de-139">Request</span></span>
<span data-ttu-id="1d6de-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1d6de-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/setDeviceName

Content-type: application/json
Content-length: 41

{
  "deviceName": "Device Name value"
}
```

### <a name="response"></a><span data-ttu-id="1d6de-141">応答</span><span class="sxs-lookup"><span data-stu-id="1d6de-141">Response</span></span>
<span data-ttu-id="1d6de-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1d6de-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




