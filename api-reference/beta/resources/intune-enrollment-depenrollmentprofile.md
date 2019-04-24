---
title: depEnrollmentProfile リソースの種類
description: depEnrollmentProfile リソースは、Apple Device enrollment program (DEP) 登録プロファイルを表します。 この種類のプロファイルは、対応するデバイスが dep を使用して登録できるようになる前に、Apple DEP シリアル番号に割り当てる必要があります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a4a365ee8a83820789ecdbf199df5997b6e683e0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454182"
---
# <a name="depenrollmentprofile-resource-type"></a><span data-ttu-id="5b5a7-104">depEnrollmentProfile リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5b5a7-104">depEnrollmentProfile resource type</span></span>

> <span data-ttu-id="5b5a7-105">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5b5a7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5b5a7-106">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5b5a7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b5a7-107">depEnrollmentProfile リソースは、Apple Device enrollment program (DEP) 登録プロファイルを表します。</span><span class="sxs-lookup"><span data-stu-id="5b5a7-107">The depEnrollmentProfile resource represents an Apple Device Enrollment Program (DEP) enrollment profile.</span></span> <span data-ttu-id="5b5a7-108">この種類のプロファイルは、対応するデバイスが dep を使用して登録できるようになる前に、Apple DEP シリアル番号に割り当てる必要があります。</span><span class="sxs-lookup"><span data-stu-id="5b5a7-108">This type of profile must be assigned to Apple DEP serial numbers before the corresponding devices can enroll via DEP.</span></span>


<span data-ttu-id="5b5a7-109">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="5b5a7-109">Inherits from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>

