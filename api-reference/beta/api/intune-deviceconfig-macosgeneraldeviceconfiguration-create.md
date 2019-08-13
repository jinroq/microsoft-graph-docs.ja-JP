---
title: Create macOSGeneralDeviceConfiguration
description: 新しい macOSGeneralDeviceConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bb283ee50e65e5e9408932dc41af1fb6497adb7b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36315380"
---
# <a name="create-macosgeneraldeviceconfiguration"></a><span data-ttu-id="7f39e-103">Create macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="7f39e-103">Create macOSGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="7f39e-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f39e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7f39e-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7f39e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f39e-106">新しい [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7f39e-106">Create a new [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7f39e-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="7f39e-107">Prerequisites</span></span>
<span data-ttu-id="7f39e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7f39e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f39e-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7f39e-110">Permission type</span></span>|<span data-ttu-id="7f39e-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7f39e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f39e-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7f39e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7f39e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f39e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7f39e-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7f39e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f39e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f39e-115">Not supported.</span></span>|
|<span data-ttu-id="7f39e-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7f39e-116">Application</span></span>|<span data-ttu-id="7f39e-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f39e-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f39e-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7f39e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7f39e-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7f39e-119">Request headers</span></span>
|<span data-ttu-id="7f39e-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7f39e-120">Header</span></span>|<span data-ttu-id="7f39e-121">値</span><span class="sxs-lookup"><span data-stu-id="7f39e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f39e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f39e-122">Authorization</span></span>|<span data-ttu-id="7f39e-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="7f39e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f39e-124">承諾</span><span class="sxs-lookup"><span data-stu-id="7f39e-124">Accept</span></span>|<span data-ttu-id="7f39e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7f39e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f39e-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="7f39e-126">Request body</span></span>
<span data-ttu-id="7f39e-127">要求本文で、macOSGeneralDeviceConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7f39e-127">In the request body, supply a JSON representation for the macOSGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="7f39e-128">次の表に、macOSGeneralDeviceConfiguration 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7f39e-128">The following table shows the properties that are required when you create the macOSGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="7f39e-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7f39e-129">Property</span></span>|<span data-ttu-id="7f39e-130">型</span><span class="sxs-lookup"><span data-stu-id="7f39e-130">Type</span></span>|<span data-ttu-id="7f39e-131">説明</span><span class="sxs-lookup"><span data-stu-id="7f39e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f39e-132">id</span><span class="sxs-lookup"><span data-stu-id="7f39e-132">id</span></span>|<span data-ttu-id="7f39e-133">文字列</span><span class="sxs-lookup"><span data-stu-id="7f39e-133">String</span></span>|<span data-ttu-id="7f39e-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7f39e-134">Key of the entity.</span></span> <span data-ttu-id="7f39e-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f39e-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7f39e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7f39e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="7f39e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f39e-137">DateTimeOffset</span></span>|<span data-ttu-id="7f39e-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="7f39e-138">DateTime the object was last modified.</span></span> <span data-ttu-id="7f39e-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f39e-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7f39e-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7f39e-140">roleScopeTagIds</span></span>|<span data-ttu-id="7f39e-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="7f39e-141">String collection</span></span>|<span data-ttu-id="7f39e-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="7f39e-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7f39e-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f39e-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7f39e-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="7f39e-144">supportsScopeTags</span></span>|<span data-ttu-id="7f39e-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f39e-145">Boolean</span></span>|<span data-ttu-id="7f39e-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7f39e-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="7f39e-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="7f39e-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="7f39e-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="7f39e-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="7f39e-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="7f39e-149">This property is read-only.</span></span> <span data-ttu-id="7f39e-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f39e-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7f39e-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="7f39e-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="7f39e-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="7f39e-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="7f39e-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="7f39e-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="7f39e-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f39e-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7f39e-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="7f39e-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="7f39e-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="7f39e-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="7f39e-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="7f39e-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="7f39e-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f39e-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7f39e-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="7f39e-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="7f39e-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="7f39e-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="7f39e-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="7f39e-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="7f39e-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f39e-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7f39e-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7f39e-163">createdDateTime</span></span>|<span data-ttu-id="7f39e-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f39e-164">DateTimeOffset</span></span>|<span data-ttu-id="7f39e-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="7f39e-165">DateTime the object was created.</span></span> <span data-ttu-id="7f39e-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f39e-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7f39e-167">description</span><span class="sxs-lookup"><span data-stu-id="7f39e-167">description</span></span>|<span data-ttu-id="7f39e-168">String</span><span class="sxs-lookup"><span data-stu-id="7f39e-168">String</span></span>|<span data-ttu-id="7f39e-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="7f39e-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7f39e-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f39e-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7f39e-171">displayName</span><span class="sxs-lookup"><span data-stu-id="7f39e-171">displayName</span></span>|<span data-ttu-id="7f39e-172">String</span><span class="sxs-lookup"><span data-stu-id="7f39e-172">String</span></span>|<span data-ttu-id="7f39e-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="7f39e-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7f39e-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f39e-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7f39e-175">version</span><span class="sxs-lookup"><span data-stu-id="7f39e-175">version</span></span>|<span data-ttu-id="7f39e-176">Int32</span><span class="sxs-lookup"><span data-stu-id="7f39e-176">Int32</span></span>|<span data-ttu-id="7f39e-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="7f39e-177">Version of the device configuration.</span></span> <span data-ttu-id="7f39e-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f39e-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7f39e-179">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="7f39e-179">compliantAppsList</span></span>|<span data-ttu-id="7f39e-180">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7f39e-180">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="7f39e-181">コンプライアンス内のアプリのリスト (CompliantAppListType によって制御される、許可リストまたは禁止リスト)。</span><span class="sxs-lookup"><span data-stu-id="7f39e-181">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="7f39e-182">このコレクションには、最大で 10000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="7f39e-182">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="7f39e-183">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="7f39e-183">compliantAppListType</span></span>|[<span data-ttu-id="7f39e-184">アプライアンスの種類</span><span class="sxs-lookup"><span data-stu-id="7f39e-184">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="7f39e-185">CompliantAppsList 内にあるリスト。</span><span class="sxs-lookup"><span data-stu-id="7f39e-185">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="7f39e-186">可能な値は、`none`、`appsInListCompliant`、`appsNotInListCompliant` です。</span><span class="sxs-lookup"><span data-stu-id="7f39e-186">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="7f39e-187">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="7f39e-187">emailInDomainSuffixes</span></span>|<span data-ttu-id="7f39e-188">String コレクション</span><span class="sxs-lookup"><span data-stu-id="7f39e-188">String collection</span></span>|<span data-ttu-id="7f39e-189">これらの文字列のいずれかに一致するサフィックスがないメール アドレスは、ドメイン外と見なされます。</span><span class="sxs-lookup"><span data-stu-id="7f39e-189">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="7f39e-190">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="7f39e-190">passwordBlockSimple</span></span>|<span data-ttu-id="7f39e-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f39e-191">Boolean</span></span>|<span data-ttu-id="7f39e-192">単純なパスワードを禁止します。</span><span class="sxs-lookup"><span data-stu-id="7f39e-192">Block simple passwords.</span></span>|
|<span data-ttu-id="7f39e-193">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="7f39e-193">passwordExpirationDays</span></span>|<span data-ttu-id="7f39e-194">Int32</span><span class="sxs-lookup"><span data-stu-id="7f39e-194">Int32</span></span>|<span data-ttu-id="7f39e-195">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="7f39e-195">Number of days before the password expires.</span></span>|
|<span data-ttu-id="7f39e-196">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="7f39e-196">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="7f39e-197">Int32</span><span class="sxs-lookup"><span data-stu-id="7f39e-197">Int32</span></span>|<span data-ttu-id="7f39e-198">パスワードが含まなければならない文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="7f39e-198">Number of character sets a password must contain.</span></span> <span data-ttu-id="7f39e-199">有効な値は 0 から 4 までです</span><span class="sxs-lookup"><span data-stu-id="7f39e-199">Valid values 0 to 4</span></span>|
|<span data-ttu-id="7f39e-200">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="7f39e-200">passwordMinimumLength</span></span>|<span data-ttu-id="7f39e-201">Int32</span><span class="sxs-lookup"><span data-stu-id="7f39e-201">Int32</span></span>|<span data-ttu-id="7f39e-202">パスワードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="7f39e-202">Minimum length of passwords.</span></span>|
|<span data-ttu-id="7f39e-203">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="7f39e-203">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="7f39e-204">Int32</span><span class="sxs-lookup"><span data-stu-id="7f39e-204">Int32</span></span>|<span data-ttu-id="7f39e-205">パスワードが要求されるまでに必要な非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="7f39e-205">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="7f39e-206">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="7f39e-206">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="7f39e-207">Int32</span><span class="sxs-lookup"><span data-stu-id="7f39e-207">Int32</span></span>|<span data-ttu-id="7f39e-208">画面がタイムアウトになるまでに必要な非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="7f39e-208">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="7f39e-209">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="7f39e-209">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="7f39e-210">Int32</span><span class="sxs-lookup"><span data-stu-id="7f39e-210">Int32</span></span>|<span data-ttu-id="7f39e-211">ブロックする、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="7f39e-211">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="7f39e-212">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="7f39e-212">passwordRequiredType</span></span>|[<span data-ttu-id="7f39e-213">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="7f39e-213">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="7f39e-214">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="7f39e-214">Type of password that is required.</span></span> <span data-ttu-id="7f39e-215">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="7f39e-215">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="7f39e-216">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="7f39e-216">passwordRequired</span></span>|<span data-ttu-id="7f39e-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f39e-217">Boolean</span></span>|<span data-ttu-id="7f39e-218">パスワードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="7f39e-218">Whether or not to require a password.</span></span>|
|<span data-ttu-id="7f39e-219">keychainBlockCloudSync</span><span class="sxs-lookup"><span data-stu-id="7f39e-219">keychainBlockCloudSync</span></span>|<span data-ttu-id="7f39e-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f39e-220">Boolean</span></span>|<span data-ttu-id="7f39e-221">ICloud のキーチェーン同期がブロックされるかどうかを示します (macOS 10.12 以降)。</span><span class="sxs-lookup"><span data-stu-id="7f39e-221">Indicates whether or not iCloud keychain synchronization is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="7f39e-222">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="7f39e-222">airPrintBlocked</span></span>|<span data-ttu-id="7f39e-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f39e-223">Boolean</span></span>|<span data-ttu-id="7f39e-224">放映印刷をブロックするかどうかを示します (macOS 10.12 以降)。</span><span class="sxs-lookup"><span data-stu-id="7f39e-224">Indicates whether or not AirPrint is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="7f39e-225">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="7f39e-225">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="7f39e-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f39e-226">Boolean</span></span>|<span data-ttu-id="7f39e-227">TLS 印刷通信 (macOS 10.13 以降) に対して信頼できる証明書が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7f39e-227">Indicates if trusted certificates are required for TLS printing communication (macOS 10.13 and later).</span></span>|
|<span data-ttu-id="7f39e-228">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="7f39e-228">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="7f39e-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f39e-229">Boolean</span></span>|<span data-ttu-id="7f39e-230">放映された印刷プリンターの iBeacon 検出をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7f39e-230">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="7f39e-231">これにより、ネットワークトラフィック (macOS 10.3 以降) のフィッシングからの、誤った放送印刷の Bluetooth ビーコンを防ぐことができます。</span><span class="sxs-lookup"><span data-stu-id="7f39e-231">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (macOS 10.3 and later).</span></span>|
|<span data-ttu-id="7f39e-232">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="7f39e-232">safariBlockAutofill</span></span>|<span data-ttu-id="7f39e-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f39e-233">Boolean</span></span>|<span data-ttu-id="7f39e-234">ユーザーによる Safari での自動入力の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7f39e-234">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="7f39e-235">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="7f39e-235">cameraBlocked</span></span>|<span data-ttu-id="7f39e-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f39e-236">Boolean</span></span>|<span data-ttu-id="7f39e-237">ユーザーによるデバイスのカメラへのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7f39e-237">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="7f39e-238">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="7f39e-238">iTunesBlockMusicService</span></span>|<span data-ttu-id="7f39e-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f39e-239">Boolean</span></span>|<span data-ttu-id="7f39e-240">ミュージックサービスを禁止するかどうかを示し、ミュージックアプリをクラシックモードに戻すかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="7f39e-240">Indicates whether or not to block Music service and revert Music app to classic mode.</span></span>|
|<span data-ttu-id="7f39e-241">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="7f39e-241">spotlightBlockInternetResults</span></span>|<span data-ttu-id="7f39e-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f39e-242">Boolean</span></span>|<span data-ttu-id="7f39e-243">スポットライトがインターネット検索の結果を返すことを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7f39e-243">Indicates whether or not to block Spotlight from returning any results from an Internet search.</span></span>|
|<span data-ttu-id="7f39e-244">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="7f39e-244">keyboardBlockDictation</span></span>|<span data-ttu-id="7f39e-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f39e-245">Boolean</span></span>|<span data-ttu-id="7f39e-246">ユーザーがディクテーション入力を使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7f39e-246">Indicates whether or not to block the user from using dictation input.</span></span>|
|<span data-ttu-id="7f39e-247">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="7f39e-247">definitionLookupBlocked</span></span>|<span data-ttu-id="7f39e-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f39e-248">Boolean</span></span>|<span data-ttu-id="7f39e-249">定義の参照をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7f39e-249">Indicates whether or not to block definition lookup.</span></span>|
|<span data-ttu-id="7f39e-250">appleWatchBlockAutoUnlock</span><span class="sxs-lookup"><span data-stu-id="7f39e-250">appleWatchBlockAutoUnlock</span></span>|<span data-ttu-id="7f39e-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f39e-251">Boolean</span></span>|<span data-ttu-id="7f39e-252">ユーザーが Apple Watch で Mac のロックを解除することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7f39e-252">Indicates whether or to block users from unlocking their Mac with Apple Watch.</span></span>|
|<span data-ttu-id="7f39e-253">iTunesBlockFileSharing</span><span class="sxs-lookup"><span data-stu-id="7f39e-253">iTunesBlockFileSharing</span></span>|<span data-ttu-id="7f39e-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f39e-254">Boolean</span></span>|<span data-ttu-id="7f39e-255">ITunes を使用してファイルを転送することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7f39e-255">Indicates whether or not to block files from being transferred using iTunes.</span></span>|
|<span data-ttu-id="7f39e-256">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="7f39e-256">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="7f39e-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f39e-257">Boolean</span></span>|<span data-ttu-id="7f39e-258">iCloud のドキュメントの同期を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7f39e-258">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="7f39e-259">iCloudBlockMail</span><span class="sxs-lookup"><span data-stu-id="7f39e-259">iCloudBlockMail</span></span>|<span data-ttu-id="7f39e-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f39e-260">Boolean</span></span>|<span data-ttu-id="7f39e-261">ICloud がメールの同期を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7f39e-261">Indicates whether or not to block iCloud from syncing mail.</span></span>|
|<span data-ttu-id="7f39e-262">iCloudBlockAddressBook</span><span class="sxs-lookup"><span data-stu-id="7f39e-262">iCloudBlockAddressBook</span></span>|<span data-ttu-id="7f39e-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f39e-263">Boolean</span></span>|<span data-ttu-id="7f39e-264">ICloud が連絡先を同期することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7f39e-264">Indicates whether or not to block iCloud from syncing contacts.</span></span>|
|<span data-ttu-id="7f39e-265">iCloudBlockCalendar</span><span class="sxs-lookup"><span data-stu-id="7f39e-265">iCloudBlockCalendar</span></span>|<span data-ttu-id="7f39e-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f39e-266">Boolean</span></span>|<span data-ttu-id="7f39e-267">ICloud が予定表を同期することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7f39e-267">Indicates whether or not to block iCloud from syncing calendars.</span></span>|
|<span data-ttu-id="7f39e-268">iCloudBlockReminders</span><span class="sxs-lookup"><span data-stu-id="7f39e-268">iCloudBlockReminders</span></span>|<span data-ttu-id="7f39e-269">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f39e-269">Boolean</span></span>|<span data-ttu-id="7f39e-270">ICloud がリマインダーの同期を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7f39e-270">Indicates whether or not to block iCloud from syncing reminders.</span></span>|
|<span data-ttu-id="7f39e-271">iCloudBlockBookmarks</span><span class="sxs-lookup"><span data-stu-id="7f39e-271">iCloudBlockBookmarks</span></span>|<span data-ttu-id="7f39e-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f39e-272">Boolean</span></span>|<span data-ttu-id="7f39e-273">ブックマークの同期を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7f39e-273">Indicates whether or not to block iCloud from syncing bookmarks.</span></span>|
|<span data-ttu-id="7f39e-274">iCloudBlockNotes</span><span class="sxs-lookup"><span data-stu-id="7f39e-274">iCloudBlockNotes</span></span>|<span data-ttu-id="7f39e-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f39e-275">Boolean</span></span>|<span data-ttu-id="7f39e-276">ICloud がノートの同期を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7f39e-276">Indicates whether or not to block iCloud from syncing notes.</span></span>|
|<span data-ttu-id="7f39e-277">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="7f39e-277">airDropBlocked</span></span>|<span data-ttu-id="7f39e-278">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f39e-278">Boolean</span></span>|<span data-ttu-id="7f39e-279">放映降下を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7f39e-279">Indicates whether or not to allow AirDrop.</span></span>|
|<span data-ttu-id="7f39e-280">passwordBlockModification</span><span class="sxs-lookup"><span data-stu-id="7f39e-280">passwordBlockModification</span></span>|<span data-ttu-id="7f39e-281">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f39e-281">Boolean</span></span>|<span data-ttu-id="7f39e-282">パスコードの変更を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7f39e-282">Indicates whether or not to allow passcode modification.</span></span>|
|<span data-ttu-id="7f39e-283">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="7f39e-283">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="7f39e-284">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f39e-284">Boolean</span></span>|<span data-ttu-id="7f39e-285">指紋によるロック解除を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7f39e-285">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="7f39e-286">passwordBlockAutoFill フィル</span><span class="sxs-lookup"><span data-stu-id="7f39e-286">passwordBlockAutoFill</span></span>|<span data-ttu-id="7f39e-287">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f39e-287">Boolean</span></span>|<span data-ttu-id="7f39e-288">パスワードのオートフィル機能を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7f39e-288">Indicates whether or not to block the AutoFill Passwords feature.</span></span>|
|<span data-ttu-id="7f39e-289">passwordBlockProximityRequests</span><span class="sxs-lookup"><span data-stu-id="7f39e-289">passwordBlockProximityRequests</span></span>|<span data-ttu-id="7f39e-290">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f39e-290">Boolean</span></span>|<span data-ttu-id="7f39e-291">近くのデバイスからのパスワードを要求することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7f39e-291">Indicates whether or not to block requesting passwords from nearby devices.</span></span>|
|<span data-ttu-id="7f39e-292">Passwordblockエア Drop共有</span><span class="sxs-lookup"><span data-stu-id="7f39e-292">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="7f39e-293">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f39e-293">Boolean</span></span>|<span data-ttu-id="7f39e-294">放映されたパスワード機能を使用してパスワードを共有することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7f39e-294">Indicates whether or not to block sharing passwords with the AirDrop passwords feature.</span></span>|
|<span data-ttu-id="7f39e-295">softwareUpdatesEnforcedDelayInDays</span><span class="sxs-lookup"><span data-stu-id="7f39e-295">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="7f39e-296">Int32</span><span class="sxs-lookup"><span data-stu-id="7f39e-296">Int32</span></span>|<span data-ttu-id="7f39e-297">監視対象デバイスに対してソフトウェア更新プログラムが delyed される日数を設定します。</span><span class="sxs-lookup"><span data-stu-id="7f39e-297">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="7f39e-298">有効な値は 0 から 90 までです</span><span class="sxs-lookup"><span data-stu-id="7f39e-298">Valid values 0 to 90</span></span>|
|<span data-ttu-id="7f39e-299">ソフトウェアの更新 Force延期</span><span class="sxs-lookup"><span data-stu-id="7f39e-299">softwareUpdatesForceDelayed</span></span>|<span data-ttu-id="7f39e-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f39e-300">Boolean</span></span>|<span data-ttu-id="7f39e-301">デバイスが監視モードのときに、ユーザーのソフトウェア更新プログラムの表示を延期するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7f39e-301">Indicates whether or not to delay user visibility of software updates when the device is in supervised mode.</span></span>|
|<span data-ttu-id="7f39e-302">contentCachingBlocked</span><span class="sxs-lookup"><span data-stu-id="7f39e-302">contentCachingBlocked</span></span>|<span data-ttu-id="7f39e-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f39e-303">Boolean</span></span>|<span data-ttu-id="7f39e-304">コンテンツのキャッシュを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7f39e-304">Indicates whether or not to allow content caching.</span></span>|
|<span data-ttu-id="7f39e-305">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="7f39e-305">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="7f39e-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f39e-306">Boolean</span></span>|<span data-ttu-id="7f39e-307">iCloud フォト ライブラリを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7f39e-307">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="7f39e-308">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="7f39e-308">screenCaptureBlocked</span></span>|<span data-ttu-id="7f39e-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f39e-309">Boolean</span></span>|<span data-ttu-id="7f39e-310">ユーザーがスクリーンショットを撮ることを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7f39e-310">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="7f39e-311">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="7f39e-311">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="7f39e-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f39e-312">Boolean</span></span>|<span data-ttu-id="7f39e-313">教室アプリによるリモート画面の監視を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7f39e-313">Indicates whether or not to allow remote screen observation by Classroom app.</span></span> <span data-ttu-id="7f39e-314">Apple School Manager または Apple Business Manager を介した MDM の登録が必要です。</span><span class="sxs-lookup"><span data-stu-id="7f39e-314">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="7f39e-315">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="7f39e-315">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="7f39e-316">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f39e-316">Boolean</span></span>|<span data-ttu-id="7f39e-317">確認のない学生の画面を表示するために、教室アプリの管理コースの教師に自動的にアクセス許可を付与するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7f39e-317">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting.</span></span> <span data-ttu-id="7f39e-318">Apple School Manager または Apple Business Manager を介した MDM の登録が必要です。</span><span class="sxs-lookup"><span data-stu-id="7f39e-318">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="7f39e-319">classroomForceAutomaticallyJoinClasses</span><span class="sxs-lookup"><span data-stu-id="7f39e-319">classroomForceAutomaticallyJoinClasses</span></span>|<span data-ttu-id="7f39e-320">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f39e-320">Boolean</span></span>|<span data-ttu-id="7f39e-321">教師に対してメッセージを表示せずに、教師の要求に対するアクセス許可を自動的に付与するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7f39e-321">Indicates whether or not to automatically give permission to the teacher's requests, without prompting the student.</span></span> <span data-ttu-id="7f39e-322">Apple School Manager または Apple Business Manager を介した MDM の登録が必要です。</span><span class="sxs-lookup"><span data-stu-id="7f39e-322">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="7f39e-323">classroomForceRequestPermissionToLeaveClasses</span><span class="sxs-lookup"><span data-stu-id="7f39e-323">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="7f39e-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f39e-324">Boolean</span></span>|<span data-ttu-id="7f39e-325">コースを終了しようとするときに教師にアクセス許可を要求するために、教室経由で管理されていないコースに登録された学生が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7f39e-325">Indicates whether a student enrolled in an unmanaged course via Classroom will be required to request permission from the teacher when attempting to leave the course.</span></span> <span data-ttu-id="7f39e-326">Apple School Manager または Apple Business Manager を介した MDM の登録が必要です。</span><span class="sxs-lookup"><span data-stu-id="7f39e-326">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="7f39e-327">classroomForceUnpromptedAppAndDeviceLock</span><span class="sxs-lookup"><span data-stu-id="7f39e-327">classroomForceUnpromptedAppAndDeviceLock</span></span>|<span data-ttu-id="7f39e-328">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f39e-328">Boolean</span></span>|<span data-ttu-id="7f39e-329">学生にメッセージを表示せずに、アプリまたはデバイスのロックを教師に許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7f39e-329">Indicates whether or not to allow the teacher to lock apps or the device without prompting the student.</span></span> <span data-ttu-id="7f39e-330">Apple School Manager または Apple Business Manager を介した MDM の登録が必要です。</span><span class="sxs-lookup"><span data-stu-id="7f39e-330">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="7f39e-331">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="7f39e-331">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="7f39e-332">ブール型</span><span class="sxs-lookup"><span data-stu-id="7f39e-332">Boolean</span></span>|<span data-ttu-id="7f39e-333">ユーザーが別の iOS または MacOS デバイス (MacOS 10.15 以降) 上の MacOS デバイスで開始した作業の継続を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7f39e-333">Indicates whether or not to block the user from continuing work that they started on a MacOS device on another iOS or MacOS device (MacOS 10.15 or later).</span></span>|



## <a name="response"></a><span data-ttu-id="7f39e-334">応答</span><span class="sxs-lookup"><span data-stu-id="7f39e-334">Response</span></span>
<span data-ttu-id="7f39e-335">このメソッドが成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7f39e-335">If successful, this method returns a `201 Created` response code and a [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f39e-336">例</span><span class="sxs-lookup"><span data-stu-id="7f39e-336">Example</span></span>

### <a name="request"></a><span data-ttu-id="7f39e-337">要求</span><span class="sxs-lookup"><span data-stu-id="7f39e-337">Request</span></span>
<span data-ttu-id="7f39e-338">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7f39e-338">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 3146

{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
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
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumCharacterSetCount": 0,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "keychainBlockCloudSync": true,
  "airPrintBlocked": true,
  "airPrintForceTrustedTLS": true,
  "airPrintBlockiBeaconDiscovery": true,
  "safariBlockAutofill": true,
  "cameraBlocked": true,
  "iTunesBlockMusicService": true,
  "spotlightBlockInternetResults": true,
  "keyboardBlockDictation": true,
  "definitionLookupBlocked": true,
  "appleWatchBlockAutoUnlock": true,
  "iTunesBlockFileSharing": true,
  "iCloudBlockDocumentSync": true,
  "iCloudBlockMail": true,
  "iCloudBlockAddressBook": true,
  "iCloudBlockCalendar": true,
  "iCloudBlockReminders": true,
  "iCloudBlockBookmarks": true,
  "iCloudBlockNotes": true,
  "airDropBlocked": true,
  "passwordBlockModification": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockAutoFill": true,
  "passwordBlockProximityRequests": true,
  "passwordBlockAirDropSharing": true,
  "softwareUpdatesEnforcedDelayInDays": 2,
  "softwareUpdatesForceDelayed": true,
  "contentCachingBlocked": true,
  "iCloudBlockPhotoLibrary": true,
  "screenCaptureBlocked": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
  "classroomForceAutomaticallyJoinClasses": true,
  "classroomForceRequestPermissionToLeaveClasses": true,
  "classroomForceUnpromptedAppAndDeviceLock": true,
  "iCloudBlockActivityContinuation": true
}
```

### <a name="response"></a><span data-ttu-id="7f39e-339">応答</span><span class="sxs-lookup"><span data-stu-id="7f39e-339">Response</span></span>
<span data-ttu-id="7f39e-p124">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7f39e-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3318

{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
  "id": "dc356aee-6aee-dc35-ee6a-35dcee6a35dc",
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
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumCharacterSetCount": 0,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "keychainBlockCloudSync": true,
  "airPrintBlocked": true,
  "airPrintForceTrustedTLS": true,
  "airPrintBlockiBeaconDiscovery": true,
  "safariBlockAutofill": true,
  "cameraBlocked": true,
  "iTunesBlockMusicService": true,
  "spotlightBlockInternetResults": true,
  "keyboardBlockDictation": true,
  "definitionLookupBlocked": true,
  "appleWatchBlockAutoUnlock": true,
  "iTunesBlockFileSharing": true,
  "iCloudBlockDocumentSync": true,
  "iCloudBlockMail": true,
  "iCloudBlockAddressBook": true,
  "iCloudBlockCalendar": true,
  "iCloudBlockReminders": true,
  "iCloudBlockBookmarks": true,
  "iCloudBlockNotes": true,
  "airDropBlocked": true,
  "passwordBlockModification": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockAutoFill": true,
  "passwordBlockProximityRequests": true,
  "passwordBlockAirDropSharing": true,
  "softwareUpdatesEnforcedDelayInDays": 2,
  "softwareUpdatesForceDelayed": true,
  "contentCachingBlocked": true,
  "iCloudBlockPhotoLibrary": true,
  "screenCaptureBlocked": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
  "classroomForceAutomaticallyJoinClasses": true,
  "classroomForceRequestPermissionToLeaveClasses": true,
  "classroomForceUnpromptedAppAndDeviceLock": true,
  "iCloudBlockActivityContinuation": true
}
```






