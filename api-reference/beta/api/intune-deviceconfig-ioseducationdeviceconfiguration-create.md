---
title: ioseアヒル ationdevicの作成
description: 新しい ioseアヒル ationdevic/デバイスオブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 252e616da77eb330432c195a6e7eb8ff8157fa58
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163841"
---
# <a name="create-ioseducationdeviceconfiguration"></a><span data-ttu-id="21413-103">ioseアヒル ationdevicの作成</span><span class="sxs-lookup"><span data-stu-id="21413-103">Create iosEducationDeviceConfiguration</span></span>

> <span data-ttu-id="21413-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="21413-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21413-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="21413-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21413-106">新しい[ioseアヒル ationdevic/](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md)デバイスオブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="21413-106">Create a new [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="21413-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="21413-107">Prerequisites</span></span>
<span data-ttu-id="21413-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="21413-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="21413-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="21413-110">Permission type</span></span>|<span data-ttu-id="21413-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="21413-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21413-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="21413-112">Delegated (work or school account)</span></span>|<span data-ttu-id="21413-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21413-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="21413-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="21413-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21413-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="21413-115">Not supported.</span></span>|
|<span data-ttu-id="21413-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="21413-116">Application</span></span>|<span data-ttu-id="21413-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="21413-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="21413-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="21413-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="21413-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="21413-119">Request headers</span></span>
|<span data-ttu-id="21413-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="21413-120">Header</span></span>|<span data-ttu-id="21413-121">値</span><span class="sxs-lookup"><span data-stu-id="21413-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21413-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="21413-122">Authorization</span></span>|<span data-ttu-id="21413-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="21413-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21413-124">承諾</span><span class="sxs-lookup"><span data-stu-id="21413-124">Accept</span></span>|<span data-ttu-id="21413-125">application/json</span><span class="sxs-lookup"><span data-stu-id="21413-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21413-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="21413-126">Request body</span></span>
<span data-ttu-id="21413-127">要求本文で、ioseアヒル ationdevic/備品オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="21413-127">In the request body, supply a JSON representation for the iosEducationDeviceConfiguration object.</span></span>

<span data-ttu-id="21413-128">次の表に、ioseアヒル ationdevicの作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="21413-128">The following table shows the properties that are required when you create the iosEducationDeviceConfiguration.</span></span>

|<span data-ttu-id="21413-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="21413-129">Property</span></span>|<span data-ttu-id="21413-130">型</span><span class="sxs-lookup"><span data-stu-id="21413-130">Type</span></span>|<span data-ttu-id="21413-131">説明</span><span class="sxs-lookup"><span data-stu-id="21413-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21413-132">id</span><span class="sxs-lookup"><span data-stu-id="21413-132">id</span></span>|<span data-ttu-id="21413-133">文字列</span><span class="sxs-lookup"><span data-stu-id="21413-133">String</span></span>|<span data-ttu-id="21413-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="21413-134">Key of the entity.</span></span> <span data-ttu-id="21413-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="21413-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="21413-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="21413-136">lastModifiedDateTime</span></span>|<span data-ttu-id="21413-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21413-137">DateTimeOffset</span></span>|<span data-ttu-id="21413-138">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="21413-138">DateTime the object was last modified.</span></span> <span data-ttu-id="21413-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="21413-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="21413-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="21413-140">roleScopeTagIds</span></span>|<span data-ttu-id="21413-141">String collection</span><span class="sxs-lookup"><span data-stu-id="21413-141">String collection</span></span>|<span data-ttu-id="21413-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="21413-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="21413-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="21413-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="21413-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="21413-144">supportsScopeTags</span></span>|<span data-ttu-id="21413-145">ブール値</span><span class="sxs-lookup"><span data-stu-id="21413-145">Boolean</span></span>|<span data-ttu-id="21413-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="21413-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="21413-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="21413-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="21413-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="21413-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="21413-149">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="21413-149">This property is read-only.</span></span> <span data-ttu-id="21413-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="21413-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="21413-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="21413-151">createdDateTime</span></span>|<span data-ttu-id="21413-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21413-152">DateTimeOffset</span></span>|<span data-ttu-id="21413-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="21413-153">DateTime the object was created.</span></span> <span data-ttu-id="21413-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="21413-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="21413-155">説明</span><span class="sxs-lookup"><span data-stu-id="21413-155">description</span></span>|<span data-ttu-id="21413-156">String</span><span class="sxs-lookup"><span data-stu-id="21413-156">String</span></span>|<span data-ttu-id="21413-157">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="21413-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="21413-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="21413-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="21413-159">displayName</span><span class="sxs-lookup"><span data-stu-id="21413-159">displayName</span></span>|<span data-ttu-id="21413-160">String</span><span class="sxs-lookup"><span data-stu-id="21413-160">String</span></span>|<span data-ttu-id="21413-161">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="21413-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="21413-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="21413-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="21413-163">version</span><span class="sxs-lookup"><span data-stu-id="21413-163">version</span></span>|<span data-ttu-id="21413-164">Int32</span><span class="sxs-lookup"><span data-stu-id="21413-164">Int32</span></span>|<span data-ttu-id="21413-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="21413-165">Version of the device configuration.</span></span> <span data-ttu-id="21413-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="21413-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="21413-167">応答</span><span class="sxs-lookup"><span data-stu-id="21413-167">Response</span></span>
<span data-ttu-id="21413-168">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[ioseアヒル ationdevicオブジェクト](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md)を返します。</span><span class="sxs-lookup"><span data-stu-id="21413-168">If successful, this method returns a `201 Created` response code and a [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21413-169">例</span><span class="sxs-lookup"><span data-stu-id="21413-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="21413-170">要求</span><span class="sxs-lookup"><span data-stu-id="21413-170">Request</span></span>
<span data-ttu-id="21413-171">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="21413-171">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="21413-172">応答</span><span class="sxs-lookup"><span data-stu-id="21413-172">Response</span></span>
<span data-ttu-id="21413-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="21413-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




