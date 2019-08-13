---
title: Create windows10SecureAssessmentConfiguration
description: 新しい windows10SecureAssessmentConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e3a9c2932ec99c27fb7d04c47effce421b7c686b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36314365"
---
# <a name="create-windows10secureassessmentconfiguration"></a><span data-ttu-id="f063d-103">Create windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="f063d-103">Create windows10SecureAssessmentConfiguration</span></span>

> <span data-ttu-id="f063d-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f063d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f063d-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f063d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f063d-106">新しい [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="f063d-106">Create a new [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f063d-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="f063d-107">Prerequisites</span></span>
<span data-ttu-id="f063d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f063d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f063d-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f063d-110">Permission type</span></span>|<span data-ttu-id="f063d-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f063d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f063d-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f063d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f063d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f063d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f063d-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f063d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f063d-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f063d-115">Not supported.</span></span>|
|<span data-ttu-id="f063d-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f063d-116">Application</span></span>|<span data-ttu-id="f063d-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f063d-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f063d-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f063d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f063d-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f063d-119">Request headers</span></span>
|<span data-ttu-id="f063d-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f063d-120">Header</span></span>|<span data-ttu-id="f063d-121">値</span><span class="sxs-lookup"><span data-stu-id="f063d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f063d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f063d-122">Authorization</span></span>|<span data-ttu-id="f063d-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="f063d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f063d-124">承諾</span><span class="sxs-lookup"><span data-stu-id="f063d-124">Accept</span></span>|<span data-ttu-id="f063d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f063d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f063d-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="f063d-126">Request body</span></span>
<span data-ttu-id="f063d-127">要求本文で、windows10SecureAssessmentConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f063d-127">In the request body, supply a JSON representation for the windows10SecureAssessmentConfiguration object.</span></span>

<span data-ttu-id="f063d-128">次の表に、windows10SecureAssessmentConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f063d-128">The following table shows the properties that are required when you create the windows10SecureAssessmentConfiguration.</span></span>

|<span data-ttu-id="f063d-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f063d-129">Property</span></span>|<span data-ttu-id="f063d-130">型</span><span class="sxs-lookup"><span data-stu-id="f063d-130">Type</span></span>|<span data-ttu-id="f063d-131">説明</span><span class="sxs-lookup"><span data-stu-id="f063d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f063d-132">id</span><span class="sxs-lookup"><span data-stu-id="f063d-132">id</span></span>|<span data-ttu-id="f063d-133">文字列</span><span class="sxs-lookup"><span data-stu-id="f063d-133">String</span></span>|<span data-ttu-id="f063d-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f063d-134">Key of the entity.</span></span> <span data-ttu-id="f063d-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f063d-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f063d-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f063d-136">lastModifiedDateTime</span></span>|<span data-ttu-id="f063d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f063d-137">DateTimeOffset</span></span>|<span data-ttu-id="f063d-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="f063d-138">DateTime the object was last modified.</span></span> <span data-ttu-id="f063d-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f063d-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f063d-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f063d-140">roleScopeTagIds</span></span>|<span data-ttu-id="f063d-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="f063d-141">String collection</span></span>|<span data-ttu-id="f063d-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="f063d-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f063d-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f063d-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f063d-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f063d-144">supportsScopeTags</span></span>|<span data-ttu-id="f063d-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="f063d-145">Boolean</span></span>|<span data-ttu-id="f063d-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f063d-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f063d-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="f063d-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f063d-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="f063d-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f063d-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="f063d-149">This property is read-only.</span></span> <span data-ttu-id="f063d-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f063d-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f063d-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f063d-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="f063d-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f063d-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="f063d-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="f063d-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="f063d-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f063d-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f063d-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f063d-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="f063d-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f063d-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="f063d-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="f063d-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="f063d-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f063d-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f063d-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="f063d-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="f063d-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="f063d-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="f063d-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="f063d-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="f063d-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f063d-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f063d-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f063d-163">createdDateTime</span></span>|<span data-ttu-id="f063d-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f063d-164">DateTimeOffset</span></span>|<span data-ttu-id="f063d-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="f063d-165">DateTime the object was created.</span></span> <span data-ttu-id="f063d-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f063d-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f063d-167">description</span><span class="sxs-lookup"><span data-stu-id="f063d-167">description</span></span>|<span data-ttu-id="f063d-168">String</span><span class="sxs-lookup"><span data-stu-id="f063d-168">String</span></span>|<span data-ttu-id="f063d-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="f063d-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f063d-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f063d-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f063d-171">displayName</span><span class="sxs-lookup"><span data-stu-id="f063d-171">displayName</span></span>|<span data-ttu-id="f063d-172">String</span><span class="sxs-lookup"><span data-stu-id="f063d-172">String</span></span>|<span data-ttu-id="f063d-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="f063d-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f063d-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f063d-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f063d-175">version</span><span class="sxs-lookup"><span data-stu-id="f063d-175">version</span></span>|<span data-ttu-id="f063d-176">Int32</span><span class="sxs-lookup"><span data-stu-id="f063d-176">Int32</span></span>|<span data-ttu-id="f063d-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="f063d-177">Version of the device configuration.</span></span> <span data-ttu-id="f063d-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f063d-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f063d-179">launchUri</span><span class="sxs-lookup"><span data-stu-id="f063d-179">launchUri</span></span>|<span data-ttu-id="f063d-180">String</span><span class="sxs-lookup"><span data-stu-id="f063d-180">String</span></span>|<span data-ttu-id="f063d-181">安全評価ブラウザーを起動すると自動的に読み込まれる評価への URL リンク。</span><span class="sxs-lookup"><span data-stu-id="f063d-181">Url link to an assessment that's automatically loaded when the secure assessment browser is launched.</span></span> <span data-ttu-id="f063d-182">有効な URL である必要があります (http\[s\]://msdn.microsoft.com/)。</span><span class="sxs-lookup"><span data-stu-id="f063d-182">It has to be a valid Url (http\[s\]://msdn.microsoft.com/).</span></span>|
|<span data-ttu-id="f063d-183">configurationAccount</span><span class="sxs-lookup"><span data-stu-id="f063d-183">configurationAccount</span></span>|<span data-ttu-id="f063d-184">String</span><span class="sxs-lookup"><span data-stu-id="f063d-184">String</span></span>|<span data-ttu-id="f063d-185">テストを受けるために Windows デバイスを構成する際に使用するアカウント。</span><span class="sxs-lookup"><span data-stu-id="f063d-185">The account used to configure the Windows device for taking the test.</span></span> <span data-ttu-id="f063d-186">ユーザーは、ドメイン アカウント (domain\user)、AAD アカウント (username@tenant.com) またはローカル アカウント (username) のいずれかです。</span><span class="sxs-lookup"><span data-stu-id="f063d-186">The user can be a domain account (domain\user), an AAD account (username@tenant.com) or a local account (username).</span></span>|
|<span data-ttu-id="f063d-187">configurationAccountType</span><span class="sxs-lookup"><span data-stu-id="f063d-187">configurationAccountType</span></span>|[<span data-ttu-id="f063d-188">secureAssessmentAccountType</span><span class="sxs-lookup"><span data-stu-id="f063d-188">secureAssessmentAccountType</span></span>](../resources/intune-deviceconfig-secureassessmentaccounttype.md)|<span data-ttu-id="f063d-189">ConfigurationAccount によって使用されるアカウントの種類。</span><span class="sxs-lookup"><span data-stu-id="f063d-189">The account type used to by ConfigurationAccount.</span></span> <span data-ttu-id="f063d-190">使用可能な値は、`azureADAccount`、`domainAccount`、`localAccount`、`localGuestAccount` です。</span><span class="sxs-lookup"><span data-stu-id="f063d-190">Possible values are: `azureADAccount`, `domainAccount`, `localAccount`, `localGuestAccount`.</span></span>|
|<span data-ttu-id="f063d-191">allowPrinting</span><span class="sxs-lookup"><span data-stu-id="f063d-191">allowPrinting</span></span>|<span data-ttu-id="f063d-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="f063d-192">Boolean</span></span>|<span data-ttu-id="f063d-193">テスト中にアプリが印刷することを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f063d-193">Indicates whether or not to allow the app from printing during the test.</span></span>|
|<span data-ttu-id="f063d-194">allowScreenCapture</span><span class="sxs-lookup"><span data-stu-id="f063d-194">allowScreenCapture</span></span>|<span data-ttu-id="f063d-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="f063d-195">Boolean</span></span>|<span data-ttu-id="f063d-196">テスト中に画面の取り込み機能を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f063d-196">Indicates whether or not to allow screen capture capability during a test.</span></span>|
|<span data-ttu-id="f063d-197">allowTextSuggestion</span><span class="sxs-lookup"><span data-stu-id="f063d-197">allowTextSuggestion</span></span>|<span data-ttu-id="f063d-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="f063d-198">Boolean</span></span>|<span data-ttu-id="f063d-199">テスト中に入力ヒントを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f063d-199">Indicates whether or not to allow text suggestions during the test.</span></span>|
|<span data-ttu-id="f063d-200">localGuestAccountName</span><span class="sxs-lookup"><span data-stu-id="f063d-200">localGuestAccountName</span></span>|<span data-ttu-id="f063d-201">String</span><span class="sxs-lookup"><span data-stu-id="f063d-201">String</span></span>|<span data-ttu-id="f063d-202">サインイン画面に表示されるローカルゲストアカウントの表示テキストを指定します。</span><span class="sxs-lookup"><span data-stu-id="f063d-202">Specifies the display text for the local guest account shown on the sign-in screen.</span></span> <span data-ttu-id="f063d-203">通常は評価の名前です。</span><span class="sxs-lookup"><span data-stu-id="f063d-203">Typically is the name of an assessment.</span></span> <span data-ttu-id="f063d-204">ユーザーがサインイン画面でローカルのゲストアカウントをクリックすると、評価アプリが指定された評価 URL で起動されます。</span><span class="sxs-lookup"><span data-stu-id="f063d-204">When the user clicks the local guest account on the sign-in screen, an assessment app is launched with a specified assessment URL.</span></span> <span data-ttu-id="f063d-205">セキュリティで保護された評価は、Windows 10、バージョン1903以降を実行しているデバイスでローカルのゲストアカウントのサインインを使用してのみ構成できます。</span><span class="sxs-lookup"><span data-stu-id="f063d-205">Secure assessments can only be configured with local guest account sign-in on devices running Windows 10, version 1903 or later.</span></span> <span data-ttu-id="f063d-206">重要な注意事項: このプロパティは、セキュリティで保護された評価のためにローカルのゲストアカウントのサインイン操作を正しく動作させるために、assessmentAppUserModelID で設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f063d-206">Important notice: this property must be set with assessmentAppUserModelID in order to make the local guest account sign-in experience work properly for secure assessments.</span></span>|
|<span data-ttu-id="f063d-207">assessmentAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="f063d-207">assessmentAppUserModelId</span></span>|<span data-ttu-id="f063d-208">String</span><span class="sxs-lookup"><span data-stu-id="f063d-208">String</span></span>|<span data-ttu-id="f063d-209">ユーザーがローカルゲストアカウントでセキュリティで保護された評価にサインインしたときに起動される評価アプリのアプリケーションユーザーモデル ID を指定します。</span><span class="sxs-lookup"><span data-stu-id="f063d-209">Specifies the application user model ID of the assessment app launched when a user signs in to a secure assessment with a local guest account.</span></span> <span data-ttu-id="f063d-210">重要な注意事項: セキュリティで保護された評価を行うために、ローカルゲストアカウントのサインイン操作を正しく動作させるには、このプロパティを localGuestAccountName で設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f063d-210">Important notice: this property must be set with localGuestAccountName in order to make the local guest account sign-in experience work properly for secure assessments.</span></span>|



## <a name="response"></a><span data-ttu-id="f063d-211">応答</span><span class="sxs-lookup"><span data-stu-id="f063d-211">Response</span></span>
<span data-ttu-id="f063d-212">このメソッドが成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f063d-212">If successful, this method returns a `201 Created` response code and a [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f063d-213">例</span><span class="sxs-lookup"><span data-stu-id="f063d-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="f063d-214">要求</span><span class="sxs-lookup"><span data-stu-id="f063d-214">Request</span></span>
<span data-ttu-id="f063d-215">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f063d-215">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1403

{
  "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "launchUri": "Launch Uri value",
  "configurationAccount": "Configuration Account value",
  "configurationAccountType": "domainAccount",
  "allowPrinting": true,
  "allowScreenCapture": true,
  "allowTextSuggestion": true,
  "localGuestAccountName": "Local Guest Account Name value",
  "assessmentAppUserModelId": "Assessment App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="f063d-216">応答</span><span class="sxs-lookup"><span data-stu-id="f063d-216">Response</span></span>
<span data-ttu-id="f063d-p118">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f063d-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1575

{
  "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
  "id": "f60d71be-71be-f60d-be71-0df6be710df6",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "launchUri": "Launch Uri value",
  "configurationAccount": "Configuration Account value",
  "configurationAccountType": "domainAccount",
  "allowPrinting": true,
  "allowScreenCapture": true,
  "allowTextSuggestion": true,
  "localGuestAccountName": "Local Guest Account Name value",
  "assessmentAppUserModelId": "Assessment App User Model Id value"
}
```






