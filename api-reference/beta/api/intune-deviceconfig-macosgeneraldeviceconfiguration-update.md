---
title: macOSGeneralDeviceConfiguration の更新
description: macOSGeneralDeviceConfiguration オブジェクトのプロパティを更新します。
ms.openlocfilehash: aad4f0ed0c0b4d30842e2e643526c0d42ff4f1a3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071625"
---
# <a name="update-macosgeneraldeviceconfiguration"></a><span data-ttu-id="31ba8-103">macOSGeneralDeviceConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="31ba8-103">Update macOSGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="31ba8-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="31ba8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="31ba8-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="31ba8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="31ba8-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="31ba8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="31ba8-107">[macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="31ba8-107">Update the properties of a [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="31ba8-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="31ba8-108">Prerequisites</span></span>
<span data-ttu-id="31ba8-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="31ba8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31ba8-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="31ba8-111">Permission type</span></span>|<span data-ttu-id="31ba8-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="31ba8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31ba8-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="31ba8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="31ba8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31ba8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="31ba8-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="31ba8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31ba8-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="31ba8-116">Not supported.</span></span>|
|<span data-ttu-id="31ba8-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="31ba8-117">Application</span></span>|<span data-ttu-id="31ba8-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="31ba8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="31ba8-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="31ba8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="31ba8-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="31ba8-120">Request headers</span></span>
|<span data-ttu-id="31ba8-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="31ba8-121">Header</span></span>|<span data-ttu-id="31ba8-122">値</span><span class="sxs-lookup"><span data-stu-id="31ba8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="31ba8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="31ba8-123">Authorization</span></span>|<span data-ttu-id="31ba8-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="31ba8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="31ba8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="31ba8-125">Accept</span></span>|<span data-ttu-id="31ba8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="31ba8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31ba8-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="31ba8-127">Request body</span></span>
<span data-ttu-id="31ba8-128">要求本文で、[macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="31ba8-128">In the request body, supply a JSON representation for the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="31ba8-129">次の表に、[macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="31ba8-129">The following table shows the properties that are required when you create the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="31ba8-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="31ba8-130">Property</span></span>|<span data-ttu-id="31ba8-131">型</span><span class="sxs-lookup"><span data-stu-id="31ba8-131">Type</span></span>|<span data-ttu-id="31ba8-132">説明</span><span class="sxs-lookup"><span data-stu-id="31ba8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31ba8-133">id</span><span class="sxs-lookup"><span data-stu-id="31ba8-133">id</span></span>|<span data-ttu-id="31ba8-134">String</span><span class="sxs-lookup"><span data-stu-id="31ba8-134">String</span></span>|<span data-ttu-id="31ba8-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="31ba8-135">Key of the entity.</span></span> <span data-ttu-id="31ba8-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="31ba8-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31ba8-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="31ba8-137">lastModifiedDateTime</span></span>|<span data-ttu-id="31ba8-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31ba8-138">DateTimeOffset</span></span>|<span data-ttu-id="31ba8-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="31ba8-139">DateTime the object was last modified.</span></span> <span data-ttu-id="31ba8-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="31ba8-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31ba8-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="31ba8-141">roleScopeTagIds</span></span>|<span data-ttu-id="31ba8-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="31ba8-142">String collection</span></span>|<span data-ttu-id="31ba8-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="31ba8-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="31ba8-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="31ba8-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31ba8-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="31ba8-145">supportsScopeTags</span></span>|<span data-ttu-id="31ba8-146">ブール値</span><span class="sxs-lookup"><span data-stu-id="31ba8-146">Boolean</span></span>|<span data-ttu-id="31ba8-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="31ba8-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="31ba8-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="31ba8-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="31ba8-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="31ba8-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="31ba8-150">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="31ba8-150">This property is read-only.</span></span> <span data-ttu-id="31ba8-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="31ba8-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31ba8-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="31ba8-152">createdDateTime</span></span>|<span data-ttu-id="31ba8-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31ba8-153">DateTimeOffset</span></span>|<span data-ttu-id="31ba8-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="31ba8-154">DateTime the object was created.</span></span> <span data-ttu-id="31ba8-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="31ba8-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31ba8-156">説明</span><span class="sxs-lookup"><span data-stu-id="31ba8-156">description</span></span>|<span data-ttu-id="31ba8-157">String</span><span class="sxs-lookup"><span data-stu-id="31ba8-157">String</span></span>|<span data-ttu-id="31ba8-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="31ba8-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="31ba8-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="31ba8-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31ba8-160">displayName</span><span class="sxs-lookup"><span data-stu-id="31ba8-160">displayName</span></span>|<span data-ttu-id="31ba8-161">String</span><span class="sxs-lookup"><span data-stu-id="31ba8-161">String</span></span>|<span data-ttu-id="31ba8-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="31ba8-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="31ba8-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="31ba8-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31ba8-164">version</span><span class="sxs-lookup"><span data-stu-id="31ba8-164">version</span></span>|<span data-ttu-id="31ba8-165">Int32</span><span class="sxs-lookup"><span data-stu-id="31ba8-165">Int32</span></span>|<span data-ttu-id="31ba8-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="31ba8-166">Version of the device configuration.</span></span> <span data-ttu-id="31ba8-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="31ba8-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31ba8-168">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="31ba8-168">compliantAppsList</span></span>|<span data-ttu-id="31ba8-169">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="31ba8-169">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="31ba8-170">コンプライアンス内のアプリのリスト (CompliantAppListType によって制御される、許可リストまたは禁止リスト)。</span><span class="sxs-lookup"><span data-stu-id="31ba8-170">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="31ba8-171">このコレクションには、最大で 10000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="31ba8-171">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="31ba8-172">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="31ba8-172">compliantAppListType</span></span>|[<span data-ttu-id="31ba8-173">appListType</span><span class="sxs-lookup"><span data-stu-id="31ba8-173">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="31ba8-174">CompliantAppsList 内にあるリスト。</span><span class="sxs-lookup"><span data-stu-id="31ba8-174">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="31ba8-175">可能な値は、`none`、`appsInListCompliant`、`appsNotInListCompliant` です。</span><span class="sxs-lookup"><span data-stu-id="31ba8-175">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="31ba8-176">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="31ba8-176">emailInDomainSuffixes</span></span>|<span data-ttu-id="31ba8-177">String コレクション</span><span class="sxs-lookup"><span data-stu-id="31ba8-177">String collection</span></span>|<span data-ttu-id="31ba8-178">これらの文字列のいずれかに一致するサフィックスがないメール アドレスは、ドメイン外と見なされます。</span><span class="sxs-lookup"><span data-stu-id="31ba8-178">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="31ba8-179">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="31ba8-179">passwordBlockSimple</span></span>|<span data-ttu-id="31ba8-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="31ba8-180">Boolean</span></span>|<span data-ttu-id="31ba8-181">単純なパスワードを禁止します。</span><span class="sxs-lookup"><span data-stu-id="31ba8-181">Block simple passwords.</span></span>|
|<span data-ttu-id="31ba8-182">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="31ba8-182">passwordExpirationDays</span></span>|<span data-ttu-id="31ba8-183">Int32</span><span class="sxs-lookup"><span data-stu-id="31ba8-183">Int32</span></span>|<span data-ttu-id="31ba8-184">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="31ba8-184">Number of days before the password expires.</span></span>|
|<span data-ttu-id="31ba8-185">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="31ba8-185">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="31ba8-186">Int32</span><span class="sxs-lookup"><span data-stu-id="31ba8-186">Int32</span></span>|<span data-ttu-id="31ba8-187">パスワードが含まなければならない文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="31ba8-187">Number of character sets a password must contain.</span></span> <span data-ttu-id="31ba8-188">有効な値は 0 から 4 までです</span><span class="sxs-lookup"><span data-stu-id="31ba8-188">Valid values 0 to 4</span></span>|
|<span data-ttu-id="31ba8-189">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="31ba8-189">passwordMinimumLength</span></span>|<span data-ttu-id="31ba8-190">Int32</span><span class="sxs-lookup"><span data-stu-id="31ba8-190">Int32</span></span>|<span data-ttu-id="31ba8-191">パスワードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="31ba8-191">Minimum length of passwords.</span></span>|
|<span data-ttu-id="31ba8-192">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="31ba8-192">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="31ba8-193">Int32</span><span class="sxs-lookup"><span data-stu-id="31ba8-193">Int32</span></span>|<span data-ttu-id="31ba8-194">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="31ba8-194">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="31ba8-195">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="31ba8-195">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="31ba8-196">Int32</span><span class="sxs-lookup"><span data-stu-id="31ba8-196">Int32</span></span>|<span data-ttu-id="31ba8-197">画面がタイムアウトになるまでの非アクティブ時間。</span><span class="sxs-lookup"><span data-stu-id="31ba8-197">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="31ba8-198">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="31ba8-198">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="31ba8-199">Int32</span><span class="sxs-lookup"><span data-stu-id="31ba8-199">Int32</span></span>|<span data-ttu-id="31ba8-200">ブロックする、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="31ba8-200">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="31ba8-201">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="31ba8-201">passwordRequiredType</span></span>|[<span data-ttu-id="31ba8-202">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="31ba8-202">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="31ba8-203">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="31ba8-203">Type of password that is required.</span></span> <span data-ttu-id="31ba8-204">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="31ba8-204">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="31ba8-205">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="31ba8-205">passwordRequired</span></span>|<span data-ttu-id="31ba8-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="31ba8-206">Boolean</span></span>|<span data-ttu-id="31ba8-207">パスワードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="31ba8-207">Whether or not to require a password.</span></span>|
|<span data-ttu-id="31ba8-208">keychainBlockCloudSync</span><span class="sxs-lookup"><span data-stu-id="31ba8-208">keychainBlockCloudSync</span></span>|<span data-ttu-id="31ba8-209">ブール値</span><span class="sxs-lookup"><span data-stu-id="31ba8-209">Boolean</span></span>|<span data-ttu-id="31ba8-210">ICloud キーチェーンの同期がブロックされている (macOS 10.12 とそれ以降) であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="31ba8-210">Indicates whether or not iCloud keychain synchronization is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="31ba8-211">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="31ba8-211">airPrintBlocked</span></span>|<span data-ttu-id="31ba8-212">ブール値</span><span class="sxs-lookup"><span data-stu-id="31ba8-212">Boolean</span></span>|<span data-ttu-id="31ba8-213">AirPrint がブロックされている (macOS 10.12 とそれ以降) であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="31ba8-213">Indicates whether or not AirPrint is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="31ba8-214">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="31ba8-214">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="31ba8-215">ブール値</span><span class="sxs-lookup"><span data-stu-id="31ba8-215">Boolean</span></span>|<span data-ttu-id="31ba8-216">信頼された証明書が TLS 印刷通信 (macOS 10.13 とそれ以降) に必要なかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="31ba8-216">Indicates if trusted certificates are required for TLS printing communication (macOS 10.13 and later).</span></span>|
|<span data-ttu-id="31ba8-217">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="31ba8-217">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="31ba8-218">ブール値</span><span class="sxs-lookup"><span data-stu-id="31ba8-218">Boolean</span></span>|<span data-ttu-id="31ba8-219">AirPrint プリンターの検出を iBeacon がブロックされているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="31ba8-219">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="31ba8-220">これには、ネットワーク トラフィック (macOS 10.3 とそれ以降) のフィッシング詐欺からの見かけ上の AirPrint Bluetooth ビーコンができなくなります。</span><span class="sxs-lookup"><span data-stu-id="31ba8-220">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (macOS 10.3 and later).</span></span>|
|<span data-ttu-id="31ba8-221">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="31ba8-221">safariBlockAutofill</span></span>|<span data-ttu-id="31ba8-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="31ba8-222">Boolean</span></span>|<span data-ttu-id="31ba8-223">ユーザーによる Safari での自動入力の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="31ba8-223">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="31ba8-224">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="31ba8-224">cameraBlocked</span></span>|<span data-ttu-id="31ba8-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="31ba8-225">Boolean</span></span>|<span data-ttu-id="31ba8-226">ユーザーによるデバイスのカメラへのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="31ba8-226">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="31ba8-227">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="31ba8-227">iTunesBlockMusicService</span></span>|<span data-ttu-id="31ba8-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="31ba8-228">Boolean</span></span>|<span data-ttu-id="31ba8-229">音楽サービスをブロックし、クラシック モードへの音楽アプリケーションを元に戻すかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="31ba8-229">Indicates whether or not to block Music service and revert Music app to classic mode.</span></span>|
|<span data-ttu-id="31ba8-230">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="31ba8-230">spotlightBlockInternetResults</span></span>|<span data-ttu-id="31ba8-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="31ba8-231">Boolean</span></span>|<span data-ttu-id="31ba8-232">スポット ライトのインターネット検索からの結果を返すことを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="31ba8-232">Indicates whether or not to block Spotlight from returning any results from an Internet search.</span></span>|
|<span data-ttu-id="31ba8-233">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="31ba8-233">keyboardBlockDictation</span></span>|<span data-ttu-id="31ba8-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="31ba8-234">Boolean</span></span>|<span data-ttu-id="31ba8-235">ディクテーション モードの入力を使用してからユーザーをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="31ba8-235">Indicates whether or not to block the user from using dictation input.</span></span>|
|<span data-ttu-id="31ba8-236">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="31ba8-236">definitionLookupBlocked</span></span>|<span data-ttu-id="31ba8-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="31ba8-237">Boolean</span></span>|<span data-ttu-id="31ba8-238">定義の参照をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="31ba8-238">Indicates whether or not to block definition lookup.</span></span>|
|<span data-ttu-id="31ba8-239">appleWatchBlockAutoUnlock</span><span class="sxs-lookup"><span data-stu-id="31ba8-239">appleWatchBlockAutoUnlock</span></span>|<span data-ttu-id="31ba8-240">ブール値</span><span class="sxs-lookup"><span data-stu-id="31ba8-240">Boolean</span></span>|<span data-ttu-id="31ba8-241">Apple Watch で、Mac のロックを解除することをユーザーに禁止するかを示します。</span><span class="sxs-lookup"><span data-stu-id="31ba8-241">Indicates whether or to block users from unlocking their Mac with Apple Watch.</span></span>|
|<span data-ttu-id="31ba8-242">iTunesBlockFileSharing</span><span class="sxs-lookup"><span data-stu-id="31ba8-242">iTunesBlockFileSharing</span></span>|<span data-ttu-id="31ba8-243">ブール値</span><span class="sxs-lookup"><span data-stu-id="31ba8-243">Boolean</span></span>|<span data-ttu-id="31ba8-244">かどうかの中からファイルをブロックするのには転送 iTunes を使用することを示します。</span><span class="sxs-lookup"><span data-stu-id="31ba8-244">Indicates whether or not to block files from being transferred using iTunes.</span></span>|
|<span data-ttu-id="31ba8-245">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="31ba8-245">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="31ba8-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="31ba8-246">Boolean</span></span>|<span data-ttu-id="31ba8-247">iCloud のドキュメントの同期を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="31ba8-247">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="31ba8-248">iCloudBlockMail</span><span class="sxs-lookup"><span data-stu-id="31ba8-248">iCloudBlockMail</span></span>|<span data-ttu-id="31ba8-249">ブール値</span><span class="sxs-lookup"><span data-stu-id="31ba8-249">Boolean</span></span>|<span data-ttu-id="31ba8-250">ICloud とのメールの同期をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="31ba8-250">Indicates whether or not to block iCloud from syncing mail.</span></span>|
|<span data-ttu-id="31ba8-251">iCloudBlockAddressBook</span><span class="sxs-lookup"><span data-stu-id="31ba8-251">iCloudBlockAddressBook</span></span>|<span data-ttu-id="31ba8-252">ブール値</span><span class="sxs-lookup"><span data-stu-id="31ba8-252">Boolean</span></span>|<span data-ttu-id="31ba8-253">ICloud との連絡先の同期をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="31ba8-253">Indicates whether or not to block iCloud from syncing contacts.</span></span>|
|<span data-ttu-id="31ba8-254">iCloudBlockCalendar</span><span class="sxs-lookup"><span data-stu-id="31ba8-254">iCloudBlockCalendar</span></span>|<span data-ttu-id="31ba8-255">ブール値</span><span class="sxs-lookup"><span data-stu-id="31ba8-255">Boolean</span></span>|<span data-ttu-id="31ba8-256">ICloud との予定表の同期をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="31ba8-256">Indicates whether or not to block iCloud from syncing calendars.</span></span>|
|<span data-ttu-id="31ba8-257">iCloudBlockReminders</span><span class="sxs-lookup"><span data-stu-id="31ba8-257">iCloudBlockReminders</span></span>|<span data-ttu-id="31ba8-258">ブール値</span><span class="sxs-lookup"><span data-stu-id="31ba8-258">Boolean</span></span>|<span data-ttu-id="31ba8-259">ICloud との同期の通知をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="31ba8-259">Indicates whether or not to block iCloud from syncing reminders.</span></span>|
|<span data-ttu-id="31ba8-260">iCloudBlockBookmarks</span><span class="sxs-lookup"><span data-stu-id="31ba8-260">iCloudBlockBookmarks</span></span>|<span data-ttu-id="31ba8-261">ブール値</span><span class="sxs-lookup"><span data-stu-id="31ba8-261">Boolean</span></span>|<span data-ttu-id="31ba8-262">ICloud からのブックマークの同期をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="31ba8-262">Indicates whether or not to block iCloud from syncing bookmarks.</span></span>|
|<span data-ttu-id="31ba8-263">iCloudBlockNotes</span><span class="sxs-lookup"><span data-stu-id="31ba8-263">iCloudBlockNotes</span></span>|<span data-ttu-id="31ba8-264">ブール値</span><span class="sxs-lookup"><span data-stu-id="31ba8-264">Boolean</span></span>|<span data-ttu-id="31ba8-265">ICloud からメモの同期をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="31ba8-265">Indicates whether or not to block iCloud from syncing notes.</span></span>|
|<span data-ttu-id="31ba8-266">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="31ba8-266">airDropBlocked</span></span>|<span data-ttu-id="31ba8-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="31ba8-267">Boolean</span></span>|<span data-ttu-id="31ba8-268">AirDrop を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="31ba8-268">Indicates whether or not to allow AirDrop.</span></span>|
|<span data-ttu-id="31ba8-269">passwordBlockModification</span><span class="sxs-lookup"><span data-stu-id="31ba8-269">passwordBlockModification</span></span>|<span data-ttu-id="31ba8-270">ブール値</span><span class="sxs-lookup"><span data-stu-id="31ba8-270">Boolean</span></span>|<span data-ttu-id="31ba8-271">パスコードの変更を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="31ba8-271">Indicates whether or not to allow passcode modification.</span></span>|
|<span data-ttu-id="31ba8-272">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="31ba8-272">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="31ba8-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="31ba8-273">Boolean</span></span>|<span data-ttu-id="31ba8-274">指紋によるロック解除を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="31ba8-274">Indicates whether or not to block fingerprint unlock.</span></span>|



## <a name="response"></a><span data-ttu-id="31ba8-275">応答</span><span class="sxs-lookup"><span data-stu-id="31ba8-275">Response</span></span>
<span data-ttu-id="31ba8-276">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="31ba8-276">If successful, this method returns a `200 OK` response code and an updated [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31ba8-277">例</span><span class="sxs-lookup"><span data-stu-id="31ba8-277">Example</span></span>
### <a name="request"></a><span data-ttu-id="31ba8-278">要求</span><span class="sxs-lookup"><span data-stu-id="31ba8-278">Request</span></span>
<span data-ttu-id="31ba8-279">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="31ba8-279">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1747

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
  "passwordBlockFingerprintUnlock": true
}
```

### <a name="response"></a><span data-ttu-id="31ba8-280">応答</span><span class="sxs-lookup"><span data-stu-id="31ba8-280">Response</span></span>
<span data-ttu-id="31ba8-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="31ba8-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1925

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
  "passwordBlockFingerprintUnlock": true
}
```





