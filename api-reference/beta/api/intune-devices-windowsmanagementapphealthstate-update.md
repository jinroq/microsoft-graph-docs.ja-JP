---
title: WindowsManagementAppHealthState を更新します。
description: WindowsManagementAppHealthState オブジェクトのプロパティを更新します。
ms.openlocfilehash: e333e974e4c6ec52da3044359db5464ce9fa47bc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074008"
---
# <a name="update-windowsmanagementapphealthstate"></a><span data-ttu-id="ca8b9-103">WindowsManagementAppHealthState を更新します。</span><span class="sxs-lookup"><span data-stu-id="ca8b9-103">Update windowsManagementAppHealthState</span></span>

> <span data-ttu-id="ca8b9-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ca8b9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ca8b9-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ca8b9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ca8b9-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ca8b9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ca8b9-107">[WindowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ca8b9-107">Update the properties of a [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ca8b9-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="ca8b9-108">Prerequisites</span></span>
<span data-ttu-id="ca8b9-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ca8b9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca8b9-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ca8b9-111">Permission type</span></span>|<span data-ttu-id="ca8b9-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ca8b9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca8b9-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ca8b9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ca8b9-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca8b9-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ca8b9-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ca8b9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca8b9-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ca8b9-116">Not supported.</span></span>|
|<span data-ttu-id="ca8b9-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ca8b9-117">Application</span></span>|<span data-ttu-id="ca8b9-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ca8b9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca8b9-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ca8b9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp/healthStates/{windowsManagementAppHealthStateId}
```

## <a name="request-headers"></a><span data-ttu-id="ca8b9-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ca8b9-120">Request headers</span></span>
|<span data-ttu-id="ca8b9-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ca8b9-121">Header</span></span>|<span data-ttu-id="ca8b9-122">値</span><span class="sxs-lookup"><span data-stu-id="ca8b9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca8b9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca8b9-123">Authorization</span></span>|<span data-ttu-id="ca8b9-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="ca8b9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca8b9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ca8b9-125">Accept</span></span>|<span data-ttu-id="ca8b9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ca8b9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca8b9-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="ca8b9-127">Request body</span></span>
<span data-ttu-id="ca8b9-128">要求の本文に[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="ca8b9-128">In the request body, supply a JSON representation for the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>

<span data-ttu-id="ca8b9-129">[WindowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="ca8b9-129">The following table shows the properties that are required when you create the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md).</span></span>

|<span data-ttu-id="ca8b9-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ca8b9-130">Property</span></span>|<span data-ttu-id="ca8b9-131">型</span><span class="sxs-lookup"><span data-stu-id="ca8b9-131">Type</span></span>|<span data-ttu-id="ca8b9-132">説明</span><span class="sxs-lookup"><span data-stu-id="ca8b9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca8b9-133">id</span><span class="sxs-lookup"><span data-stu-id="ca8b9-133">id</span></span>|<span data-ttu-id="ca8b9-134">String</span><span class="sxs-lookup"><span data-stu-id="ca8b9-134">String</span></span>|<span data-ttu-id="ca8b9-135">Windows 管理アプリケーションの正常性状態の一意の識別子</span><span class="sxs-lookup"><span data-stu-id="ca8b9-135">Unique Identifier for the Windows management app health state</span></span>|
|<span data-ttu-id="ca8b9-136">healthState</span><span class="sxs-lookup"><span data-stu-id="ca8b9-136">healthState</span></span>|[<span data-ttu-id="ca8b9-137">healthState</span><span class="sxs-lookup"><span data-stu-id="ca8b9-137">healthState</span></span>](../resources/intune-devices-healthstate.md)|<span data-ttu-id="ca8b9-138">Windows 管理アプリケーションの正常性状態。</span><span class="sxs-lookup"><span data-stu-id="ca8b9-138">Windows management app health state.</span></span> <span data-ttu-id="ca8b9-139">可能な値は、`unknown`、`healthy`、`unhealthy` です。</span><span class="sxs-lookup"><span data-stu-id="ca8b9-139">Possible values are: `unknown`, `healthy`, `unhealthy`.</span></span>|
|<span data-ttu-id="ca8b9-140">installedVersion</span><span class="sxs-lookup"><span data-stu-id="ca8b9-140">installedVersion</span></span>|<span data-ttu-id="ca8b9-141">String</span><span class="sxs-lookup"><span data-stu-id="ca8b9-141">String</span></span>|<span data-ttu-id="ca8b9-142">Windows 管理アプリケーションは、バージョンをインストールします。</span><span class="sxs-lookup"><span data-stu-id="ca8b9-142">Windows management app installed version.</span></span>|
|<span data-ttu-id="ca8b9-143">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="ca8b9-143">lastCheckInDateTime</span></span>|<span data-ttu-id="ca8b9-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca8b9-144">DateTimeOffset</span></span>|<span data-ttu-id="ca8b9-145">Windows 管理アプリケーション最後のチェックインの時間です。</span><span class="sxs-lookup"><span data-stu-id="ca8b9-145">Windows management app last check-in time.</span></span>|
|<span data-ttu-id="ca8b9-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="ca8b9-146">deviceName</span></span>|<span data-ttu-id="ca8b9-147">String</span><span class="sxs-lookup"><span data-stu-id="ca8b9-147">String</span></span>|<span data-ttu-id="ca8b9-148">Windows 管理アプリケーションがインストールされているデバイスの名前です。</span><span class="sxs-lookup"><span data-stu-id="ca8b9-148">Name of the device on which Windows management app is installed.</span></span>|
|<span data-ttu-id="ca8b9-149">deviceOSVersion</span><span class="sxs-lookup"><span data-stu-id="ca8b9-149">deviceOSVersion</span></span>|<span data-ttu-id="ca8b9-150">String</span><span class="sxs-lookup"><span data-stu-id="ca8b9-150">String</span></span>|<span data-ttu-id="ca8b9-151">Windows 管理アプリケーションがインストールされているデバイスの 10 の Windows OS のバージョンです。</span><span class="sxs-lookup"><span data-stu-id="ca8b9-151">Windows 10 OS version of the device on which Windows management app is installed.</span></span>|



## <a name="response"></a><span data-ttu-id="ca8b9-152">応答</span><span class="sxs-lookup"><span data-stu-id="ca8b9-152">Response</span></span>
<span data-ttu-id="ca8b9-153">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="ca8b9-153">If successful, this method returns a `200 OK` response code and an updated [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca8b9-154">例</span><span class="sxs-lookup"><span data-stu-id="ca8b9-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="ca8b9-155">要求</span><span class="sxs-lookup"><span data-stu-id="ca8b9-155">Request</span></span>
<span data-ttu-id="ca8b9-156">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ca8b9-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp/healthStates/{windowsManagementAppHealthStateId}
Content-type: application/json
Content-length: 230

{
  "healthState": "healthy",
  "installedVersion": "Installed Version value",
  "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00",
  "deviceName": "Device Name value",
  "deviceOSVersion": "Device OSVersion value"
}
```

### <a name="response"></a><span data-ttu-id="ca8b9-157">応答</span><span class="sxs-lookup"><span data-stu-id="ca8b9-157">Response</span></span>
<span data-ttu-id="ca8b9-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ca8b9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 349

{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthState",
  "id": "5c7e50fb-50fb-5c7e-fb50-7e5cfb507e5c",
  "healthState": "healthy",
  "installedVersion": "Installed Version value",
  "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00",
  "deviceName": "Device Name value",
  "deviceOSVersion": "Device OSVersion value"
}
```





