---
title: wipe action
description: デバイスをワイプする
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5d50366cef1660aec80137562e912746b81f162f
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33909492"
---
# <a name="wipe-action"></a><span data-ttu-id="82def-103">ワイプ アクション</span><span class="sxs-lookup"><span data-stu-id="82def-103">wipe action</span></span>

> <span data-ttu-id="82def-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="82def-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82def-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="82def-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82def-106">デバイスをワイプする</span><span class="sxs-lookup"><span data-stu-id="82def-106">Wipe a device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="82def-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="82def-107">Prerequisites</span></span>
<span data-ttu-id="82def-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="82def-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82def-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="82def-110">Permission type</span></span>|<span data-ttu-id="82def-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="82def-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82def-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="82def-112">Delegated (work or school account)</span></span>|<span data-ttu-id="82def-113">Devicemanagementmanageddevices all、DeviceManagementManagedDevices. すべて</span><span class="sxs-lookup"><span data-stu-id="82def-113">DeviceManagementManagedDevices.PriviligedOperation.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="82def-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="82def-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82def-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="82def-115">Not supported.</span></span>|
|<span data-ttu-id="82def-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="82def-116">Application</span></span>|<span data-ttu-id="82def-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="82def-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="82def-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="82def-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/wipe
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/wipe
```

## <a name="request-headers"></a><span data-ttu-id="82def-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="82def-119">Request headers</span></span>
|<span data-ttu-id="82def-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="82def-120">Header</span></span>|<span data-ttu-id="82def-121">値</span><span class="sxs-lookup"><span data-stu-id="82def-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82def-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="82def-122">Authorization</span></span>|<span data-ttu-id="82def-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="82def-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82def-124">承諾</span><span class="sxs-lookup"><span data-stu-id="82def-124">Accept</span></span>|<span data-ttu-id="82def-125">application/json</span><span class="sxs-lookup"><span data-stu-id="82def-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82def-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="82def-126">Request body</span></span>
<span data-ttu-id="82def-127">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="82def-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="82def-128">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="82def-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="82def-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="82def-129">Property</span></span>|<span data-ttu-id="82def-130">型</span><span class="sxs-lookup"><span data-stu-id="82def-130">Type</span></span>|<span data-ttu-id="82def-131">説明</span><span class="sxs-lookup"><span data-stu-id="82def-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82def-132">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="82def-132">keepEnrollmentData</span></span>|<span data-ttu-id="82def-133">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="82def-133">Boolean</span></span>|<span data-ttu-id="82def-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="82def-134">Not yet documented</span></span>|
|<span data-ttu-id="82def-135">keepUserData</span><span class="sxs-lookup"><span data-stu-id="82def-135">keepUserData</span></span>|<span data-ttu-id="82def-136">ブール値</span><span class="sxs-lookup"><span data-stu-id="82def-136">Boolean</span></span>|<span data-ttu-id="82def-137">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="82def-137">Not yet documented</span></span>|
|<span data-ttu-id="82def-138">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="82def-138">macOsUnlockCode</span></span>|<span data-ttu-id="82def-139">文字列</span><span class="sxs-lookup"><span data-stu-id="82def-139">String</span></span>|<span data-ttu-id="82def-140">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="82def-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="82def-141">応答</span><span class="sxs-lookup"><span data-stu-id="82def-141">Response</span></span>
<span data-ttu-id="82def-142">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="82def-142">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="82def-143">例</span><span class="sxs-lookup"><span data-stu-id="82def-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="82def-144">要求</span><span class="sxs-lookup"><span data-stu-id="82def-144">Request</span></span>
<span data-ttu-id="82def-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="82def-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/wipe

Content-type: application/json
Content-length: 109

{
  "keepEnrollmentData": true,
  "keepUserData": true,
  "macOsUnlockCode": "Mac Os Unlock Code value"
}
```

### <a name="response"></a><span data-ttu-id="82def-146">応答</span><span class="sxs-lookup"><span data-stu-id="82def-146">Response</span></span>
<span data-ttu-id="82def-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="82def-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




