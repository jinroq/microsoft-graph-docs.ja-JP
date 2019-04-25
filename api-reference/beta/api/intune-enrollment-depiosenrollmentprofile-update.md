---
title: depIOSEnrollmentProfile の更新
description: depIOSEnrollmentProfile オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3141aaf65cb7d7fca01cf9a9849aaed7ee310bbc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32533955"
---
# <a name="update-depiosenrollmentprofile"></a><span data-ttu-id="d63b4-103">depIOSEnrollmentProfile の更新</span><span class="sxs-lookup"><span data-stu-id="d63b4-103">Update depIOSEnrollmentProfile</span></span>

> <span data-ttu-id="d63b4-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d63b4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d63b4-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d63b4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d63b4-106">[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d63b4-106">Update the properties of a [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d63b4-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="d63b4-107">Prerequisites</span></span>
<span data-ttu-id="d63b4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d63b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d63b4-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d63b4-110">Permission type</span></span>|<span data-ttu-id="d63b4-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d63b4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d63b4-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d63b4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d63b4-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d63b4-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d63b4-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d63b4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d63b4-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d63b4-115">Not supported.</span></span>|
|<span data-ttu-id="d63b4-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d63b4-116">Application</span></span>|<span data-ttu-id="d63b4-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d63b4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d63b4-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d63b4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="d63b4-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d63b4-119">Request headers</span></span>
|<span data-ttu-id="d63b4-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d63b4-120">Header</span></span>|<span data-ttu-id="d63b4-121">値</span><span class="sxs-lookup"><span data-stu-id="d63b4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d63b4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d63b4-122">Authorization</span></span>|<span data-ttu-id="d63b4-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="d63b4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d63b4-124">承諾</span><span class="sxs-lookup"><span data-stu-id="d63b4-124">Accept</span></span>|<span data-ttu-id="d63b4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d63b4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d63b4-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="d63b4-126">Request body</span></span>
<span data-ttu-id="d63b4-127">要求本文で、 [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d63b4-127">In the request body, supply a JSON representation for the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

<span data-ttu-id="d63b4-128">次の表に、 [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d63b4-128">The following table shows the properties that are required when you create the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md).</span></span>

|<span data-ttu-id="d63b4-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d63b4-129">Property</span></span>|<span data-ttu-id="d63b4-130">型</span><span class="sxs-lookup"><span data-stu-id="d63b4-130">Type</span></span>|<span data-ttu-id="d63b4-131">説明</span><span class="sxs-lookup"><span data-stu-id="d63b4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d63b4-132">id</span><span class="sxs-lookup"><span data-stu-id="d63b4-132">id</span></span>|<span data-ttu-id="d63b4-133">String</span><span class="sxs-lookup"><span data-stu-id="d63b4-133">String</span></span>|<span data-ttu-id="d63b4-134">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたオブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="d63b4-134">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d63b4-135">displayName</span><span class="sxs-lookup"><span data-stu-id="d63b4-135">displayName</span></span>|<span data-ttu-id="d63b4-136">String</span><span class="sxs-lookup"><span data-stu-id="d63b4-136">String</span></span>|<span data-ttu-id="d63b4-137">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたプロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="d63b4-137">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d63b4-138">description</span><span class="sxs-lookup"><span data-stu-id="d63b4-138">description</span></span>|<span data-ttu-id="d63b4-139">String</span><span class="sxs-lookup"><span data-stu-id="d63b4-139">String</span></span>|<span data-ttu-id="d63b4-140">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたプロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="d63b4-140">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d63b4-141">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="d63b4-141">requiresUserAuthentication</span></span>|<span data-ttu-id="d63b4-142">ブール値</span><span class="sxs-lookup"><span data-stu-id="d63b4-142">Boolean</span></span>|<span data-ttu-id="d63b4-143">プロファイルが[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承したユーザー認証を必要とするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d63b4-143">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d63b4-144">configurationendpointurl</span><span class="sxs-lookup"><span data-stu-id="d63b4-144">configurationEndpointUrl</span></span>|<span data-ttu-id="d63b4-145">String</span><span class="sxs-lookup"><span data-stu-id="d63b4-145">String</span></span>|<span data-ttu-id="d63b4-146">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承された登録に使用する構成エンドポイント url</span><span class="sxs-lookup"><span data-stu-id="d63b4-146">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d63b4-147">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="d63b4-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="d63b4-148">ブール値</span><span class="sxs-lookup"><span data-stu-id="d63b4-148">Boolean</span></span>|<span data-ttu-id="d63b4-149">会社のポータルではなく、Apple セットアップアシスタントを使用して認証することを示します。</span><span class="sxs-lookup"><span data-stu-id="d63b4-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="d63b4-150">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="d63b4-150">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d63b4-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="d63b4-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="d63b4-152">ブール値</span><span class="sxs-lookup"><span data-stu-id="d63b4-152">Boolean</span></span>|<span data-ttu-id="d63b4-153">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたセットアップアシスタントの登録済みデバイスで、会社のポータルが必要であることを示します。</span><span class="sxs-lookup"><span data-stu-id="d63b4-153">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d63b4-154">isDefault</span><span class="sxs-lookup"><span data-stu-id="d63b4-154">isDefault</span></span>|<span data-ttu-id="d63b4-155">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="d63b4-155">Boolean</span></span>|<span data-ttu-id="d63b4-156">これが[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承された既定のプロファイルであるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d63b4-156">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d63b4-157">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="d63b4-157">supervisedModeEnabled</span></span>|<span data-ttu-id="d63b4-158">ブール値</span><span class="sxs-lookup"><span data-stu-id="d63b4-158">Boolean</span></span>|<span data-ttu-id="d63b4-159">監視モード、有効にする場合は True、それ以外の場合は false。</span><span class="sxs-lookup"><span data-stu-id="d63b4-159">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="d63b4-160">詳細https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intuneについては、「」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d63b4-160">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="d63b4-161">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="d63b4-161">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d63b4-162">supportdepartment</span><span class="sxs-lookup"><span data-stu-id="d63b4-162">supportDepartment</span></span>|<span data-ttu-id="d63b4-163">String</span><span class="sxs-lookup"><span data-stu-id="d63b4-163">String</span></span>|<span data-ttu-id="d63b4-164">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたサポート部署情報</span><span class="sxs-lookup"><span data-stu-id="d63b4-164">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d63b4-165">pass codedisabled</span><span class="sxs-lookup"><span data-stu-id="d63b4-165">passCodeDisabled</span></span>|<span data-ttu-id="d63b4-166">ブール値</span><span class="sxs-lookup"><span data-stu-id="d63b4-166">Boolean</span></span>|<span data-ttu-id="d63b4-167">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたパスコードセットアップウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="d63b4-167">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d63b4-168">ismandatory</span><span class="sxs-lookup"><span data-stu-id="d63b4-168">isMandatory</span></span>|<span data-ttu-id="d63b4-169">ブール値</span><span class="sxs-lookup"><span data-stu-id="d63b4-169">Boolean</span></span>|<span data-ttu-id="d63b4-170">プロファイルが[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d63b4-170">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d63b4-171">locationdisabled</span><span class="sxs-lookup"><span data-stu-id="d63b4-171">locationDisabled</span></span>|<span data-ttu-id="d63b4-172">ブール値</span><span class="sxs-lookup"><span data-stu-id="d63b4-172">Boolean</span></span>|<span data-ttu-id="d63b4-173">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承された場所サービスのセットアップウィンドウが無効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d63b4-173">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d63b4-174">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="d63b4-174">supportPhoneNumber</span></span>|<span data-ttu-id="d63b4-175">String</span><span class="sxs-lookup"><span data-stu-id="d63b4-175">String</span></span>|<span data-ttu-id="d63b4-176">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたサポート電話番号</span><span class="sxs-lookup"><span data-stu-id="d63b4-176">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d63b4-177">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="d63b4-177">profileRemovalDisabled</span></span>|<span data-ttu-id="d63b4-178">ブール値</span><span class="sxs-lookup"><span data-stu-id="d63b4-178">Boolean</span></span>|<span data-ttu-id="d63b4-179">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたプロファイル削除オプションが無効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d63b4-179">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d63b4-180">restoreblocked</span><span class="sxs-lookup"><span data-stu-id="d63b4-180">restoreBlocked</span></span>|<span data-ttu-id="d63b4-181">ブール値</span><span class="sxs-lookup"><span data-stu-id="d63b4-181">Boolean</span></span>|<span data-ttu-id="d63b4-182">復元のセットアップウィンドウが[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d63b4-182">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d63b4-183">りんご eiddisabled</span><span class="sxs-lookup"><span data-stu-id="d63b4-183">appleIdDisabled</span></span>|<span data-ttu-id="d63b4-184">ブール値</span><span class="sxs-lookup"><span data-stu-id="d63b4-184">Boolean</span></span>|<span data-ttu-id="d63b4-185">Apple id のセットアップウィンドウが無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="d63b4-185">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d63b4-186">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="d63b4-186">termsAndConditionsDisabled</span></span>|<span data-ttu-id="d63b4-187">ブール値</span><span class="sxs-lookup"><span data-stu-id="d63b4-187">Boolean</span></span>|<span data-ttu-id="d63b4-188">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承された [使用条件] 設定ウィンドウを無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d63b4-188">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d63b4-189">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="d63b4-189">touchIdDisabled</span></span>|<span data-ttu-id="d63b4-190">ブール値</span><span class="sxs-lookup"><span data-stu-id="d63b4-190">Boolean</span></span>|<span data-ttu-id="d63b4-191">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたタッチ id セットアップウィンドウを無効にするかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="d63b4-191">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d63b4-192">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="d63b4-192">applePayDisabled</span></span>|<span data-ttu-id="d63b4-193">ブール値</span><span class="sxs-lookup"><span data-stu-id="d63b4-193">Boolean</span></span>|<span data-ttu-id="d63b4-194">Apple の [支払い設定] ウィンドウが無効にされているかどうかを[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="d63b4-194">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d63b4-195">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="d63b4-195">zoomDisabled</span></span>|<span data-ttu-id="d63b4-196">ブール値</span><span class="sxs-lookup"><span data-stu-id="d63b4-196">Boolean</span></span>|<span data-ttu-id="d63b4-197">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたズーム設定ウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="d63b4-197">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d63b4-198">siridisabled</span><span class="sxs-lookup"><span data-stu-id="d63b4-198">siriDisabled</span></span>|<span data-ttu-id="d63b4-199">ブール値</span><span class="sxs-lookup"><span data-stu-id="d63b4-199">Boolean</span></span>|<span data-ttu-id="d63b4-200">siri セットアップウィンドウが無効であるかどうかを示します ( [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承)</span><span class="sxs-lookup"><span data-stu-id="d63b4-200">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d63b4-201">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="d63b4-201">diagnosticsDisabled</span></span>|<span data-ttu-id="d63b4-202">ブール値</span><span class="sxs-lookup"><span data-stu-id="d63b4-202">Boolean</span></span>|<span data-ttu-id="d63b4-203">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承された診断セットアップウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="d63b4-203">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d63b4-204">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="d63b4-204">displayToneSetupDisabled</span></span>|<span data-ttu-id="d63b4-205">ブール値</span><span class="sxs-lookup"><span data-stu-id="d63b4-205">Boolean</span></span>|<span data-ttu-id="d63b4-206">displaytone セットアップ画面が無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="d63b4-206">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d63b4-207">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="d63b4-207">privacyPaneDisabled</span></span>|<span data-ttu-id="d63b4-208">ブール値</span><span class="sxs-lookup"><span data-stu-id="d63b4-208">Boolean</span></span>|<span data-ttu-id="d63b4-209">プライバシー画面が無効にされているかどうかを示します。 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="d63b4-209">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d63b4-210">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="d63b4-210">deviceNameTemplate</span></span>|<span data-ttu-id="d63b4-211">String</span><span class="sxs-lookup"><span data-stu-id="d63b4-211">String</span></span>|<span data-ttu-id="d63b4-212">リテラルまたは名前のパターンを設定します。</span><span class="sxs-lookup"><span data-stu-id="d63b4-212">Sets a literal or name pattern.</span></span> <span data-ttu-id="d63b4-213">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="d63b4-213">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d63b4-214">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="d63b4-214">iTunesPairingMode</span></span>|[<span data-ttu-id="d63b4-215">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="d63b4-215">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="d63b4-216">iTunes ペアリングモードを示します。</span><span class="sxs-lookup"><span data-stu-id="d63b4-216">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="d63b4-217">使用可能な値は、`disallow`、`allow`、`requiresCertificate` です。</span><span class="sxs-lookup"><span data-stu-id="d63b4-217">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="d63b4-218">managementcertificates</span><span class="sxs-lookup"><span data-stu-id="d63b4-218">managementCertificates</span></span>|<span data-ttu-id="d63b4-219">[managementcertificatewiththumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d63b4-219">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="d63b4-220">Apple Configurator の管理証明書</span><span class="sxs-lookup"><span data-stu-id="d63b4-220">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="d63b4-221">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="d63b4-221">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="d63b4-222">ブール値</span><span class="sxs-lookup"><span data-stu-id="d63b4-222">Boolean</span></span>|<span data-ttu-id="d63b4-223">Android からの復元が無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="d63b4-223">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="d63b4-224">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="d63b4-224">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="d63b4-225">ブール値</span><span class="sxs-lookup"><span data-stu-id="d63b4-225">Boolean</span></span>|<span data-ttu-id="d63b4-226">構成済みの確認をデバイスが待機する必要があるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="d63b4-226">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="d63b4-227">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="d63b4-227">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="d63b4-228">Int32</span><span class="sxs-lookup"><span data-stu-id="d63b4-228">Int32</span></span>|<span data-ttu-id="d63b4-229">これにより、共有 iPad を使用できるユーザーの最大数が指定されます。</span><span class="sxs-lookup"><span data-stu-id="d63b4-229">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="d63b4-230">共有 iPad モードでのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="d63b4-230">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="d63b4-231">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="d63b4-231">enableSharedIPad</span></span>|<span data-ttu-id="d63b4-232">ブール値</span><span class="sxs-lookup"><span data-stu-id="d63b4-232">Boolean</span></span>|<span data-ttu-id="d63b4-233">これは、デバイスを、複数のユーザーシナリオを有効にするモードで登録するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d63b4-233">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="d63b4-234">共有 ipad にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="d63b4-234">Only applicable in shared iPads.</span></span>|
|<span data-ttu-id="d63b4-235">companyPortalVppTokenId</span><span class="sxs-lookup"><span data-stu-id="d63b4-235">companyPortalVppTokenId</span></span>|<span data-ttu-id="d63b4-236">String</span><span class="sxs-lookup"><span data-stu-id="d63b4-236">String</span></span>|<span data-ttu-id="d63b4-237">設定されている場合は、ポータルサイトのライセンスを展開するためにどの Vpp トークンを使用する必要があるかを示します。</span><span class="sxs-lookup"><span data-stu-id="d63b4-237">If set, indicates which Vpp token should be used to deploy the Company Portal w/ device licensing.</span></span> <span data-ttu-id="d63b4-238">このプロパティを設定するためには、' enableAuthenticationViaCompanyPortal ' を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d63b4-238">'enableAuthenticationViaCompanyPortal' must be set in order for this property to be set.</span></span>|
|<span data-ttu-id="d63b4-239">enableSingleAppEnrollmentMode</span><span class="sxs-lookup"><span data-stu-id="d63b4-239">enableSingleAppEnrollmentMode</span></span>|<span data-ttu-id="d63b4-240">ブール値</span><span class="sxs-lookup"><span data-stu-id="d63b4-240">Boolean</span></span>|<span data-ttu-id="d63b4-241">デバイスに対して、1つのアプリモードを有効にし、登録時にアプリロックを適用するように指示します。</span><span class="sxs-lookup"><span data-stu-id="d63b4-241">Tells the device to enable single app mode and apply app-lock during enrollment.</span></span> <span data-ttu-id="d63b4-242">既定値は false です。</span><span class="sxs-lookup"><span data-stu-id="d63b4-242">Default is false.</span></span> <span data-ttu-id="d63b4-243">このプロパティを設定するには、' enableAuthenticationViaCompanyPortal ' および ' companyPortalVppTokenId ' を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d63b4-243">'enableAuthenticationViaCompanyPortal' and 'companyPortalVppTokenId' must be set for this property to be set.</span></span>|
|<span data-ttu-id="d63b4-244">ホームボタンの無効化</span><span class="sxs-lookup"><span data-stu-id="d63b4-244">homeButtonScreenDisabled</span></span>|<span data-ttu-id="d63b4-245">ブール値</span><span class="sxs-lookup"><span data-stu-id="d63b4-245">Boolean</span></span>|<span data-ttu-id="d63b4-246">[ホームボタンの感度] 画面を無効にするかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="d63b4-246">Indicates if home button sensitivity screen is disabled</span></span>|
|<span data-ttu-id="d63b4-247">iMessageAndFaceTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="d63b4-247">iMessageAndFaceTimeScreenDisabled</span></span>|<span data-ttu-id="d63b4-248">ブール値</span><span class="sxs-lookup"><span data-stu-id="d63b4-248">Boolean</span></span>|<span data-ttu-id="d63b4-249">iMessage および FaceTime の画面が無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="d63b4-249">Indicates if iMessage and FaceTime screen is disabled</span></span>|
|<span data-ttu-id="d63b4-250">onboardingscreendisabled</span><span class="sxs-lookup"><span data-stu-id="d63b4-250">onBoardingScreenDisabled</span></span>|<span data-ttu-id="d63b4-251">ブール値</span><span class="sxs-lookup"><span data-stu-id="d63b4-251">Boolean</span></span>|<span data-ttu-id="d63b4-252">オンボードのセットアップ画面が無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="d63b4-252">Indicates if onboarding setup screen is disabled</span></span>|
|<span data-ttu-id="d63b4-253">screenTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="d63b4-253">screenTimeScreenDisabled</span></span>|<span data-ttu-id="d63b4-254">ブール値</span><span class="sxs-lookup"><span data-stu-id="d63b4-254">Boolean</span></span>|<span data-ttu-id="d63b4-255">画面のタイムアウト設定を無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d63b4-255">Indicates if screen timeout setup is disabled</span></span>|
|<span data-ttu-id="d63b4-256">シムの設定を無効にする</span><span class="sxs-lookup"><span data-stu-id="d63b4-256">simSetupScreenDisabled</span></span>|<span data-ttu-id="d63b4-257">ブール値</span><span class="sxs-lookup"><span data-stu-id="d63b4-257">Boolean</span></span>|<span data-ttu-id="d63b4-258">[シム] セットアップ画面が無効であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d63b4-258">Indicates if the SIMSetup screen is disabled</span></span>|
|<span data-ttu-id="d63b4-259">ソフトウェアの更新 creendisabled</span><span class="sxs-lookup"><span data-stu-id="d63b4-259">softwareUpdateScreenDisabled</span></span>|<span data-ttu-id="d63b4-260">ブール値</span><span class="sxs-lookup"><span data-stu-id="d63b4-260">Boolean</span></span>|<span data-ttu-id="d63b4-261">必須の [ソフトウェアの更新] 画面が無効であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d63b4-261">Indicates if the mandatory sofware update screen is disabled</span></span>|
|<span data-ttu-id="d63b4-262">watchMigrationScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="d63b4-262">watchMigrationScreenDisabled</span></span>|<span data-ttu-id="d63b4-263">ブール値</span><span class="sxs-lookup"><span data-stu-id="d63b4-263">Boolean</span></span>|<span data-ttu-id="d63b4-264">[移行の監視] 画面が無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="d63b4-264">Indicates if the watch migration screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="d63b4-265">応答</span><span class="sxs-lookup"><span data-stu-id="d63b4-265">Response</span></span>
<span data-ttu-id="d63b4-266">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d63b4-266">If successful, this method returns a `200 OK` response code and an updated [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d63b4-267">例</span><span class="sxs-lookup"><span data-stu-id="d63b4-267">Example</span></span>

### <a name="request"></a><span data-ttu-id="d63b4-268">要求</span><span class="sxs-lookup"><span data-stu-id="d63b4-268">Request</span></span>
<span data-ttu-id="d63b4-269">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d63b4-269">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d63b4-270">応答</span><span class="sxs-lookup"><span data-stu-id="d63b4-270">Response</span></span>
<span data-ttu-id="d63b4-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d63b4-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





