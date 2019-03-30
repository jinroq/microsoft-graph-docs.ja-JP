---
title: depIOSEnrollmentProfile の更新
description: depIOSEnrollmentProfile オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ea708a5ffe661f8024c027d1ac9ef10877474cd6
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30986944"
---
# <a name="update-depiosenrollmentprofile"></a><span data-ttu-id="fc327-103">depIOSEnrollmentProfile の更新</span><span class="sxs-lookup"><span data-stu-id="fc327-103">Update depIOSEnrollmentProfile</span></span>

> <span data-ttu-id="fc327-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fc327-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc327-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="fc327-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc327-106">[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="fc327-106">Update the properties of a [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fc327-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="fc327-107">Prerequisites</span></span>
<span data-ttu-id="fc327-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fc327-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc327-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fc327-110">Permission type</span></span>|<span data-ttu-id="fc327-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="fc327-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc327-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fc327-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fc327-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc327-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fc327-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fc327-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc327-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fc327-115">Not supported.</span></span>|
|<span data-ttu-id="fc327-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fc327-116">Application</span></span>|<span data-ttu-id="fc327-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fc327-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc327-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fc327-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="fc327-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fc327-119">Request headers</span></span>
|<span data-ttu-id="fc327-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fc327-120">Header</span></span>|<span data-ttu-id="fc327-121">値</span><span class="sxs-lookup"><span data-stu-id="fc327-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fc327-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc327-122">Authorization</span></span>|<span data-ttu-id="fc327-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="fc327-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fc327-124">承諾</span><span class="sxs-lookup"><span data-stu-id="fc327-124">Accept</span></span>|<span data-ttu-id="fc327-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fc327-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc327-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="fc327-126">Request body</span></span>
<span data-ttu-id="fc327-127">要求本文で、 [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="fc327-127">In the request body, supply a JSON representation for the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

<span data-ttu-id="fc327-128">次の表に、 [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="fc327-128">The following table shows the properties that are required when you create the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md).</span></span>

|<span data-ttu-id="fc327-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fc327-129">Property</span></span>|<span data-ttu-id="fc327-130">型</span><span class="sxs-lookup"><span data-stu-id="fc327-130">Type</span></span>|<span data-ttu-id="fc327-131">説明</span><span class="sxs-lookup"><span data-stu-id="fc327-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc327-132">id</span><span class="sxs-lookup"><span data-stu-id="fc327-132">id</span></span>|<span data-ttu-id="fc327-133">String</span><span class="sxs-lookup"><span data-stu-id="fc327-133">String</span></span>|<span data-ttu-id="fc327-134">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたオブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="fc327-134">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="fc327-135">displayName</span><span class="sxs-lookup"><span data-stu-id="fc327-135">displayName</span></span>|<span data-ttu-id="fc327-136">String</span><span class="sxs-lookup"><span data-stu-id="fc327-136">String</span></span>|<span data-ttu-id="fc327-137">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたプロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="fc327-137">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="fc327-138">description</span><span class="sxs-lookup"><span data-stu-id="fc327-138">description</span></span>|<span data-ttu-id="fc327-139">String</span><span class="sxs-lookup"><span data-stu-id="fc327-139">String</span></span>|<span data-ttu-id="fc327-140">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたプロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="fc327-140">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="fc327-141">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="fc327-141">requiresUserAuthentication</span></span>|<span data-ttu-id="fc327-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc327-142">Boolean</span></span>|<span data-ttu-id="fc327-143">プロファイルが[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承したユーザー認証を必要とするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="fc327-143">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="fc327-144">configurationendpointurl</span><span class="sxs-lookup"><span data-stu-id="fc327-144">configurationEndpointUrl</span></span>|<span data-ttu-id="fc327-145">String</span><span class="sxs-lookup"><span data-stu-id="fc327-145">String</span></span>|<span data-ttu-id="fc327-146">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承された登録に使用する構成エンドポイント url</span><span class="sxs-lookup"><span data-stu-id="fc327-146">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="fc327-147">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="fc327-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="fc327-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc327-148">Boolean</span></span>|<span data-ttu-id="fc327-149">会社のポータルではなく、Apple セットアップアシスタントを使用して認証することを示します。</span><span class="sxs-lookup"><span data-stu-id="fc327-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="fc327-150">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="fc327-150">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="fc327-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="fc327-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="fc327-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc327-152">Boolean</span></span>|<span data-ttu-id="fc327-153">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたセットアップアシスタントの登録済みデバイスで、会社のポータルが必要であることを示します。</span><span class="sxs-lookup"><span data-stu-id="fc327-153">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="fc327-154">isDefault</span><span class="sxs-lookup"><span data-stu-id="fc327-154">isDefault</span></span>|<span data-ttu-id="fc327-155">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="fc327-155">Boolean</span></span>|<span data-ttu-id="fc327-156">これが[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承された既定のプロファイルであるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="fc327-156">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fc327-157">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="fc327-157">supervisedModeEnabled</span></span>|<span data-ttu-id="fc327-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc327-158">Boolean</span></span>|<span data-ttu-id="fc327-159">監視モード、有効にする場合は True、それ以外の場合は false。</span><span class="sxs-lookup"><span data-stu-id="fc327-159">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="fc327-160">詳細https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intuneについては、「」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fc327-160">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="fc327-161">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="fc327-161">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fc327-162">supportdepartment</span><span class="sxs-lookup"><span data-stu-id="fc327-162">supportDepartment</span></span>|<span data-ttu-id="fc327-163">String</span><span class="sxs-lookup"><span data-stu-id="fc327-163">String</span></span>|<span data-ttu-id="fc327-164">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたサポート部署情報</span><span class="sxs-lookup"><span data-stu-id="fc327-164">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fc327-165">pass codedisabled</span><span class="sxs-lookup"><span data-stu-id="fc327-165">passCodeDisabled</span></span>|<span data-ttu-id="fc327-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc327-166">Boolean</span></span>|<span data-ttu-id="fc327-167">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたパスコードセットアップウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="fc327-167">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fc327-168">ismandatory</span><span class="sxs-lookup"><span data-stu-id="fc327-168">isMandatory</span></span>|<span data-ttu-id="fc327-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc327-169">Boolean</span></span>|<span data-ttu-id="fc327-170">プロファイルが[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="fc327-170">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fc327-171">locationdisabled</span><span class="sxs-lookup"><span data-stu-id="fc327-171">locationDisabled</span></span>|<span data-ttu-id="fc327-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc327-172">Boolean</span></span>|<span data-ttu-id="fc327-173">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承された場所サービスのセットアップウィンドウが無効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="fc327-173">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fc327-174">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="fc327-174">supportPhoneNumber</span></span>|<span data-ttu-id="fc327-175">String</span><span class="sxs-lookup"><span data-stu-id="fc327-175">String</span></span>|<span data-ttu-id="fc327-176">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたサポート電話番号</span><span class="sxs-lookup"><span data-stu-id="fc327-176">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fc327-177">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="fc327-177">profileRemovalDisabled</span></span>|<span data-ttu-id="fc327-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc327-178">Boolean</span></span>|<span data-ttu-id="fc327-179">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたプロファイル削除オプションが無効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="fc327-179">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fc327-180">restoreblocked</span><span class="sxs-lookup"><span data-stu-id="fc327-180">restoreBlocked</span></span>|<span data-ttu-id="fc327-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc327-181">Boolean</span></span>|<span data-ttu-id="fc327-182">復元のセットアップウィンドウが[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="fc327-182">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fc327-183">りんご eiddisabled</span><span class="sxs-lookup"><span data-stu-id="fc327-183">appleIdDisabled</span></span>|<span data-ttu-id="fc327-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc327-184">Boolean</span></span>|<span data-ttu-id="fc327-185">Apple id のセットアップウィンドウが無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="fc327-185">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fc327-186">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="fc327-186">termsAndConditionsDisabled</span></span>|<span data-ttu-id="fc327-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc327-187">Boolean</span></span>|<span data-ttu-id="fc327-188">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承された [使用条件] 設定ウィンドウを無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="fc327-188">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fc327-189">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="fc327-189">touchIdDisabled</span></span>|<span data-ttu-id="fc327-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc327-190">Boolean</span></span>|<span data-ttu-id="fc327-191">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたタッチ id セットアップウィンドウを無効にするかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="fc327-191">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fc327-192">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="fc327-192">applePayDisabled</span></span>|<span data-ttu-id="fc327-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc327-193">Boolean</span></span>|<span data-ttu-id="fc327-194">Apple の [支払い設定] ウィンドウが無効にされているかどうかを[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="fc327-194">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fc327-195">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="fc327-195">zoomDisabled</span></span>|<span data-ttu-id="fc327-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc327-196">Boolean</span></span>|<span data-ttu-id="fc327-197">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたズーム設定ウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="fc327-197">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fc327-198">siridisabled</span><span class="sxs-lookup"><span data-stu-id="fc327-198">siriDisabled</span></span>|<span data-ttu-id="fc327-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc327-199">Boolean</span></span>|<span data-ttu-id="fc327-200">siri セットアップウィンドウが無効であるかどうかを示します ( [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承)</span><span class="sxs-lookup"><span data-stu-id="fc327-200">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fc327-201">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="fc327-201">diagnosticsDisabled</span></span>|<span data-ttu-id="fc327-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc327-202">Boolean</span></span>|<span data-ttu-id="fc327-203">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承された診断セットアップウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="fc327-203">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fc327-204">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="fc327-204">displayToneSetupDisabled</span></span>|<span data-ttu-id="fc327-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc327-205">Boolean</span></span>|<span data-ttu-id="fc327-206">displaytone セットアップ画面が無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="fc327-206">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fc327-207">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="fc327-207">privacyPaneDisabled</span></span>|<span data-ttu-id="fc327-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc327-208">Boolean</span></span>|<span data-ttu-id="fc327-209">プライバシー画面が無効にされているかどうかを示します。 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="fc327-209">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fc327-210">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="fc327-210">iTunesPairingMode</span></span>|[<span data-ttu-id="fc327-211">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="fc327-211">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="fc327-212">iTunes ペアリングモードを示します。</span><span class="sxs-lookup"><span data-stu-id="fc327-212">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="fc327-213">使用可能な値は、`disallow`、`allow`、`requiresCertificate` です。</span><span class="sxs-lookup"><span data-stu-id="fc327-213">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="fc327-214">managementcertificates</span><span class="sxs-lookup"><span data-stu-id="fc327-214">managementCertificates</span></span>|<span data-ttu-id="fc327-215">[managementcertificatewiththumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="fc327-215">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="fc327-216">Apple Configurator の管理証明書</span><span class="sxs-lookup"><span data-stu-id="fc327-216">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="fc327-217">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="fc327-217">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="fc327-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc327-218">Boolean</span></span>|<span data-ttu-id="fc327-219">Android からの復元が無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="fc327-219">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="fc327-220">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="fc327-220">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="fc327-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc327-221">Boolean</span></span>|<span data-ttu-id="fc327-222">構成済みの確認をデバイスが待機する必要があるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="fc327-222">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="fc327-223">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="fc327-223">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="fc327-224">Int32</span><span class="sxs-lookup"><span data-stu-id="fc327-224">Int32</span></span>|<span data-ttu-id="fc327-225">これにより、共有 iPad を使用できるユーザーの最大数が指定されます。</span><span class="sxs-lookup"><span data-stu-id="fc327-225">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="fc327-226">共有 iPad モードでのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="fc327-226">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="fc327-227">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="fc327-227">enableSharedIPad</span></span>|<span data-ttu-id="fc327-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc327-228">Boolean</span></span>|<span data-ttu-id="fc327-229">これは、デバイスを、複数のユーザーシナリオを有効にするモードで登録するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="fc327-229">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="fc327-230">共有 ipad にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="fc327-230">Only applicable in shared iPads.</span></span>|
|<span data-ttu-id="fc327-231">companyPortalVppTokenId</span><span class="sxs-lookup"><span data-stu-id="fc327-231">companyPortalVppTokenId</span></span>|<span data-ttu-id="fc327-232">String</span><span class="sxs-lookup"><span data-stu-id="fc327-232">String</span></span>|<span data-ttu-id="fc327-233">設定されている場合は、ポータルサイトのライセンスを展開するためにどの Vpp トークンを使用する必要があるかを示します。</span><span class="sxs-lookup"><span data-stu-id="fc327-233">If set, indicates which Vpp token should be used to deploy the Company Portal w/ device licensing.</span></span> <span data-ttu-id="fc327-234">このプロパティを設定するためには、' enableAuthenticationViaCompanyPortal ' を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="fc327-234">'enableAuthenticationViaCompanyPortal' must be set in order for this property to be set.</span></span>|
|<span data-ttu-id="fc327-235">enableSingleAppEnrollmentMode</span><span class="sxs-lookup"><span data-stu-id="fc327-235">enableSingleAppEnrollmentMode</span></span>|<span data-ttu-id="fc327-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc327-236">Boolean</span></span>|<span data-ttu-id="fc327-237">デバイスに対して、1つのアプリモードを有効にし、登録時にアプリロックを適用するように指示します。</span><span class="sxs-lookup"><span data-stu-id="fc327-237">Tells the device to enable single app mode and apply app-lock during enrollment.</span></span> <span data-ttu-id="fc327-238">既定値は false です。</span><span class="sxs-lookup"><span data-stu-id="fc327-238">Default is false.</span></span> <span data-ttu-id="fc327-239">このプロパティを設定するには、' enableAuthenticationViaCompanyPortal ' および ' companyPortalVppTokenId ' を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="fc327-239">'enableAuthenticationViaCompanyPortal' and 'companyPortalVppTokenId' must be set for this property to be set.</span></span>|
|<span data-ttu-id="fc327-240">ホームボタンの無効化</span><span class="sxs-lookup"><span data-stu-id="fc327-240">homeButtonScreenDisabled</span></span>|<span data-ttu-id="fc327-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc327-241">Boolean</span></span>|<span data-ttu-id="fc327-242">[ホームボタンの感度] 画面を無効にするかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="fc327-242">Indicates if home button sensitivity screen is disabled</span></span>|
|<span data-ttu-id="fc327-243">iMessageAndFaceTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="fc327-243">iMessageAndFaceTimeScreenDisabled</span></span>|<span data-ttu-id="fc327-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc327-244">Boolean</span></span>|<span data-ttu-id="fc327-245">iMessage および FaceTime の画面が無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="fc327-245">Indicates if iMessage and FaceTime screen is disabled</span></span>|
|<span data-ttu-id="fc327-246">onboardingscreendisabled</span><span class="sxs-lookup"><span data-stu-id="fc327-246">onBoardingScreenDisabled</span></span>|<span data-ttu-id="fc327-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc327-247">Boolean</span></span>|<span data-ttu-id="fc327-248">オンボードのセットアップ画面が無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="fc327-248">Indicates if onboarding setup screen is disabled</span></span>|
|<span data-ttu-id="fc327-249">screenTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="fc327-249">screenTimeScreenDisabled</span></span>|<span data-ttu-id="fc327-250">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc327-250">Boolean</span></span>|<span data-ttu-id="fc327-251">画面のタイムアウト設定を無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="fc327-251">Indicates if screen timeout setup is disabled</span></span>|
|<span data-ttu-id="fc327-252">シムの設定を無効にする</span><span class="sxs-lookup"><span data-stu-id="fc327-252">simSetupScreenDisabled</span></span>|<span data-ttu-id="fc327-253">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc327-253">Boolean</span></span>|<span data-ttu-id="fc327-254">[シム] セットアップ画面が無効であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="fc327-254">Indicates if the SIMSetup screen is disabled</span></span>|
|<span data-ttu-id="fc327-255">ソフトウェアの更新 creendisabled</span><span class="sxs-lookup"><span data-stu-id="fc327-255">softwareUpdateScreenDisabled</span></span>|<span data-ttu-id="fc327-256">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc327-256">Boolean</span></span>|<span data-ttu-id="fc327-257">必須の [ソフトウェアの更新] 画面が無効であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="fc327-257">Indicates if the mandatory sofware update screen is disabled</span></span>|
|<span data-ttu-id="fc327-258">watchMigrationScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="fc327-258">watchMigrationScreenDisabled</span></span>|<span data-ttu-id="fc327-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc327-259">Boolean</span></span>|<span data-ttu-id="fc327-260">[移行の監視] 画面が無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="fc327-260">Indicates if the watch migration screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="fc327-261">応答</span><span class="sxs-lookup"><span data-stu-id="fc327-261">Response</span></span>
<span data-ttu-id="fc327-262">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="fc327-262">If successful, this method returns a `200 OK` response code and an updated [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc327-263">例</span><span class="sxs-lookup"><span data-stu-id="fc327-263">Example</span></span>

### <a name="request"></a><span data-ttu-id="fc327-264">要求</span><span class="sxs-lookup"><span data-stu-id="fc327-264">Request</span></span>
<span data-ttu-id="fc327-265">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fc327-265">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
Content-type: application/json
Content-length: 1736

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

### <a name="response"></a><span data-ttu-id="fc327-266">応答</span><span class="sxs-lookup"><span data-stu-id="fc327-266">Response</span></span>
<span data-ttu-id="fc327-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fc327-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1785

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




