---
title: WindowsManagementAppHealthState を作成します。
description: 新しい windowsManagementAppHealthState オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: 5fec23dec7510c0b7b1a53b0be7d2dfe507959f3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359081"
---
# <a name="create-windowsmanagementapphealthstate"></a><span data-ttu-id="b43c4-103">WindowsManagementAppHealthState を作成します。</span><span class="sxs-lookup"><span data-stu-id="b43c4-103">Create windowsManagementAppHealthState</span></span>

> <span data-ttu-id="b43c4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b43c4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b43c4-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b43c4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b43c4-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b43c4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b43c4-107">新しい[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="b43c4-107">Create a new [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b43c4-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="b43c4-108">Prerequisites</span></span>
<span data-ttu-id="b43c4-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b43c4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b43c4-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b43c4-111">Permission type</span></span>|<span data-ttu-id="b43c4-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b43c4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b43c4-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b43c4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b43c4-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b43c4-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b43c4-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b43c4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b43c4-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b43c4-116">Not supported.</span></span>|
|<span data-ttu-id="b43c4-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b43c4-117">Application</span></span>|<span data-ttu-id="b43c4-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b43c4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b43c4-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b43c4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsManagementApp/healthStates
```

## <a name="request-headers"></a><span data-ttu-id="b43c4-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b43c4-120">Request headers</span></span>
|<span data-ttu-id="b43c4-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b43c4-121">Header</span></span>|<span data-ttu-id="b43c4-122">値</span><span class="sxs-lookup"><span data-stu-id="b43c4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b43c4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b43c4-123">Authorization</span></span>|<span data-ttu-id="b43c4-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b43c4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b43c4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b43c4-125">Accept</span></span>|<span data-ttu-id="b43c4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b43c4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b43c4-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="b43c4-127">Request body</span></span>
<span data-ttu-id="b43c4-128">要求の本文に windowsManagementAppHealthState オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="b43c4-128">In the request body, supply a JSON representation for the windowsManagementAppHealthState object.</span></span>

<span data-ttu-id="b43c4-129">次の表は、windowsManagementAppHealthState を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b43c4-129">The following table shows the properties that are required when you create the windowsManagementAppHealthState.</span></span>

|<span data-ttu-id="b43c4-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b43c4-130">Property</span></span>|<span data-ttu-id="b43c4-131">種類</span><span class="sxs-lookup"><span data-stu-id="b43c4-131">Type</span></span>|<span data-ttu-id="b43c4-132">説明</span><span class="sxs-lookup"><span data-stu-id="b43c4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b43c4-133">ID</span><span class="sxs-lookup"><span data-stu-id="b43c4-133">id</span></span>|<span data-ttu-id="b43c4-134">String</span><span class="sxs-lookup"><span data-stu-id="b43c4-134">String</span></span>|<span data-ttu-id="b43c4-135">Windows 管理アプリケーションの正常性状態の一意の識別子</span><span class="sxs-lookup"><span data-stu-id="b43c4-135">Unique Identifier for the Windows management app health state</span></span>|
|<span data-ttu-id="b43c4-136">healthState</span><span class="sxs-lookup"><span data-stu-id="b43c4-136">healthState</span></span>|[<span data-ttu-id="b43c4-137">healthState</span><span class="sxs-lookup"><span data-stu-id="b43c4-137">healthState</span></span>](../resources/intune-devices-healthstate.md)|<span data-ttu-id="b43c4-138">Windows 管理アプリケーションの正常性状態。</span><span class="sxs-lookup"><span data-stu-id="b43c4-138">Windows management app health state.</span></span> <span data-ttu-id="b43c4-139">可能な値は、`unknown`、`healthy`、`unhealthy` です。</span><span class="sxs-lookup"><span data-stu-id="b43c4-139">Possible values are: `unknown`, `healthy`, `unhealthy`.</span></span>|
|<span data-ttu-id="b43c4-140">installedVersion</span><span class="sxs-lookup"><span data-stu-id="b43c4-140">installedVersion</span></span>|<span data-ttu-id="b43c4-141">String</span><span class="sxs-lookup"><span data-stu-id="b43c4-141">String</span></span>|<span data-ttu-id="b43c4-142">Windows 管理アプリケーションは、バージョンをインストールします。</span><span class="sxs-lookup"><span data-stu-id="b43c4-142">Windows management app installed version.</span></span>|
|<span data-ttu-id="b43c4-143">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="b43c4-143">lastCheckInDateTime</span></span>|<span data-ttu-id="b43c4-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b43c4-144">DateTimeOffset</span></span>|<span data-ttu-id="b43c4-145">Windows 管理アプリケーション最後のチェックインの時間です。</span><span class="sxs-lookup"><span data-stu-id="b43c4-145">Windows management app last check-in time.</span></span>|
|<span data-ttu-id="b43c4-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="b43c4-146">deviceName</span></span>|<span data-ttu-id="b43c4-147">String</span><span class="sxs-lookup"><span data-stu-id="b43c4-147">String</span></span>|<span data-ttu-id="b43c4-148">Windows 管理アプリケーションがインストールされているデバイスの名前です。</span><span class="sxs-lookup"><span data-stu-id="b43c4-148">Name of the device on which Windows management app is installed.</span></span>|
|<span data-ttu-id="b43c4-149">deviceOSVersion</span><span class="sxs-lookup"><span data-stu-id="b43c4-149">deviceOSVersion</span></span>|<span data-ttu-id="b43c4-150">String</span><span class="sxs-lookup"><span data-stu-id="b43c4-150">String</span></span>|<span data-ttu-id="b43c4-151">Windows 管理アプリケーションがインストールされているデバイスの 10 の Windows OS のバージョンです。</span><span class="sxs-lookup"><span data-stu-id="b43c4-151">Windows 10 OS version of the device on which Windows management app is installed.</span></span>|



## <a name="response"></a><span data-ttu-id="b43c4-152">応答</span><span class="sxs-lookup"><span data-stu-id="b43c4-152">Response</span></span>
<span data-ttu-id="b43c4-153">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="b43c4-153">If successful, this method returns a `201 Created` response code and a [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b43c4-154">例</span><span class="sxs-lookup"><span data-stu-id="b43c4-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="b43c4-155">要求</span><span class="sxs-lookup"><span data-stu-id="b43c4-155">Request</span></span>
<span data-ttu-id="b43c4-156">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b43c4-156">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp/healthStates
Content-type: application/json
Content-length: 300

{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthState",
  "healthState": "healthy",
  "installedVersion": "Installed Version value",
  "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00",
  "deviceName": "Device Name value",
  "deviceOSVersion": "Device OSVersion value"
}
```

### <a name="response"></a><span data-ttu-id="b43c4-157">応答</span><span class="sxs-lookup"><span data-stu-id="b43c4-157">Response</span></span>
<span data-ttu-id="b43c4-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b43c4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





