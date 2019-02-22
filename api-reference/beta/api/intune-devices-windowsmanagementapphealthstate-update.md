---
title: windowsmanagementapphealthstate を更新する
description: windowsmanagementapphealthstate オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: de6314de3699821f15125d75241d3df509d52c64
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160551"
---
# <a name="update-windowsmanagementapphealthstate"></a><span data-ttu-id="c5f71-103">windowsmanagementapphealthstate を更新する</span><span class="sxs-lookup"><span data-stu-id="c5f71-103">Update windowsManagementAppHealthState</span></span>

> <span data-ttu-id="c5f71-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c5f71-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5f71-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c5f71-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5f71-106">[windowsmanagementapphealthstate](../resources/intune-devices-windowsmanagementapphealthstate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c5f71-106">Update the properties of a [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c5f71-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="c5f71-107">Prerequisites</span></span>
<span data-ttu-id="c5f71-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c5f71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c5f71-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c5f71-110">Permission type</span></span>|<span data-ttu-id="c5f71-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c5f71-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5f71-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c5f71-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c5f71-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5f71-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c5f71-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c5f71-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5f71-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c5f71-115">Not supported.</span></span>|
|<span data-ttu-id="c5f71-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c5f71-116">Application</span></span>|<span data-ttu-id="c5f71-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c5f71-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5f71-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c5f71-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp/healthStates/{windowsManagementAppHealthStateId}
```

## <a name="request-headers"></a><span data-ttu-id="c5f71-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c5f71-119">Request headers</span></span>
|<span data-ttu-id="c5f71-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c5f71-120">Header</span></span>|<span data-ttu-id="c5f71-121">値</span><span class="sxs-lookup"><span data-stu-id="c5f71-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5f71-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5f71-122">Authorization</span></span>|<span data-ttu-id="c5f71-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="c5f71-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5f71-124">承諾</span><span class="sxs-lookup"><span data-stu-id="c5f71-124">Accept</span></span>|<span data-ttu-id="c5f71-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c5f71-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5f71-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="c5f71-126">Request body</span></span>
<span data-ttu-id="c5f71-127">要求本文で、 [windowsmanagementapphealthstate](../resources/intune-devices-windowsmanagementapphealthstate.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c5f71-127">In the request body, supply a JSON representation for the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>

<span data-ttu-id="c5f71-128">次の表に、 [windowsmanagementapphealthstate](../resources/intune-devices-windowsmanagementapphealthstate.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="c5f71-128">The following table shows the properties that are required when you create the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md).</span></span>

|<span data-ttu-id="c5f71-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c5f71-129">Property</span></span>|<span data-ttu-id="c5f71-130">型</span><span class="sxs-lookup"><span data-stu-id="c5f71-130">Type</span></span>|<span data-ttu-id="c5f71-131">説明</span><span class="sxs-lookup"><span data-stu-id="c5f71-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5f71-132">id</span><span class="sxs-lookup"><span data-stu-id="c5f71-132">id</span></span>|<span data-ttu-id="c5f71-133">文字列</span><span class="sxs-lookup"><span data-stu-id="c5f71-133">String</span></span>|<span data-ttu-id="c5f71-134">Windows management アプリの正常性状態の一意識別子</span><span class="sxs-lookup"><span data-stu-id="c5f71-134">Unique Identifier for the Windows management app health state</span></span>|
|<span data-ttu-id="c5f71-135">healthState</span><span class="sxs-lookup"><span data-stu-id="c5f71-135">healthState</span></span>|[<span data-ttu-id="c5f71-136">healthState</span><span class="sxs-lookup"><span data-stu-id="c5f71-136">healthState</span></span>](../resources/intune-devices-healthstate.md)|<span data-ttu-id="c5f71-137">Windows management アプリの正常性状態。</span><span class="sxs-lookup"><span data-stu-id="c5f71-137">Windows management app health state.</span></span> <span data-ttu-id="c5f71-138">可能な値は `unknown`、`healthy`、`unhealthy` です。</span><span class="sxs-lookup"><span data-stu-id="c5f71-138">Possible values are: `unknown`, `healthy`, `unhealthy`.</span></span>|
|<span data-ttu-id="c5f71-139">バージョン</span><span class="sxs-lookup"><span data-stu-id="c5f71-139">installedVersion</span></span>|<span data-ttu-id="c5f71-140">String</span><span class="sxs-lookup"><span data-stu-id="c5f71-140">String</span></span>|<span data-ttu-id="c5f71-141">Windows management アプリがインストールされているバージョン。</span><span class="sxs-lookup"><span data-stu-id="c5f71-141">Windows management app installed version.</span></span>|
|<span data-ttu-id="c5f71-142">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="c5f71-142">lastCheckInDateTime</span></span>|<span data-ttu-id="c5f71-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5f71-143">DateTimeOffset</span></span>|<span data-ttu-id="c5f71-144">Windows management アプリの最終チェックイン時刻。</span><span class="sxs-lookup"><span data-stu-id="c5f71-144">Windows management app last check-in time.</span></span>|
|<span data-ttu-id="c5f71-145">deviceName</span><span class="sxs-lookup"><span data-stu-id="c5f71-145">deviceName</span></span>|<span data-ttu-id="c5f71-146">String</span><span class="sxs-lookup"><span data-stu-id="c5f71-146">String</span></span>|<span data-ttu-id="c5f71-147">Windows management アプリがインストールされているデバイスの名前。</span><span class="sxs-lookup"><span data-stu-id="c5f71-147">Name of the device on which Windows management app is installed.</span></span>|
|<span data-ttu-id="c5f71-148">deviceosversion</span><span class="sxs-lookup"><span data-stu-id="c5f71-148">deviceOSVersion</span></span>|<span data-ttu-id="c5f71-149">String</span><span class="sxs-lookup"><span data-stu-id="c5f71-149">String</span></span>|<span data-ttu-id="c5f71-150">windows 管理アプリがインストールされているデバイスの windows 10 OS バージョン。</span><span class="sxs-lookup"><span data-stu-id="c5f71-150">Windows 10 OS version of the device on which Windows management app is installed.</span></span>|



## <a name="response"></a><span data-ttu-id="c5f71-151">応答</span><span class="sxs-lookup"><span data-stu-id="c5f71-151">Response</span></span>
<span data-ttu-id="c5f71-152">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[windowsmanagementapphealthstate](../resources/intune-devices-windowsmanagementapphealthstate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c5f71-152">If successful, this method returns a `200 OK` response code and an updated [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5f71-153">例</span><span class="sxs-lookup"><span data-stu-id="c5f71-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5f71-154">要求</span><span class="sxs-lookup"><span data-stu-id="c5f71-154">Request</span></span>
<span data-ttu-id="c5f71-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c5f71-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp/healthStates/{windowsManagementAppHealthStateId}
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

### <a name="response"></a><span data-ttu-id="c5f71-156">応答</span><span class="sxs-lookup"><span data-stu-id="c5f71-156">Response</span></span>
<span data-ttu-id="c5f71-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c5f71-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




