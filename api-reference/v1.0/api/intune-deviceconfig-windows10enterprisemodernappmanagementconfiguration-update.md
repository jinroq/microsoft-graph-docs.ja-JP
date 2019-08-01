---
title: windows10EnterpriseModernAppManagementConfiguration の更新
description: windows10EnterpriseModernAppManagementConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 16162da1d914eb967a256dbbd64e007ca8c3c99c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35997324"
---
# <a name="update-windows10enterprisemodernappmanagementconfiguration"></a><span data-ttu-id="38080-103">windows10EnterpriseModernAppManagementConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="38080-103">Update windows10EnterpriseModernAppManagementConfiguration</span></span>

> <span data-ttu-id="38080-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="38080-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38080-105">[windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="38080-105">Update the properties of a [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="38080-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="38080-106">Prerequisites</span></span>
<span data-ttu-id="38080-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="38080-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38080-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="38080-109">Permission type</span></span>|<span data-ttu-id="38080-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="38080-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38080-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="38080-111">Delegated (work or school account)</span></span>|<span data-ttu-id="38080-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38080-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="38080-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="38080-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38080-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="38080-114">Not supported.</span></span>|
|<span data-ttu-id="38080-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="38080-115">Application</span></span>|<span data-ttu-id="38080-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="38080-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="38080-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="38080-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="38080-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="38080-118">Request headers</span></span>
|<span data-ttu-id="38080-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="38080-119">Header</span></span>|<span data-ttu-id="38080-120">値</span><span class="sxs-lookup"><span data-stu-id="38080-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38080-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="38080-121">Authorization</span></span>|<span data-ttu-id="38080-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="38080-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="38080-123">承諾</span><span class="sxs-lookup"><span data-stu-id="38080-123">Accept</span></span>|<span data-ttu-id="38080-124">application/json</span><span class="sxs-lookup"><span data-stu-id="38080-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38080-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="38080-125">Request body</span></span>
<span data-ttu-id="38080-126">要求本文で、[windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="38080-126">In the request body, supply a JSON representation for the [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object.</span></span>

<span data-ttu-id="38080-127">次の表に、[windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="38080-127">The following table shows the properties that are required when you create the [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md).</span></span>

|<span data-ttu-id="38080-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="38080-128">Property</span></span>|<span data-ttu-id="38080-129">型</span><span class="sxs-lookup"><span data-stu-id="38080-129">Type</span></span>|<span data-ttu-id="38080-130">説明</span><span class="sxs-lookup"><span data-stu-id="38080-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38080-131">id</span><span class="sxs-lookup"><span data-stu-id="38080-131">id</span></span>|<span data-ttu-id="38080-132">文字列</span><span class="sxs-lookup"><span data-stu-id="38080-132">String</span></span>|<span data-ttu-id="38080-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="38080-133">Key of the entity.</span></span> <span data-ttu-id="38080-134">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="38080-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38080-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="38080-135">lastModifiedDateTime</span></span>|<span data-ttu-id="38080-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38080-136">DateTimeOffset</span></span>|<span data-ttu-id="38080-137">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="38080-137">DateTime the object was last modified.</span></span> <span data-ttu-id="38080-138">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="38080-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38080-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="38080-139">createdDateTime</span></span>|<span data-ttu-id="38080-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38080-140">DateTimeOffset</span></span>|<span data-ttu-id="38080-141">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="38080-141">DateTime the object was created.</span></span> <span data-ttu-id="38080-142">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="38080-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38080-143">description</span><span class="sxs-lookup"><span data-stu-id="38080-143">description</span></span>|<span data-ttu-id="38080-144">String</span><span class="sxs-lookup"><span data-stu-id="38080-144">String</span></span>|<span data-ttu-id="38080-145">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="38080-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="38080-146">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="38080-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38080-147">displayName</span><span class="sxs-lookup"><span data-stu-id="38080-147">displayName</span></span>|<span data-ttu-id="38080-148">String</span><span class="sxs-lookup"><span data-stu-id="38080-148">String</span></span>|<span data-ttu-id="38080-149">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="38080-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="38080-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="38080-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38080-151">version</span><span class="sxs-lookup"><span data-stu-id="38080-151">version</span></span>|<span data-ttu-id="38080-152">Int32</span><span class="sxs-lookup"><span data-stu-id="38080-152">Int32</span></span>|<span data-ttu-id="38080-153">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="38080-153">Version of the device configuration.</span></span> <span data-ttu-id="38080-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="38080-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38080-155">uninstallBuiltInApps</span><span class="sxs-lookup"><span data-stu-id="38080-155">uninstallBuiltInApps</span></span>|<span data-ttu-id="38080-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="38080-156">Boolean</span></span>|<span data-ttu-id="38080-157">組み込みの Windows アプリの固定リストをアンインストールするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="38080-157">Indicates whether or not to uninstall a fixed list of built-in Windows apps.</span></span>|



## <a name="response"></a><span data-ttu-id="38080-158">応答</span><span class="sxs-lookup"><span data-stu-id="38080-158">Response</span></span>
<span data-ttu-id="38080-159">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="38080-159">If successful, this method returns a `200 OK` response code and an updated [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38080-160">例</span><span class="sxs-lookup"><span data-stu-id="38080-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="38080-161">要求</span><span class="sxs-lookup"><span data-stu-id="38080-161">Request</span></span>
<span data-ttu-id="38080-162">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="38080-162">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 222

{
  "@odata.type": "#microsoft.graph.windows10EnterpriseModernAppManagementConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "uninstallBuiltInApps": true
}
```

### <a name="response"></a><span data-ttu-id="38080-163">応答</span><span class="sxs-lookup"><span data-stu-id="38080-163">Response</span></span>
<span data-ttu-id="38080-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="38080-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 394

{
  "@odata.type": "#microsoft.graph.windows10EnterpriseModernAppManagementConfiguration",
  "id": "d6577687-7687-d657-8776-57d6877657d6",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "uninstallBuiltInApps": true
}
```



