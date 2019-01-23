---
title: macOSGeneralDeviceConfiguration の更新
description: macOSGeneralDeviceConfiguration オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: dab8bbb23b2237be19556fc28bfb4cda2d466f4c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407565"
---
# <a name="update-macosgeneraldeviceconfiguration"></a><span data-ttu-id="f41b5-103">macOSGeneralDeviceConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="f41b5-103">Update macOSGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="f41b5-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f41b5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f41b5-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f41b5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f41b5-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f41b5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f41b5-107">[macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f41b5-107">Update the properties of a [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f41b5-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="f41b5-108">Prerequisites</span></span>
<span data-ttu-id="f41b5-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f41b5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f41b5-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f41b5-111">Permission type</span></span>|<span data-ttu-id="f41b5-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f41b5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f41b5-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f41b5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f41b5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f41b5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f41b5-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f41b5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f41b5-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f41b5-116">Not supported.</span></span>|
|<span data-ttu-id="f41b5-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f41b5-117">Application</span></span>|<span data-ttu-id="f41b5-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f41b5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f41b5-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f41b5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f41b5-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f41b5-120">Request headers</span></span>
|<span data-ttu-id="f41b5-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f41b5-121">Header</span></span>|<span data-ttu-id="f41b5-122">値</span><span class="sxs-lookup"><span data-stu-id="f41b5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f41b5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f41b5-123">Authorization</span></span>|<span data-ttu-id="f41b5-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="f41b5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f41b5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f41b5-125">Accept</span></span>|<span data-ttu-id="f41b5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f41b5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f41b5-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="f41b5-127">Request body</span></span>
<span data-ttu-id="f41b5-128">要求本文で、[macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f41b5-128">In the request body, supply a JSON representation for the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="f41b5-129">次の表に、[macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f41b5-129">The following table shows the properties that are required when you create the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="f41b5-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f41b5-130">Property</span></span>|<span data-ttu-id="f41b5-131">型</span><span class="sxs-lookup"><span data-stu-id="f41b5-131">Type</span></span>|<span data-ttu-id="f41b5-132">説明</span><span class="sxs-lookup"><span data-stu-id="f41b5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f41b5-133">id</span><span class="sxs-lookup"><span data-stu-id="f41b5-133">id</span></span>|<span data-ttu-id="f41b5-134">String</span><span class="sxs-lookup"><span data-stu-id="f41b5-134">String</span></span>|<span data-ttu-id="f41b5-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f41b5-135">Key of the entity.</span></span> <span data-ttu-id="f41b5-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f41b5-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f41b5-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f41b5-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f41b5-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f41b5-138">DateTimeOffset</span></span>|<span data-ttu-id="f41b5-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="f41b5-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f41b5-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f41b5-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f41b5-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f41b5-141">roleScopeTagIds</span></span>|<span data-ttu-id="f41b5-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="f41b5-142">String collection</span></span>|<span data-ttu-id="f41b5-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="f41b5-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f41b5-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f41b5-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f41b5-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f41b5-145">supportsScopeTags</span></span>|<span data-ttu-id="f41b5-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="f41b5-146">Boolean</span></span>|<span data-ttu-id="f41b5-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f41b5-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f41b5-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="f41b5-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f41b5-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="f41b5-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f41b5-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="f41b5-150">This property is read-only.</span></span> <span data-ttu-id="f41b5-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f41b5-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f41b5-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f41b5-152">createdDateTime</span></span>|<span data-ttu-id="f41b5-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f41b5-153">DateTimeOffset</span></span>|<span data-ttu-id="f41b5-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="f41b5-154">DateTime the object was created.</span></span> <span data-ttu-id="f41b5-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f41b5-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f41b5-156">説明</span><span class="sxs-lookup"><span data-stu-id="f41b5-156">description</span></span>|<span data-ttu-id="f41b5-157">String</span><span class="sxs-lookup"><span data-stu-id="f41b5-157">String</span></span>|<span data-ttu-id="f41b5-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="f41b5-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f41b5-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f41b5-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f41b5-160">displayName</span><span class="sxs-lookup"><span data-stu-id="f41b5-160">displayName</span></span>|<span data-ttu-id="f41b5-161">String</span><span class="sxs-lookup"><span data-stu-id="f41b5-161">String</span></span>|<span data-ttu-id="f41b5-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="f41b5-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f41b5-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f41b5-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f41b5-164">version</span><span class="sxs-lookup"><span data-stu-id="f41b5-164">version</span></span>|<span data-ttu-id="f41b5-165">Int32</span><span class="sxs-lookup"><span data-stu-id="f41b5-165">Int32</span></span>|<span data-ttu-id="f41b5-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="f41b5-166">Version of the device configuration.</span></span> <span data-ttu-id="f41b5-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f41b5-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f41b5-168">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="f41b5-168">compliantAppsList</span></span>|<span data-ttu-id="f41b5-169">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f41b5-169">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="f41b5-170">コンプライアンス内のアプリのリスト (CompliantAppListType によって制御される、許可リストまたは禁止リスト)。</span><span class="sxs-lookup"><span data-stu-id="f41b5-170">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="f41b5-171">このコレクションには、最大で 10000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="f41b5-171">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="f41b5-172">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="f41b5-172">compliantAppListType</span></span>|[<span data-ttu-id="f41b5-173">appListType</span><span class="sxs-lookup"><span data-stu-id="f41b5-173">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="f41b5-174">CompliantAppsList 内にあるリスト。</span><span class="sxs-lookup"><span data-stu-id="f41b5-174">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="f41b5-175">可能な値は、`none`、`appsInListCompliant`、`appsNotInListCompliant` です。</span><span class="sxs-lookup"><span data-stu-id="f41b5-175">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="f41b5-176">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="f41b5-176">emailInDomainSuffixes</span></span>|<span data-ttu-id="f41b5-177">String コレクション</span><span class="sxs-lookup"><span data-stu-id="f41b5-177">String collection</span></span>|<span data-ttu-id="f41b5-178">これらの文字列のいずれかに一致するサフィックスがないメール アドレスは、ドメイン外と見なされます。</span><span class="sxs-lookup"><span data-stu-id="f41b5-178">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="f41b5-179">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="f41b5-179">passwordBlockSimple</span></span>|<span data-ttu-id="f41b5-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="f41b5-180">Boolean</span></span>|<span data-ttu-id="f41b5-181">単純なパスワードを禁止します。</span><span class="sxs-lookup"><span data-stu-id="f41b5-181">Block simple passwords.</span></span>|
|<span data-ttu-id="f41b5-182">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="f41b5-182">passwordExpirationDays</span></span>|<span data-ttu-id="f41b5-183">Int32</span><span class="sxs-lookup"><span data-stu-id="f41b5-183">Int32</span></span>|<span data-ttu-id="f41b5-184">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="f41b5-184">Number of days before the password expires.</span></span>|
|<span data-ttu-id="f41b5-185">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="f41b5-185">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="f41b5-186">Int32</span><span class="sxs-lookup"><span data-stu-id="f41b5-186">Int32</span></span>|<span data-ttu-id="f41b5-187">パスワードが含まなければならない文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="f41b5-187">Number of character sets a password must contain.</span></span> <span data-ttu-id="f41b5-188">有効な値は 0 から 4 までです</span><span class="sxs-lookup"><span data-stu-id="f41b5-188">Valid values 0 to 4</span></span>|
|<span data-ttu-id="f41b5-189">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="f41b5-189">passwordMinimumLength</span></span>|<span data-ttu-id="f41b5-190">Int32</span><span class="sxs-lookup"><span data-stu-id="f41b5-190">Int32</span></span>|<span data-ttu-id="f41b5-191">パスワードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="f41b5-191">Minimum length of passwords.</span></span>|
|<span data-ttu-id="f41b5-192">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="f41b5-192">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="f41b5-193">Int32</span><span class="sxs-lookup"><span data-stu-id="f41b5-193">Int32</span></span>|<span data-ttu-id="f41b5-194">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="f41b5-194">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="f41b5-195">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="f41b5-195">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="f41b5-196">Int32</span><span class="sxs-lookup"><span data-stu-id="f41b5-196">Int32</span></span>|<span data-ttu-id="f41b5-197">画面がタイムアウトになるまでの非アクティブ時間。</span><span class="sxs-lookup"><span data-stu-id="f41b5-197">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="f41b5-198">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="f41b5-198">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="f41b5-199">Int32</span><span class="sxs-lookup"><span data-stu-id="f41b5-199">Int32</span></span>|<span data-ttu-id="f41b5-200">ブロックする、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="f41b5-200">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="f41b5-201">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="f41b5-201">passwordRequiredType</span></span>|[<span data-ttu-id="f41b5-202">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="f41b5-202">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="f41b5-203">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="f41b5-203">Type of password that is required.</span></span> <span data-ttu-id="f41b5-204">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="f41b5-204">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="f41b5-205">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="f41b5-205">passwordRequired</span></span>|<span data-ttu-id="f41b5-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="f41b5-206">Boolean</span></span>|<span data-ttu-id="f41b5-207">パスワードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="f41b5-207">Whether or not to require a password.</span></span>|
|<span data-ttu-id="f41b5-208">keychainBlockCloudSync</span><span class="sxs-lookup"><span data-stu-id="f41b5-208">keychainBlockCloudSync</span></span>|<span data-ttu-id="f41b5-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="f41b5-209">Boolean</span></span>|<span data-ttu-id="f41b5-210">ICloud キーチェーンの同期がブロックされている (macOS 10.12 とそれ以降) であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f41b5-210">Indicates whether or not iCloud keychain synchronization is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="f41b5-211">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="f41b5-211">airPrintBlocked</span></span>|<span data-ttu-id="f41b5-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="f41b5-212">Boolean</span></span>|<span data-ttu-id="f41b5-213">AirPrint がブロックされている (macOS 10.12 とそれ以降) であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f41b5-213">Indicates whether or not AirPrint is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="f41b5-214">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="f41b5-214">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="f41b5-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="f41b5-215">Boolean</span></span>|<span data-ttu-id="f41b5-216">信頼された証明書が TLS 印刷通信 (macOS 10.13 とそれ以降) に必要なかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f41b5-216">Indicates if trusted certificates are required for TLS printing communication (macOS 10.13 and later).</span></span>|
|<span data-ttu-id="f41b5-217">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="f41b5-217">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="f41b5-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="f41b5-218">Boolean</span></span>|<span data-ttu-id="f41b5-219">AirPrint プリンターの検出を iBeacon がブロックされているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f41b5-219">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="f41b5-220">これには、ネットワーク トラフィック (macOS 10.3 とそれ以降) のフィッシング詐欺からの見かけ上の AirPrint Bluetooth ビーコンができなくなります。</span><span class="sxs-lookup"><span data-stu-id="f41b5-220">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (macOS 10.3 and later).</span></span>|
|<span data-ttu-id="f41b5-221">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="f41b5-221">safariBlockAutofill</span></span>|<span data-ttu-id="f41b5-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="f41b5-222">Boolean</span></span>|<span data-ttu-id="f41b5-223">ユーザーによる Safari での自動入力の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f41b5-223">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="f41b5-224">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="f41b5-224">cameraBlocked</span></span>|<span data-ttu-id="f41b5-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="f41b5-225">Boolean</span></span>|<span data-ttu-id="f41b5-226">ユーザーによるデバイスのカメラへのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f41b5-226">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="f41b5-227">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="f41b5-227">iTunesBlockMusicService</span></span>|<span data-ttu-id="f41b5-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="f41b5-228">Boolean</span></span>|<span data-ttu-id="f41b5-229">音楽サービスをブロックし、クラシック モードへの音楽アプリケーションを元に戻すかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f41b5-229">Indicates whether or not to block Music service and revert Music app to classic mode.</span></span>|
|<span data-ttu-id="f41b5-230">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="f41b5-230">spotlightBlockInternetResults</span></span>|<span data-ttu-id="f41b5-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="f41b5-231">Boolean</span></span>|<span data-ttu-id="f41b5-232">スポット ライトのインターネット検索からの結果を返すことを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f41b5-232">Indicates whether or not to block Spotlight from returning any results from an Internet search.</span></span>|
|<span data-ttu-id="f41b5-233">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="f41b5-233">keyboardBlockDictation</span></span>|<span data-ttu-id="f41b5-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="f41b5-234">Boolean</span></span>|<span data-ttu-id="f41b5-235">ディクテーション モードの入力を使用してからユーザーをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f41b5-235">Indicates whether or not to block the user from using dictation input.</span></span>|
|<span data-ttu-id="f41b5-236">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="f41b5-236">definitionLookupBlocked</span></span>|<span data-ttu-id="f41b5-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="f41b5-237">Boolean</span></span>|<span data-ttu-id="f41b5-238">定義の参照をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f41b5-238">Indicates whether or not to block definition lookup.</span></span>|
|<span data-ttu-id="f41b5-239">appleWatchBlockAutoUnlock</span><span class="sxs-lookup"><span data-stu-id="f41b5-239">appleWatchBlockAutoUnlock</span></span>|<span data-ttu-id="f41b5-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="f41b5-240">Boolean</span></span>|<span data-ttu-id="f41b5-241">Apple Watch で、Mac のロックを解除することをユーザーに禁止するかを示します。</span><span class="sxs-lookup"><span data-stu-id="f41b5-241">Indicates whether or to block users from unlocking their Mac with Apple Watch.</span></span>|
|<span data-ttu-id="f41b5-242">iTunesBlockFileSharing</span><span class="sxs-lookup"><span data-stu-id="f41b5-242">iTunesBlockFileSharing</span></span>|<span data-ttu-id="f41b5-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="f41b5-243">Boolean</span></span>|<span data-ttu-id="f41b5-244">かどうかの中からファイルをブロックするのには転送 iTunes を使用することを示します。</span><span class="sxs-lookup"><span data-stu-id="f41b5-244">Indicates whether or not to block files from being transferred using iTunes.</span></span>|
|<span data-ttu-id="f41b5-245">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="f41b5-245">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="f41b5-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="f41b5-246">Boolean</span></span>|<span data-ttu-id="f41b5-247">iCloud のドキュメントの同期を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f41b5-247">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="f41b5-248">iCloudBlockMail</span><span class="sxs-lookup"><span data-stu-id="f41b5-248">iCloudBlockMail</span></span>|<span data-ttu-id="f41b5-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="f41b5-249">Boolean</span></span>|<span data-ttu-id="f41b5-250">ICloud とのメールの同期をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f41b5-250">Indicates whether or not to block iCloud from syncing mail.</span></span>|
|<span data-ttu-id="f41b5-251">iCloudBlockAddressBook</span><span class="sxs-lookup"><span data-stu-id="f41b5-251">iCloudBlockAddressBook</span></span>|<span data-ttu-id="f41b5-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="f41b5-252">Boolean</span></span>|<span data-ttu-id="f41b5-253">ICloud との連絡先の同期をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f41b5-253">Indicates whether or not to block iCloud from syncing contacts.</span></span>|
|<span data-ttu-id="f41b5-254">iCloudBlockCalendar</span><span class="sxs-lookup"><span data-stu-id="f41b5-254">iCloudBlockCalendar</span></span>|<span data-ttu-id="f41b5-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="f41b5-255">Boolean</span></span>|<span data-ttu-id="f41b5-256">ICloud との予定表の同期をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f41b5-256">Indicates whether or not to block iCloud from syncing calendars.</span></span>|
|<span data-ttu-id="f41b5-257">iCloudBlockReminders</span><span class="sxs-lookup"><span data-stu-id="f41b5-257">iCloudBlockReminders</span></span>|<span data-ttu-id="f41b5-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="f41b5-258">Boolean</span></span>|<span data-ttu-id="f41b5-259">ICloud との同期の通知をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f41b5-259">Indicates whether or not to block iCloud from syncing reminders.</span></span>|
|<span data-ttu-id="f41b5-260">iCloudBlockBookmarks</span><span class="sxs-lookup"><span data-stu-id="f41b5-260">iCloudBlockBookmarks</span></span>|<span data-ttu-id="f41b5-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="f41b5-261">Boolean</span></span>|<span data-ttu-id="f41b5-262">ICloud からのブックマークの同期をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f41b5-262">Indicates whether or not to block iCloud from syncing bookmarks.</span></span>|
|<span data-ttu-id="f41b5-263">iCloudBlockNotes</span><span class="sxs-lookup"><span data-stu-id="f41b5-263">iCloudBlockNotes</span></span>|<span data-ttu-id="f41b5-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="f41b5-264">Boolean</span></span>|<span data-ttu-id="f41b5-265">ICloud からメモの同期をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f41b5-265">Indicates whether or not to block iCloud from syncing notes.</span></span>|
|<span data-ttu-id="f41b5-266">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="f41b5-266">airDropBlocked</span></span>|<span data-ttu-id="f41b5-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="f41b5-267">Boolean</span></span>|<span data-ttu-id="f41b5-268">AirDrop を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f41b5-268">Indicates whether or not to allow AirDrop.</span></span>|
|<span data-ttu-id="f41b5-269">passwordBlockModification</span><span class="sxs-lookup"><span data-stu-id="f41b5-269">passwordBlockModification</span></span>|<span data-ttu-id="f41b5-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="f41b5-270">Boolean</span></span>|<span data-ttu-id="f41b5-271">パスコードの変更を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f41b5-271">Indicates whether or not to allow passcode modification.</span></span>|
|<span data-ttu-id="f41b5-272">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="f41b5-272">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="f41b5-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="f41b5-273">Boolean</span></span>|<span data-ttu-id="f41b5-274">指紋によるロック解除を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f41b5-274">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="f41b5-275">passwordBlockAutoFill</span><span class="sxs-lookup"><span data-stu-id="f41b5-275">passwordBlockAutoFill</span></span>|<span data-ttu-id="f41b5-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="f41b5-276">Boolean</span></span>|<span data-ttu-id="f41b5-277">オートフィルのパスワード機能をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f41b5-277">Indicates whether or not to block the AutoFill Passwords feature.</span></span>|
|<span data-ttu-id="f41b5-278">passwordBlockProximityRequests</span><span class="sxs-lookup"><span data-stu-id="f41b5-278">passwordBlockProximityRequests</span></span>|<span data-ttu-id="f41b5-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="f41b5-279">Boolean</span></span>|<span data-ttu-id="f41b5-280">近くにあるデバイスからパスワードを要求をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f41b5-280">Indicates whether or not to block requesting passwords from nearby devices.</span></span>|
|<span data-ttu-id="f41b5-281">passwordBlockAirDropSharing</span><span class="sxs-lookup"><span data-stu-id="f41b5-281">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="f41b5-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="f41b5-282">Boolean</span></span>|<span data-ttu-id="f41b5-283">AirDrop のパスワード機能を使用して共有のパスワードをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f41b5-283">Indicates whether or not to block sharing passwords with the AirDrop passwords feature.</span></span>|



## <a name="response"></a><span data-ttu-id="f41b5-284">応答</span><span class="sxs-lookup"><span data-stu-id="f41b5-284">Response</span></span>
<span data-ttu-id="f41b5-285">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="f41b5-285">If successful, this method returns a `200 OK` response code and an updated [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f41b5-286">例</span><span class="sxs-lookup"><span data-stu-id="f41b5-286">Example</span></span>

### <a name="request"></a><span data-ttu-id="f41b5-287">要求</span><span class="sxs-lookup"><span data-stu-id="f41b5-287">Request</span></span>
<span data-ttu-id="f41b5-288">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f41b5-288">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1870

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
  "passwordBlockAirDropSharing": true
}
```

### <a name="response"></a><span data-ttu-id="f41b5-289">応答</span><span class="sxs-lookup"><span data-stu-id="f41b5-289">Response</span></span>
<span data-ttu-id="f41b5-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f41b5-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2042

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
  "passwordBlockAirDropSharing": true
}
```