## <a name="methods"></a><span data-ttu-id="5b5a7-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="5b5a7-110">Methods</span></span>
|<span data-ttu-id="5b5a7-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="5b5a7-111">Method</span></span>|<span data-ttu-id="5b5a7-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="5b5a7-112">Return Type</span></span>|<span data-ttu-id="5b5a7-113">説明</span><span class="sxs-lookup"><span data-stu-id="5b5a7-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5b5a7-114">リスト depEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="5b5a7-114">List depEnrollmentProfiles</span></span>](../api/intune-enrollment-depenrollmentprofile-list.md)|<span data-ttu-id="5b5a7-115">[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="5b5a7-115">[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) collection</span></span>|<span data-ttu-id="5b5a7-116">[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="5b5a7-116">List properties and relationships of the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="5b5a7-117">depEnrollmentProfile を取得する</span><span class="sxs-lookup"><span data-stu-id="5b5a7-117">Get depEnrollmentProfile</span></span>](../api/intune-enrollment-depenrollmentprofile-get.md)|[<span data-ttu-id="5b5a7-118">depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="5b5a7-118">depEnrollmentProfile</span></span>](../resources/intune-enrollment-depenrollmentprofile.md)|<span data-ttu-id="5b5a7-119">[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="5b5a7-119">Read properties and relationships of the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="5b5a7-120">depEnrollmentProfile を作成する</span><span class="sxs-lookup"><span data-stu-id="5b5a7-120">Create depEnrollmentProfile</span></span>](../api/intune-enrollment-depenrollmentprofile-create.md)|[<span data-ttu-id="5b5a7-121">depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="5b5a7-121">depEnrollmentProfile</span></span>](../resources/intune-enrollment-depenrollmentprofile.md)|<span data-ttu-id="5b5a7-122">新しい[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="5b5a7-122">Create a new [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="5b5a7-123">depEnrollmentProfile の削除</span><span class="sxs-lookup"><span data-stu-id="5b5a7-123">Delete depEnrollmentProfile</span></span>](../api/intune-enrollment-depenrollmentprofile-delete.md)|<span data-ttu-id="5b5a7-124">None</span><span class="sxs-lookup"><span data-stu-id="5b5a7-124">None</span></span>|<span data-ttu-id="5b5a7-125">[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="5b5a7-125">Deletes a [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md).</span></span>|
|[<span data-ttu-id="5b5a7-126">depEnrollmentProfile の更新</span><span class="sxs-lookup"><span data-stu-id="5b5a7-126">Update depEnrollmentProfile</span></span>](../api/intune-enrollment-depenrollmentprofile-update.md)|[<span data-ttu-id="5b5a7-127">depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="5b5a7-127">depEnrollmentProfile</span></span>](../resources/intune-enrollment-depenrollmentprofile.md)|<span data-ttu-id="5b5a7-128">[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="5b5a7-128">Update the properties of a [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5b5a7-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5b5a7-129">Properties</span></span>
|<span data-ttu-id="5b5a7-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5b5a7-130">Property</span></span>|<span data-ttu-id="5b5a7-131">型</span><span class="sxs-lookup"><span data-stu-id="5b5a7-131">Type</span></span>|<span data-ttu-id="5b5a7-132">説明</span><span class="sxs-lookup"><span data-stu-id="5b5a7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b5a7-133">id</span><span class="sxs-lookup"><span data-stu-id="5b5a7-133">id</span></span>|<span data-ttu-id="5b5a7-134">String</span><span class="sxs-lookup"><span data-stu-id="5b5a7-134">String</span></span>|<span data-ttu-id="5b5a7-135">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたオブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="5b5a7-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="5b5a7-136">displayName</span><span class="sxs-lookup"><span data-stu-id="5b5a7-136">displayName</span></span>|<span data-ttu-id="5b5a7-137">String</span><span class="sxs-lookup"><span data-stu-id="5b5a7-137">String</span></span>|<span data-ttu-id="5b5a7-138">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたプロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="5b5a7-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="5b5a7-139">説明</span><span class="sxs-lookup"><span data-stu-id="5b5a7-139">description</span></span>|<span data-ttu-id="5b5a7-140">String</span><span class="sxs-lookup"><span data-stu-id="5b5a7-140">String</span></span>|<span data-ttu-id="5b5a7-141">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたプロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="5b5a7-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="5b5a7-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="5b5a7-142">requiresUserAuthentication</span></span>|<span data-ttu-id="5b5a7-143">ブール型</span><span class="sxs-lookup"><span data-stu-id="5b5a7-143">Boolean</span></span>|<span data-ttu-id="5b5a7-144">プロファイルが[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承したユーザー認証を必要とするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5b5a7-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="5b5a7-145">configurationendpointurl</span><span class="sxs-lookup"><span data-stu-id="5b5a7-145">configurationEndpointUrl</span></span>|<span data-ttu-id="5b5a7-146">String</span><span class="sxs-lookup"><span data-stu-id="5b5a7-146">String</span></span>|<span data-ttu-id="5b5a7-147">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承された登録に使用する構成エンドポイント url</span><span class="sxs-lookup"><span data-stu-id="5b5a7-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="5b5a7-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="5b5a7-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="5b5a7-149">ブール型</span><span class="sxs-lookup"><span data-stu-id="5b5a7-149">Boolean</span></span>|<span data-ttu-id="5b5a7-150">会社のポータルではなく、Apple セットアップアシスタントを使用して認証することを示します。</span><span class="sxs-lookup"><span data-stu-id="5b5a7-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="5b5a7-151">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="5b5a7-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="5b5a7-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="5b5a7-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="5b5a7-153">ブール型</span><span class="sxs-lookup"><span data-stu-id="5b5a7-153">Boolean</span></span>|<span data-ttu-id="5b5a7-154">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたセットアップアシスタントの登録済みデバイスで、会社のポータルが必要であることを示します。</span><span class="sxs-lookup"><span data-stu-id="5b5a7-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="5b5a7-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="5b5a7-155">isDefault</span></span>|<span data-ttu-id="5b5a7-156">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="5b5a7-156">Boolean</span></span>|<span data-ttu-id="5b5a7-157">これが既定のプロファイルであるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="5b5a7-157">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="5b5a7-158">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="5b5a7-158">supervisedModeEnabled</span></span>|<span data-ttu-id="5b5a7-159">ブール型</span><span class="sxs-lookup"><span data-stu-id="5b5a7-159">Boolean</span></span>|<span data-ttu-id="5b5a7-160">監視モード、有効にする場合は True、それ以外の場合は false。</span><span class="sxs-lookup"><span data-stu-id="5b5a7-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="5b5a7-161">詳細https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intuneについては、「」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5b5a7-161">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="5b5a7-162">supportdepartment</span><span class="sxs-lookup"><span data-stu-id="5b5a7-162">supportDepartment</span></span>|<span data-ttu-id="5b5a7-163">String</span><span class="sxs-lookup"><span data-stu-id="5b5a7-163">String</span></span>|<span data-ttu-id="5b5a7-164">サポート部門の情報</span><span class="sxs-lookup"><span data-stu-id="5b5a7-164">Support department information</span></span>|
|<span data-ttu-id="5b5a7-165">pass codedisabled</span><span class="sxs-lookup"><span data-stu-id="5b5a7-165">passCodeDisabled</span></span>|<span data-ttu-id="5b5a7-166">ブール型</span><span class="sxs-lookup"><span data-stu-id="5b5a7-166">Boolean</span></span>|<span data-ttu-id="5b5a7-167">パスコードセットアップウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="5b5a7-167">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="5b5a7-168">ismandatory</span><span class="sxs-lookup"><span data-stu-id="5b5a7-168">isMandatory</span></span>|<span data-ttu-id="5b5a7-169">ブール型</span><span class="sxs-lookup"><span data-stu-id="5b5a7-169">Boolean</span></span>|<span data-ttu-id="5b5a7-170">プロファイルが必須であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="5b5a7-170">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="5b5a7-171">locationdisabled</span><span class="sxs-lookup"><span data-stu-id="5b5a7-171">locationDisabled</span></span>|<span data-ttu-id="5b5a7-172">ブール型</span><span class="sxs-lookup"><span data-stu-id="5b5a7-172">Boolean</span></span>|<span data-ttu-id="5b5a7-173">場所サービスの設定ウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="5b5a7-173">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="5b5a7-174">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="5b5a7-174">supportPhoneNumber</span></span>|<span data-ttu-id="5b5a7-175">String</span><span class="sxs-lookup"><span data-stu-id="5b5a7-175">String</span></span>|<span data-ttu-id="5b5a7-176">サポート電話番号</span><span class="sxs-lookup"><span data-stu-id="5b5a7-176">Support phone number</span></span>|
|<span data-ttu-id="5b5a7-177">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="5b5a7-177">iTunesPairingMode</span></span>|[<span data-ttu-id="5b5a7-178">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="5b5a7-178">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="5b5a7-179">iTunes ペアリングモードを示します。</span><span class="sxs-lookup"><span data-stu-id="5b5a7-179">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="5b5a7-180">使用可能な値は、`disallow`、`allow`、`requiresCertificate` です。</span><span class="sxs-lookup"><span data-stu-id="5b5a7-180">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="5b5a7-181">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="5b5a7-181">profileRemovalDisabled</span></span>|<span data-ttu-id="5b5a7-182">ブール型</span><span class="sxs-lookup"><span data-stu-id="5b5a7-182">Boolean</span></span>|<span data-ttu-id="5b5a7-183">プロファイルの削除オプションが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="5b5a7-183">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="5b5a7-184">managementcertificates</span><span class="sxs-lookup"><span data-stu-id="5b5a7-184">managementCertificates</span></span>|<span data-ttu-id="5b5a7-185">[managementcertificatewiththumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="5b5a7-185">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="5b5a7-186">Apple Configurator の管理証明書</span><span class="sxs-lookup"><span data-stu-id="5b5a7-186">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="5b5a7-187">restoreblocked</span><span class="sxs-lookup"><span data-stu-id="5b5a7-187">restoreBlocked</span></span>|<span data-ttu-id="5b5a7-188">ブール型</span><span class="sxs-lookup"><span data-stu-id="5b5a7-188">Boolean</span></span>|<span data-ttu-id="5b5a7-189">セットアップウィンドウの復元がブロックされているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="5b5a7-189">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="5b5a7-190">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="5b5a7-190">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="5b5a7-191">ブール型</span><span class="sxs-lookup"><span data-stu-id="5b5a7-191">Boolean</span></span>|<span data-ttu-id="5b5a7-192">Android からの復元が無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="5b5a7-192">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="5b5a7-193">りんご eiddisabled</span><span class="sxs-lookup"><span data-stu-id="5b5a7-193">appleIdDisabled</span></span>|<span data-ttu-id="5b5a7-194">ブール型</span><span class="sxs-lookup"><span data-stu-id="5b5a7-194">Boolean</span></span>|<span data-ttu-id="5b5a7-195">Apple id のセットアップウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="5b5a7-195">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="5b5a7-196">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="5b5a7-196">termsAndConditionsDisabled</span></span>|<span data-ttu-id="5b5a7-197">ブール型</span><span class="sxs-lookup"><span data-stu-id="5b5a7-197">Boolean</span></span>|<span data-ttu-id="5b5a7-198">[使用条件] セットアップウィンドウが無効かどうかを示します</span><span class="sxs-lookup"><span data-stu-id="5b5a7-198">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="5b5a7-199">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="5b5a7-199">touchIdDisabled</span></span>|<span data-ttu-id="5b5a7-200">ブール型</span><span class="sxs-lookup"><span data-stu-id="5b5a7-200">Boolean</span></span>|<span data-ttu-id="5b5a7-201">タッチ id のセットアップウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="5b5a7-201">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="5b5a7-202">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="5b5a7-202">applePayDisabled</span></span>|<span data-ttu-id="5b5a7-203">ブール型</span><span class="sxs-lookup"><span data-stu-id="5b5a7-203">Boolean</span></span>|<span data-ttu-id="5b5a7-204">Apple の支払い設定ウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="5b5a7-204">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="5b5a7-205">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="5b5a7-205">zoomDisabled</span></span>|<span data-ttu-id="5b5a7-206">ブール型</span><span class="sxs-lookup"><span data-stu-id="5b5a7-206">Boolean</span></span>|<span data-ttu-id="5b5a7-207">ズーム設定ウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="5b5a7-207">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="5b5a7-208">siridisabled</span><span class="sxs-lookup"><span data-stu-id="5b5a7-208">siriDisabled</span></span>|<span data-ttu-id="5b5a7-209">ブール型</span><span class="sxs-lookup"><span data-stu-id="5b5a7-209">Boolean</span></span>|<span data-ttu-id="5b5a7-210">siri セットアップウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="5b5a7-210">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="5b5a7-211">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="5b5a7-211">diagnosticsDisabled</span></span>|<span data-ttu-id="5b5a7-212">ブール型</span><span class="sxs-lookup"><span data-stu-id="5b5a7-212">Boolean</span></span>|<span data-ttu-id="5b5a7-213">診断セットアップウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="5b5a7-213">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="5b5a7-214">macosregistrationdisabled</span><span class="sxs-lookup"><span data-stu-id="5b5a7-214">macOSRegistrationDisabled</span></span>|<span data-ttu-id="5b5a7-215">ブール型</span><span class="sxs-lookup"><span data-stu-id="5b5a7-215">Boolean</span></span>|<span data-ttu-id="5b5a7-216">Mac OS 登録が無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="5b5a7-216">Indicates if Mac OS registration is disabled</span></span>|
|<span data-ttu-id="5b5a7-217">macOSFileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="5b5a7-217">macOSFileVaultDisabled</span></span>|<span data-ttu-id="5b5a7-218">ブール型</span><span class="sxs-lookup"><span data-stu-id="5b5a7-218">Boolean</span></span>|<span data-ttu-id="5b5a7-219">Mac OS ファイルボルトが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="5b5a7-219">Indicates if Mac OS file vault is disabled</span></span>|
|<span data-ttu-id="5b5a7-220">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="5b5a7-220">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="5b5a7-221">ブール型</span><span class="sxs-lookup"><span data-stu-id="5b5a7-221">Boolean</span></span>|<span data-ttu-id="5b5a7-222">構成済みの確認をデバイスが待機する必要があるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="5b5a7-222">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="5b5a7-223">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="5b5a7-223">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="5b5a7-224">Int32</span><span class="sxs-lookup"><span data-stu-id="5b5a7-224">Int32</span></span>|<span data-ttu-id="5b5a7-225">これにより、共有 iPad を使用できるユーザーの最大数が指定されます。</span><span class="sxs-lookup"><span data-stu-id="5b5a7-225">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="5b5a7-226">共有 iPad モードでのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="5b5a7-226">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="5b5a7-227">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="5b5a7-227">enableSharedIPad</span></span>|<span data-ttu-id="5b5a7-228">ブール型</span><span class="sxs-lookup"><span data-stu-id="5b5a7-228">Boolean</span></span>|<span data-ttu-id="5b5a7-229">これは、デバイスを、複数のユーザーシナリオを有効にするモードで登録するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5b5a7-229">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="5b5a7-230">共有 ipad にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="5b5a7-230">Only applicable in shared iPads.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5b5a7-231">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5b5a7-231">Relationships</span></span>
<span data-ttu-id="5b5a7-232">なし</span><span class="sxs-lookup"><span data-stu-id="5b5a7-232">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5b5a7-233">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5b5a7-233">JSON Representation</span></span>
<span data-ttu-id="5b5a7-234">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5b5a7-234">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.depEnrollmentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.depEnrollmentProfile",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "String",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true,
  "isDefault": true,
  "supervisedModeEnabled": true,
  "supportDepartment": "String",
  "passCodeDisabled": true,
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "String",
  "iTunesPairingMode": "String",
  "profileRemovalDisabled": true,
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
      "thumbprint": "String",
      "certificate": "String"
    }
  ],
  "restoreBlocked": true,
  "restoreFromAndroidDisabled": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "macOSRegistrationDisabled": true,
  "macOSFileVaultDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 1024,
  "enableSharedIPad": true
}
```





