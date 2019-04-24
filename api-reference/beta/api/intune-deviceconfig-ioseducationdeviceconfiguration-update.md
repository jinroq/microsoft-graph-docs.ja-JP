---
title: ioseアヒル/devic/デバイスの更新
description: ioseアヒル ationdevic/デバイスオブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: af2b9d5b1523db07fdbd8ebe79ec74c0d22bbf97
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32467380"
---
# <a name="update-ioseducationdeviceconfiguration"></a><span data-ttu-id="7f619-103">ioseアヒル/devic/デバイスの更新</span><span class="sxs-lookup"><span data-stu-id="7f619-103">Update iosEducationDeviceConfiguration</span></span>

> <span data-ttu-id="7f619-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f619-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7f619-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7f619-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f619-106">[ioseアヒル ationdevic/](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md)デバイスオブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7f619-106">Update the properties of a [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7f619-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="7f619-107">Prerequisites</span></span>
<span data-ttu-id="7f619-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7f619-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f619-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7f619-110">Permission type</span></span>|<span data-ttu-id="7f619-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7f619-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f619-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7f619-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7f619-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f619-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7f619-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7f619-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f619-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f619-115">Not supported.</span></span>|
|<span data-ttu-id="7f619-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7f619-116">Application</span></span>|<span data-ttu-id="7f619-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f619-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f619-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7f619-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="7f619-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7f619-119">Request headers</span></span>
|<span data-ttu-id="7f619-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7f619-120">Header</span></span>|<span data-ttu-id="7f619-121">値</span><span class="sxs-lookup"><span data-stu-id="7f619-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f619-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f619-122">Authorization</span></span>|<span data-ttu-id="7f619-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="7f619-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f619-124">承諾</span><span class="sxs-lookup"><span data-stu-id="7f619-124">Accept</span></span>|<span data-ttu-id="7f619-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7f619-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f619-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="7f619-126">Request body</span></span>
<span data-ttu-id="7f619-127">要求本文で、 [ioseアヒル ationdevic/](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md)備品オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7f619-127">In the request body, supply a JSON representation for the [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) object.</span></span>

<span data-ttu-id="7f619-128">次の表に、 [ioseアヒル ationdevicの](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md)作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7f619-128">The following table shows the properties that are required when you create the [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md).</span></span>

|<span data-ttu-id="7f619-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7f619-129">Property</span></span>|<span data-ttu-id="7f619-130">型</span><span class="sxs-lookup"><span data-stu-id="7f619-130">Type</span></span>|<span data-ttu-id="7f619-131">説明</span><span class="sxs-lookup"><span data-stu-id="7f619-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f619-132">id</span><span class="sxs-lookup"><span data-stu-id="7f619-132">id</span></span>|<span data-ttu-id="7f619-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="7f619-133">String</span></span>|<span data-ttu-id="7f619-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7f619-134">Key of the entity.</span></span> <span data-ttu-id="7f619-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f619-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7f619-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7f619-136">lastModifiedDateTime</span></span>|<span data-ttu-id="7f619-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f619-137">DateTimeOffset</span></span>|<span data-ttu-id="7f619-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="7f619-138">DateTime the object was last modified.</span></span> <span data-ttu-id="7f619-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f619-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7f619-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7f619-140">roleScopeTagIds</span></span>|<span data-ttu-id="7f619-141">String collection</span><span class="sxs-lookup"><span data-stu-id="7f619-141">String collection</span></span>|<span data-ttu-id="7f619-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="7f619-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7f619-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f619-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7f619-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="7f619-144">supportsScopeTags</span></span>|<span data-ttu-id="7f619-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f619-145">Boolean</span></span>|<span data-ttu-id="7f619-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7f619-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="7f619-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="7f619-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="7f619-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="7f619-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="7f619-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="7f619-149">This property is read-only.</span></span> <span data-ttu-id="7f619-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f619-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7f619-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7f619-151">createdDateTime</span></span>|<span data-ttu-id="7f619-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f619-152">DateTimeOffset</span></span>|<span data-ttu-id="7f619-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="7f619-153">DateTime the object was created.</span></span> <span data-ttu-id="7f619-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f619-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7f619-155">説明</span><span class="sxs-lookup"><span data-stu-id="7f619-155">description</span></span>|<span data-ttu-id="7f619-156">String</span><span class="sxs-lookup"><span data-stu-id="7f619-156">String</span></span>|<span data-ttu-id="7f619-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="7f619-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7f619-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f619-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7f619-159">displayName</span><span class="sxs-lookup"><span data-stu-id="7f619-159">displayName</span></span>|<span data-ttu-id="7f619-160">String</span><span class="sxs-lookup"><span data-stu-id="7f619-160">String</span></span>|<span data-ttu-id="7f619-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="7f619-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7f619-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f619-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7f619-163">version</span><span class="sxs-lookup"><span data-stu-id="7f619-163">version</span></span>|<span data-ttu-id="7f619-164">Int32</span><span class="sxs-lookup"><span data-stu-id="7f619-164">Int32</span></span>|<span data-ttu-id="7f619-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="7f619-165">Version of the device configuration.</span></span> <span data-ttu-id="7f619-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f619-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="7f619-167">応答</span><span class="sxs-lookup"><span data-stu-id="7f619-167">Response</span></span>
<span data-ttu-id="7f619-168">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[ioseアヒル ationdevic/](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md)デバイスオブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7f619-168">If successful, this method returns a `200 OK` response code and an updated [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f619-169">例</span><span class="sxs-lookup"><span data-stu-id="7f619-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="7f619-170">要求</span><span class="sxs-lookup"><span data-stu-id="7f619-170">Request</span></span>
<span data-ttu-id="7f619-171">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7f619-171">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 261

{
  "@odata.type": "#microsoft.graph.iosEducationDeviceConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="7f619-172">応答</span><span class="sxs-lookup"><span data-stu-id="7f619-172">Response</span></span>
<span data-ttu-id="7f619-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7f619-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 433

{
  "@odata.type": "#microsoft.graph.iosEducationDeviceConfiguration",
  "id": "3d563be4-3be4-3d56-e43b-563de43b563d",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```





