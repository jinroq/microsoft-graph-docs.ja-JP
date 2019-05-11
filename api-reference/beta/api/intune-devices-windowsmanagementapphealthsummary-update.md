---
title: WindowsManagementAppHealthSummary の更新
description: WindowsManagementAppHealthSummary オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 323e8fdf611b25676f2b1337829a162eedb83f58
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33909100"
---
# <a name="update-windowsmanagementapphealthsummary"></a><span data-ttu-id="33ff1-103">WindowsManagementAppHealthSummary の更新</span><span class="sxs-lookup"><span data-stu-id="33ff1-103">Update windowsManagementAppHealthSummary</span></span>

> <span data-ttu-id="33ff1-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="33ff1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="33ff1-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="33ff1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33ff1-106">[WindowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="33ff1-106">Update the properties of a [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="33ff1-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="33ff1-107">Prerequisites</span></span>
<span data-ttu-id="33ff1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="33ff1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33ff1-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="33ff1-110">Permission type</span></span>|<span data-ttu-id="33ff1-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="33ff1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33ff1-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="33ff1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="33ff1-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33ff1-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="33ff1-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="33ff1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33ff1-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="33ff1-115">Not supported.</span></span>|
|<span data-ttu-id="33ff1-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="33ff1-116">Application</span></span>|<span data-ttu-id="33ff1-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="33ff1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="33ff1-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="33ff1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp/healthSummary
```

## <a name="request-headers"></a><span data-ttu-id="33ff1-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="33ff1-119">Request headers</span></span>
|<span data-ttu-id="33ff1-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="33ff1-120">Header</span></span>|<span data-ttu-id="33ff1-121">値</span><span class="sxs-lookup"><span data-stu-id="33ff1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33ff1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="33ff1-122">Authorization</span></span>|<span data-ttu-id="33ff1-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="33ff1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33ff1-124">承諾</span><span class="sxs-lookup"><span data-stu-id="33ff1-124">Accept</span></span>|<span data-ttu-id="33ff1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="33ff1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33ff1-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="33ff1-126">Request body</span></span>
<span data-ttu-id="33ff1-127">要求本文で、 [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="33ff1-127">In the request body, supply a JSON representation for the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>

<span data-ttu-id="33ff1-128">次の表に、 [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="33ff1-128">The following table shows the properties that are required when you create the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md).</span></span>

|<span data-ttu-id="33ff1-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="33ff1-129">Property</span></span>|<span data-ttu-id="33ff1-130">型</span><span class="sxs-lookup"><span data-stu-id="33ff1-130">Type</span></span>|<span data-ttu-id="33ff1-131">説明</span><span class="sxs-lookup"><span data-stu-id="33ff1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33ff1-132">id</span><span class="sxs-lookup"><span data-stu-id="33ff1-132">id</span></span>|<span data-ttu-id="33ff1-133">String</span><span class="sxs-lookup"><span data-stu-id="33ff1-133">String</span></span>|<span data-ttu-id="33ff1-134">Windows management app health summary エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="33ff1-134">Key of the Windows management app health summary entity.</span></span>|
|<span data-ttu-id="33ff1-135">healthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="33ff1-135">healthyDeviceCount</span></span>|<span data-ttu-id="33ff1-136">Int32</span><span class="sxs-lookup"><span data-stu-id="33ff1-136">Int32</span></span>|<span data-ttu-id="33ff1-137">正常なデバイス数。</span><span class="sxs-lookup"><span data-stu-id="33ff1-137">Healthy device count.</span></span>|
|<span data-ttu-id="33ff1-138">unhealthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="33ff1-138">unhealthyDeviceCount</span></span>|<span data-ttu-id="33ff1-139">Int32</span><span class="sxs-lookup"><span data-stu-id="33ff1-139">Int32</span></span>|<span data-ttu-id="33ff1-140">異常なデバイス数。</span><span class="sxs-lookup"><span data-stu-id="33ff1-140">Unhealthy device count.</span></span>|
|<span data-ttu-id="33ff1-141">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="33ff1-141">unknownDeviceCount</span></span>|<span data-ttu-id="33ff1-142">Int32</span><span class="sxs-lookup"><span data-stu-id="33ff1-142">Int32</span></span>|<span data-ttu-id="33ff1-143">デバイス数が不明です。</span><span class="sxs-lookup"><span data-stu-id="33ff1-143">Unknown device count.</span></span>|



## <a name="response"></a><span data-ttu-id="33ff1-144">応答</span><span class="sxs-lookup"><span data-stu-id="33ff1-144">Response</span></span>
<span data-ttu-id="33ff1-145">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="33ff1-145">If successful, this method returns a `200 OK` response code and an updated [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33ff1-146">例</span><span class="sxs-lookup"><span data-stu-id="33ff1-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="33ff1-147">要求</span><span class="sxs-lookup"><span data-stu-id="33ff1-147">Request</span></span>
<span data-ttu-id="33ff1-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="33ff1-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp/healthSummary
Content-type: application/json
Content-length: 161

{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthSummary",
  "healthyDeviceCount": 2,
  "unhealthyDeviceCount": 4,
  "unknownDeviceCount": 2
}
```

### <a name="response"></a><span data-ttu-id="33ff1-149">応答</span><span class="sxs-lookup"><span data-stu-id="33ff1-149">Response</span></span>
<span data-ttu-id="33ff1-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="33ff1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 210

{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthSummary",
  "id": "a9d38a9e-8a9e-a9d3-9e8a-d3a99e8ad3a9",
  "healthyDeviceCount": 2,
  "unhealthyDeviceCount": 4,
  "unknownDeviceCount": 2
}
```




