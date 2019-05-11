---
title: windows10SecureAssessmentConfiguration の更新
description: windows10SecureAssessmentConfiguration オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3c7750158f9f0bb90ffacabd6871cca5b2de7192
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33918438"
---
# <a name="update-windows10secureassessmentconfiguration"></a><span data-ttu-id="66e2a-103">windows10SecureAssessmentConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="66e2a-103">Update windows10SecureAssessmentConfiguration</span></span>

> <span data-ttu-id="66e2a-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="66e2a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66e2a-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="66e2a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66e2a-106">[windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="66e2a-106">Update the properties of a [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="66e2a-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="66e2a-107">Prerequisites</span></span>
<span data-ttu-id="66e2a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="66e2a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66e2a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="66e2a-110">Permission type</span></span>|<span data-ttu-id="66e2a-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="66e2a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66e2a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="66e2a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="66e2a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66e2a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="66e2a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="66e2a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66e2a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="66e2a-115">Not supported.</span></span>|
|<span data-ttu-id="66e2a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="66e2a-116">Application</span></span>|<span data-ttu-id="66e2a-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="66e2a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="66e2a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="66e2a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="66e2a-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="66e2a-119">Request headers</span></span>
|<span data-ttu-id="66e2a-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="66e2a-120">Header</span></span>|<span data-ttu-id="66e2a-121">値</span><span class="sxs-lookup"><span data-stu-id="66e2a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="66e2a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="66e2a-122">Authorization</span></span>|<span data-ttu-id="66e2a-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="66e2a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="66e2a-124">承諾</span><span class="sxs-lookup"><span data-stu-id="66e2a-124">Accept</span></span>|<span data-ttu-id="66e2a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="66e2a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="66e2a-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="66e2a-126">Request body</span></span>
<span data-ttu-id="66e2a-127">要求本文で、[windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="66e2a-127">In the request body, supply a JSON representation for the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

<span data-ttu-id="66e2a-128">次の表に、[windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="66e2a-128">The following table shows the properties that are required when you create the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span></span>

|<span data-ttu-id="66e2a-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="66e2a-129">Property</span></span>|<span data-ttu-id="66e2a-130">型</span><span class="sxs-lookup"><span data-stu-id="66e2a-130">Type</span></span>|<span data-ttu-id="66e2a-131">説明</span><span class="sxs-lookup"><span data-stu-id="66e2a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66e2a-132">id</span><span class="sxs-lookup"><span data-stu-id="66e2a-132">id</span></span>|<span data-ttu-id="66e2a-133">文字列</span><span class="sxs-lookup"><span data-stu-id="66e2a-133">String</span></span>|<span data-ttu-id="66e2a-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="66e2a-134">Key of the entity.</span></span> <span data-ttu-id="66e2a-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="66e2a-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66e2a-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="66e2a-136">lastModifiedDateTime</span></span>|<span data-ttu-id="66e2a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66e2a-137">DateTimeOffset</span></span>|<span data-ttu-id="66e2a-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="66e2a-138">DateTime the object was last modified.</span></span> <span data-ttu-id="66e2a-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="66e2a-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66e2a-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="66e2a-140">roleScopeTagIds</span></span>|<span data-ttu-id="66e2a-141">String collection</span><span class="sxs-lookup"><span data-stu-id="66e2a-141">String collection</span></span>|<span data-ttu-id="66e2a-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="66e2a-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="66e2a-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="66e2a-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66e2a-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="66e2a-144">supportsScopeTags</span></span>|<span data-ttu-id="66e2a-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="66e2a-145">Boolean</span></span>|<span data-ttu-id="66e2a-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="66e2a-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="66e2a-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="66e2a-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="66e2a-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="66e2a-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="66e2a-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="66e2a-149">This property is read-only.</span></span> <span data-ttu-id="66e2a-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="66e2a-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66e2a-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="66e2a-151">createdDateTime</span></span>|<span data-ttu-id="66e2a-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66e2a-152">DateTimeOffset</span></span>|<span data-ttu-id="66e2a-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="66e2a-153">DateTime the object was created.</span></span> <span data-ttu-id="66e2a-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="66e2a-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66e2a-155">description</span><span class="sxs-lookup"><span data-stu-id="66e2a-155">description</span></span>|<span data-ttu-id="66e2a-156">String</span><span class="sxs-lookup"><span data-stu-id="66e2a-156">String</span></span>|<span data-ttu-id="66e2a-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="66e2a-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="66e2a-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="66e2a-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66e2a-159">displayName</span><span class="sxs-lookup"><span data-stu-id="66e2a-159">displayName</span></span>|<span data-ttu-id="66e2a-160">String</span><span class="sxs-lookup"><span data-stu-id="66e2a-160">String</span></span>|<span data-ttu-id="66e2a-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="66e2a-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="66e2a-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="66e2a-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66e2a-163">version</span><span class="sxs-lookup"><span data-stu-id="66e2a-163">version</span></span>|<span data-ttu-id="66e2a-164">Int32</span><span class="sxs-lookup"><span data-stu-id="66e2a-164">Int32</span></span>|<span data-ttu-id="66e2a-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="66e2a-165">Version of the device configuration.</span></span> <span data-ttu-id="66e2a-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="66e2a-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66e2a-167">launchUri</span><span class="sxs-lookup"><span data-stu-id="66e2a-167">launchUri</span></span>|<span data-ttu-id="66e2a-168">String</span><span class="sxs-lookup"><span data-stu-id="66e2a-168">String</span></span>|<span data-ttu-id="66e2a-169">安全評価ブラウザーを起動すると自動的に読み込まれる評価への URL リンク。</span><span class="sxs-lookup"><span data-stu-id="66e2a-169">Url link to an assessment that's automatically loaded when the secure assessment browser is launched.</span></span> <span data-ttu-id="66e2a-170">有効な URL である必要があります (http\[s\]://msdn.microsoft.com/)。</span><span class="sxs-lookup"><span data-stu-id="66e2a-170">It has to be a valid Url (http\[s\]://msdn.microsoft.com/).</span></span>|
|<span data-ttu-id="66e2a-171">configurationAccount</span><span class="sxs-lookup"><span data-stu-id="66e2a-171">configurationAccount</span></span>|<span data-ttu-id="66e2a-172">String</span><span class="sxs-lookup"><span data-stu-id="66e2a-172">String</span></span>|<span data-ttu-id="66e2a-173">テストを受けるために Windows デバイスを構成する際に使用するアカウント。</span><span class="sxs-lookup"><span data-stu-id="66e2a-173">The account used to configure the Windows device for taking the test.</span></span> <span data-ttu-id="66e2a-174">ユーザーは、ドメイン アカウント (domain\user)、AAD アカウント (username@tenant.com) またはローカル アカウント (username) のいずれかです。</span><span class="sxs-lookup"><span data-stu-id="66e2a-174">The user can be a domain account (domain\user), an AAD account (username@tenant.com) or a local account (username).</span></span>|
|<span data-ttu-id="66e2a-175">configurationAccountType</span><span class="sxs-lookup"><span data-stu-id="66e2a-175">configurationAccountType</span></span>|[<span data-ttu-id="66e2a-176">secureAssessmentAccountType</span><span class="sxs-lookup"><span data-stu-id="66e2a-176">secureAssessmentAccountType</span></span>](../resources/intune-deviceconfig-secureassessmentaccounttype.md)|<span data-ttu-id="66e2a-177">ConfigurationAccount によって使用されるアカウントの種類。</span><span class="sxs-lookup"><span data-stu-id="66e2a-177">The account type used to by ConfigurationAccount.</span></span> <span data-ttu-id="66e2a-178">可能な値は、`azureADAccount`、`domainAccount`、`localAccount` です。</span><span class="sxs-lookup"><span data-stu-id="66e2a-178">Possible values are: `azureADAccount`, `domainAccount`, `localAccount`.</span></span>|
|<span data-ttu-id="66e2a-179">allowPrinting</span><span class="sxs-lookup"><span data-stu-id="66e2a-179">allowPrinting</span></span>|<span data-ttu-id="66e2a-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="66e2a-180">Boolean</span></span>|<span data-ttu-id="66e2a-181">テスト中にアプリが印刷することを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="66e2a-181">Indicates whether or not to allow the app from printing during the test.</span></span>|
|<span data-ttu-id="66e2a-182">allowScreenCapture</span><span class="sxs-lookup"><span data-stu-id="66e2a-182">allowScreenCapture</span></span>|<span data-ttu-id="66e2a-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="66e2a-183">Boolean</span></span>|<span data-ttu-id="66e2a-184">テスト中に画面の取り込み機能を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="66e2a-184">Indicates whether or not to allow screen capture capability during a test.</span></span>|
|<span data-ttu-id="66e2a-185">allowTextSuggestion</span><span class="sxs-lookup"><span data-stu-id="66e2a-185">allowTextSuggestion</span></span>|<span data-ttu-id="66e2a-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="66e2a-186">Boolean</span></span>|<span data-ttu-id="66e2a-187">テスト中に入力ヒントを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="66e2a-187">Indicates whether or not to allow text suggestions during the test.</span></span>|



## <a name="response"></a><span data-ttu-id="66e2a-188">応答</span><span class="sxs-lookup"><span data-stu-id="66e2a-188">Response</span></span>
<span data-ttu-id="66e2a-189">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="66e2a-189">If successful, this method returns a `200 OK` response code and an updated [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66e2a-190">例</span><span class="sxs-lookup"><span data-stu-id="66e2a-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="66e2a-191">要求</span><span class="sxs-lookup"><span data-stu-id="66e2a-191">Request</span></span>
<span data-ttu-id="66e2a-192">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="66e2a-192">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 499

{
  "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "launchUri": "Launch Uri value",
  "configurationAccount": "Configuration Account value",
  "configurationAccountType": "domainAccount",
  "allowPrinting": true,
  "allowScreenCapture": true,
  "allowTextSuggestion": true
}
```

### <a name="response"></a><span data-ttu-id="66e2a-193">応答</span><span class="sxs-lookup"><span data-stu-id="66e2a-193">Response</span></span>
<span data-ttu-id="66e2a-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="66e2a-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 671

{
  "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
  "id": "f60d71be-71be-f60d-be71-0df6be710df6",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "launchUri": "Launch Uri value",
  "configurationAccount": "Configuration Account value",
  "configurationAccountType": "domainAccount",
  "allowPrinting": true,
  "allowScreenCapture": true,
  "allowTextSuggestion": true
}
```




