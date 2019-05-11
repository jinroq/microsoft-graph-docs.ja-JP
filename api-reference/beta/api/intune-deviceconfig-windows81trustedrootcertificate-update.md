---
title: Windows81TrustedRootCertificate の更新
description: Windows81TrustedRootCertificate オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 188a2c8f3e8e4f5cf168a406dce2fffab82bf581
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33918186"
---
# <a name="update-windows81trustedrootcertificate"></a><span data-ttu-id="21540-103">Windows81TrustedRootCertificate の更新</span><span class="sxs-lookup"><span data-stu-id="21540-103">Update windows81TrustedRootCertificate</span></span>

> <span data-ttu-id="21540-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="21540-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21540-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="21540-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21540-106">[Windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="21540-106">Update the properties of a [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="21540-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="21540-107">Prerequisites</span></span>
<span data-ttu-id="21540-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="21540-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21540-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="21540-110">Permission type</span></span>|<span data-ttu-id="21540-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="21540-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21540-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="21540-112">Delegated (work or school account)</span></span>|<span data-ttu-id="21540-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21540-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="21540-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="21540-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21540-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="21540-115">Not supported.</span></span>|
|<span data-ttu-id="21540-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="21540-116">Application</span></span>|<span data-ttu-id="21540-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="21540-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="21540-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="21540-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/rootCertificate
```

## <a name="request-headers"></a><span data-ttu-id="21540-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="21540-119">Request headers</span></span>
|<span data-ttu-id="21540-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="21540-120">Header</span></span>|<span data-ttu-id="21540-121">値</span><span class="sxs-lookup"><span data-stu-id="21540-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21540-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="21540-122">Authorization</span></span>|<span data-ttu-id="21540-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="21540-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21540-124">承諾</span><span class="sxs-lookup"><span data-stu-id="21540-124">Accept</span></span>|<span data-ttu-id="21540-125">application/json</span><span class="sxs-lookup"><span data-stu-id="21540-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21540-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="21540-126">Request body</span></span>
<span data-ttu-id="21540-127">要求本文で、 [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="21540-127">In the request body, supply a JSON representation for the [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object.</span></span>

<span data-ttu-id="21540-128">次の表に、 [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="21540-128">The following table shows the properties that are required when you create the [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md).</span></span>

|<span data-ttu-id="21540-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="21540-129">Property</span></span>|<span data-ttu-id="21540-130">型</span><span class="sxs-lookup"><span data-stu-id="21540-130">Type</span></span>|<span data-ttu-id="21540-131">説明</span><span class="sxs-lookup"><span data-stu-id="21540-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21540-132">id</span><span class="sxs-lookup"><span data-stu-id="21540-132">id</span></span>|<span data-ttu-id="21540-133">文字列</span><span class="sxs-lookup"><span data-stu-id="21540-133">String</span></span>|<span data-ttu-id="21540-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="21540-134">Key of the entity.</span></span> <span data-ttu-id="21540-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="21540-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="21540-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="21540-136">lastModifiedDateTime</span></span>|<span data-ttu-id="21540-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21540-137">DateTimeOffset</span></span>|<span data-ttu-id="21540-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="21540-138">DateTime the object was last modified.</span></span> <span data-ttu-id="21540-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="21540-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="21540-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="21540-140">roleScopeTagIds</span></span>|<span data-ttu-id="21540-141">String collection</span><span class="sxs-lookup"><span data-stu-id="21540-141">String collection</span></span>|<span data-ttu-id="21540-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="21540-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="21540-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="21540-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="21540-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="21540-144">supportsScopeTags</span></span>|<span data-ttu-id="21540-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="21540-145">Boolean</span></span>|<span data-ttu-id="21540-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="21540-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="21540-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="21540-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="21540-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="21540-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="21540-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="21540-149">This property is read-only.</span></span> <span data-ttu-id="21540-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="21540-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="21540-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="21540-151">createdDateTime</span></span>|<span data-ttu-id="21540-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21540-152">DateTimeOffset</span></span>|<span data-ttu-id="21540-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="21540-153">DateTime the object was created.</span></span> <span data-ttu-id="21540-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="21540-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="21540-155">description</span><span class="sxs-lookup"><span data-stu-id="21540-155">description</span></span>|<span data-ttu-id="21540-156">String</span><span class="sxs-lookup"><span data-stu-id="21540-156">String</span></span>|<span data-ttu-id="21540-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="21540-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="21540-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="21540-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="21540-159">displayName</span><span class="sxs-lookup"><span data-stu-id="21540-159">displayName</span></span>|<span data-ttu-id="21540-160">String</span><span class="sxs-lookup"><span data-stu-id="21540-160">String</span></span>|<span data-ttu-id="21540-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="21540-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="21540-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="21540-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="21540-163">version</span><span class="sxs-lookup"><span data-stu-id="21540-163">version</span></span>|<span data-ttu-id="21540-164">Int32</span><span class="sxs-lookup"><span data-stu-id="21540-164">Int32</span></span>|<span data-ttu-id="21540-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="21540-165">Version of the device configuration.</span></span> <span data-ttu-id="21540-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="21540-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="21540-167">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="21540-167">trustedRootCertificate</span></span>|<span data-ttu-id="21540-168">Binary</span><span class="sxs-lookup"><span data-stu-id="21540-168">Binary</span></span>|<span data-ttu-id="21540-169">信頼できるルート証明書</span><span class="sxs-lookup"><span data-stu-id="21540-169">Trusted Root Certificate</span></span>|
|<span data-ttu-id="21540-170">certFileName</span><span class="sxs-lookup"><span data-stu-id="21540-170">certFileName</span></span>|<span data-ttu-id="21540-171">String</span><span class="sxs-lookup"><span data-stu-id="21540-171">String</span></span>|<span data-ttu-id="21540-172">UI に表示されるファイル名。</span><span class="sxs-lookup"><span data-stu-id="21540-172">File name to display in UI.</span></span>|
|<span data-ttu-id="21540-173">destinationStore</span><span class="sxs-lookup"><span data-stu-id="21540-173">destinationStore</span></span>|[<span data-ttu-id="21540-174">certificateDestinationStore</span><span class="sxs-lookup"><span data-stu-id="21540-174">certificateDestinationStore</span></span>](../resources/intune-deviceconfig-certificatedestinationstore.md)|<span data-ttu-id="21540-175">信頼されたルート証明書の保存先の場所。</span><span class="sxs-lookup"><span data-stu-id="21540-175">Destination store location for the Trusted Root Certificate.</span></span> <span data-ttu-id="21540-176">可能な値は、`computerCertStoreRoot`、`computerCertStoreIntermediate`、`userCertStoreIntermediate` です。</span><span class="sxs-lookup"><span data-stu-id="21540-176">Possible values are: `computerCertStoreRoot`, `computerCertStoreIntermediate`, `userCertStoreIntermediate`.</span></span>|



## <a name="response"></a><span data-ttu-id="21540-177">応答</span><span class="sxs-lookup"><span data-stu-id="21540-177">Response</span></span>
<span data-ttu-id="21540-178">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="21540-178">If successful, this method returns a `200 OK` response code and an updated [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21540-179">例</span><span class="sxs-lookup"><span data-stu-id="21540-179">Example</span></span>

### <a name="request"></a><span data-ttu-id="21540-180">要求</span><span class="sxs-lookup"><span data-stu-id="21540-180">Request</span></span>
<span data-ttu-id="21540-181">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="21540-181">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}
Content-type: application/json
Content-length: 425

{
  "@odata.type": "#microsoft.graph.windows81TrustedRootCertificate",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
  "certFileName": "Cert File Name value",
  "destinationStore": "computerCertStoreIntermediate"
}
```

### <a name="response"></a><span data-ttu-id="21540-182">応答</span><span class="sxs-lookup"><span data-stu-id="21540-182">Response</span></span>
<span data-ttu-id="21540-p111">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="21540-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 597

{
  "@odata.type": "#microsoft.graph.windows81TrustedRootCertificate",
  "id": "3fb588f9-88f9-3fb5-f988-b53ff988b53f",
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
  "certFileName": "Cert File Name value",
  "destinationStore": "computerCertStoreIntermediate"
}
```




