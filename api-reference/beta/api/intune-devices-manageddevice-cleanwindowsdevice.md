---
title: cleanWindowsDevice アクション
description: Windows デバイスをクリーンにします
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 892316771f422376f95f44f502296c50589d0565
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410295"
---
# <a name="cleanwindowsdevice-action"></a><span data-ttu-id="95904-103">cleanWindowsDevice アクション</span><span class="sxs-lookup"><span data-stu-id="95904-103">cleanWindowsDevice action</span></span>

> <span data-ttu-id="95904-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="95904-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="95904-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95904-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="95904-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="95904-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95904-107">Windows デバイスをクリーンにします</span><span class="sxs-lookup"><span data-stu-id="95904-107">Clean Windows device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="95904-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="95904-108">Prerequisites</span></span>
<span data-ttu-id="95904-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="95904-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="95904-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="95904-111">Permission type</span></span>|<span data-ttu-id="95904-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="95904-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95904-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="95904-113">Delegated (work or school account)</span></span>|<span data-ttu-id="95904-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="95904-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="95904-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="95904-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95904-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95904-116">Not supported.</span></span>|
|<span data-ttu-id="95904-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="95904-117">Application</span></span>|<span data-ttu-id="95904-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95904-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="95904-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="95904-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/cleanWindowsDevice
POST /deviceManagement/managedDevices/{managedDeviceId}/cleanWindowsDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/cleanWindowsDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/cleanWindowsDevice
```

## <a name="request-headers"></a><span data-ttu-id="95904-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="95904-120">Request headers</span></span>
|<span data-ttu-id="95904-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="95904-121">Header</span></span>|<span data-ttu-id="95904-122">値</span><span class="sxs-lookup"><span data-stu-id="95904-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95904-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="95904-123">Authorization</span></span>|<span data-ttu-id="95904-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="95904-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95904-125">Accept</span><span class="sxs-lookup"><span data-stu-id="95904-125">Accept</span></span>|<span data-ttu-id="95904-126">application/json</span><span class="sxs-lookup"><span data-stu-id="95904-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95904-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="95904-127">Request body</span></span>
<span data-ttu-id="95904-128">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="95904-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="95904-129">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="95904-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="95904-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="95904-130">Property</span></span>|<span data-ttu-id="95904-131">型</span><span class="sxs-lookup"><span data-stu-id="95904-131">Type</span></span>|<span data-ttu-id="95904-132">説明</span><span class="sxs-lookup"><span data-stu-id="95904-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95904-133">keepUserData</span><span class="sxs-lookup"><span data-stu-id="95904-133">keepUserData</span></span>|<span data-ttu-id="95904-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="95904-134">Boolean</span></span>|<span data-ttu-id="95904-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="95904-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="95904-136">応答</span><span class="sxs-lookup"><span data-stu-id="95904-136">Response</span></span>
<span data-ttu-id="95904-137">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="95904-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="95904-138">例</span><span class="sxs-lookup"><span data-stu-id="95904-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="95904-139">要求</span><span class="sxs-lookup"><span data-stu-id="95904-139">Request</span></span>
<span data-ttu-id="95904-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="95904-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/cleanWindowsDevice

Content-type: application/json
Content-length: 28

{
  "keepUserData": true
}
```

### <a name="response"></a><span data-ttu-id="95904-141">応答</span><span class="sxs-lookup"><span data-stu-id="95904-141">Response</span></span>
<span data-ttu-id="95904-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="95904-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




