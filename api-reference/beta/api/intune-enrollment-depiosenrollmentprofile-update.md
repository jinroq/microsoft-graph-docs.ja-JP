---
title: DepIOSEnrollmentProfile の更新
description: DepIOSEnrollmentProfile オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 12998cd361e51b4c4c9c6ecb0ddad946b6605295
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33908778"
---
# <a name="update-depiosenrollmentprofile"></a><span data-ttu-id="6ad52-103">DepIOSEnrollmentProfile の更新</span><span class="sxs-lookup"><span data-stu-id="6ad52-103">Update depIOSEnrollmentProfile</span></span>

> <span data-ttu-id="6ad52-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6ad52-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ad52-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6ad52-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ad52-106">[DepIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6ad52-106">Update the properties of a [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6ad52-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="6ad52-107">Prerequisites</span></span>
<span data-ttu-id="6ad52-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6ad52-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ad52-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6ad52-110">Permission type</span></span>|<span data-ttu-id="6ad52-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6ad52-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6ad52-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6ad52-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6ad52-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ad52-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6ad52-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6ad52-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ad52-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6ad52-115">Not supported.</span></span>|
|<span data-ttu-id="6ad52-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6ad52-116">Application</span></span>|<span data-ttu-id="6ad52-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6ad52-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ad52-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6ad52-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="6ad52-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6ad52-119">Request headers</span></span>
|<span data-ttu-id="6ad52-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6ad52-120">Header</span></span>|<span data-ttu-id="6ad52-121">値</span><span class="sxs-lookup"><span data-stu-id="6ad52-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6ad52-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ad52-122">Authorization</span></span>|<span data-ttu-id="6ad52-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="6ad52-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6ad52-124">承諾</span><span class="sxs-lookup"><span data-stu-id="6ad52-124">Accept</span></span>|<span data-ttu-id="6ad52-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6ad52-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ad52-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="6ad52-126">Request body</span></span>
<span data-ttu-id="6ad52-127">要求本文で、 [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6ad52-127">In the request body, supply a JSON representation for the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

<span data-ttu-id="6ad52-128">次の表に、 [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="6ad52-128">The following table shows the properties that are required when you create the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md).</span></span>

|<span data-ttu-id="6ad52-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6ad52-129">Property</span></span>|<span data-ttu-id="6ad52-130">型</span><span class="sxs-lookup"><span data-stu-id="6ad52-130">Type</span></span>|<span data-ttu-id="6ad52-131">説明</span><span class="sxs-lookup"><span data-stu-id="6ad52-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ad52-132">id</span><span class="sxs-lookup"><span data-stu-id="6ad52-132">id</span></span>|<span data-ttu-id="6ad52-133">文字列</span><span class="sxs-lookup"><span data-stu-id="6ad52-133">String</span></span>|<span data-ttu-id="6ad52-134">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたオブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="6ad52-134">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="6ad52-135">displayName</span><span class="sxs-lookup"><span data-stu-id="6ad52-135">displayName</span></span>|<span data-ttu-id="6ad52-136">String</span><span class="sxs-lookup"><span data-stu-id="6ad52-136">String</span></span>|<span data-ttu-id="6ad52-137">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたプロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="6ad52-137">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="6ad52-138">description</span><span class="sxs-lookup"><span data-stu-id="6ad52-138">description</span></span>|<span data-ttu-id="6ad52-139">String</span><span class="sxs-lookup"><span data-stu-id="6ad52-139">String</span></span>|<span data-ttu-id="6ad52-140">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたプロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="6ad52-140">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="6ad52-141">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="6ad52-141">requiresUserAuthentication</span></span>|<span data-ttu-id="6ad52-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ad52-142">Boolean</span></span>|<span data-ttu-id="6ad52-143">プロファイルが[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承したユーザー認証を必要とするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6ad52-143">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="6ad52-144">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="6ad52-144">configurationEndpointUrl</span></span>|<span data-ttu-id="6ad52-145">String</span><span class="sxs-lookup"><span data-stu-id="6ad52-145">String</span></span>|<span data-ttu-id="6ad52-146">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承された登録に使用する構成エンドポイント url</span><span class="sxs-lookup"><span data-stu-id="6ad52-146">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="6ad52-147">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="6ad52-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="6ad52-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ad52-148">Boolean</span></span>|<span data-ttu-id="6ad52-149">会社のポータルではなく、Apple セットアップアシスタントを使用して認証することを示します。</span><span class="sxs-lookup"><span data-stu-id="6ad52-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="6ad52-150">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="6ad52-150">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="6ad52-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="6ad52-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="6ad52-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ad52-152">Boolean</span></span>|<span data-ttu-id="6ad52-153">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたセットアップアシスタントの登録済みデバイスで、会社のポータルが必要であることを示します。</span><span class="sxs-lookup"><span data-stu-id="6ad52-153">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="6ad52-154">isDefault</span><span class="sxs-lookup"><span data-stu-id="6ad52-154">isDefault</span></span>|<span data-ttu-id="6ad52-155">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="6ad52-155">Boolean</span></span>|<span data-ttu-id="6ad52-156">これが[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承された既定のプロファイルであるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6ad52-156">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6ad52-157">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="6ad52-157">supervisedModeEnabled</span></span>|<span data-ttu-id="6ad52-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ad52-158">Boolean</span></span>|<span data-ttu-id="6ad52-159">監視モード、有効にする場合は True、それ以外の場合は false。</span><span class="sxs-lookup"><span data-stu-id="6ad52-159">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="6ad52-160">詳細https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intuneについては、「」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6ad52-160">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="6ad52-161">[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="6ad52-161">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6ad52-162">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="6ad52-162">supportDepartment</span></span>|<span data-ttu-id="6ad52-163">String</span><span class="sxs-lookup"><span data-stu-id="6ad52-163">String</span></span>|<span data-ttu-id="6ad52-164">[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたサポート部署情報</span><span class="sxs-lookup"><span data-stu-id="6ad52-164">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6ad52-165">Pass Codedisabled</span><span class="sxs-lookup"><span data-stu-id="6ad52-165">passCodeDisabled</span></span>|<span data-ttu-id="6ad52-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ad52-166">Boolean</span></span>|<span data-ttu-id="6ad52-167">[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたパスコードセットアップウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="6ad52-167">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6ad52-168">isMandatory</span><span class="sxs-lookup"><span data-stu-id="6ad52-168">isMandatory</span></span>|<span data-ttu-id="6ad52-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ad52-169">Boolean</span></span>|<span data-ttu-id="6ad52-170">プロファイルが[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6ad52-170">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6ad52-171">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="6ad52-171">locationDisabled</span></span>|<span data-ttu-id="6ad52-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ad52-172">Boolean</span></span>|<span data-ttu-id="6ad52-173">[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承された場所サービスのセットアップウィンドウが無効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6ad52-173">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6ad52-174">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="6ad52-174">supportPhoneNumber</span></span>|<span data-ttu-id="6ad52-175">String</span><span class="sxs-lookup"><span data-stu-id="6ad52-175">String</span></span>|<span data-ttu-id="6ad52-176">[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたサポート電話番号</span><span class="sxs-lookup"><span data-stu-id="6ad52-176">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6ad52-177">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="6ad52-177">profileRemovalDisabled</span></span>|<span data-ttu-id="6ad52-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ad52-178">Boolean</span></span>|<span data-ttu-id="6ad52-179">[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたプロファイル削除オプションが無効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6ad52-179">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6ad52-180">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="6ad52-180">restoreBlocked</span></span>|<span data-ttu-id="6ad52-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ad52-181">Boolean</span></span>|<span data-ttu-id="6ad52-182">復元のセットアップウィンドウが[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6ad52-182">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6ad52-183">りんご Eiddisabled</span><span class="sxs-lookup"><span data-stu-id="6ad52-183">appleIdDisabled</span></span>|<span data-ttu-id="6ad52-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ad52-184">Boolean</span></span>|<span data-ttu-id="6ad52-185">Apple id のセットアップウィンドウが無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="6ad52-185">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6ad52-186">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="6ad52-186">termsAndConditionsDisabled</span></span>|<span data-ttu-id="6ad52-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ad52-187">Boolean</span></span>|<span data-ttu-id="6ad52-188">[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承された [使用条件] 設定ウィンドウを無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6ad52-188">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6ad52-189">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="6ad52-189">touchIdDisabled</span></span>|<span data-ttu-id="6ad52-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ad52-190">Boolean</span></span>|<span data-ttu-id="6ad52-191">[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたタッチ id セットアップウィンドウを無効にするかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="6ad52-191">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6ad52-192">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="6ad52-192">applePayDisabled</span></span>|<span data-ttu-id="6ad52-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ad52-193">Boolean</span></span>|<span data-ttu-id="6ad52-194">Apple の [支払い設定] ウィンドウが無効にされているかどうかを[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="6ad52-194">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6ad52-195">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="6ad52-195">zoomDisabled</span></span>|<span data-ttu-id="6ad52-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ad52-196">Boolean</span></span>|<span data-ttu-id="6ad52-197">[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたズーム設定ウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="6ad52-197">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6ad52-198">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="6ad52-198">siriDisabled</span></span>|<span data-ttu-id="6ad52-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ad52-199">Boolean</span></span>|<span data-ttu-id="6ad52-200">Siri セットアップウィンドウが無効であるかどうかを示します ( [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承)</span><span class="sxs-lookup"><span data-stu-id="6ad52-200">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6ad52-201">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="6ad52-201">diagnosticsDisabled</span></span>|<span data-ttu-id="6ad52-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ad52-202">Boolean</span></span>|<span data-ttu-id="6ad52-203">[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承された診断セットアップウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="6ad52-203">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6ad52-204">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="6ad52-204">displayToneSetupDisabled</span></span>|<span data-ttu-id="6ad52-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ad52-205">Boolean</span></span>|<span data-ttu-id="6ad52-206">Displaytone セットアップ画面が無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="6ad52-206">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6ad52-207">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="6ad52-207">privacyPaneDisabled</span></span>|<span data-ttu-id="6ad52-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ad52-208">Boolean</span></span>|<span data-ttu-id="6ad52-209">プライバシー画面が無効にされているかどうかを示します。 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="6ad52-209">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6ad52-210">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="6ad52-210">deviceNameTemplate</span></span>|<span data-ttu-id="6ad52-211">String</span><span class="sxs-lookup"><span data-stu-id="6ad52-211">String</span></span>|<span data-ttu-id="6ad52-212">リテラルまたは名前のパターンを設定します。</span><span class="sxs-lookup"><span data-stu-id="6ad52-212">Sets a literal or name pattern.</span></span> <span data-ttu-id="6ad52-213">[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="6ad52-213">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6ad52-214">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="6ad52-214">iTunesPairingMode</span></span>|[<span data-ttu-id="6ad52-215">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="6ad52-215">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="6ad52-216">ITunes ペアリングモードを示します。</span><span class="sxs-lookup"><span data-stu-id="6ad52-216">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="6ad52-217">可能な値は、`disallow`、`allow`、`requiresCertificate` です。</span><span class="sxs-lookup"><span data-stu-id="6ad52-217">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="6ad52-218">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="6ad52-218">managementCertificates</span></span>|<span data-ttu-id="6ad52-219">[Managementcertificatewiththumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="6ad52-219">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="6ad52-220">Apple Configurator の管理証明書</span><span class="sxs-lookup"><span data-stu-id="6ad52-220">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="6ad52-221">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="6ad52-221">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="6ad52-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ad52-222">Boolean</span></span>|<span data-ttu-id="6ad52-223">Android からの復元が無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="6ad52-223">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="6ad52-224">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="6ad52-224">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="6ad52-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ad52-225">Boolean</span></span>|<span data-ttu-id="6ad52-226">構成済みの確認をデバイスが待機する必要があるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="6ad52-226">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="6ad52-227">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="6ad52-227">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="6ad52-228">Int32</span><span class="sxs-lookup"><span data-stu-id="6ad52-228">Int32</span></span>|<span data-ttu-id="6ad52-229">これにより、共有 iPad を使用できるユーザーの最大数が指定されます。</span><span class="sxs-lookup"><span data-stu-id="6ad52-229">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="6ad52-230">共有 iPad モードでのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="6ad52-230">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="6ad52-231">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="6ad52-231">enableSharedIPad</span></span>|<span data-ttu-id="6ad52-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ad52-232">Boolean</span></span>|<span data-ttu-id="6ad52-233">これは、デバイスを、複数のユーザーシナリオを有効にするモードで登録するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6ad52-233">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="6ad52-234">共有 Ipad にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="6ad52-234">Only applicable in shared iPads.</span></span>|
|<span data-ttu-id="6ad52-235">companyPortalVppTokenId</span><span class="sxs-lookup"><span data-stu-id="6ad52-235">companyPortalVppTokenId</span></span>|<span data-ttu-id="6ad52-236">String</span><span class="sxs-lookup"><span data-stu-id="6ad52-236">String</span></span>|<span data-ttu-id="6ad52-237">設定されている場合は、ポータルサイトのライセンスを展開するためにどの Vpp トークンを使用する必要があるかを示します。</span><span class="sxs-lookup"><span data-stu-id="6ad52-237">If set, indicates which Vpp token should be used to deploy the Company Portal w/ device licensing.</span></span> <span data-ttu-id="6ad52-238">このプロパティを設定するためには、' enableAuthenticationViaCompanyPortal ' を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6ad52-238">'enableAuthenticationViaCompanyPortal' must be set in order for this property to be set.</span></span>|
|<span data-ttu-id="6ad52-239">enableSingleAppEnrollmentMode</span><span class="sxs-lookup"><span data-stu-id="6ad52-239">enableSingleAppEnrollmentMode</span></span>|<span data-ttu-id="6ad52-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ad52-240">Boolean</span></span>|<span data-ttu-id="6ad52-241">デバイスに対して、1つのアプリモードを有効にし、登録時にアプリロックを適用するように指示します。</span><span class="sxs-lookup"><span data-stu-id="6ad52-241">Tells the device to enable single app mode and apply app-lock during enrollment.</span></span> <span data-ttu-id="6ad52-242">既定値は false です。</span><span class="sxs-lookup"><span data-stu-id="6ad52-242">Default is false.</span></span> <span data-ttu-id="6ad52-243">このプロパティを設定するには、' enableAuthenticationViaCompanyPortal ' および ' companyPortalVppTokenId ' を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6ad52-243">'enableAuthenticationViaCompanyPortal' and 'companyPortalVppTokenId' must be set for this property to be set.</span></span>|
|<span data-ttu-id="6ad52-244">ホームボタンの無効化</span><span class="sxs-lookup"><span data-stu-id="6ad52-244">homeButtonScreenDisabled</span></span>|<span data-ttu-id="6ad52-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ad52-245">Boolean</span></span>|<span data-ttu-id="6ad52-246">[ホームボタンの感度] 画面を無効にするかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="6ad52-246">Indicates if home button sensitivity screen is disabled</span></span>|
|<span data-ttu-id="6ad52-247">iMessageAndFaceTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="6ad52-247">iMessageAndFaceTimeScreenDisabled</span></span>|<span data-ttu-id="6ad52-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ad52-248">Boolean</span></span>|<span data-ttu-id="6ad52-249">IMessage および FaceTime の画面が無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="6ad52-249">Indicates if iMessage and FaceTime screen is disabled</span></span>|
|<span data-ttu-id="6ad52-250">onBoardingScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="6ad52-250">onBoardingScreenDisabled</span></span>|<span data-ttu-id="6ad52-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ad52-251">Boolean</span></span>|<span data-ttu-id="6ad52-252">オンボードのセットアップ画面が無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="6ad52-252">Indicates if onboarding setup screen is disabled</span></span>|
|<span data-ttu-id="6ad52-253">screenTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="6ad52-253">screenTimeScreenDisabled</span></span>|<span data-ttu-id="6ad52-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ad52-254">Boolean</span></span>|<span data-ttu-id="6ad52-255">画面のタイムアウト設定を無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6ad52-255">Indicates if screen timeout setup is disabled</span></span>|
|<span data-ttu-id="6ad52-256">シムの設定を無効にする</span><span class="sxs-lookup"><span data-stu-id="6ad52-256">simSetupScreenDisabled</span></span>|<span data-ttu-id="6ad52-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ad52-257">Boolean</span></span>|<span data-ttu-id="6ad52-258">[シム] セットアップ画面が無効であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6ad52-258">Indicates if the SIMSetup screen is disabled</span></span>|
|<span data-ttu-id="6ad52-259">ソフトウェアの更新 Creendisabled</span><span class="sxs-lookup"><span data-stu-id="6ad52-259">softwareUpdateScreenDisabled</span></span>|<span data-ttu-id="6ad52-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ad52-260">Boolean</span></span>|<span data-ttu-id="6ad52-261">必須の [ソフトウェアの更新] 画面が無効であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6ad52-261">Indicates if the mandatory sofware update screen is disabled</span></span>|
|<span data-ttu-id="6ad52-262">watchMigrationScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="6ad52-262">watchMigrationScreenDisabled</span></span>|<span data-ttu-id="6ad52-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ad52-263">Boolean</span></span>|<span data-ttu-id="6ad52-264">[移行の監視] 画面が無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="6ad52-264">Indicates if the watch migration screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="6ad52-265">応答</span><span class="sxs-lookup"><span data-stu-id="6ad52-265">Response</span></span>
<span data-ttu-id="6ad52-266">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6ad52-266">If successful, this method returns a `200 OK` response code and an updated [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ad52-267">例</span><span class="sxs-lookup"><span data-stu-id="6ad52-267">Example</span></span>

### <a name="request"></a><span data-ttu-id="6ad52-268">要求</span><span class="sxs-lookup"><span data-stu-id="6ad52-268">Request</span></span>
<span data-ttu-id="6ad52-269">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6ad52-269">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
Content-type: application/json
Content-length: 1791

{
  "@odata.type": "#microsoft.graph.depIOSEnrollmentProfile",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true,
  "isDefault": true,
  "supervisedModeEnabled": true,
  "supportDepartment": "Support Department value",
  "passCodeDisabled": true,
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "Support Phone Number value",
  "profileRemovalDisabled": true,
  "restoreBlocked": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "displayToneSetupDisabled": true,
  "privacyPaneDisabled": true,
  "deviceNameTemplate": "Device Name Template value",
  "iTunesPairingMode": "allow",
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
      "thumbprint": "Thumbprint value",
      "certificate": "Certificate value"
    }
  ],
  "restoreFromAndroidDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 10,
  "enableSharedIPad": true,
  "companyPortalVppTokenId": "Company Portal Vpp Token Id value",
  "enableSingleAppEnrollmentMode": true,
  "homeButtonScreenDisabled": true,
  "iMessageAndFaceTimeScreenDisabled": true,
  "onBoardingScreenDisabled": true,
  "screenTimeScreenDisabled": true,
  "simSetupScreenDisabled": true,
  "softwareUpdateScreenDisabled": true,
  "watchMigrationScreenDisabled": true
}
```

### <a name="response"></a><span data-ttu-id="6ad52-270">応答</span><span class="sxs-lookup"><span data-stu-id="6ad52-270">Response</span></span>
<span data-ttu-id="6ad52-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6ad52-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1840

{
  "@odata.type": "#microsoft.graph.depIOSEnrollmentProfile",
  "id": "1ec10a60-0a60-1ec1-600a-c11e600ac11e",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true,
  "isDefault": true,
  "supervisedModeEnabled": true,
  "supportDepartment": "Support Department value",
  "passCodeDisabled": true,
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "Support Phone Number value",
  "profileRemovalDisabled": true,
  "restoreBlocked": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "displayToneSetupDisabled": true,
  "privacyPaneDisabled": true,
  "deviceNameTemplate": "Device Name Template value",
  "iTunesPairingMode": "allow",
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
      "thumbprint": "Thumbprint value",
      "certificate": "Certificate value"
    }
  ],
  "restoreFromAndroidDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 10,
  "enableSharedIPad": true,
  "companyPortalVppTokenId": "Company Portal Vpp Token Id value",
  "enableSingleAppEnrollmentMode": true,
  "homeButtonScreenDisabled": true,
  "iMessageAndFaceTimeScreenDisabled": true,
  "onBoardingScreenDisabled": true,
  "screenTimeScreenDisabled": true,
  "simSetupScreenDisabled": true,
  "softwareUpdateScreenDisabled": true,
  "watchMigrationScreenDisabled": true
}
```




