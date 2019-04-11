---
title: androidDeviceOwnerCompliancePolicy の更新
description: androidDeviceOwnerCompliancePolicy オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5f75c206698bbc5f47e3e43abf722ed8f648645e
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31809291"
---
# <a name="update-androiddeviceownercompliancepolicy"></a><span data-ttu-id="7b14c-103">androidDeviceOwnerCompliancePolicy の更新</span><span class="sxs-lookup"><span data-stu-id="7b14c-103">Update androidDeviceOwnerCompliancePolicy</span></span>

> <span data-ttu-id="7b14c-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7b14c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7b14c-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7b14c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b14c-106">[androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7b14c-106">Update the properties of a [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7b14c-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="7b14c-107">Prerequisites</span></span>
<span data-ttu-id="7b14c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7b14c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b14c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7b14c-110">Permission type</span></span>|<span data-ttu-id="7b14c-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7b14c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b14c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7b14c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7b14c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b14c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7b14c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7b14c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b14c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7b14c-115">Not supported.</span></span>|
|<span data-ttu-id="7b14c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7b14c-116">Application</span></span>|<span data-ttu-id="7b14c-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7b14c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b14c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7b14c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="7b14c-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7b14c-119">Request headers</span></span>
|<span data-ttu-id="7b14c-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7b14c-120">Header</span></span>|<span data-ttu-id="7b14c-121">値</span><span class="sxs-lookup"><span data-stu-id="7b14c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7b14c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b14c-122">Authorization</span></span>|<span data-ttu-id="7b14c-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="7b14c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7b14c-124">承諾</span><span class="sxs-lookup"><span data-stu-id="7b14c-124">Accept</span></span>|<span data-ttu-id="7b14c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7b14c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b14c-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="7b14c-126">Request body</span></span>
<span data-ttu-id="7b14c-127">要求本文で、 [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7b14c-127">In the request body, supply a JSON representation for the [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object.</span></span>

<span data-ttu-id="7b14c-128">次の表に、 [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7b14c-128">The following table shows the properties that are required when you create the [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md).</span></span>

|<span data-ttu-id="7b14c-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7b14c-129">Property</span></span>|<span data-ttu-id="7b14c-130">型</span><span class="sxs-lookup"><span data-stu-id="7b14c-130">Type</span></span>|<span data-ttu-id="7b14c-131">説明</span><span class="sxs-lookup"><span data-stu-id="7b14c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b14c-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7b14c-132">roleScopeTagIds</span></span>|<span data-ttu-id="7b14c-133">String コレクション</span><span class="sxs-lookup"><span data-stu-id="7b14c-133">String collection</span></span>|<span data-ttu-id="7b14c-134">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="7b14c-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7b14c-135">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7b14c-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7b14c-136">id</span><span class="sxs-lookup"><span data-stu-id="7b14c-136">id</span></span>|<span data-ttu-id="7b14c-137">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="7b14c-137">String</span></span>|<span data-ttu-id="7b14c-138">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7b14c-138">Key of the entity.</span></span> <span data-ttu-id="7b14c-139">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7b14c-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7b14c-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7b14c-140">createdDateTime</span></span>|<span data-ttu-id="7b14c-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b14c-141">DateTimeOffset</span></span>|<span data-ttu-id="7b14c-142">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="7b14c-142">DateTime the object was created.</span></span> <span data-ttu-id="7b14c-143">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7b14c-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7b14c-144">説明</span><span class="sxs-lookup"><span data-stu-id="7b14c-144">description</span></span>|<span data-ttu-id="7b14c-145">String</span><span class="sxs-lookup"><span data-stu-id="7b14c-145">String</span></span>|<span data-ttu-id="7b14c-146">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="7b14c-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7b14c-147">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7b14c-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7b14c-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7b14c-148">lastModifiedDateTime</span></span>|<span data-ttu-id="7b14c-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b14c-149">DateTimeOffset</span></span>|<span data-ttu-id="7b14c-150">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="7b14c-150">DateTime the object was last modified.</span></span> <span data-ttu-id="7b14c-151">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7b14c-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7b14c-152">displayName</span><span class="sxs-lookup"><span data-stu-id="7b14c-152">displayName</span></span>|<span data-ttu-id="7b14c-153">String</span><span class="sxs-lookup"><span data-stu-id="7b14c-153">String</span></span>|<span data-ttu-id="7b14c-154">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="7b14c-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7b14c-155">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7b14c-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7b14c-156">version</span><span class="sxs-lookup"><span data-stu-id="7b14c-156">version</span></span>|<span data-ttu-id="7b14c-157">Int32</span><span class="sxs-lookup"><span data-stu-id="7b14c-157">Int32</span></span>|<span data-ttu-id="7b14c-158">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="7b14c-158">Version of the device configuration.</span></span> <span data-ttu-id="7b14c-159">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7b14c-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7b14c-160">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="7b14c-160">osMinimumVersion</span></span>|<span data-ttu-id="7b14c-161">文字列</span><span class="sxs-lookup"><span data-stu-id="7b14c-161">String</span></span>|<span data-ttu-id="7b14c-162">Android の最小バージョン。</span><span class="sxs-lookup"><span data-stu-id="7b14c-162">Minimum Android version.</span></span>|
|<span data-ttu-id="7b14c-163">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="7b14c-163">osMaximumVersion</span></span>|<span data-ttu-id="7b14c-164">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="7b14c-164">String</span></span>|<span data-ttu-id="7b14c-165">Android の最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="7b14c-165">Maximum Android version.</span></span>|
|<span data-ttu-id="7b14c-166">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="7b14c-166">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="7b14c-167">String</span><span class="sxs-lookup"><span data-stu-id="7b14c-167">String</span></span>|<span data-ttu-id="7b14c-168">Android セキュリティ パッチの最小レベル。</span><span class="sxs-lookup"><span data-stu-id="7b14c-168">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="7b14c-169">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="7b14c-169">passwordRequired</span></span>|<span data-ttu-id="7b14c-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b14c-170">Boolean</span></span>|<span data-ttu-id="7b14c-171">デバイスのロックを解除するパスワードを要求します。</span><span class="sxs-lookup"><span data-stu-id="7b14c-171">Require a password to unlock device.</span></span>|
|<span data-ttu-id="7b14c-172">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="7b14c-172">passwordMinimumLength</span></span>|<span data-ttu-id="7b14c-173">Int32</span><span class="sxs-lookup"><span data-stu-id="7b14c-173">Int32</span></span>|<span data-ttu-id="7b14c-174">パスワードの最小文字数。</span><span class="sxs-lookup"><span data-stu-id="7b14c-174">Minimum password length.</span></span> <span data-ttu-id="7b14c-175">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="7b14c-175">Valid values 4 to 16</span></span>|
|<span data-ttu-id="7b14c-176">passwordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="7b14c-176">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="7b14c-177">Int32</span><span class="sxs-lookup"><span data-stu-id="7b14c-177">Int32</span></span>|<span data-ttu-id="7b14c-178">デバイスパスワードに必要な文字の最小数を示します。</span><span class="sxs-lookup"><span data-stu-id="7b14c-178">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="7b14c-179">有効な値は1から16までです</span><span class="sxs-lookup"><span data-stu-id="7b14c-179">Valid values 1 to 16</span></span>|
|<span data-ttu-id="7b14c-180">passwordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="7b14c-180">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="7b14c-181">Int32</span><span class="sxs-lookup"><span data-stu-id="7b14c-181">Int32</span></span>|<span data-ttu-id="7b14c-182">デバイスパスワードに必要な小文字の最小文字数を示します。</span><span class="sxs-lookup"><span data-stu-id="7b14c-182">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="7b14c-183">有効な値は1から16までです</span><span class="sxs-lookup"><span data-stu-id="7b14c-183">Valid values 1 to 16</span></span>|
|<span data-ttu-id="7b14c-184">passwordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="7b14c-184">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="7b14c-185">Int32</span><span class="sxs-lookup"><span data-stu-id="7b14c-185">Int32</span></span>|<span data-ttu-id="7b14c-186">デバイスパスワードに必要な文字以外の文字の最小数を示します。</span><span class="sxs-lookup"><span data-stu-id="7b14c-186">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="7b14c-187">有効な値は1から16までです</span><span class="sxs-lookup"><span data-stu-id="7b14c-187">Valid values 1 to 16</span></span>|
|<span data-ttu-id="7b14c-188">passwordminimumnumericcharacters</span><span class="sxs-lookup"><span data-stu-id="7b14c-188">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="7b14c-189">Int32</span><span class="sxs-lookup"><span data-stu-id="7b14c-189">Int32</span></span>|<span data-ttu-id="7b14c-190">デバイスパスワードに必要な最小文字数を示します。</span><span class="sxs-lookup"><span data-stu-id="7b14c-190">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="7b14c-191">有効な値は1から16までです</span><span class="sxs-lookup"><span data-stu-id="7b14c-191">Valid values 1 to 16</span></span>|
|<span data-ttu-id="7b14c-192">passwordminimumシンボル文字</span><span class="sxs-lookup"><span data-stu-id="7b14c-192">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="7b14c-193">Int32</span><span class="sxs-lookup"><span data-stu-id="7b14c-193">Int32</span></span>|<span data-ttu-id="7b14c-194">デバイスパスワードに必要な最小記号文字数を示します。</span><span class="sxs-lookup"><span data-stu-id="7b14c-194">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="7b14c-195">有効な値は1から16までです</span><span class="sxs-lookup"><span data-stu-id="7b14c-195">Valid values 1 to 16</span></span>|
|<span data-ttu-id="7b14c-196">passwordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="7b14c-196">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="7b14c-197">Int32</span><span class="sxs-lookup"><span data-stu-id="7b14c-197">Int32</span></span>|<span data-ttu-id="7b14c-198">デバイスのパスワードに必要な大文字の文字の最小文字数を示します。</span><span class="sxs-lookup"><span data-stu-id="7b14c-198">Indicates the minimum number of upper case letter characters required for device password.</span></span> <span data-ttu-id="7b14c-199">有効な値は1から16までです</span><span class="sxs-lookup"><span data-stu-id="7b14c-199">Valid values 1 to 16</span></span>|
|<span data-ttu-id="7b14c-200">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="7b14c-200">passwordRequiredType</span></span>|[<span data-ttu-id="7b14c-201">androiddeviceownerrequiredpasswordtype</span><span class="sxs-lookup"><span data-stu-id="7b14c-201">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="7b14c-202">パスワードの文字の種類。</span><span class="sxs-lookup"><span data-stu-id="7b14c-202">Type of characters in password.</span></span> <span data-ttu-id="7b14c-203">可能な値は、`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric` です。</span><span class="sxs-lookup"><span data-stu-id="7b14c-203">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`.</span></span>|
|<span data-ttu-id="7b14c-204">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="7b14c-204">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="7b14c-205">Int32</span><span class="sxs-lookup"><span data-stu-id="7b14c-205">Int32</span></span>|<span data-ttu-id="7b14c-206">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="7b14c-206">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="7b14c-207">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="7b14c-207">passwordExpirationDays</span></span>|<span data-ttu-id="7b14c-208">Int32</span><span class="sxs-lookup"><span data-stu-id="7b14c-208">Int32</span></span>|<span data-ttu-id="7b14c-209">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="7b14c-209">Number of days before the password expires.</span></span> <span data-ttu-id="7b14c-210">有効な値は 1 から 365 までです</span><span class="sxs-lookup"><span data-stu-id="7b14c-210">Valid values 1 to 365</span></span>|
|<span data-ttu-id="7b14c-211">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="7b14c-211">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="7b14c-212">Int32</span><span class="sxs-lookup"><span data-stu-id="7b14c-212">Int32</span></span>|<span data-ttu-id="7b14c-213">禁止する、以前のパスワードの数です。</span><span class="sxs-lookup"><span data-stu-id="7b14c-213">Number of previous passwords to block.</span></span> <span data-ttu-id="7b14c-214">有効な値は 1 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="7b14c-214">Valid values 1 to 24</span></span>|
|<span data-ttu-id="7b14c-215">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="7b14c-215">storageRequireEncryption</span></span>|<span data-ttu-id="7b14c-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b14c-216">Boolean</span></span>|<span data-ttu-id="7b14c-217">Android デバイスでの暗号化を要求します。</span><span class="sxs-lookup"><span data-stu-id="7b14c-217">Require encryption on Android devices.</span></span>|



## <a name="response"></a><span data-ttu-id="7b14c-218">応答</span><span class="sxs-lookup"><span data-stu-id="7b14c-218">Response</span></span>
<span data-ttu-id="7b14c-219">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7b14c-219">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b14c-220">例</span><span class="sxs-lookup"><span data-stu-id="7b14c-220">Example</span></span>

### <a name="request"></a><span data-ttu-id="7b14c-221">要求</span><span class="sxs-lookup"><span data-stu-id="7b14c-221">Request</span></span>
<span data-ttu-id="7b14c-222">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7b14c-222">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 932

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordMinimumLetterCharacters": 15,
  "passwordMinimumLowerCaseCharacters": 2,
  "passwordMinimumNonLetterCharacters": 2,
  "passwordMinimumNumericCharacters": 0,
  "passwordMinimumSymbolCharacters": 15,
  "passwordMinimumUpperCaseCharacters": 2,
  "passwordRequiredType": "required",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordPreviousPasswordCountToBlock": 4,
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="7b14c-223">応答</span><span class="sxs-lookup"><span data-stu-id="7b14c-223">Response</span></span>
<span data-ttu-id="7b14c-p119">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7b14c-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1104

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "be2464b4-64b4-be24-b464-24beb46424be",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordMinimumLetterCharacters": 15,
  "passwordMinimumLowerCaseCharacters": 2,
  "passwordMinimumNonLetterCharacters": 2,
  "passwordMinimumNumericCharacters": 0,
  "passwordMinimumSymbolCharacters": 15,
  "passwordMinimumUpperCaseCharacters": 2,
  "passwordRequiredType": "required",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordPreviousPasswordCountToBlock": 4,
  "storageRequireEncryption": true
}
```





