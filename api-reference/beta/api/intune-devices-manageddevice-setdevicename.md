---
title: setDeviceName アクション
description: デバイスのデバイス名を設定します。
author: tfitzmac
ms.openlocfilehash: 9856e9698da807e3bb3af1a3c30fa7e138569f48
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352172"
---
# <a name="setdevicename-action"></a><span data-ttu-id="da740-103">setDeviceName アクション</span><span class="sxs-lookup"><span data-stu-id="da740-103">setDeviceName action</span></span>

> <span data-ttu-id="da740-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="da740-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="da740-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="da740-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="da740-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="da740-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="da740-107">デバイスのデバイス名を設定します。</span><span class="sxs-lookup"><span data-stu-id="da740-107">Set device name of the device.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="da740-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="da740-108">Prerequisites</span></span>
<span data-ttu-id="da740-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="da740-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da740-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="da740-111">Permission type</span></span>|<span data-ttu-id="da740-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="da740-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da740-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="da740-113">Delegated (work or school account)</span></span>|<span data-ttu-id="da740-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="da740-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="da740-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="da740-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da740-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="da740-116">Not supported.</span></span>|
|<span data-ttu-id="da740-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="da740-117">Application</span></span>|<span data-ttu-id="da740-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="da740-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="da740-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="da740-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="da740-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="da740-120">Request headers</span></span>
|<span data-ttu-id="da740-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="da740-121">Header</span></span>|<span data-ttu-id="da740-122">値</span><span class="sxs-lookup"><span data-stu-id="da740-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da740-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="da740-123">Authorization</span></span>|<span data-ttu-id="da740-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="da740-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da740-125">Accept</span><span class="sxs-lookup"><span data-stu-id="da740-125">Accept</span></span>|<span data-ttu-id="da740-126">application/json</span><span class="sxs-lookup"><span data-stu-id="da740-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da740-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="da740-127">Request body</span></span>
<span data-ttu-id="da740-128">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="da740-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="da740-129">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="da740-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="da740-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="da740-130">Property</span></span>|<span data-ttu-id="da740-131">種類</span><span class="sxs-lookup"><span data-stu-id="da740-131">Type</span></span>|<span data-ttu-id="da740-132">説明</span><span class="sxs-lookup"><span data-stu-id="da740-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da740-133">deviceName</span><span class="sxs-lookup"><span data-stu-id="da740-133">deviceName</span></span>|<span data-ttu-id="da740-134">String</span><span class="sxs-lookup"><span data-stu-id="da740-134">String</span></span>|<span data-ttu-id="da740-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="da740-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="da740-136">応答</span><span class="sxs-lookup"><span data-stu-id="da740-136">Response</span></span>
<span data-ttu-id="da740-137">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="da740-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="da740-138">例</span><span class="sxs-lookup"><span data-stu-id="da740-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="da740-139">要求</span><span class="sxs-lookup"><span data-stu-id="da740-139">Request</span></span>
<span data-ttu-id="da740-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="da740-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/setDeviceName

Content-type: application/json
Content-length: 41

{
  "deviceName": "Device Name value"
}
```

### <a name="response"></a><span data-ttu-id="da740-141">応答</span><span class="sxs-lookup"><span data-stu-id="da740-141">Response</span></span>
<span data-ttu-id="da740-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="da740-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





