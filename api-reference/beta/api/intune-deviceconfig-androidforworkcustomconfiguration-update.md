---
title: androidforwork customconfiguration の更新
description: androidforwork customconfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8ccbc1c2af6795bbeaf2c408f51d19ba9f2acee5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32479338"
---
# <a name="update-androidforworkcustomconfiguration"></a><span data-ttu-id="a4fde-103">androidforwork customconfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="a4fde-103">Update androidForWorkCustomConfiguration</span></span>

> <span data-ttu-id="a4fde-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a4fde-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4fde-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a4fde-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4fde-106">[androidforwork customconfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a4fde-106">Update the properties of a [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a4fde-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="a4fde-107">Prerequisites</span></span>
<span data-ttu-id="a4fde-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a4fde-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4fde-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a4fde-110">Permission type</span></span>|<span data-ttu-id="a4fde-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a4fde-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4fde-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a4fde-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a4fde-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4fde-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a4fde-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a4fde-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4fde-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a4fde-115">Not supported.</span></span>|
|<span data-ttu-id="a4fde-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a4fde-116">Application</span></span>|<span data-ttu-id="a4fde-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a4fde-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4fde-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a4fde-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a4fde-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a4fde-119">Request headers</span></span>
|<span data-ttu-id="a4fde-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a4fde-120">Header</span></span>|<span data-ttu-id="a4fde-121">値</span><span class="sxs-lookup"><span data-stu-id="a4fde-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4fde-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4fde-122">Authorization</span></span>|<span data-ttu-id="a4fde-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="a4fde-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4fde-124">承諾</span><span class="sxs-lookup"><span data-stu-id="a4fde-124">Accept</span></span>|<span data-ttu-id="a4fde-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a4fde-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4fde-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="a4fde-126">Request body</span></span>
<span data-ttu-id="a4fde-127">要求本文で、 [androidforwork customconfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a4fde-127">In the request body, supply a JSON representation for the [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) object.</span></span>

<span data-ttu-id="a4fde-128">次の表に、 [androidforwork customconfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a4fde-128">The following table shows the properties that are required when you create the [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md).</span></span>

|<span data-ttu-id="a4fde-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a4fde-129">Property</span></span>|<span data-ttu-id="a4fde-130">型</span><span class="sxs-lookup"><span data-stu-id="a4fde-130">Type</span></span>|<span data-ttu-id="a4fde-131">説明</span><span class="sxs-lookup"><span data-stu-id="a4fde-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4fde-132">id</span><span class="sxs-lookup"><span data-stu-id="a4fde-132">id</span></span>|<span data-ttu-id="a4fde-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="a4fde-133">String</span></span>|<span data-ttu-id="a4fde-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a4fde-134">Key of the entity.</span></span> <span data-ttu-id="a4fde-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a4fde-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a4fde-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a4fde-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a4fde-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4fde-137">DateTimeOffset</span></span>|<span data-ttu-id="a4fde-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="a4fde-138">DateTime the object was last modified.</span></span> <span data-ttu-id="a4fde-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a4fde-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a4fde-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a4fde-140">roleScopeTagIds</span></span>|<span data-ttu-id="a4fde-141">String collection</span><span class="sxs-lookup"><span data-stu-id="a4fde-141">String collection</span></span>|<span data-ttu-id="a4fde-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="a4fde-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a4fde-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a4fde-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a4fde-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a4fde-144">supportsScopeTags</span></span>|<span data-ttu-id="a4fde-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="a4fde-145">Boolean</span></span>|<span data-ttu-id="a4fde-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a4fde-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a4fde-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="a4fde-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a4fde-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="a4fde-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a4fde-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="a4fde-149">This property is read-only.</span></span> <span data-ttu-id="a4fde-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a4fde-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a4fde-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a4fde-151">createdDateTime</span></span>|<span data-ttu-id="a4fde-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4fde-152">DateTimeOffset</span></span>|<span data-ttu-id="a4fde-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="a4fde-153">DateTime the object was created.</span></span> <span data-ttu-id="a4fde-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a4fde-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a4fde-155">説明</span><span class="sxs-lookup"><span data-stu-id="a4fde-155">description</span></span>|<span data-ttu-id="a4fde-156">String</span><span class="sxs-lookup"><span data-stu-id="a4fde-156">String</span></span>|<span data-ttu-id="a4fde-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="a4fde-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a4fde-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a4fde-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a4fde-159">displayName</span><span class="sxs-lookup"><span data-stu-id="a4fde-159">displayName</span></span>|<span data-ttu-id="a4fde-160">String</span><span class="sxs-lookup"><span data-stu-id="a4fde-160">String</span></span>|<span data-ttu-id="a4fde-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="a4fde-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a4fde-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a4fde-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a4fde-163">version</span><span class="sxs-lookup"><span data-stu-id="a4fde-163">version</span></span>|<span data-ttu-id="a4fde-164">Int32</span><span class="sxs-lookup"><span data-stu-id="a4fde-164">Int32</span></span>|<span data-ttu-id="a4fde-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="a4fde-165">Version of the device configuration.</span></span> <span data-ttu-id="a4fde-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a4fde-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a4fde-167">omaSettings</span><span class="sxs-lookup"><span data-stu-id="a4fde-167">omaSettings</span></span>|<span data-ttu-id="a4fde-168">[omaSetting](../resources/intune-deviceconfig-omasetting.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a4fde-168">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="a4fde-169">OMA 設定。</span><span class="sxs-lookup"><span data-stu-id="a4fde-169">OMA settings.</span></span> <span data-ttu-id="a4fde-170">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="a4fde-170">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="a4fde-171">応答</span><span class="sxs-lookup"><span data-stu-id="a4fde-171">Response</span></span>
<span data-ttu-id="a4fde-172">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[androidforwork customconfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a4fde-172">If successful, this method returns a `200 OK` response code and an updated [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4fde-173">例</span><span class="sxs-lookup"><span data-stu-id="a4fde-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="a4fde-174">要求</span><span class="sxs-lookup"><span data-stu-id="a4fde-174">Request</span></span>
<span data-ttu-id="a4fde-175">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a4fde-175">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 501

{
  "@odata.type": "#microsoft.graph.androidForWorkCustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="a4fde-176">応答</span><span class="sxs-lookup"><span data-stu-id="a4fde-176">Response</span></span>
<span data-ttu-id="a4fde-p111">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a4fde-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 673

{
  "@odata.type": "#microsoft.graph.androidForWorkCustomConfiguration",
  "id": "cca8b2bb-b2bb-cca8-bbb2-a8ccbbb2a8cc",
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





