---
title: windowsHealthMonitoringConfiguration を作成する
description: 新しい windowsHealthMonitoringConfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 66b078cea72fc3090b315cf590767b2613585069
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/14/2019
ms.locfileid: "30631578"
---
# <a name="create-windowshealthmonitoringconfiguration"></a><span data-ttu-id="54bb2-103">windowsHealthMonitoringConfiguration を作成する</span><span class="sxs-lookup"><span data-stu-id="54bb2-103">Create windowsHealthMonitoringConfiguration</span></span>

> <span data-ttu-id="54bb2-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="54bb2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="54bb2-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="54bb2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54bb2-106">新しい[windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="54bb2-106">Create a new [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="54bb2-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="54bb2-107">Prerequisites</span></span>
<span data-ttu-id="54bb2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="54bb2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="54bb2-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="54bb2-110">Permission type</span></span>|<span data-ttu-id="54bb2-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="54bb2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54bb2-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="54bb2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="54bb2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54bb2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="54bb2-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="54bb2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54bb2-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="54bb2-115">Not supported.</span></span>|
|<span data-ttu-id="54bb2-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="54bb2-116">Application</span></span>|<span data-ttu-id="54bb2-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="54bb2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="54bb2-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="54bb2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="54bb2-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="54bb2-119">Request headers</span></span>
|<span data-ttu-id="54bb2-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="54bb2-120">Header</span></span>|<span data-ttu-id="54bb2-121">値</span><span class="sxs-lookup"><span data-stu-id="54bb2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54bb2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="54bb2-122">Authorization</span></span>|<span data-ttu-id="54bb2-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="54bb2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="54bb2-124">承諾</span><span class="sxs-lookup"><span data-stu-id="54bb2-124">Accept</span></span>|<span data-ttu-id="54bb2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="54bb2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54bb2-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="54bb2-126">Request body</span></span>
<span data-ttu-id="54bb2-127">要求本文で、windowsHealthMonitoringConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="54bb2-127">In the request body, supply a JSON representation for the windowsHealthMonitoringConfiguration object.</span></span>

<span data-ttu-id="54bb2-128">次の表に、windowsHealthMonitoringConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="54bb2-128">The following table shows the properties that are required when you create the windowsHealthMonitoringConfiguration.</span></span>

