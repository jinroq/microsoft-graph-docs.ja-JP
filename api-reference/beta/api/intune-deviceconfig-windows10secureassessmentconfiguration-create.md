---
title: Create windows10SecureAssessmentConfiguration
description: 新しい windows10SecureAssessmentConfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f0f5428d517433bf499cf22d85c6a589ea331d66
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30975904"
---
# <a name="create-windows10secureassessmentconfiguration"></a><span data-ttu-id="2fb3e-103">Create windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="2fb3e-103">Create windows10SecureAssessmentConfiguration</span></span>

> <span data-ttu-id="2fb3e-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2fb3e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2fb3e-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2fb3e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2fb3e-106">新しい [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="2fb3e-106">Create a new [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2fb3e-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="2fb3e-107">Prerequisites</span></span>
<span data-ttu-id="2fb3e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2fb3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2fb3e-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2fb3e-110">Permission type</span></span>|<span data-ttu-id="2fb3e-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2fb3e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2fb3e-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2fb3e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2fb3e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2fb3e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2fb3e-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2fb3e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2fb3e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2fb3e-115">Not supported.</span></span>|
|<span data-ttu-id="2fb3e-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2fb3e-116">Application</span></span>|<span data-ttu-id="2fb3e-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2fb3e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2fb3e-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2fb3e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2fb3e-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2fb3e-119">Request headers</span></span>
|<span data-ttu-id="2fb3e-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2fb3e-120">Header</span></span>|<span data-ttu-id="2fb3e-121">値</span><span class="sxs-lookup"><span data-stu-id="2fb3e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2fb3e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2fb3e-122">Authorization</span></span>|<span data-ttu-id="2fb3e-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="2fb3e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2fb3e-124">承諾</span><span class="sxs-lookup"><span data-stu-id="2fb3e-124">Accept</span></span>|<span data-ttu-id="2fb3e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2fb3e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2fb3e-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="2fb3e-126">Request body</span></span>
<span data-ttu-id="2fb3e-127">要求本文で、windows10SecureAssessmentConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2fb3e-127">In the request body, supply a JSON representation for the windows10SecureAssessmentConfiguration object.</span></span>

<span data-ttu-id="2fb3e-128">次の表に、windows10SecureAssessmentConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="2fb3e-128">The following table shows the properties that are required when you create the windows10SecureAssessmentConfiguration.</span></span>

|<span data-ttu-id="2fb3e-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2fb3e-129">Property</span></span>|<span data-ttu-id="2fb3e-130">型</span><span class="sxs-lookup"><span data-stu-id="2fb3e-130">Type</span></span>|<span data-ttu-id="2fb3e-131">説明</span><span class="sxs-lookup"><span data-stu-id="2fb3e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2fb3e-132">id</span><span class="sxs-lookup"><span data-stu-id="2fb3e-132">id</span></span>|<span data-ttu-id="2fb3e-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="2fb3e-133">String</span></span>|<span data-ttu-id="2fb3e-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="2fb3e-134">Key of the entity.</span></span> <span data-ttu-id="2fb3e-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2fb3e-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2fb3e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2fb3e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="2fb3e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2fb3e-137">DateTimeOffset</span></span>|<span data-ttu-id="2fb3e-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="2fb3e-138">DateTime the object was last modified.</span></span> <span data-ttu-id="2fb3e-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2fb3e-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2fb3e-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2fb3e-140">roleScopeTagIds</span></span>|<span data-ttu-id="2fb3e-141">String collection</span><span class="sxs-lookup"><span data-stu-id="2fb3e-141">String collection</span></span>|<span data-ttu-id="2fb3e-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="2fb3e-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2fb3e-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2fb3e-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2fb3e-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="2fb3e-144">supportsScopeTags</span></span>|<span data-ttu-id="2fb3e-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="2fb3e-145">Boolean</span></span>|<span data-ttu-id="2fb3e-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2fb3e-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2fb3e-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="2fb3e-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2fb3e-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="2fb3e-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2fb3e-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="2fb3e-149">This property is read-only.</span></span> <span data-ttu-id="2fb3e-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2fb3e-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2fb3e-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2fb3e-151">createdDateTime</span></span>|<span data-ttu-id="2fb3e-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2fb3e-152">DateTimeOffset</span></span>|<span data-ttu-id="2fb3e-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="2fb3e-153">DateTime the object was created.</span></span> <span data-ttu-id="2fb3e-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2fb3e-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2fb3e-155">description</span><span class="sxs-lookup"><span data-stu-id="2fb3e-155">description</span></span>|<span data-ttu-id="2fb3e-156">String</span><span class="sxs-lookup"><span data-stu-id="2fb3e-156">String</span></span>|<span data-ttu-id="2fb3e-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="2fb3e-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2fb3e-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2fb3e-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2fb3e-159">displayName</span><span class="sxs-lookup"><span data-stu-id="2fb3e-159">displayName</span></span>|<span data-ttu-id="2fb3e-160">String</span><span class="sxs-lookup"><span data-stu-id="2fb3e-160">String</span></span>|<span data-ttu-id="2fb3e-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="2fb3e-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2fb3e-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2fb3e-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2fb3e-163">version</span><span class="sxs-lookup"><span data-stu-id="2fb3e-163">version</span></span>|<span data-ttu-id="2fb3e-164">Int32</span><span class="sxs-lookup"><span data-stu-id="2fb3e-164">Int32</span></span>|<span data-ttu-id="2fb3e-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="2fb3e-165">Version of the device configuration.</span></span> <span data-ttu-id="2fb3e-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2fb3e-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2fb3e-167">launchUri</span><span class="sxs-lookup"><span data-stu-id="2fb3e-167">launchUri</span></span>|<span data-ttu-id="2fb3e-168">String</span><span class="sxs-lookup"><span data-stu-id="2fb3e-168">String</span></span>|<span data-ttu-id="2fb3e-169">安全評価ブラウザーを起動すると自動的に読み込まれる評価への URL リンク。</span><span class="sxs-lookup"><span data-stu-id="2fb3e-169">Url link to an assessment that's automatically loaded when the secure assessment browser is launched.</span></span> <span data-ttu-id="2fb3e-170">有効な URL である必要があります (http\[s\]://msdn.microsoft.com/)。</span><span class="sxs-lookup"><span data-stu-id="2fb3e-170">It has to be a valid Url (http\[s\]://msdn.microsoft.com/).</span></span>|
|<span data-ttu-id="2fb3e-171">configurationAccount</span><span class="sxs-lookup"><span data-stu-id="2fb3e-171">configurationAccount</span></span>|<span data-ttu-id="2fb3e-172">String</span><span class="sxs-lookup"><span data-stu-id="2fb3e-172">String</span></span>|<span data-ttu-id="2fb3e-173">テストを受けるために Windows デバイスを構成する際に使用するアカウント。</span><span class="sxs-lookup"><span data-stu-id="2fb3e-173">The account used to configure the Windows device for taking the test.</span></span> <span data-ttu-id="2fb3e-174">ユーザーは、ドメイン アカウント (domain\user)、AAD アカウント (username@tenant.com) またはローカル アカウント (username) のいずれかです。</span><span class="sxs-lookup"><span data-stu-id="2fb3e-174">The user can be a domain account (domain\user), an AAD account (username@tenant.com) or a local account (username).</span></span>|
|<span data-ttu-id="2fb3e-175">configurationaccounttype</span><span class="sxs-lookup"><span data-stu-id="2fb3e-175">configurationAccountType</span></span>|[<span data-ttu-id="2fb3e-176">secureAssessmentAccountType</span><span class="sxs-lookup"><span data-stu-id="2fb3e-176">secureAssessmentAccountType</span></span>](../resources/intune-deviceconfig-secureassessmentaccounttype.md)|<span data-ttu-id="2fb3e-177">configurationaccount によって使用されるアカウントの種類。</span><span class="sxs-lookup"><span data-stu-id="2fb3e-177">The account type used to by ConfigurationAccount.</span></span> <span data-ttu-id="2fb3e-178">使用可能な値は、`azureADAccount`、`domainAccount`、`localAccount` です。</span><span class="sxs-lookup"><span data-stu-id="2fb3e-178">Possible values are: `azureADAccount`, `domainAccount`, `localAccount`.</span></span>|
|<span data-ttu-id="2fb3e-179">allowPrinting</span><span class="sxs-lookup"><span data-stu-id="2fb3e-179">allowPrinting</span></span>|<span data-ttu-id="2fb3e-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="2fb3e-180">Boolean</span></span>|<span data-ttu-id="2fb3e-181">テスト中にアプリが印刷することを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2fb3e-181">Indicates whether or not to allow the app from printing during the test.</span></span>|
|<span data-ttu-id="2fb3e-182">allowScreenCapture</span><span class="sxs-lookup"><span data-stu-id="2fb3e-182">allowScreenCapture</span></span>|<span data-ttu-id="2fb3e-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="2fb3e-183">Boolean</span></span>|<span data-ttu-id="2fb3e-184">テスト中に画面の取り込み機能を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2fb3e-184">Indicates whether or not to allow screen capture capability during a test.</span></span>|
|<span data-ttu-id="2fb3e-185">allowTextSuggestion</span><span class="sxs-lookup"><span data-stu-id="2fb3e-185">allowTextSuggestion</span></span>|<span data-ttu-id="2fb3e-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="2fb3e-186">Boolean</span></span>|<span data-ttu-id="2fb3e-187">テスト中に入力ヒントを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2fb3e-187">Indicates whether or not to allow text suggestions during the test.</span></span>|



## <a name="response"></a><span data-ttu-id="2fb3e-188">応答</span><span class="sxs-lookup"><span data-stu-id="2fb3e-188">Response</span></span>
<span data-ttu-id="2fb3e-189">このメソッドが成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2fb3e-189">If successful, this method returns a `201 Created` response code and a [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2fb3e-190">例</span><span class="sxs-lookup"><span data-stu-id="2fb3e-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="2fb3e-191">要求</span><span class="sxs-lookup"><span data-stu-id="2fb3e-191">Request</span></span>
<span data-ttu-id="2fb3e-192">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2fb3e-192">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="2fb3e-193">応答</span><span class="sxs-lookup"><span data-stu-id="2fb3e-193">Response</span></span>
<span data-ttu-id="2fb3e-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2fb3e-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




