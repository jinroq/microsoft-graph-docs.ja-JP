---
title: iosTrustedRootCertificate を作成する
description: 新しい iosTrustedRootCertificate オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 48647c20f7f6ba5f995e01b0221f57d868ae67ab
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31804082"
---
# <a name="create-iostrustedrootcertificate"></a><span data-ttu-id="faab2-103">iosTrustedRootCertificate を作成する</span><span class="sxs-lookup"><span data-stu-id="faab2-103">Create iosTrustedRootCertificate</span></span>

> <span data-ttu-id="faab2-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="faab2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="faab2-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="faab2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="faab2-106">新しい[iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="faab2-106">Create a new [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="faab2-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="faab2-107">Prerequisites</span></span>
<span data-ttu-id="faab2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="faab2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="faab2-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="faab2-110">Permission type</span></span>|<span data-ttu-id="faab2-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="faab2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="faab2-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="faab2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="faab2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="faab2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="faab2-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="faab2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="faab2-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="faab2-115">Not supported.</span></span>|
|<span data-ttu-id="faab2-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="faab2-116">Application</span></span>|<span data-ttu-id="faab2-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="faab2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="faab2-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="faab2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEnterpriseWiFiConfiguration/rootCertificatesForServerValidation
```

## <a name="request-headers"></a><span data-ttu-id="faab2-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="faab2-119">Request headers</span></span>
|<span data-ttu-id="faab2-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="faab2-120">Header</span></span>|<span data-ttu-id="faab2-121">値</span><span class="sxs-lookup"><span data-stu-id="faab2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="faab2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="faab2-122">Authorization</span></span>|<span data-ttu-id="faab2-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="faab2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="faab2-124">承諾</span><span class="sxs-lookup"><span data-stu-id="faab2-124">Accept</span></span>|<span data-ttu-id="faab2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="faab2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="faab2-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="faab2-126">Request body</span></span>
<span data-ttu-id="faab2-127">要求本文で、iosTrustedRootCertificate オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="faab2-127">In the request body, supply a JSON representation for the iosTrustedRootCertificate object.</span></span>

<span data-ttu-id="faab2-128">次の表に、iosTrustedRootCertificate の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="faab2-128">The following table shows the properties that are required when you create the iosTrustedRootCertificate.</span></span>

|<span data-ttu-id="faab2-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="faab2-129">Property</span></span>|<span data-ttu-id="faab2-130">型</span><span class="sxs-lookup"><span data-stu-id="faab2-130">Type</span></span>|<span data-ttu-id="faab2-131">説明</span><span class="sxs-lookup"><span data-stu-id="faab2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="faab2-132">id</span><span class="sxs-lookup"><span data-stu-id="faab2-132">id</span></span>|<span data-ttu-id="faab2-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="faab2-133">String</span></span>|<span data-ttu-id="faab2-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="faab2-134">Key of the entity.</span></span> <span data-ttu-id="faab2-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="faab2-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faab2-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="faab2-136">lastModifiedDateTime</span></span>|<span data-ttu-id="faab2-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="faab2-137">DateTimeOffset</span></span>|<span data-ttu-id="faab2-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="faab2-138">DateTime the object was last modified.</span></span> <span data-ttu-id="faab2-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="faab2-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faab2-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="faab2-140">roleScopeTagIds</span></span>|<span data-ttu-id="faab2-141">String コレクション</span><span class="sxs-lookup"><span data-stu-id="faab2-141">String collection</span></span>|<span data-ttu-id="faab2-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="faab2-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="faab2-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="faab2-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faab2-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="faab2-144">supportsScopeTags</span></span>|<span data-ttu-id="faab2-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="faab2-145">Boolean</span></span>|<span data-ttu-id="faab2-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="faab2-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="faab2-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="faab2-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="faab2-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="faab2-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="faab2-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="faab2-149">This property is read-only.</span></span> <span data-ttu-id="faab2-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="faab2-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faab2-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="faab2-151">createdDateTime</span></span>|<span data-ttu-id="faab2-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="faab2-152">DateTimeOffset</span></span>|<span data-ttu-id="faab2-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="faab2-153">DateTime the object was created.</span></span> <span data-ttu-id="faab2-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="faab2-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faab2-155">説明</span><span class="sxs-lookup"><span data-stu-id="faab2-155">description</span></span>|<span data-ttu-id="faab2-156">String</span><span class="sxs-lookup"><span data-stu-id="faab2-156">String</span></span>|<span data-ttu-id="faab2-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="faab2-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="faab2-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="faab2-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faab2-159">displayName</span><span class="sxs-lookup"><span data-stu-id="faab2-159">displayName</span></span>|<span data-ttu-id="faab2-160">String</span><span class="sxs-lookup"><span data-stu-id="faab2-160">String</span></span>|<span data-ttu-id="faab2-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="faab2-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="faab2-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="faab2-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faab2-163">version</span><span class="sxs-lookup"><span data-stu-id="faab2-163">version</span></span>|<span data-ttu-id="faab2-164">Int32</span><span class="sxs-lookup"><span data-stu-id="faab2-164">Int32</span></span>|<span data-ttu-id="faab2-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="faab2-165">Version of the device configuration.</span></span> <span data-ttu-id="faab2-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="faab2-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faab2-167">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="faab2-167">trustedRootCertificate</span></span>|<span data-ttu-id="faab2-168">Binary</span><span class="sxs-lookup"><span data-stu-id="faab2-168">Binary</span></span>|<span data-ttu-id="faab2-169">信頼されたルート証明書。</span><span class="sxs-lookup"><span data-stu-id="faab2-169">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="faab2-170">certfilename</span><span class="sxs-lookup"><span data-stu-id="faab2-170">certFileName</span></span>|<span data-ttu-id="faab2-171">文字列</span><span class="sxs-lookup"><span data-stu-id="faab2-171">String</span></span>|<span data-ttu-id="faab2-172">UI に表示されるファイル名。</span><span class="sxs-lookup"><span data-stu-id="faab2-172">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="faab2-173">応答</span><span class="sxs-lookup"><span data-stu-id="faab2-173">Response</span></span>
<span data-ttu-id="faab2-174">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="faab2-174">If successful, this method returns a `201 Created` response code and a [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="faab2-175">例</span><span class="sxs-lookup"><span data-stu-id="faab2-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="faab2-176">要求</span><span class="sxs-lookup"><span data-stu-id="faab2-176">Request</span></span>
<span data-ttu-id="faab2-177">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="faab2-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEnterpriseWiFiConfiguration/rootCertificatesForServerValidation
Content-type: application/json
Content-length: 363

{
  "@odata.type": "#microsoft.graph.iosTrustedRootCertificate",
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

### <a name="response"></a><span data-ttu-id="faab2-178">応答</span><span class="sxs-lookup"><span data-stu-id="faab2-178">Response</span></span>
<span data-ttu-id="faab2-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="faab2-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 535

{
  "@odata.type": "#microsoft.graph.iosTrustedRootCertificate",
  "id": "9bc72bb8-2bb8-9bc7-b82b-c79bb82bc79b",
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