|<span data-ttu-id="54bb2-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="54bb2-129">Property</span></span>|<span data-ttu-id="54bb2-130">型</span><span class="sxs-lookup"><span data-stu-id="54bb2-130">Type</span></span>|<span data-ttu-id="54bb2-131">説明</span><span class="sxs-lookup"><span data-stu-id="54bb2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54bb2-132">id</span><span class="sxs-lookup"><span data-stu-id="54bb2-132">id</span></span>|<span data-ttu-id="54bb2-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="54bb2-133">String</span></span>|<span data-ttu-id="54bb2-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="54bb2-134">Key of the entity.</span></span> <span data-ttu-id="54bb2-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="54bb2-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54bb2-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="54bb2-136">lastModifiedDateTime</span></span>|<span data-ttu-id="54bb2-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54bb2-137">DateTimeOffset</span></span>|<span data-ttu-id="54bb2-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="54bb2-138">DateTime the object was last modified.</span></span> <span data-ttu-id="54bb2-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="54bb2-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54bb2-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="54bb2-140">roleScopeTagIds</span></span>|<span data-ttu-id="54bb2-141">String collection</span><span class="sxs-lookup"><span data-stu-id="54bb2-141">String collection</span></span>|<span data-ttu-id="54bb2-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="54bb2-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="54bb2-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="54bb2-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54bb2-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="54bb2-144">supportsScopeTags</span></span>|<span data-ttu-id="54bb2-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="54bb2-145">Boolean</span></span>|<span data-ttu-id="54bb2-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="54bb2-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="54bb2-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="54bb2-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="54bb2-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="54bb2-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="54bb2-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="54bb2-149">This property is read-only.</span></span> <span data-ttu-id="54bb2-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="54bb2-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54bb2-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="54bb2-151">createdDateTime</span></span>|<span data-ttu-id="54bb2-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54bb2-152">DateTimeOffset</span></span>|<span data-ttu-id="54bb2-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="54bb2-153">DateTime the object was created.</span></span> <span data-ttu-id="54bb2-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="54bb2-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54bb2-155">description</span><span class="sxs-lookup"><span data-stu-id="54bb2-155">description</span></span>|<span data-ttu-id="54bb2-156">String</span><span class="sxs-lookup"><span data-stu-id="54bb2-156">String</span></span>|<span data-ttu-id="54bb2-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="54bb2-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="54bb2-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="54bb2-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54bb2-159">displayName</span><span class="sxs-lookup"><span data-stu-id="54bb2-159">displayName</span></span>|<span data-ttu-id="54bb2-160">String</span><span class="sxs-lookup"><span data-stu-id="54bb2-160">String</span></span>|<span data-ttu-id="54bb2-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="54bb2-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="54bb2-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="54bb2-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54bb2-163">version</span><span class="sxs-lookup"><span data-stu-id="54bb2-163">version</span></span>|<span data-ttu-id="54bb2-164">Int32</span><span class="sxs-lookup"><span data-stu-id="54bb2-164">Int32</span></span>|<span data-ttu-id="54bb2-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="54bb2-165">Version of the device configuration.</span></span> <span data-ttu-id="54bb2-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="54bb2-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54bb2-167">allowDeviceHealthMonitoring</span><span class="sxs-lookup"><span data-stu-id="54bb2-167">allowDeviceHealthMonitoring</span></span>|[<span data-ttu-id="54bb2-168">購入</span><span class="sxs-lookup"><span data-stu-id="54bb2-168">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="54bb2-169">デバイス上でのデバイスの正常性の監視を有効にします。</span><span class="sxs-lookup"><span data-stu-id="54bb2-169">Enables device health monitoring on the device.</span></span> <span data-ttu-id="54bb2-170">使用可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="54bb2-170">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="54bb2-171">configDeviceHealthMonitoringScope</span><span class="sxs-lookup"><span data-stu-id="54bb2-171">configDeviceHealthMonitoringScope</span></span>|[<span data-ttu-id="54bb2-172">windowsHealthMonitoringScope</span><span class="sxs-lookup"><span data-stu-id="54bb2-172">windowsHealthMonitoringScope</span></span>](../resources/intune-deviceconfig-windowshealthmonitoringscope.md)|<span data-ttu-id="54bb2-173">ある正常性監視が有効になっているデバイスから収集されたイベントのセット。</span><span class="sxs-lookup"><span data-stu-id="54bb2-173">Sepcifies set of events collected from the device where health monitoring is enabled.</span></span> <span data-ttu-id="54bb2-174">可能な値は、`undefined`、`healthMonitoring`、`bootPerformance` です。</span><span class="sxs-lookup"><span data-stu-id="54bb2-174">Possible values are: `undefined`, `healthMonitoring`, `bootPerformance`.</span></span>|



## <a name="response"></a><span data-ttu-id="54bb2-175">応答</span><span class="sxs-lookup"><span data-stu-id="54bb2-175">Response</span></span>
<span data-ttu-id="54bb2-176">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="54bb2-176">If successful, this method returns a `201 Created` response code and a [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54bb2-177">例</span><span class="sxs-lookup"><span data-stu-id="54bb2-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="54bb2-178">要求</span><span class="sxs-lookup"><span data-stu-id="54bb2-178">Request</span></span>
<span data-ttu-id="54bb2-179">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="54bb2-179">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="54bb2-180">応答</span><span class="sxs-lookup"><span data-stu-id="54bb2-180">Response</span></span>
<span data-ttu-id="54bb2-p112">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="54bb2-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




