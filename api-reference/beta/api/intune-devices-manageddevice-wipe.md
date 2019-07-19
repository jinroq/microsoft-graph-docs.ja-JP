---
title: wipe action
description: デバイスをワイプする
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7b7c1c39104180e6edc82fc49b21d2df05687340
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34958131"
---
# <a name="wipe-action"></a><span data-ttu-id="fe3e5-103">ワイプ アクション</span><span class="sxs-lookup"><span data-stu-id="fe3e5-103">wipe action</span></span>

> <span data-ttu-id="fe3e5-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fe3e5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fe3e5-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="fe3e5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe3e5-106">デバイスをワイプする</span><span class="sxs-lookup"><span data-stu-id="fe3e5-106">Wipe a device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fe3e5-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="fe3e5-107">Prerequisites</span></span>
<span data-ttu-id="fe3e5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fe3e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe3e5-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fe3e5-110">Permission type</span></span>|<span data-ttu-id="fe3e5-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="fe3e5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe3e5-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fe3e5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fe3e5-113">Devicemanagementmanageddevices all、DeviceManagementManagedDevices. すべて</span><span class="sxs-lookup"><span data-stu-id="fe3e5-113">DeviceManagementManagedDevices.PriviligedOperation.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="fe3e5-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fe3e5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe3e5-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fe3e5-115">Not supported.</span></span>|
|<span data-ttu-id="fe3e5-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fe3e5-116">Application</span></span>|<span data-ttu-id="fe3e5-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fe3e5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe3e5-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fe3e5-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="fe3e5-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fe3e5-119">Request headers</span></span>
|<span data-ttu-id="fe3e5-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fe3e5-120">Header</span></span>|<span data-ttu-id="fe3e5-121">値</span><span class="sxs-lookup"><span data-stu-id="fe3e5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe3e5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe3e5-122">Authorization</span></span>|<span data-ttu-id="fe3e5-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="fe3e5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe3e5-124">承諾</span><span class="sxs-lookup"><span data-stu-id="fe3e5-124">Accept</span></span>|<span data-ttu-id="fe3e5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fe3e5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe3e5-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="fe3e5-126">Request body</span></span>
<span data-ttu-id="fe3e5-127">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="fe3e5-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="fe3e5-128">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="fe3e5-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="fe3e5-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fe3e5-129">Property</span></span>|<span data-ttu-id="fe3e5-130">型</span><span class="sxs-lookup"><span data-stu-id="fe3e5-130">Type</span></span>|<span data-ttu-id="fe3e5-131">説明</span><span class="sxs-lookup"><span data-stu-id="fe3e5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe3e5-132">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="fe3e5-132">keepEnrollmentData</span></span>|<span data-ttu-id="fe3e5-133">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="fe3e5-133">Boolean</span></span>|<span data-ttu-id="fe3e5-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="fe3e5-134">Not yet documented</span></span>|
|<span data-ttu-id="fe3e5-135">keepUserData</span><span class="sxs-lookup"><span data-stu-id="fe3e5-135">keepUserData</span></span>|<span data-ttu-id="fe3e5-136">ブール値</span><span class="sxs-lookup"><span data-stu-id="fe3e5-136">Boolean</span></span>|<span data-ttu-id="fe3e5-137">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="fe3e5-137">Not yet documented</span></span>|
|<span data-ttu-id="fe3e5-138">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="fe3e5-138">macOsUnlockCode</span></span>|<span data-ttu-id="fe3e5-139">文字列</span><span class="sxs-lookup"><span data-stu-id="fe3e5-139">String</span></span>|<span data-ttu-id="fe3e5-140">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="fe3e5-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="fe3e5-141">応答</span><span class="sxs-lookup"><span data-stu-id="fe3e5-141">Response</span></span>
<span data-ttu-id="fe3e5-142">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="fe3e5-142">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fe3e5-143">例</span><span class="sxs-lookup"><span data-stu-id="fe3e5-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="fe3e5-144">要求</span><span class="sxs-lookup"><span data-stu-id="fe3e5-144">Request</span></span>
<span data-ttu-id="fe3e5-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fe3e5-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fe3e5-146">応答</span><span class="sxs-lookup"><span data-stu-id="fe3e5-146">Response</span></span>
<span data-ttu-id="fe3e5-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fe3e5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





