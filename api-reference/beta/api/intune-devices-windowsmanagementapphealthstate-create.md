---
title: windowsmanagementapphealthstate を作成する
description: 新しい windowsmanagementapphealthstate オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c275825fb5222fcb1a77ed2bd8abce6d76c75594
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534375"
---
# <a name="create-windowsmanagementapphealthstate"></a><span data-ttu-id="e76c1-103">windowsmanagementapphealthstate を作成する</span><span class="sxs-lookup"><span data-stu-id="e76c1-103">Create windowsManagementAppHealthState</span></span>

> <span data-ttu-id="e76c1-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e76c1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e76c1-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e76c1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e76c1-106">新しい[windowsmanagementapphealthstate](../resources/intune-devices-windowsmanagementapphealthstate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="e76c1-106">Create a new [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e76c1-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="e76c1-107">Prerequisites</span></span>
<span data-ttu-id="e76c1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e76c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e76c1-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e76c1-110">Permission type</span></span>|<span data-ttu-id="e76c1-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e76c1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e76c1-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e76c1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e76c1-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e76c1-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e76c1-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e76c1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e76c1-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e76c1-115">Not supported.</span></span>|
|<span data-ttu-id="e76c1-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e76c1-116">Application</span></span>|<span data-ttu-id="e76c1-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e76c1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e76c1-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e76c1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsManagementApp/healthStates
```

## <a name="request-headers"></a><span data-ttu-id="e76c1-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e76c1-119">Request headers</span></span>
|<span data-ttu-id="e76c1-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e76c1-120">Header</span></span>|<span data-ttu-id="e76c1-121">値</span><span class="sxs-lookup"><span data-stu-id="e76c1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e76c1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e76c1-122">Authorization</span></span>|<span data-ttu-id="e76c1-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="e76c1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e76c1-124">承諾</span><span class="sxs-lookup"><span data-stu-id="e76c1-124">Accept</span></span>|<span data-ttu-id="e76c1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e76c1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e76c1-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="e76c1-126">Request body</span></span>
<span data-ttu-id="e76c1-127">要求本文で、windowsmanagementapphealthstate オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e76c1-127">In the request body, supply a JSON representation for the windowsManagementAppHealthState object.</span></span>

<span data-ttu-id="e76c1-128">次の表に、windowsmanagementapphealthstate の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e76c1-128">The following table shows the properties that are required when you create the windowsManagementAppHealthState.</span></span>

|<span data-ttu-id="e76c1-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e76c1-129">Property</span></span>|<span data-ttu-id="e76c1-130">型</span><span class="sxs-lookup"><span data-stu-id="e76c1-130">Type</span></span>|<span data-ttu-id="e76c1-131">説明</span><span class="sxs-lookup"><span data-stu-id="e76c1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e76c1-132">id</span><span class="sxs-lookup"><span data-stu-id="e76c1-132">id</span></span>|<span data-ttu-id="e76c1-133">String</span><span class="sxs-lookup"><span data-stu-id="e76c1-133">String</span></span>|<span data-ttu-id="e76c1-134">Windows management アプリの正常性状態の一意識別子</span><span class="sxs-lookup"><span data-stu-id="e76c1-134">Unique Identifier for the Windows management app health state</span></span>|
|<span data-ttu-id="e76c1-135">healthState</span><span class="sxs-lookup"><span data-stu-id="e76c1-135">healthState</span></span>|[<span data-ttu-id="e76c1-136">healthState</span><span class="sxs-lookup"><span data-stu-id="e76c1-136">healthState</span></span>](../resources/intune-devices-healthstate.md)|<span data-ttu-id="e76c1-137">Windows management アプリの正常性状態。</span><span class="sxs-lookup"><span data-stu-id="e76c1-137">Windows management app health state.</span></span> <span data-ttu-id="e76c1-138">使用可能な値は、`unknown`、`healthy`、`unhealthy` です。</span><span class="sxs-lookup"><span data-stu-id="e76c1-138">Possible values are: `unknown`, `healthy`, `unhealthy`.</span></span>|
|<span data-ttu-id="e76c1-139">バージョン</span><span class="sxs-lookup"><span data-stu-id="e76c1-139">installedVersion</span></span>|<span data-ttu-id="e76c1-140">String</span><span class="sxs-lookup"><span data-stu-id="e76c1-140">String</span></span>|<span data-ttu-id="e76c1-141">Windows management アプリがインストールされているバージョン。</span><span class="sxs-lookup"><span data-stu-id="e76c1-141">Windows management app installed version.</span></span>|
|<span data-ttu-id="e76c1-142">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="e76c1-142">lastCheckInDateTime</span></span>|<span data-ttu-id="e76c1-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e76c1-143">DateTimeOffset</span></span>|<span data-ttu-id="e76c1-144">Windows management アプリの最終チェックイン時刻。</span><span class="sxs-lookup"><span data-stu-id="e76c1-144">Windows management app last check-in time.</span></span>|
|<span data-ttu-id="e76c1-145">deviceName</span><span class="sxs-lookup"><span data-stu-id="e76c1-145">deviceName</span></span>|<span data-ttu-id="e76c1-146">String</span><span class="sxs-lookup"><span data-stu-id="e76c1-146">String</span></span>|<span data-ttu-id="e76c1-147">Windows management アプリがインストールされているデバイスの名前。</span><span class="sxs-lookup"><span data-stu-id="e76c1-147">Name of the device on which Windows management app is installed.</span></span>|
|<span data-ttu-id="e76c1-148">deviceosversion</span><span class="sxs-lookup"><span data-stu-id="e76c1-148">deviceOSVersion</span></span>|<span data-ttu-id="e76c1-149">String</span><span class="sxs-lookup"><span data-stu-id="e76c1-149">String</span></span>|<span data-ttu-id="e76c1-150">windows 管理アプリがインストールされているデバイスの windows 10 OS バージョン。</span><span class="sxs-lookup"><span data-stu-id="e76c1-150">Windows 10 OS version of the device on which Windows management app is installed.</span></span>|



## <a name="response"></a><span data-ttu-id="e76c1-151">応答</span><span class="sxs-lookup"><span data-stu-id="e76c1-151">Response</span></span>
<span data-ttu-id="e76c1-152">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[windowsmanagementapphealthstate](../resources/intune-devices-windowsmanagementapphealthstate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e76c1-152">If successful, this method returns a `201 Created` response code and a [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e76c1-153">例</span><span class="sxs-lookup"><span data-stu-id="e76c1-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="e76c1-154">要求</span><span class="sxs-lookup"><span data-stu-id="e76c1-154">Request</span></span>
<span data-ttu-id="e76c1-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e76c1-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e76c1-156">応答</span><span class="sxs-lookup"><span data-stu-id="e76c1-156">Response</span></span>
<span data-ttu-id="e76c1-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e76c1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





