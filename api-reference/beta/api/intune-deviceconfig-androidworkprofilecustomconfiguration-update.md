---
title: androidWorkProfileCustomConfiguration の更新
description: androidWorkProfileCustomConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 87d070e0edb73dc282f230361487199a50c9ebc8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149631"
---
# <a name="update-androidworkprofilecustomconfiguration"></a><span data-ttu-id="c4ddc-103">androidWorkProfileCustomConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="c4ddc-103">Update androidWorkProfileCustomConfiguration</span></span>

> <span data-ttu-id="c4ddc-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c4ddc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c4ddc-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c4ddc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4ddc-106">[androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c4ddc-106">Update the properties of a [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c4ddc-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="c4ddc-107">Prerequisites</span></span>
<span data-ttu-id="c4ddc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c4ddc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c4ddc-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c4ddc-110">Permission type</span></span>|<span data-ttu-id="c4ddc-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c4ddc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4ddc-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c4ddc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c4ddc-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4ddc-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c4ddc-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c4ddc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4ddc-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c4ddc-115">Not supported.</span></span>|
|<span data-ttu-id="c4ddc-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c4ddc-116">Application</span></span>|<span data-ttu-id="c4ddc-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c4ddc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4ddc-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c4ddc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c4ddc-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c4ddc-119">Request headers</span></span>
|<span data-ttu-id="c4ddc-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c4ddc-120">Header</span></span>|<span data-ttu-id="c4ddc-121">値</span><span class="sxs-lookup"><span data-stu-id="c4ddc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c4ddc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4ddc-122">Authorization</span></span>|<span data-ttu-id="c4ddc-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="c4ddc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c4ddc-124">承諾</span><span class="sxs-lookup"><span data-stu-id="c4ddc-124">Accept</span></span>|<span data-ttu-id="c4ddc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c4ddc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4ddc-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="c4ddc-126">Request body</span></span>
<span data-ttu-id="c4ddc-127">要求本文で、 [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c4ddc-127">In the request body, supply a JSON representation for the [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>

<span data-ttu-id="c4ddc-128">次の表に、 [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="c4ddc-128">The following table shows the properties that are required when you create the [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md).</span></span>

|<span data-ttu-id="c4ddc-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c4ddc-129">Property</span></span>|<span data-ttu-id="c4ddc-130">型</span><span class="sxs-lookup"><span data-stu-id="c4ddc-130">Type</span></span>|<span data-ttu-id="c4ddc-131">説明</span><span class="sxs-lookup"><span data-stu-id="c4ddc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4ddc-132">id</span><span class="sxs-lookup"><span data-stu-id="c4ddc-132">id</span></span>|<span data-ttu-id="c4ddc-133">文字列</span><span class="sxs-lookup"><span data-stu-id="c4ddc-133">String</span></span>|<span data-ttu-id="c4ddc-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c4ddc-134">Key of the entity.</span></span> <span data-ttu-id="c4ddc-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c4ddc-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4ddc-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c4ddc-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c4ddc-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4ddc-137">DateTimeOffset</span></span>|<span data-ttu-id="c4ddc-138">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="c4ddc-138">DateTime the object was last modified.</span></span> <span data-ttu-id="c4ddc-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c4ddc-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4ddc-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c4ddc-140">roleScopeTagIds</span></span>|<span data-ttu-id="c4ddc-141">String コレクション</span><span class="sxs-lookup"><span data-stu-id="c4ddc-141">String collection</span></span>|<span data-ttu-id="c4ddc-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="c4ddc-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c4ddc-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c4ddc-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4ddc-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c4ddc-144">supportsScopeTags</span></span>|<span data-ttu-id="c4ddc-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="c4ddc-145">Boolean</span></span>|<span data-ttu-id="c4ddc-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c4ddc-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c4ddc-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="c4ddc-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c4ddc-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="c4ddc-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c4ddc-149">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="c4ddc-149">This property is read-only.</span></span> <span data-ttu-id="c4ddc-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c4ddc-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4ddc-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c4ddc-151">createdDateTime</span></span>|<span data-ttu-id="c4ddc-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4ddc-152">DateTimeOffset</span></span>|<span data-ttu-id="c4ddc-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="c4ddc-153">DateTime the object was created.</span></span> <span data-ttu-id="c4ddc-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c4ddc-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4ddc-155">説明</span><span class="sxs-lookup"><span data-stu-id="c4ddc-155">description</span></span>|<span data-ttu-id="c4ddc-156">String</span><span class="sxs-lookup"><span data-stu-id="c4ddc-156">String</span></span>|<span data-ttu-id="c4ddc-157">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="c4ddc-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c4ddc-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c4ddc-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4ddc-159">displayName</span><span class="sxs-lookup"><span data-stu-id="c4ddc-159">displayName</span></span>|<span data-ttu-id="c4ddc-160">String</span><span class="sxs-lookup"><span data-stu-id="c4ddc-160">String</span></span>|<span data-ttu-id="c4ddc-161">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="c4ddc-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c4ddc-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c4ddc-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4ddc-163">version</span><span class="sxs-lookup"><span data-stu-id="c4ddc-163">version</span></span>|<span data-ttu-id="c4ddc-164">Int32</span><span class="sxs-lookup"><span data-stu-id="c4ddc-164">Int32</span></span>|<span data-ttu-id="c4ddc-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="c4ddc-165">Version of the device configuration.</span></span> <span data-ttu-id="c4ddc-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c4ddc-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4ddc-167">omaSettings</span><span class="sxs-lookup"><span data-stu-id="c4ddc-167">omaSettings</span></span>|<span data-ttu-id="c4ddc-168">[omaSetting](../resources/intune-deviceconfig-omasetting.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c4ddc-168">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="c4ddc-169">OMA 設定。</span><span class="sxs-lookup"><span data-stu-id="c4ddc-169">OMA settings.</span></span> <span data-ttu-id="c4ddc-170">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="c4ddc-170">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="c4ddc-171">応答</span><span class="sxs-lookup"><span data-stu-id="c4ddc-171">Response</span></span>
<span data-ttu-id="c4ddc-172">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c4ddc-172">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4ddc-173">例</span><span class="sxs-lookup"><span data-stu-id="c4ddc-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="c4ddc-174">要求</span><span class="sxs-lookup"><span data-stu-id="c4ddc-174">Request</span></span>
<span data-ttu-id="c4ddc-175">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c4ddc-175">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 505

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="c4ddc-176">応答</span><span class="sxs-lookup"><span data-stu-id="c4ddc-176">Response</span></span>
<span data-ttu-id="c4ddc-p111">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c4ddc-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 677

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
  "id": "76c5d59b-d59b-76c5-9bd5-c5769bd5c576",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```




