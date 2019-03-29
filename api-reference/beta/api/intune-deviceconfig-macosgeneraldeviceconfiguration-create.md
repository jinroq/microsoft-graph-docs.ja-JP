---
title: Create macOSGeneralDeviceConfiguration
description: 新しい macOSGeneralDeviceConfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a813ee14200b07dc86d92acef01fb2cf1928d52a
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30975085"
---
# <a name="create-macosgeneraldeviceconfiguration"></a><span data-ttu-id="c5f82-103">Create macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="c5f82-103">Create macOSGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="c5f82-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c5f82-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5f82-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c5f82-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5f82-106">新しい [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c5f82-106">Create a new [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c5f82-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="c5f82-107">Prerequisites</span></span>
<span data-ttu-id="c5f82-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c5f82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5f82-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c5f82-110">Permission type</span></span>|<span data-ttu-id="c5f82-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c5f82-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5f82-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c5f82-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c5f82-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5f82-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c5f82-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c5f82-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5f82-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c5f82-115">Not supported.</span></span>|
|<span data-ttu-id="c5f82-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c5f82-116">Application</span></span>|<span data-ttu-id="c5f82-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c5f82-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5f82-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c5f82-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c5f82-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c5f82-119">Request headers</span></span>
|<span data-ttu-id="c5f82-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c5f82-120">Header</span></span>|<span data-ttu-id="c5f82-121">値</span><span class="sxs-lookup"><span data-stu-id="c5f82-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5f82-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5f82-122">Authorization</span></span>|<span data-ttu-id="c5f82-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="c5f82-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5f82-124">承諾</span><span class="sxs-lookup"><span data-stu-id="c5f82-124">Accept</span></span>|<span data-ttu-id="c5f82-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c5f82-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5f82-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="c5f82-126">Request body</span></span>
<span data-ttu-id="c5f82-127">要求本文で、macOSGeneralDeviceConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c5f82-127">In the request body, supply a JSON representation for the macOSGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="c5f82-128">次の表に、macOSGeneralDeviceConfiguration 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="c5f82-128">The following table shows the properties that are required when you create the macOSGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="c5f82-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c5f82-129">Property</span></span>|<span data-ttu-id="c5f82-130">型</span><span class="sxs-lookup"><span data-stu-id="c5f82-130">Type</span></span>|<span data-ttu-id="c5f82-131">説明</span><span class="sxs-lookup"><span data-stu-id="c5f82-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5f82-132">id</span><span class="sxs-lookup"><span data-stu-id="c5f82-132">id</span></span>|<span data-ttu-id="c5f82-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="c5f82-133">String</span></span>|<span data-ttu-id="c5f82-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c5f82-134">Key of the entity.</span></span> <span data-ttu-id="c5f82-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c5f82-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5f82-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c5f82-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c5f82-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5f82-137">DateTimeOffset</span></span>|<span data-ttu-id="c5f82-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="c5f82-138">DateTime the object was last modified.</span></span> <span data-ttu-id="c5f82-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c5f82-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5f82-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c5f82-140">roleScopeTagIds</span></span>|<span data-ttu-id="c5f82-141">String collection</span><span class="sxs-lookup"><span data-stu-id="c5f82-141">String collection</span></span>|<span data-ttu-id="c5f82-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="c5f82-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c5f82-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c5f82-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5f82-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c5f82-144">supportsScopeTags</span></span>|<span data-ttu-id="c5f82-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5f82-145">Boolean</span></span>|<span data-ttu-id="c5f82-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c5f82-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c5f82-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="c5f82-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c5f82-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="c5f82-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c5f82-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="c5f82-149">This property is read-only.</span></span> <span data-ttu-id="c5f82-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c5f82-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5f82-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c5f82-151">createdDateTime</span></span>|<span data-ttu-id="c5f82-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5f82-152">DateTimeOffset</span></span>|<span data-ttu-id="c5f82-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="c5f82-153">DateTime the object was created.</span></span> <span data-ttu-id="c5f82-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c5f82-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5f82-155">description</span><span class="sxs-lookup"><span data-stu-id="c5f82-155">description</span></span>|<span data-ttu-id="c5f82-156">String</span><span class="sxs-lookup"><span data-stu-id="c5f82-156">String</span></span>|<span data-ttu-id="c5f82-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="c5f82-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c5f82-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c5f82-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5f82-159">displayName</span><span class="sxs-lookup"><span data-stu-id="c5f82-159">displayName</span></span>|<span data-ttu-id="c5f82-160">String</span><span class="sxs-lookup"><span data-stu-id="c5f82-160">String</span></span>|<span data-ttu-id="c5f82-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="c5f82-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c5f82-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c5f82-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5f82-163">version</span><span class="sxs-lookup"><span data-stu-id="c5f82-163">version</span></span>|<span data-ttu-id="c5f82-164">Int32</span><span class="sxs-lookup"><span data-stu-id="c5f82-164">Int32</span></span>|<span data-ttu-id="c5f82-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="c5f82-165">Version of the device configuration.</span></span> <span data-ttu-id="c5f82-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c5f82-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5f82-167">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="c5f82-167">compliantAppsList</span></span>|<span data-ttu-id="c5f82-168">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c5f82-168">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="c5f82-169">コンプライアンス内のアプリのリスト (CompliantAppListType によって制御される、許可リストまたは禁止リスト)。</span><span class="sxs-lookup"><span data-stu-id="c5f82-169">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="c5f82-170">このコレクションには、最大で 10000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="c5f82-170">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="c5f82-171">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="c5f82-171">compliantAppListType</span></span>|[<span data-ttu-id="c5f82-172">アプライアンスの種類</span><span class="sxs-lookup"><span data-stu-id="c5f82-172">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="c5f82-173">CompliantAppsList 内にあるリスト。</span><span class="sxs-lookup"><span data-stu-id="c5f82-173">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="c5f82-174">使用可能な値は、`none`、`appsInListCompliant`、`appsNotInListCompliant` です。</span><span class="sxs-lookup"><span data-stu-id="c5f82-174">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="c5f82-175">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="c5f82-175">emailInDomainSuffixes</span></span>|<span data-ttu-id="c5f82-176">String コレクション</span><span class="sxs-lookup"><span data-stu-id="c5f82-176">String collection</span></span>|<span data-ttu-id="c5f82-177">これらの文字列のいずれかに一致するサフィックスがないメール アドレスは、ドメイン外と見なされます。</span><span class="sxs-lookup"><span data-stu-id="c5f82-177">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="c5f82-178">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="c5f82-178">passwordBlockSimple</span></span>|<span data-ttu-id="c5f82-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5f82-179">Boolean</span></span>|<span data-ttu-id="c5f82-180">単純なパスワードを禁止します。</span><span class="sxs-lookup"><span data-stu-id="c5f82-180">Block simple passwords.</span></span>|
|<span data-ttu-id="c5f82-181">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="c5f82-181">passwordExpirationDays</span></span>|<span data-ttu-id="c5f82-182">Int32</span><span class="sxs-lookup"><span data-stu-id="c5f82-182">Int32</span></span>|<span data-ttu-id="c5f82-183">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="c5f82-183">Number of days before the password expires.</span></span>|
|<span data-ttu-id="c5f82-184">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="c5f82-184">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="c5f82-185">Int32</span><span class="sxs-lookup"><span data-stu-id="c5f82-185">Int32</span></span>|<span data-ttu-id="c5f82-186">パスワードが含まなければならない文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="c5f82-186">Number of character sets a password must contain.</span></span> <span data-ttu-id="c5f82-187">有効な値は 0 から 4 までです</span><span class="sxs-lookup"><span data-stu-id="c5f82-187">Valid values 0 to 4</span></span>|
|<span data-ttu-id="c5f82-188">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="c5f82-188">passwordMinimumLength</span></span>|<span data-ttu-id="c5f82-189">Int32</span><span class="sxs-lookup"><span data-stu-id="c5f82-189">Int32</span></span>|<span data-ttu-id="c5f82-190">パスワードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="c5f82-190">Minimum length of passwords.</span></span>|
|<span data-ttu-id="c5f82-191">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="c5f82-191">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="c5f82-192">Int32</span><span class="sxs-lookup"><span data-stu-id="c5f82-192">Int32</span></span>|<span data-ttu-id="c5f82-193">パスワードが要求されるまでに必要な非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="c5f82-193">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="c5f82-194">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="c5f82-194">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="c5f82-195">Int32</span><span class="sxs-lookup"><span data-stu-id="c5f82-195">Int32</span></span>|<span data-ttu-id="c5f82-196">画面がタイムアウトになるまでに必要な非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="c5f82-196">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="c5f82-197">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="c5f82-197">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="c5f82-198">Int32</span><span class="sxs-lookup"><span data-stu-id="c5f82-198">Int32</span></span>|<span data-ttu-id="c5f82-199">ブロックする、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="c5f82-199">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="c5f82-200">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="c5f82-200">passwordRequiredType</span></span>|[<span data-ttu-id="c5f82-201">requiredpasswordtype</span><span class="sxs-lookup"><span data-stu-id="c5f82-201">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="c5f82-202">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="c5f82-202">Type of password that is required.</span></span> <span data-ttu-id="c5f82-203">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="c5f82-203">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="c5f82-204">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="c5f82-204">passwordRequired</span></span>|<span data-ttu-id="c5f82-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5f82-205">Boolean</span></span>|<span data-ttu-id="c5f82-206">パスワードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="c5f82-206">Whether or not to require a password.</span></span>|
|<span data-ttu-id="c5f82-207">keychainBlockCloudSync</span><span class="sxs-lookup"><span data-stu-id="c5f82-207">keychainBlockCloudSync</span></span>|<span data-ttu-id="c5f82-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5f82-208">Boolean</span></span>|<span data-ttu-id="c5f82-209">iCloud のキーチェーン同期がブロックされるかどうかを示します (macOS 10.12 以降)。</span><span class="sxs-lookup"><span data-stu-id="c5f82-209">Indicates whether or not iCloud keychain synchronization is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="c5f82-210">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="c5f82-210">airPrintBlocked</span></span>|<span data-ttu-id="c5f82-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5f82-211">Boolean</span></span>|<span data-ttu-id="c5f82-212">放映印刷をブロックするかどうかを示します (macOS 10.12 以降)。</span><span class="sxs-lookup"><span data-stu-id="c5f82-212">Indicates whether or not AirPrint is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="c5f82-213">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="c5f82-213">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="c5f82-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5f82-214">Boolean</span></span>|<span data-ttu-id="c5f82-215">TLS 印刷通信 (macOS 10.13 以降) に対して信頼できる証明書が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c5f82-215">Indicates if trusted certificates are required for TLS printing communication (macOS 10.13 and later).</span></span>|
|<span data-ttu-id="c5f82-216">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="c5f82-216">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="c5f82-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5f82-217">Boolean</span></span>|<span data-ttu-id="c5f82-218">放映された印刷プリンターの ibeacon 検出をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c5f82-218">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="c5f82-219">これにより、ネットワークトラフィック (macOS 10.3 以降) のフィッシングからの、誤った放送印刷の Bluetooth ビーコンを防ぐことができます。</span><span class="sxs-lookup"><span data-stu-id="c5f82-219">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (macOS 10.3 and later).</span></span>|
|<span data-ttu-id="c5f82-220">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="c5f82-220">safariBlockAutofill</span></span>|<span data-ttu-id="c5f82-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5f82-221">Boolean</span></span>|<span data-ttu-id="c5f82-222">ユーザーによる Safari での自動入力の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c5f82-222">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="c5f82-223">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="c5f82-223">cameraBlocked</span></span>|<span data-ttu-id="c5f82-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5f82-224">Boolean</span></span>|<span data-ttu-id="c5f82-225">ユーザーによるデバイスのカメラへのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c5f82-225">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="c5f82-226">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="c5f82-226">iTunesBlockMusicService</span></span>|<span data-ttu-id="c5f82-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5f82-227">Boolean</span></span>|<span data-ttu-id="c5f82-228">ミュージックサービスを禁止するかどうかを示し、ミュージックアプリをクラシックモードに戻すかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="c5f82-228">Indicates whether or not to block Music service and revert Music app to classic mode.</span></span>|
|<span data-ttu-id="c5f82-229">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="c5f82-229">spotlightBlockInternetResults</span></span>|<span data-ttu-id="c5f82-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5f82-230">Boolean</span></span>|<span data-ttu-id="c5f82-231">スポットライトがインターネット検索の結果を返すことを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c5f82-231">Indicates whether or not to block Spotlight from returning any results from an Internet search.</span></span>|
|<span data-ttu-id="c5f82-232">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="c5f82-232">keyboardBlockDictation</span></span>|<span data-ttu-id="c5f82-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5f82-233">Boolean</span></span>|<span data-ttu-id="c5f82-234">ユーザーがディクテーション入力を使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c5f82-234">Indicates whether or not to block the user from using dictation input.</span></span>|
|<span data-ttu-id="c5f82-235">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="c5f82-235">definitionLookupBlocked</span></span>|<span data-ttu-id="c5f82-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5f82-236">Boolean</span></span>|<span data-ttu-id="c5f82-237">定義の参照をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c5f82-237">Indicates whether or not to block definition lookup.</span></span>|
|<span data-ttu-id="c5f82-238">appleWatchBlockAutoUnlock</span><span class="sxs-lookup"><span data-stu-id="c5f82-238">appleWatchBlockAutoUnlock</span></span>|<span data-ttu-id="c5f82-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5f82-239">Boolean</span></span>|<span data-ttu-id="c5f82-240">ユーザーが Apple Watch で Mac のロックを解除することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c5f82-240">Indicates whether or to block users from unlocking their Mac with Apple Watch.</span></span>|
|<span data-ttu-id="c5f82-241">itunesblockfilesharing</span><span class="sxs-lookup"><span data-stu-id="c5f82-241">iTunesBlockFileSharing</span></span>|<span data-ttu-id="c5f82-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5f82-242">Boolean</span></span>|<span data-ttu-id="c5f82-243">iTunes を使用してファイルを転送することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c5f82-243">Indicates whether or not to block files from being transferred using iTunes.</span></span>|
|<span data-ttu-id="c5f82-244">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="c5f82-244">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="c5f82-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5f82-245">Boolean</span></span>|<span data-ttu-id="c5f82-246">iCloud のドキュメントの同期を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c5f82-246">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="c5f82-247">iCloudBlockMail</span><span class="sxs-lookup"><span data-stu-id="c5f82-247">iCloudBlockMail</span></span>|<span data-ttu-id="c5f82-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5f82-248">Boolean</span></span>|<span data-ttu-id="c5f82-249">iCloud がメールの同期を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c5f82-249">Indicates whether or not to block iCloud from syncing mail.</span></span>|
|<span data-ttu-id="c5f82-250">iCloudBlockAddressBook</span><span class="sxs-lookup"><span data-stu-id="c5f82-250">iCloudBlockAddressBook</span></span>|<span data-ttu-id="c5f82-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5f82-251">Boolean</span></span>|<span data-ttu-id="c5f82-252">iCloud が連絡先を同期することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c5f82-252">Indicates whether or not to block iCloud from syncing contacts.</span></span>|
|<span data-ttu-id="c5f82-253">iCloudBlockCalendar</span><span class="sxs-lookup"><span data-stu-id="c5f82-253">iCloudBlockCalendar</span></span>|<span data-ttu-id="c5f82-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5f82-254">Boolean</span></span>|<span data-ttu-id="c5f82-255">iCloud が予定表を同期することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c5f82-255">Indicates whether or not to block iCloud from syncing calendars.</span></span>|
|<span data-ttu-id="c5f82-256">iCloudBlockReminders</span><span class="sxs-lookup"><span data-stu-id="c5f82-256">iCloudBlockReminders</span></span>|<span data-ttu-id="c5f82-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5f82-257">Boolean</span></span>|<span data-ttu-id="c5f82-258">iCloud がリマインダーの同期を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c5f82-258">Indicates whether or not to block iCloud from syncing reminders.</span></span>|
|<span data-ttu-id="c5f82-259">iCloudBlockBookmarks</span><span class="sxs-lookup"><span data-stu-id="c5f82-259">iCloudBlockBookmarks</span></span>|<span data-ttu-id="c5f82-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5f82-260">Boolean</span></span>|<span data-ttu-id="c5f82-261">ブックマークの同期を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c5f82-261">Indicates whether or not to block iCloud from syncing bookmarks.</span></span>|
|<span data-ttu-id="c5f82-262">iCloudBlockNotes</span><span class="sxs-lookup"><span data-stu-id="c5f82-262">iCloudBlockNotes</span></span>|<span data-ttu-id="c5f82-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5f82-263">Boolean</span></span>|<span data-ttu-id="c5f82-264">iCloud がノートの同期を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c5f82-264">Indicates whether or not to block iCloud from syncing notes.</span></span>|
|<span data-ttu-id="c5f82-265">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="c5f82-265">airDropBlocked</span></span>|<span data-ttu-id="c5f82-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5f82-266">Boolean</span></span>|<span data-ttu-id="c5f82-267">放映降下を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c5f82-267">Indicates whether or not to allow AirDrop.</span></span>|
|<span data-ttu-id="c5f82-268">passwordblockmodification</span><span class="sxs-lookup"><span data-stu-id="c5f82-268">passwordBlockModification</span></span>|<span data-ttu-id="c5f82-269">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5f82-269">Boolean</span></span>|<span data-ttu-id="c5f82-270">パスコードの変更を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c5f82-270">Indicates whether or not to allow passcode modification.</span></span>|
|<span data-ttu-id="c5f82-271">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="c5f82-271">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="c5f82-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5f82-272">Boolean</span></span>|<span data-ttu-id="c5f82-273">指紋によるロック解除を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c5f82-273">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="c5f82-274">passwordblockautofill フィル</span><span class="sxs-lookup"><span data-stu-id="c5f82-274">passwordBlockAutoFill</span></span>|<span data-ttu-id="c5f82-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5f82-275">Boolean</span></span>|<span data-ttu-id="c5f82-276">パスワードのオートフィル機能を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c5f82-276">Indicates whether or not to block the AutoFill Passwords feature.</span></span>|
|<span data-ttu-id="c5f82-277">passwordBlockProximityRequests</span><span class="sxs-lookup"><span data-stu-id="c5f82-277">passwordBlockProximityRequests</span></span>|<span data-ttu-id="c5f82-278">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5f82-278">Boolean</span></span>|<span data-ttu-id="c5f82-279">近くのデバイスからのパスワードを要求することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c5f82-279">Indicates whether or not to block requesting passwords from nearby devices.</span></span>|
|<span data-ttu-id="c5f82-280">passwordblockエア drop共有</span><span class="sxs-lookup"><span data-stu-id="c5f82-280">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="c5f82-281">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5f82-281">Boolean</span></span>|<span data-ttu-id="c5f82-282">放映されたパスワード機能を使用してパスワードを共有することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c5f82-282">Indicates whether or not to block sharing passwords with the AirDrop passwords feature.</span></span>|
|<span data-ttu-id="c5f82-283">softwareUpdatesEnforcedDelayInDays</span><span class="sxs-lookup"><span data-stu-id="c5f82-283">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="c5f82-284">Int32</span><span class="sxs-lookup"><span data-stu-id="c5f82-284">Int32</span></span>|<span data-ttu-id="c5f82-285">監視対象デバイスに対してソフトウェア更新プログラムが delyed される日数を設定します。</span><span class="sxs-lookup"><span data-stu-id="c5f82-285">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="c5f82-286">有効な値は 0 から 90 までです</span><span class="sxs-lookup"><span data-stu-id="c5f82-286">Valid values 0 to 90</span></span>|
|<span data-ttu-id="c5f82-287">ソフトウェアの更新 force延期</span><span class="sxs-lookup"><span data-stu-id="c5f82-287">softwareUpdatesForceDelayed</span></span>|<span data-ttu-id="c5f82-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5f82-288">Boolean</span></span>|<span data-ttu-id="c5f82-289">デバイスが監視モードのときに、ユーザーのソフトウェア更新プログラムの表示を延期するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c5f82-289">Indicates whether or not to delay user visibility of software updates when the device is in supervised mode.</span></span>|
|<span data-ttu-id="c5f82-290">contentcachingblocked</span><span class="sxs-lookup"><span data-stu-id="c5f82-290">contentCachingBlocked</span></span>|<span data-ttu-id="c5f82-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5f82-291">Boolean</span></span>|<span data-ttu-id="c5f82-292">コンテンツのキャッシュを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c5f82-292">Indicates whether or not to allow content caching.</span></span>|



## <a name="response"></a><span data-ttu-id="c5f82-293">応答</span><span class="sxs-lookup"><span data-stu-id="c5f82-293">Response</span></span>
<span data-ttu-id="c5f82-294">このメソッドが成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c5f82-294">If successful, this method returns a `201 Created` response code and a [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5f82-295">例</span><span class="sxs-lookup"><span data-stu-id="c5f82-295">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5f82-296">要求</span><span class="sxs-lookup"><span data-stu-id="c5f82-296">Request</span></span>
<span data-ttu-id="c5f82-297">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c5f82-297">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1988

{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
  "contentCachingBlocked": true
}
```

### <a name="response"></a><span data-ttu-id="c5f82-298">応答</span><span class="sxs-lookup"><span data-stu-id="c5f82-298">Response</span></span>
<span data-ttu-id="c5f82-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c5f82-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2160

{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
  "id": "dc356aee-6aee-dc35-ee6a-35dcee6a35dc",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
  "contentCachingBlocked": true
}
```




