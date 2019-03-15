---
title: windowsHealthMonitoringConfiguration の更新
description: windowsHealthMonitoringConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d19801400b75cfb712e5249d53938012bdb9b1d8
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/14/2019
ms.locfileid: "30631591"
---
# <a name="update-windowshealthmonitoringconfiguration"></a><span data-ttu-id="e1696-103">windowsHealthMonitoringConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="e1696-103">Update windowsHealthMonitoringConfiguration</span></span>

> <span data-ttu-id="e1696-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e1696-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1696-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e1696-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1696-106">[windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e1696-106">Update the properties of a [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e1696-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="e1696-107">Prerequisites</span></span>
<span data-ttu-id="e1696-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e1696-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e1696-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e1696-110">Permission type</span></span>|<span data-ttu-id="e1696-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e1696-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1696-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e1696-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e1696-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1696-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e1696-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e1696-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1696-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e1696-115">Not supported.</span></span>|
|<span data-ttu-id="e1696-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e1696-116">Application</span></span>|<span data-ttu-id="e1696-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e1696-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1696-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e1696-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e1696-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e1696-119">Request headers</span></span>
|<span data-ttu-id="e1696-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e1696-120">Header</span></span>|<span data-ttu-id="e1696-121">値</span><span class="sxs-lookup"><span data-stu-id="e1696-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1696-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1696-122">Authorization</span></span>|<span data-ttu-id="e1696-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="e1696-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1696-124">承諾</span><span class="sxs-lookup"><span data-stu-id="e1696-124">Accept</span></span>|<span data-ttu-id="e1696-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e1696-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1696-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="e1696-126">Request body</span></span>
<span data-ttu-id="e1696-127">要求本文で、 [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e1696-127">In the request body, supply a JSON representation for the [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object.</span></span>

<span data-ttu-id="e1696-128">次の表に、 [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e1696-128">The following table shows the properties that are required when you create the [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md).</span></span>

|<span data-ttu-id="e1696-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e1696-129">Property</span></span>|<span data-ttu-id="e1696-130">型</span><span class="sxs-lookup"><span data-stu-id="e1696-130">Type</span></span>|<span data-ttu-id="e1696-131">説明</span><span class="sxs-lookup"><span data-stu-id="e1696-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1696-132">id</span><span class="sxs-lookup"><span data-stu-id="e1696-132">id</span></span>|<span data-ttu-id="e1696-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="e1696-133">String</span></span>|<span data-ttu-id="e1696-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e1696-134">Key of the entity.</span></span> <span data-ttu-id="e1696-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e1696-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e1696-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e1696-136">lastModifiedDateTime</span></span>|<span data-ttu-id="e1696-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1696-137">DateTimeOffset</span></span>|<span data-ttu-id="e1696-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="e1696-138">DateTime the object was last modified.</span></span> <span data-ttu-id="e1696-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e1696-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e1696-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e1696-140">roleScopeTagIds</span></span>|<span data-ttu-id="e1696-141">String collection</span><span class="sxs-lookup"><span data-stu-id="e1696-141">String collection</span></span>|<span data-ttu-id="e1696-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="e1696-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e1696-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e1696-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e1696-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="e1696-144">supportsScopeTags</span></span>|<span data-ttu-id="e1696-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1696-145">Boolean</span></span>|<span data-ttu-id="e1696-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e1696-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e1696-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="e1696-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e1696-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="e1696-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e1696-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="e1696-149">This property is read-only.</span></span> <span data-ttu-id="e1696-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e1696-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e1696-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e1696-151">createdDateTime</span></span>|<span data-ttu-id="e1696-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1696-152">DateTimeOffset</span></span>|<span data-ttu-id="e1696-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="e1696-153">DateTime the object was created.</span></span> <span data-ttu-id="e1696-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e1696-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e1696-155">description</span><span class="sxs-lookup"><span data-stu-id="e1696-155">description</span></span>|<span data-ttu-id="e1696-156">String</span><span class="sxs-lookup"><span data-stu-id="e1696-156">String</span></span>|<span data-ttu-id="e1696-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="e1696-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e1696-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e1696-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e1696-159">displayName</span><span class="sxs-lookup"><span data-stu-id="e1696-159">displayName</span></span>|<span data-ttu-id="e1696-160">String</span><span class="sxs-lookup"><span data-stu-id="e1696-160">String</span></span>|<span data-ttu-id="e1696-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="e1696-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e1696-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e1696-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e1696-163">version</span><span class="sxs-lookup"><span data-stu-id="e1696-163">version</span></span>|<span data-ttu-id="e1696-164">Int32</span><span class="sxs-lookup"><span data-stu-id="e1696-164">Int32</span></span>|<span data-ttu-id="e1696-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="e1696-165">Version of the device configuration.</span></span> <span data-ttu-id="e1696-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e1696-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e1696-167">allowDeviceHealthMonitoring</span><span class="sxs-lookup"><span data-stu-id="e1696-167">allowDeviceHealthMonitoring</span></span>|[<span data-ttu-id="e1696-168">購入</span><span class="sxs-lookup"><span data-stu-id="e1696-168">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="e1696-169">デバイス上でのデバイスの正常性の監視を有効にします。</span><span class="sxs-lookup"><span data-stu-id="e1696-169">Enables device health monitoring on the device.</span></span> <span data-ttu-id="e1696-170">使用可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="e1696-170">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="e1696-171">configDeviceHealthMonitoringScope</span><span class="sxs-lookup"><span data-stu-id="e1696-171">configDeviceHealthMonitoringScope</span></span>|[<span data-ttu-id="e1696-172">windowsHealthMonitoringScope</span><span class="sxs-lookup"><span data-stu-id="e1696-172">windowsHealthMonitoringScope</span></span>](../resources/intune-deviceconfig-windowshealthmonitoringscope.md)|<span data-ttu-id="e1696-173">ある正常性監視が有効になっているデバイスから収集されたイベントのセット。</span><span class="sxs-lookup"><span data-stu-id="e1696-173">Sepcifies set of events collected from the device where health monitoring is enabled.</span></span> <span data-ttu-id="e1696-174">可能な値は、`undefined`、`healthMonitoring`、`bootPerformance` です。</span><span class="sxs-lookup"><span data-stu-id="e1696-174">Possible values are: `undefined`, `healthMonitoring`, `bootPerformance`.</span></span>|



## <a name="response"></a><span data-ttu-id="e1696-175">応答</span><span class="sxs-lookup"><span data-stu-id="e1696-175">Response</span></span>
<span data-ttu-id="e1696-176">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e1696-176">If successful, this method returns a `200 OK` response code and an updated [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1696-177">例</span><span class="sxs-lookup"><span data-stu-id="e1696-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="e1696-178">要求</span><span class="sxs-lookup"><span data-stu-id="e1696-178">Request</span></span>
<span data-ttu-id="e1696-179">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e1696-179">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 371

{
  "@odata.type": "#microsoft.graph.windowsHealthMonitoringConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "allowDeviceHealthMonitoring": "enabled",
  "configDeviceHealthMonitoringScope": "healthMonitoring"
}
```

### <a name="response"></a><span data-ttu-id="e1696-180">応答</span><span class="sxs-lookup"><span data-stu-id="e1696-180">Response</span></span>
<span data-ttu-id="e1696-p112">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e1696-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 543

{
  "@odata.type": "#microsoft.graph.windowsHealthMonitoringConfiguration",
  "id": "3439bcec-bcec-3439-ecbc-3934ecbc3934",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "allowDeviceHealthMonitoring": "enabled",
  "configDeviceHealthMonitoringScope": "healthMonitoring"
}
```




