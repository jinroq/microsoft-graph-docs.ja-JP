---
title: Create windows10SecureAssessmentConfiguration
description: 新しい windows10SecureAssessmentConfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5b3de73a09bf187aa97b2d53f21a435ee4e054e2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953379"
---
# <a name="create-windows10secureassessmentconfiguration"></a><span data-ttu-id="e5cbe-103">Create windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="e5cbe-103">Create windows10SecureAssessmentConfiguration</span></span>

> <span data-ttu-id="e5cbe-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e5cbe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e5cbe-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e5cbe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e5cbe-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e5cbe-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e5cbe-107">新しい [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="e5cbe-107">Create a new [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e5cbe-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="e5cbe-108">Prerequisites</span></span>
<span data-ttu-id="e5cbe-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e5cbe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5cbe-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e5cbe-111">Permission type</span></span>|<span data-ttu-id="e5cbe-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e5cbe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5cbe-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e5cbe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e5cbe-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5cbe-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e5cbe-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e5cbe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5cbe-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e5cbe-116">Not supported.</span></span>|
|<span data-ttu-id="e5cbe-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e5cbe-117">Application</span></span>|<span data-ttu-id="e5cbe-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e5cbe-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5cbe-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e5cbe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e5cbe-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e5cbe-120">Request headers</span></span>
|<span data-ttu-id="e5cbe-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e5cbe-121">Header</span></span>|<span data-ttu-id="e5cbe-122">値</span><span class="sxs-lookup"><span data-stu-id="e5cbe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5cbe-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5cbe-123">Authorization</span></span>|<span data-ttu-id="e5cbe-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="e5cbe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5cbe-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e5cbe-125">Accept</span></span>|<span data-ttu-id="e5cbe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e5cbe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5cbe-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="e5cbe-127">Request body</span></span>
<span data-ttu-id="e5cbe-128">要求本文で、windows10SecureAssessmentConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e5cbe-128">In the request body, supply a JSON representation for the windows10SecureAssessmentConfiguration object.</span></span>

<span data-ttu-id="e5cbe-129">次の表に、windows10SecureAssessmentConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e5cbe-129">The following table shows the properties that are required when you create the windows10SecureAssessmentConfiguration.</span></span>

|<span data-ttu-id="e5cbe-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e5cbe-130">Property</span></span>|<span data-ttu-id="e5cbe-131">型</span><span class="sxs-lookup"><span data-stu-id="e5cbe-131">Type</span></span>|<span data-ttu-id="e5cbe-132">説明</span><span class="sxs-lookup"><span data-stu-id="e5cbe-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5cbe-133">id</span><span class="sxs-lookup"><span data-stu-id="e5cbe-133">id</span></span>|<span data-ttu-id="e5cbe-134">String</span><span class="sxs-lookup"><span data-stu-id="e5cbe-134">String</span></span>|<span data-ttu-id="e5cbe-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e5cbe-135">Key of the entity.</span></span> <span data-ttu-id="e5cbe-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e5cbe-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5cbe-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e5cbe-137">lastModifiedDateTime</span></span>|<span data-ttu-id="e5cbe-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5cbe-138">DateTimeOffset</span></span>|<span data-ttu-id="e5cbe-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="e5cbe-139">DateTime the object was last modified.</span></span> <span data-ttu-id="e5cbe-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e5cbe-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5cbe-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e5cbe-141">roleScopeTagIds</span></span>|<span data-ttu-id="e5cbe-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="e5cbe-142">String collection</span></span>|<span data-ttu-id="e5cbe-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="e5cbe-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e5cbe-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e5cbe-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5cbe-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="e5cbe-145">supportsScopeTags</span></span>|<span data-ttu-id="e5cbe-146">ブール型</span><span class="sxs-lookup"><span data-stu-id="e5cbe-146">Boolean</span></span>|<span data-ttu-id="e5cbe-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e5cbe-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e5cbe-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="e5cbe-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e5cbe-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="e5cbe-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e5cbe-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="e5cbe-150">This property is read-only.</span></span> <span data-ttu-id="e5cbe-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e5cbe-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5cbe-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e5cbe-152">createdDateTime</span></span>|<span data-ttu-id="e5cbe-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5cbe-153">DateTimeOffset</span></span>|<span data-ttu-id="e5cbe-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="e5cbe-154">DateTime the object was created.</span></span> <span data-ttu-id="e5cbe-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e5cbe-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5cbe-156">説明</span><span class="sxs-lookup"><span data-stu-id="e5cbe-156">description</span></span>|<span data-ttu-id="e5cbe-157">String</span><span class="sxs-lookup"><span data-stu-id="e5cbe-157">String</span></span>|<span data-ttu-id="e5cbe-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="e5cbe-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e5cbe-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e5cbe-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5cbe-160">displayName</span><span class="sxs-lookup"><span data-stu-id="e5cbe-160">displayName</span></span>|<span data-ttu-id="e5cbe-161">String</span><span class="sxs-lookup"><span data-stu-id="e5cbe-161">String</span></span>|<span data-ttu-id="e5cbe-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="e5cbe-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e5cbe-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e5cbe-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5cbe-164">version</span><span class="sxs-lookup"><span data-stu-id="e5cbe-164">version</span></span>|<span data-ttu-id="e5cbe-165">Int32</span><span class="sxs-lookup"><span data-stu-id="e5cbe-165">Int32</span></span>|<span data-ttu-id="e5cbe-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="e5cbe-166">Version of the device configuration.</span></span> <span data-ttu-id="e5cbe-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e5cbe-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5cbe-168">launchUri</span><span class="sxs-lookup"><span data-stu-id="e5cbe-168">launchUri</span></span>|<span data-ttu-id="e5cbe-169">String</span><span class="sxs-lookup"><span data-stu-id="e5cbe-169">String</span></span>|<span data-ttu-id="e5cbe-170">安全性評価ブラウザーを起動すると自動的に読み込まれる評価への URL リンク。</span><span class="sxs-lookup"><span data-stu-id="e5cbe-170">Url link to an assessment that's automatically loaded when the secure assessment browser is launched.</span></span> <span data-ttu-id="e5cbe-171">有効な URL である必要があります (http\[s\]://msdn.microsoft.com/)。</span><span class="sxs-lookup"><span data-stu-id="e5cbe-171">It has to be a valid Url (http\[s\]://msdn.microsoft.com/).</span></span>|
|<span data-ttu-id="e5cbe-172">configurationAccount</span><span class="sxs-lookup"><span data-stu-id="e5cbe-172">configurationAccount</span></span>|<span data-ttu-id="e5cbe-173">String</span><span class="sxs-lookup"><span data-stu-id="e5cbe-173">String</span></span>|<span data-ttu-id="e5cbe-174">Windows デバイスにテストを受けさせる際に、それを構成するために使用するアカウント。</span><span class="sxs-lookup"><span data-stu-id="e5cbe-174">The account used to configure the Windows device for taking the test.</span></span> <span data-ttu-id="e5cbe-175">ユーザーは、ドメイン アカウント (domain\user)、AAD アカウント (username@tenant.com)、ローカル アカウント (username) のいずれでも可能です。</span><span class="sxs-lookup"><span data-stu-id="e5cbe-175">The user can be a domain account (domain\user), an AAD account (username@tenant.com) or a local account (username).</span></span>|
|<span data-ttu-id="e5cbe-176">configurationAccountType</span><span class="sxs-lookup"><span data-stu-id="e5cbe-176">configurationAccountType</span></span>|[<span data-ttu-id="e5cbe-177">secureAssessmentAccountType</span><span class="sxs-lookup"><span data-stu-id="e5cbe-177">secureAssessmentAccountType</span></span>](../resources/intune-deviceconfig-secureassessmentaccounttype.md)|<span data-ttu-id="e5cbe-178">ConfigurationAccount するために使用するアカウントの種類です。</span><span class="sxs-lookup"><span data-stu-id="e5cbe-178">The account type used to by ConfigurationAccount.</span></span> <span data-ttu-id="e5cbe-179">可能な値は、`azureADAccount`、`domainAccount`、`localAccount` です。</span><span class="sxs-lookup"><span data-stu-id="e5cbe-179">Possible values are: `azureADAccount`, `domainAccount`, `localAccount`.</span></span>|
|<span data-ttu-id="e5cbe-180">allowPrinting</span><span class="sxs-lookup"><span data-stu-id="e5cbe-180">allowPrinting</span></span>|<span data-ttu-id="e5cbe-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5cbe-181">Boolean</span></span>|<span data-ttu-id="e5cbe-182">テスト中にアプリが印刷することを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e5cbe-182">Indicates whether or not to allow the app from printing during the test.</span></span>|
|<span data-ttu-id="e5cbe-183">allowScreenCapture</span><span class="sxs-lookup"><span data-stu-id="e5cbe-183">allowScreenCapture</span></span>|<span data-ttu-id="e5cbe-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5cbe-184">Boolean</span></span>|<span data-ttu-id="e5cbe-185">テスト中に画面キャプチャ機能を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e5cbe-185">Indicates whether or not to allow screen capture capability during a test.</span></span>|
|<span data-ttu-id="e5cbe-186">allowTextSuggestion</span><span class="sxs-lookup"><span data-stu-id="e5cbe-186">allowTextSuggestion</span></span>|<span data-ttu-id="e5cbe-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5cbe-187">Boolean</span></span>|<span data-ttu-id="e5cbe-188">テスト中に入力ヒントを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e5cbe-188">Indicates whether or not to allow text suggestions during the test.</span></span>|



## <a name="response"></a><span data-ttu-id="e5cbe-189">応答</span><span class="sxs-lookup"><span data-stu-id="e5cbe-189">Response</span></span>
<span data-ttu-id="e5cbe-190">このメソッドが成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e5cbe-190">If successful, this method returns a `201 Created` response code and a [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5cbe-191">例</span><span class="sxs-lookup"><span data-stu-id="e5cbe-191">Example</span></span>
### <a name="request"></a><span data-ttu-id="e5cbe-192">要求</span><span class="sxs-lookup"><span data-stu-id="e5cbe-192">Request</span></span>
<span data-ttu-id="e5cbe-193">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e5cbe-193">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 563

{
  "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="e5cbe-194">応答</span><span class="sxs-lookup"><span data-stu-id="e5cbe-194">Response</span></span>
<span data-ttu-id="e5cbe-p114">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e5cbe-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





