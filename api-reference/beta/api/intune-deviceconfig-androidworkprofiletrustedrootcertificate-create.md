---
title: androidwork profiletrustedrootcertificate の作成
description: 新しい androidwork profiletrustedrootcertificate オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 372859d25ab2269803d638d174fad9972d187a4c
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31771713"
---
# <a name="create-androidworkprofiletrustedrootcertificate"></a><span data-ttu-id="71029-103">androidwork profiletrustedrootcertificate の作成</span><span class="sxs-lookup"><span data-stu-id="71029-103">Create androidWorkProfileTrustedRootCertificate</span></span>

> <span data-ttu-id="71029-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="71029-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71029-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="71029-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71029-106">新しい[androidwork profiletrustedrootcertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="71029-106">Create a new [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="71029-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="71029-107">Prerequisites</span></span>
<span data-ttu-id="71029-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="71029-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71029-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="71029-110">Permission type</span></span>|<span data-ttu-id="71029-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="71029-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71029-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="71029-112">Delegated (work or school account)</span></span>|<span data-ttu-id="71029-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71029-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="71029-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="71029-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71029-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="71029-115">Not supported.</span></span>|
|<span data-ttu-id="71029-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="71029-116">Application</span></span>|<span data-ttu-id="71029-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="71029-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="71029-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="71029-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="71029-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="71029-119">Request headers</span></span>
|<span data-ttu-id="71029-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="71029-120">Header</span></span>|<span data-ttu-id="71029-121">値</span><span class="sxs-lookup"><span data-stu-id="71029-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71029-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="71029-122">Authorization</span></span>|<span data-ttu-id="71029-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="71029-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71029-124">承諾</span><span class="sxs-lookup"><span data-stu-id="71029-124">Accept</span></span>|<span data-ttu-id="71029-125">application/json</span><span class="sxs-lookup"><span data-stu-id="71029-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71029-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="71029-126">Request body</span></span>
<span data-ttu-id="71029-127">要求本文で、androidwork profiletrustedrootcertificate オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="71029-127">In the request body, supply a JSON representation for the androidWorkProfileTrustedRootCertificate object.</span></span>

<span data-ttu-id="71029-128">次の表に、androidwork profiletrustedrootcertificate の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="71029-128">The following table shows the properties that are required when you create the androidWorkProfileTrustedRootCertificate.</span></span>

|<span data-ttu-id="71029-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="71029-129">Property</span></span>|<span data-ttu-id="71029-130">型</span><span class="sxs-lookup"><span data-stu-id="71029-130">Type</span></span>|<span data-ttu-id="71029-131">説明</span><span class="sxs-lookup"><span data-stu-id="71029-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71029-132">id</span><span class="sxs-lookup"><span data-stu-id="71029-132">id</span></span>|<span data-ttu-id="71029-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="71029-133">String</span></span>|<span data-ttu-id="71029-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="71029-134">Key of the entity.</span></span> <span data-ttu-id="71029-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="71029-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71029-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="71029-136">lastModifiedDateTime</span></span>|<span data-ttu-id="71029-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71029-137">DateTimeOffset</span></span>|<span data-ttu-id="71029-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="71029-138">DateTime the object was last modified.</span></span> <span data-ttu-id="71029-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="71029-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71029-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="71029-140">roleScopeTagIds</span></span>|<span data-ttu-id="71029-141">String コレクション</span><span class="sxs-lookup"><span data-stu-id="71029-141">String collection</span></span>|<span data-ttu-id="71029-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="71029-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="71029-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="71029-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71029-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="71029-144">supportsScopeTags</span></span>|<span data-ttu-id="71029-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="71029-145">Boolean</span></span>|<span data-ttu-id="71029-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="71029-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="71029-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="71029-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="71029-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="71029-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="71029-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="71029-149">This property is read-only.</span></span> <span data-ttu-id="71029-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="71029-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71029-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="71029-151">createdDateTime</span></span>|<span data-ttu-id="71029-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71029-152">DateTimeOffset</span></span>|<span data-ttu-id="71029-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="71029-153">DateTime the object was created.</span></span> <span data-ttu-id="71029-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="71029-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71029-155">説明</span><span class="sxs-lookup"><span data-stu-id="71029-155">description</span></span>|<span data-ttu-id="71029-156">String</span><span class="sxs-lookup"><span data-stu-id="71029-156">String</span></span>|<span data-ttu-id="71029-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="71029-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="71029-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="71029-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71029-159">displayName</span><span class="sxs-lookup"><span data-stu-id="71029-159">displayName</span></span>|<span data-ttu-id="71029-160">String</span><span class="sxs-lookup"><span data-stu-id="71029-160">String</span></span>|<span data-ttu-id="71029-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="71029-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="71029-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="71029-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71029-163">version</span><span class="sxs-lookup"><span data-stu-id="71029-163">version</span></span>|<span data-ttu-id="71029-164">Int32</span><span class="sxs-lookup"><span data-stu-id="71029-164">Int32</span></span>|<span data-ttu-id="71029-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="71029-165">Version of the device configuration.</span></span> <span data-ttu-id="71029-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="71029-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71029-167">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="71029-167">trustedRootCertificate</span></span>|<span data-ttu-id="71029-168">Binary</span><span class="sxs-lookup"><span data-stu-id="71029-168">Binary</span></span>|<span data-ttu-id="71029-169">信頼できるルート証明書</span><span class="sxs-lookup"><span data-stu-id="71029-169">Trusted Root Certificate</span></span>|
|<span data-ttu-id="71029-170">certfilename</span><span class="sxs-lookup"><span data-stu-id="71029-170">certFileName</span></span>|<span data-ttu-id="71029-171">文字列</span><span class="sxs-lookup"><span data-stu-id="71029-171">String</span></span>|<span data-ttu-id="71029-172">UI に表示されるファイル名。</span><span class="sxs-lookup"><span data-stu-id="71029-172">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="71029-173">応答</span><span class="sxs-lookup"><span data-stu-id="71029-173">Response</span></span>
<span data-ttu-id="71029-174">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[androidwork profiletrustedrootrootcertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="71029-174">If successful, this method returns a `201 Created` response code and a [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71029-175">例</span><span class="sxs-lookup"><span data-stu-id="71029-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="71029-176">要求</span><span class="sxs-lookup"><span data-stu-id="71029-176">Request</span></span>
<span data-ttu-id="71029-177">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="71029-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 378

{
  "@odata.type": "#microsoft.graph.androidWorkProfileTrustedRootCertificate",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
  "certFileName": "Cert File Name value"
}
```

### <a name="response"></a><span data-ttu-id="71029-178">応答</span><span class="sxs-lookup"><span data-stu-id="71029-178">Response</span></span>
<span data-ttu-id="71029-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="71029-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 550

{
  "@odata.type": "#microsoft.graph.androidWorkProfileTrustedRootCertificate",
  "id": "37cc7454-7454-37cc-5474-cc375474cc37",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
  "certFileName": "Cert File Name value"
}
```





