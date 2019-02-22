---
title: depIOSEnrollmentProfile の更新
description: depIOSEnrollmentProfile オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 89ce85e09ee9ad59c19c67401238e2f0f950eaba
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167733"
---
# <a name="update-depiosenrollmentprofile"></a><span data-ttu-id="6a565-103">depIOSEnrollmentProfile の更新</span><span class="sxs-lookup"><span data-stu-id="6a565-103">Update depIOSEnrollmentProfile</span></span>

> <span data-ttu-id="6a565-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a565-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a565-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6a565-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a565-106">[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6a565-106">Update the properties of a [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6a565-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="6a565-107">Prerequisites</span></span>
<span data-ttu-id="6a565-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6a565-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6a565-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6a565-110">Permission type</span></span>|<span data-ttu-id="6a565-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6a565-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a565-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6a565-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6a565-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a565-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6a565-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6a565-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a565-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a565-115">Not supported.</span></span>|
|<span data-ttu-id="6a565-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6a565-116">Application</span></span>|<span data-ttu-id="6a565-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a565-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a565-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6a565-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="6a565-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6a565-119">Request headers</span></span>
|<span data-ttu-id="6a565-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6a565-120">Header</span></span>|<span data-ttu-id="6a565-121">値</span><span class="sxs-lookup"><span data-stu-id="6a565-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a565-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a565-122">Authorization</span></span>|<span data-ttu-id="6a565-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="6a565-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a565-124">承諾</span><span class="sxs-lookup"><span data-stu-id="6a565-124">Accept</span></span>|<span data-ttu-id="6a565-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6a565-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a565-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="6a565-126">Request body</span></span>
<span data-ttu-id="6a565-127">要求本文で、 [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6a565-127">In the request body, supply a JSON representation for the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

<span data-ttu-id="6a565-128">次の表に、 [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="6a565-128">The following table shows the properties that are required when you create the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md).</span></span>

|<span data-ttu-id="6a565-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6a565-129">Property</span></span>|<span data-ttu-id="6a565-130">型</span><span class="sxs-lookup"><span data-stu-id="6a565-130">Type</span></span>|<span data-ttu-id="6a565-131">説明</span><span class="sxs-lookup"><span data-stu-id="6a565-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a565-132">id</span><span class="sxs-lookup"><span data-stu-id="6a565-132">id</span></span>|<span data-ttu-id="6a565-133">文字列</span><span class="sxs-lookup"><span data-stu-id="6a565-133">String</span></span>|<span data-ttu-id="6a565-134">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたオブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="6a565-134">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="6a565-135">displayName</span><span class="sxs-lookup"><span data-stu-id="6a565-135">displayName</span></span>|<span data-ttu-id="6a565-136">String</span><span class="sxs-lookup"><span data-stu-id="6a565-136">String</span></span>|<span data-ttu-id="6a565-137">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたプロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="6a565-137">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="6a565-138">説明</span><span class="sxs-lookup"><span data-stu-id="6a565-138">description</span></span>|<span data-ttu-id="6a565-139">String</span><span class="sxs-lookup"><span data-stu-id="6a565-139">String</span></span>|<span data-ttu-id="6a565-140">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたプロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="6a565-140">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="6a565-141">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="6a565-141">requiresUserAuthentication</span></span>|<span data-ttu-id="6a565-142">ブール値</span><span class="sxs-lookup"><span data-stu-id="6a565-142">Boolean</span></span>|<span data-ttu-id="6a565-143">プロファイルが[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承したユーザー認証を必要とするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6a565-143">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="6a565-144">configurationendpointurl</span><span class="sxs-lookup"><span data-stu-id="6a565-144">configurationEndpointUrl</span></span>|<span data-ttu-id="6a565-145">String</span><span class="sxs-lookup"><span data-stu-id="6a565-145">String</span></span>|<span data-ttu-id="6a565-146">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承された登録に使用する構成エンドポイント url</span><span class="sxs-lookup"><span data-stu-id="6a565-146">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="6a565-147">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="6a565-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="6a565-148">ブール値</span><span class="sxs-lookup"><span data-stu-id="6a565-148">Boolean</span></span>|<span data-ttu-id="6a565-149">会社のポータルではなく、Apple セットアップアシスタントを使用して認証することを示します。</span><span class="sxs-lookup"><span data-stu-id="6a565-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="6a565-150">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="6a565-150">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="6a565-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="6a565-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="6a565-152">ブール値</span><span class="sxs-lookup"><span data-stu-id="6a565-152">Boolean</span></span>|<span data-ttu-id="6a565-153">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたセットアップアシスタントの登録済みデバイスで、会社のポータルが必要であることを示します。</span><span class="sxs-lookup"><span data-stu-id="6a565-153">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="6a565-154">isDefault</span><span class="sxs-lookup"><span data-stu-id="6a565-154">isDefault</span></span>|<span data-ttu-id="6a565-155">ブール値</span><span class="sxs-lookup"><span data-stu-id="6a565-155">Boolean</span></span>|<span data-ttu-id="6a565-156">これが[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承された既定のプロファイルであるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6a565-156">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6a565-157">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="6a565-157">supervisedModeEnabled</span></span>|<span data-ttu-id="6a565-158">ブール値</span><span class="sxs-lookup"><span data-stu-id="6a565-158">Boolean</span></span>|<span data-ttu-id="6a565-159">監視モード、有効にする場合は True、それ以外の場合は false。</span><span class="sxs-lookup"><span data-stu-id="6a565-159">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="6a565-160">詳細https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intuneについては、「」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6a565-160">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="6a565-161">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="6a565-161">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6a565-162">supportdepartment</span><span class="sxs-lookup"><span data-stu-id="6a565-162">supportDepartment</span></span>|<span data-ttu-id="6a565-163">String</span><span class="sxs-lookup"><span data-stu-id="6a565-163">String</span></span>|<span data-ttu-id="6a565-164">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたサポート部署情報</span><span class="sxs-lookup"><span data-stu-id="6a565-164">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6a565-165">pass codedisabled</span><span class="sxs-lookup"><span data-stu-id="6a565-165">passCodeDisabled</span></span>|<span data-ttu-id="6a565-166">ブール値</span><span class="sxs-lookup"><span data-stu-id="6a565-166">Boolean</span></span>|<span data-ttu-id="6a565-167">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたパスコードセットアップウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="6a565-167">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6a565-168">ismandatory</span><span class="sxs-lookup"><span data-stu-id="6a565-168">isMandatory</span></span>|<span data-ttu-id="6a565-169">ブール値</span><span class="sxs-lookup"><span data-stu-id="6a565-169">Boolean</span></span>|<span data-ttu-id="6a565-170">プロファイルが[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6a565-170">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6a565-171">locationdisabled</span><span class="sxs-lookup"><span data-stu-id="6a565-171">locationDisabled</span></span>|<span data-ttu-id="6a565-172">ブール値</span><span class="sxs-lookup"><span data-stu-id="6a565-172">Boolean</span></span>|<span data-ttu-id="6a565-173">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承された場所サービスのセットアップウィンドウが無効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6a565-173">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6a565-174">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="6a565-174">supportPhoneNumber</span></span>|<span data-ttu-id="6a565-175">String</span><span class="sxs-lookup"><span data-stu-id="6a565-175">String</span></span>|<span data-ttu-id="6a565-176">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたサポート電話番号</span><span class="sxs-lookup"><span data-stu-id="6a565-176">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6a565-177">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="6a565-177">profileRemovalDisabled</span></span>|<span data-ttu-id="6a565-178">ブール値</span><span class="sxs-lookup"><span data-stu-id="6a565-178">Boolean</span></span>|<span data-ttu-id="6a565-179">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたプロファイル削除オプションが無効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6a565-179">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6a565-180">restoreblocked</span><span class="sxs-lookup"><span data-stu-id="6a565-180">restoreBlocked</span></span>|<span data-ttu-id="6a565-181">ブール値</span><span class="sxs-lookup"><span data-stu-id="6a565-181">Boolean</span></span>|<span data-ttu-id="6a565-182">復元のセットアップウィンドウが[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6a565-182">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6a565-183">りんご eiddisabled</span><span class="sxs-lookup"><span data-stu-id="6a565-183">appleIdDisabled</span></span>|<span data-ttu-id="6a565-184">ブール値</span><span class="sxs-lookup"><span data-stu-id="6a565-184">Boolean</span></span>|<span data-ttu-id="6a565-185">Apple id のセットアップウィンドウが無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="6a565-185">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6a565-186">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="6a565-186">termsAndConditionsDisabled</span></span>|<span data-ttu-id="6a565-187">ブール値</span><span class="sxs-lookup"><span data-stu-id="6a565-187">Boolean</span></span>|<span data-ttu-id="6a565-188">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承された [使用条件] 設定ウィンドウを無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6a565-188">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6a565-189">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="6a565-189">touchIdDisabled</span></span>|<span data-ttu-id="6a565-190">ブール値</span><span class="sxs-lookup"><span data-stu-id="6a565-190">Boolean</span></span>|<span data-ttu-id="6a565-191">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたタッチ id セットアップウィンドウを無効にするかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="6a565-191">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6a565-192">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="6a565-192">applePayDisabled</span></span>|<span data-ttu-id="6a565-193">ブール値</span><span class="sxs-lookup"><span data-stu-id="6a565-193">Boolean</span></span>|<span data-ttu-id="6a565-194">Apple の [支払い設定] ウィンドウが無効にされているかどうかを[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="6a565-194">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6a565-195">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="6a565-195">zoomDisabled</span></span>|<span data-ttu-id="6a565-196">ブール値</span><span class="sxs-lookup"><span data-stu-id="6a565-196">Boolean</span></span>|<span data-ttu-id="6a565-197">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたズーム設定ウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="6a565-197">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6a565-198">siridisabled</span><span class="sxs-lookup"><span data-stu-id="6a565-198">siriDisabled</span></span>|<span data-ttu-id="6a565-199">ブール値</span><span class="sxs-lookup"><span data-stu-id="6a565-199">Boolean</span></span>|<span data-ttu-id="6a565-200">siri セットアップウィンドウが無効であるかどうかを示します ( [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承)</span><span class="sxs-lookup"><span data-stu-id="6a565-200">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6a565-201">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="6a565-201">diagnosticsDisabled</span></span>|<span data-ttu-id="6a565-202">ブール値</span><span class="sxs-lookup"><span data-stu-id="6a565-202">Boolean</span></span>|<span data-ttu-id="6a565-203">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承された診断セットアップウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="6a565-203">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6a565-204">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="6a565-204">displayToneSetupDisabled</span></span>|<span data-ttu-id="6a565-205">ブール値</span><span class="sxs-lookup"><span data-stu-id="6a565-205">Boolean</span></span>|<span data-ttu-id="6a565-206">displaytone セットアップ画面が無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="6a565-206">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6a565-207">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="6a565-207">privacyPaneDisabled</span></span>|<span data-ttu-id="6a565-208">ブール値</span><span class="sxs-lookup"><span data-stu-id="6a565-208">Boolean</span></span>|<span data-ttu-id="6a565-209">プライバシー画面が無効にされているかどうかを示します。 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="6a565-209">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6a565-210">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="6a565-210">iTunesPairingMode</span></span>|[<span data-ttu-id="6a565-211">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="6a565-211">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="6a565-212">iTunes ペアリングモードを示します。</span><span class="sxs-lookup"><span data-stu-id="6a565-212">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="6a565-213">可能な値は `disallow`、`allow`、`requiresCertificate` です。</span><span class="sxs-lookup"><span data-stu-id="6a565-213">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="6a565-214">managementcertificates</span><span class="sxs-lookup"><span data-stu-id="6a565-214">managementCertificates</span></span>|<span data-ttu-id="6a565-215">[managementcertificatewiththumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="6a565-215">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="6a565-216">Apple Configurator の管理証明書</span><span class="sxs-lookup"><span data-stu-id="6a565-216">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="6a565-217">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="6a565-217">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="6a565-218">ブール値</span><span class="sxs-lookup"><span data-stu-id="6a565-218">Boolean</span></span>|<span data-ttu-id="6a565-219">Android からの復元が無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="6a565-219">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="6a565-220">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="6a565-220">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="6a565-221">ブール値</span><span class="sxs-lookup"><span data-stu-id="6a565-221">Boolean</span></span>|<span data-ttu-id="6a565-222">構成済みの確認をデバイスが待機する必要があるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="6a565-222">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="6a565-223">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="6a565-223">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="6a565-224">Int32</span><span class="sxs-lookup"><span data-stu-id="6a565-224">Int32</span></span>|<span data-ttu-id="6a565-225">これにより、共有 iPad を使用できるユーザーの最大数が指定されます。</span><span class="sxs-lookup"><span data-stu-id="6a565-225">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="6a565-226">共有 iPad モードでのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="6a565-226">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="6a565-227">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="6a565-227">enableSharedIPad</span></span>|<span data-ttu-id="6a565-228">ブール値</span><span class="sxs-lookup"><span data-stu-id="6a565-228">Boolean</span></span>|<span data-ttu-id="6a565-229">これは、デバイスを、複数のユーザーシナリオを有効にするモードで登録するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6a565-229">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="6a565-230">共有 ipad にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="6a565-230">Only applicable in shared iPads.</span></span>|
|<span data-ttu-id="6a565-231">companyPortalVppTokenId</span><span class="sxs-lookup"><span data-stu-id="6a565-231">companyPortalVppTokenId</span></span>|<span data-ttu-id="6a565-232">String</span><span class="sxs-lookup"><span data-stu-id="6a565-232">String</span></span>|<span data-ttu-id="6a565-233">設定されている場合は、ポータルサイトのライセンスを展開するためにどの Vpp トークンを使用する必要があるかを示します。</span><span class="sxs-lookup"><span data-stu-id="6a565-233">If set, indicates which Vpp token should be used to deploy the Company Portal w/ device licensing.</span></span> <span data-ttu-id="6a565-234">このプロパティを設定するためには、' enableAuthenticationViaCompanyPortal ' を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6a565-234">'enableAuthenticationViaCompanyPortal' must be set in order for this property to be set.</span></span>|
|<span data-ttu-id="6a565-235">enableSingleAppEnrollmentMode</span><span class="sxs-lookup"><span data-stu-id="6a565-235">enableSingleAppEnrollmentMode</span></span>|<span data-ttu-id="6a565-236">ブール値</span><span class="sxs-lookup"><span data-stu-id="6a565-236">Boolean</span></span>|<span data-ttu-id="6a565-237">デバイスに対して、1つのアプリモードを有効にし、登録時にアプリロックを適用するように指示します。</span><span class="sxs-lookup"><span data-stu-id="6a565-237">Tells the device to enable single app mode and apply app-lock during enrollment.</span></span> <span data-ttu-id="6a565-238">既定値は false です。</span><span class="sxs-lookup"><span data-stu-id="6a565-238">Default is false.</span></span> <span data-ttu-id="6a565-239">このプロパティを設定するには、' enableAuthenticationViaCompanyPortal ' および ' companyPortalVppTokenId ' を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6a565-239">'enableAuthenticationViaCompanyPortal' and 'companyPortalVppTokenId' must be set for this property to be set.</span></span>|
|<span data-ttu-id="6a565-240">ホームボタンの無効化</span><span class="sxs-lookup"><span data-stu-id="6a565-240">homeButtonScreenDisabled</span></span>|<span data-ttu-id="6a565-241">ブール値</span><span class="sxs-lookup"><span data-stu-id="6a565-241">Boolean</span></span>|<span data-ttu-id="6a565-242">[ホームボタンの感度] 画面を無効にするかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="6a565-242">Indicates if home button sensitivity screen is disabled</span></span>|
|<span data-ttu-id="6a565-243">iMessageAndFaceTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="6a565-243">iMessageAndFaceTimeScreenDisabled</span></span>|<span data-ttu-id="6a565-244">ブール値</span><span class="sxs-lookup"><span data-stu-id="6a565-244">Boolean</span></span>|<span data-ttu-id="6a565-245">iMessage および FaceTime の画面が無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="6a565-245">Indicates if iMessage and FaceTime screen is disabled</span></span>|
|<span data-ttu-id="6a565-246">onboardingscreendisabled</span><span class="sxs-lookup"><span data-stu-id="6a565-246">onBoardingScreenDisabled</span></span>|<span data-ttu-id="6a565-247">ブール値</span><span class="sxs-lookup"><span data-stu-id="6a565-247">Boolean</span></span>|<span data-ttu-id="6a565-248">オンボードのセットアップ画面が無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="6a565-248">Indicates if onboarding setup screen is disabled</span></span>|
|<span data-ttu-id="6a565-249">screenTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="6a565-249">screenTimeScreenDisabled</span></span>|<span data-ttu-id="6a565-250">ブール値</span><span class="sxs-lookup"><span data-stu-id="6a565-250">Boolean</span></span>|<span data-ttu-id="6a565-251">画面のタイムアウト設定を無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6a565-251">Indicates if screen timeout setup is disabled</span></span>|
|<span data-ttu-id="6a565-252">シムの設定を無効にする</span><span class="sxs-lookup"><span data-stu-id="6a565-252">simSetupScreenDisabled</span></span>|<span data-ttu-id="6a565-253">ブール値</span><span class="sxs-lookup"><span data-stu-id="6a565-253">Boolean</span></span>|<span data-ttu-id="6a565-254">[シム] セットアップ画面が無効であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6a565-254">Indicates if the SIMSetup screen is disabled</span></span>|
|<span data-ttu-id="6a565-255">ソフトウェアの更新 creendisabled</span><span class="sxs-lookup"><span data-stu-id="6a565-255">softwareUpdateScreenDisabled</span></span>|<span data-ttu-id="6a565-256">ブール値</span><span class="sxs-lookup"><span data-stu-id="6a565-256">Boolean</span></span>|<span data-ttu-id="6a565-257">必須の [ソフトウェアの更新] 画面が無効であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6a565-257">Indicates if the mandatory sofware update screen is disabled</span></span>|
|<span data-ttu-id="6a565-258">watchMigrationScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="6a565-258">watchMigrationScreenDisabled</span></span>|<span data-ttu-id="6a565-259">ブール値</span><span class="sxs-lookup"><span data-stu-id="6a565-259">Boolean</span></span>|<span data-ttu-id="6a565-260">[移行の監視] 画面が無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="6a565-260">Indicates if the watch migration screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="6a565-261">応答</span><span class="sxs-lookup"><span data-stu-id="6a565-261">Response</span></span>
<span data-ttu-id="6a565-262">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6a565-262">If successful, this method returns a `200 OK` response code and an updated [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a565-263">例</span><span class="sxs-lookup"><span data-stu-id="6a565-263">Example</span></span>

### <a name="request"></a><span data-ttu-id="6a565-264">要求</span><span class="sxs-lookup"><span data-stu-id="6a565-264">Request</span></span>
<span data-ttu-id="6a565-265">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6a565-265">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6a565-266">応答</span><span class="sxs-lookup"><span data-stu-id="6a565-266">Response</span></span>
<span data-ttu-id="6a565-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6a565-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




