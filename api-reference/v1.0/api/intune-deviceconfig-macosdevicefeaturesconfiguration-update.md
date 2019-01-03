---
title: macOSDeviceFeaturesConfiguration の更新
description: macOSDeviceFeaturesConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: aecefa3e348613fa2aa0f9974f2aafbce56c8051
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348455"
---
# <a name="update-macosdevicefeaturesconfiguration"></a><span data-ttu-id="017d3-103">macOSDeviceFeaturesConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="017d3-103">Update macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="017d3-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="017d3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="017d3-105">[macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="017d3-105">Update the properties of a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="017d3-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="017d3-106">Prerequisites</span></span>
<span data-ttu-id="017d3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="017d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="017d3-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="017d3-109">Permission type</span></span>|<span data-ttu-id="017d3-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="017d3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="017d3-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="017d3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="017d3-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="017d3-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="017d3-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="017d3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="017d3-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="017d3-114">Not supported.</span></span>|
|<span data-ttu-id="017d3-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="017d3-115">Application</span></span>|<span data-ttu-id="017d3-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="017d3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="017d3-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="017d3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="017d3-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="017d3-118">Request headers</span></span>
|<span data-ttu-id="017d3-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="017d3-119">Header</span></span>|<span data-ttu-id="017d3-120">値</span><span class="sxs-lookup"><span data-stu-id="017d3-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="017d3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="017d3-121">Authorization</span></span>|<span data-ttu-id="017d3-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="017d3-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="017d3-123">Accept</span><span class="sxs-lookup"><span data-stu-id="017d3-123">Accept</span></span>|<span data-ttu-id="017d3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="017d3-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="017d3-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="017d3-125">Request body</span></span>
<span data-ttu-id="017d3-126">要求本文で、[macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="017d3-126">In the request body, supply a JSON representation for the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

<span data-ttu-id="017d3-127">次の表に、[macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="017d3-127">The following table shows the properties that are required when you create the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span></span>

|<span data-ttu-id="017d3-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="017d3-128">Property</span></span>|<span data-ttu-id="017d3-129">種類</span><span class="sxs-lookup"><span data-stu-id="017d3-129">Type</span></span>|<span data-ttu-id="017d3-130">説明</span><span class="sxs-lookup"><span data-stu-id="017d3-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="017d3-131">ID</span><span class="sxs-lookup"><span data-stu-id="017d3-131">id</span></span>|<span data-ttu-id="017d3-132">String</span><span class="sxs-lookup"><span data-stu-id="017d3-132">String</span></span>|<span data-ttu-id="017d3-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="017d3-133">Key of the entity.</span></span> <span data-ttu-id="017d3-134">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="017d3-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="017d3-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="017d3-135">lastModifiedDateTime</span></span>|<span data-ttu-id="017d3-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="017d3-136">DateTimeOffset</span></span>|<span data-ttu-id="017d3-137">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="017d3-137">DateTime the object was last modified.</span></span> <span data-ttu-id="017d3-138">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="017d3-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="017d3-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="017d3-139">createdDateTime</span></span>|<span data-ttu-id="017d3-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="017d3-140">DateTimeOffset</span></span>|<span data-ttu-id="017d3-141">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="017d3-141">DateTime the object was created.</span></span> <span data-ttu-id="017d3-142">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="017d3-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="017d3-143">説明</span><span class="sxs-lookup"><span data-stu-id="017d3-143">description</span></span>|<span data-ttu-id="017d3-144">String</span><span class="sxs-lookup"><span data-stu-id="017d3-144">String</span></span>|<span data-ttu-id="017d3-145">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="017d3-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="017d3-146">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="017d3-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="017d3-147">displayName</span><span class="sxs-lookup"><span data-stu-id="017d3-147">displayName</span></span>|<span data-ttu-id="017d3-148">String</span><span class="sxs-lookup"><span data-stu-id="017d3-148">String</span></span>|<span data-ttu-id="017d3-149">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="017d3-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="017d3-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="017d3-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="017d3-151">version</span><span class="sxs-lookup"><span data-stu-id="017d3-151">version</span></span>|<span data-ttu-id="017d3-152">Int32</span><span class="sxs-lookup"><span data-stu-id="017d3-152">Int32</span></span>|<span data-ttu-id="017d3-153">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="017d3-153">Version of the device configuration.</span></span> <span data-ttu-id="017d3-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="017d3-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="017d3-155">応答</span><span class="sxs-lookup"><span data-stu-id="017d3-155">Response</span></span>
<span data-ttu-id="017d3-156">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="017d3-156">If successful, this method returns a `200 OK` response code and an updated [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="017d3-157">例</span><span class="sxs-lookup"><span data-stu-id="017d3-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="017d3-158">要求</span><span class="sxs-lookup"><span data-stu-id="017d3-158">Request</span></span>
<span data-ttu-id="017d3-159">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="017d3-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 170

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="017d3-160">応答</span><span class="sxs-lookup"><span data-stu-id="017d3-160">Response</span></span>
<span data-ttu-id="017d3-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="017d3-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 342

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
  "id": "49fa957d-957d-49fa-7d95-fa497d95fa49",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```


