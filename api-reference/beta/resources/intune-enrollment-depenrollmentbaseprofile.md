---
title: depEnrollmentBaseProfile リソースの種類
description: DepEnrollmentBaseProfile リソースでは、アップル デバイスの登録プログラム (DEP) の登録プロファイルを表します。 このタイプのプロファイルは、DEP. を使用して対応するデバイスを登録する前に、Apple の DEP のシリアル番号を割り当てる必要があります。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f8b820959e5515a575e4f074a2762794a15e7f5c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423756"
---
# <a name="depenrollmentbaseprofile-resource-type"></a><span data-ttu-id="ae1c0-104">depEnrollmentBaseProfile リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ae1c0-104">depEnrollmentBaseProfile resource type</span></span>

> <span data-ttu-id="ae1c0-105">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ae1c0-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ae1c0-106">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae1c0-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ae1c0-107">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ae1c0-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae1c0-108">DepEnrollmentBaseProfile リソースでは、アップル デバイスの登録プログラム (DEP) の登録プロファイルを表します。</span><span class="sxs-lookup"><span data-stu-id="ae1c0-108">The DepEnrollmentBaseProfile resource represents an Apple Device Enrollment Program (DEP) enrollment profile.</span></span> <span data-ttu-id="ae1c0-109">このタイプのプロファイルは、DEP. を使用して対応するデバイスを登録する前に、Apple の DEP のシリアル番号を割り当てる必要があります。</span><span class="sxs-lookup"><span data-stu-id="ae1c0-109">This type of profile must be assigned to Apple DEP serial numbers before the corresponding devices can enroll via DEP.</span></span>


<span data-ttu-id="ae1c0-110">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="ae1c0-110">Inherits from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>

## <a name="methods"></a><span data-ttu-id="ae1c0-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="ae1c0-111">Methods</span></span>
|<span data-ttu-id="ae1c0-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="ae1c0-112">Method</span></span>|<span data-ttu-id="ae1c0-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ae1c0-113">Return Type</span></span>|<span data-ttu-id="ae1c0-114">説明</span><span class="sxs-lookup"><span data-stu-id="ae1c0-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ae1c0-115">リスト depEnrollmentBaseProfiles</span><span class="sxs-lookup"><span data-stu-id="ae1c0-115">List depEnrollmentBaseProfiles</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-list.md)|<span data-ttu-id="ae1c0-116">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ae1c0-116">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) collection</span></span>|<span data-ttu-id="ae1c0-117">[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="ae1c0-117">List properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) objects.</span></span>|
|[<span data-ttu-id="ae1c0-118">DepEnrollmentBaseProfile を取得します。</span><span class="sxs-lookup"><span data-stu-id="ae1c0-118">Get depEnrollmentBaseProfile</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-get.md)|[<span data-ttu-id="ae1c0-119">depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="ae1c0-119">depEnrollmentBaseProfile</span></span>](../resources/intune-enrollment-depenrollmentbaseprofile.md)|<span data-ttu-id="ae1c0-120">[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ae1c0-120">Read properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ae1c0-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ae1c0-121">Properties</span></span>
|<span data-ttu-id="ae1c0-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ae1c0-122">Property</span></span>|<span data-ttu-id="ae1c0-123">型</span><span class="sxs-lookup"><span data-stu-id="ae1c0-123">Type</span></span>|<span data-ttu-id="ae1c0-124">説明</span><span class="sxs-lookup"><span data-stu-id="ae1c0-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae1c0-125">id</span><span class="sxs-lookup"><span data-stu-id="ae1c0-125">id</span></span>|<span data-ttu-id="ae1c0-126">String</span><span class="sxs-lookup"><span data-stu-id="ae1c0-126">String</span></span>|<span data-ttu-id="ae1c0-127">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるオブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="ae1c0-127">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ae1c0-128">displayName</span><span class="sxs-lookup"><span data-stu-id="ae1c0-128">displayName</span></span>|<span data-ttu-id="ae1c0-129">String</span><span class="sxs-lookup"><span data-stu-id="ae1c0-129">String</span></span>|<span data-ttu-id="ae1c0-130">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるプロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="ae1c0-130">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ae1c0-131">説明</span><span class="sxs-lookup"><span data-stu-id="ae1c0-131">description</span></span>|<span data-ttu-id="ae1c0-132">String</span><span class="sxs-lookup"><span data-stu-id="ae1c0-132">String</span></span>|<span data-ttu-id="ae1c0-133">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるプロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="ae1c0-133">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ae1c0-134">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="ae1c0-134">requiresUserAuthentication</span></span>|<span data-ttu-id="ae1c0-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae1c0-135">Boolean</span></span>|<span data-ttu-id="ae1c0-136">プロファイルに[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるのユーザー認証が必要なかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="ae1c0-136">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ae1c0-137">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="ae1c0-137">configurationEndpointUrl</span></span>|<span data-ttu-id="ae1c0-138">String</span><span class="sxs-lookup"><span data-stu-id="ae1c0-138">String</span></span>|<span data-ttu-id="ae1c0-139">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から登録の継承を使用するエンドポイントの url を構成</span><span class="sxs-lookup"><span data-stu-id="ae1c0-139">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ae1c0-140">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="ae1c0-140">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="ae1c0-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae1c0-141">Boolean</span></span>|<span data-ttu-id="ae1c0-142">アップルらくらく企業ポータルではなくを使用して認証することを示します。</span><span class="sxs-lookup"><span data-stu-id="ae1c0-142">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="ae1c0-143">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="ae1c0-143">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ae1c0-144">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="ae1c0-144">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="ae1c0-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae1c0-145">Boolean</span></span>|<span data-ttu-id="ae1c0-146">継承セットアップ アシスタントが登録されているデバイスは、 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)からの会社のポータルが必要であることを示します。</span><span class="sxs-lookup"><span data-stu-id="ae1c0-146">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ae1c0-147">isDefault</span><span class="sxs-lookup"><span data-stu-id="ae1c0-147">isDefault</span></span>|<span data-ttu-id="ae1c0-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae1c0-148">Boolean</span></span>|<span data-ttu-id="ae1c0-149">これは、既定のプロファイルであるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="ae1c0-149">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="ae1c0-150">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="ae1c0-150">supervisedModeEnabled</span></span>|<span data-ttu-id="ae1c0-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae1c0-151">Boolean</span></span>|<span data-ttu-id="ae1c0-152">コールを管理モードを有効にする、false それ以外の場合は True です。</span><span class="sxs-lookup"><span data-stu-id="ae1c0-152">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="ae1c0-153">参照してくださいhttps://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intuneの追加情報です。</span><span class="sxs-lookup"><span data-stu-id="ae1c0-153">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="ae1c0-154">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="ae1c0-154">supportDepartment</span></span>|<span data-ttu-id="ae1c0-155">String</span><span class="sxs-lookup"><span data-stu-id="ae1c0-155">String</span></span>|<span data-ttu-id="ae1c0-156">サポート部門の情報</span><span class="sxs-lookup"><span data-stu-id="ae1c0-156">Support department information</span></span>|
|<span data-ttu-id="ae1c0-157">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="ae1c0-157">passCodeDisabled</span></span>|<span data-ttu-id="ae1c0-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae1c0-158">Boolean</span></span>|<span data-ttu-id="ae1c0-159">パスコードの設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="ae1c0-159">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="ae1c0-160">isMandatory</span><span class="sxs-lookup"><span data-stu-id="ae1c0-160">isMandatory</span></span>|<span data-ttu-id="ae1c0-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae1c0-161">Boolean</span></span>|<span data-ttu-id="ae1c0-162">プロファイルが必須かどうかを</span><span class="sxs-lookup"><span data-stu-id="ae1c0-162">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="ae1c0-163">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="ae1c0-163">locationDisabled</span></span>|<span data-ttu-id="ae1c0-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae1c0-164">Boolean</span></span>|<span data-ttu-id="ae1c0-165">場所サービス セットアップ] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="ae1c0-165">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="ae1c0-166">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="ae1c0-166">supportPhoneNumber</span></span>|<span data-ttu-id="ae1c0-167">String</span><span class="sxs-lookup"><span data-stu-id="ae1c0-167">String</span></span>|<span data-ttu-id="ae1c0-168">サポート電話番号</span><span class="sxs-lookup"><span data-stu-id="ae1c0-168">Support phone number</span></span>|
|<span data-ttu-id="ae1c0-169">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="ae1c0-169">profileRemovalDisabled</span></span>|<span data-ttu-id="ae1c0-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae1c0-170">Boolean</span></span>|<span data-ttu-id="ae1c0-171">プロファイルの削除オプションが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="ae1c0-171">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="ae1c0-172">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="ae1c0-172">restoreBlocked</span></span>|<span data-ttu-id="ae1c0-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae1c0-173">Boolean</span></span>|<span data-ttu-id="ae1c0-174">復元の設定] ウィンドウがブロックされていることを示します。</span><span class="sxs-lookup"><span data-stu-id="ae1c0-174">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="ae1c0-175">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="ae1c0-175">appleIdDisabled</span></span>|<span data-ttu-id="ae1c0-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae1c0-176">Boolean</span></span>|<span data-ttu-id="ae1c0-177">Apple id の設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="ae1c0-177">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="ae1c0-178">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="ae1c0-178">termsAndConditionsDisabled</span></span>|<span data-ttu-id="ae1c0-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae1c0-179">Boolean</span></span>|<span data-ttu-id="ae1c0-180">'条項および条件' の設定ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="ae1c0-180">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="ae1c0-181">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="ae1c0-181">touchIdDisabled</span></span>|<span data-ttu-id="ae1c0-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae1c0-182">Boolean</span></span>|<span data-ttu-id="ae1c0-183">タッチ id の設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="ae1c0-183">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="ae1c0-184">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="ae1c0-184">applePayDisabled</span></span>|<span data-ttu-id="ae1c0-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae1c0-185">Boolean</span></span>|<span data-ttu-id="ae1c0-186">アップル支払設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="ae1c0-186">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="ae1c0-187">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="ae1c0-187">zoomDisabled</span></span>|<span data-ttu-id="ae1c0-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae1c0-188">Boolean</span></span>|<span data-ttu-id="ae1c0-189">ズームの設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="ae1c0-189">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="ae1c0-190">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="ae1c0-190">siriDisabled</span></span>|<span data-ttu-id="ae1c0-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae1c0-191">Boolean</span></span>|<span data-ttu-id="ae1c0-192">Siri の設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="ae1c0-192">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="ae1c0-193">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="ae1c0-193">diagnosticsDisabled</span></span>|<span data-ttu-id="ae1c0-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae1c0-194">Boolean</span></span>|<span data-ttu-id="ae1c0-195">診断設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="ae1c0-195">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="ae1c0-196">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="ae1c0-196">displayToneSetupDisabled</span></span>|<span data-ttu-id="ae1c0-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae1c0-197">Boolean</span></span>|<span data-ttu-id="ae1c0-198">Displaytone セットアップ画面が無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="ae1c0-198">Indicates if displaytone setup screen is disabled</span></span>|
|<span data-ttu-id="ae1c0-199">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="ae1c0-199">privacyPaneDisabled</span></span>|<span data-ttu-id="ae1c0-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae1c0-200">Boolean</span></span>|<span data-ttu-id="ae1c0-201">プライバシー画面が無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="ae1c0-201">Indicates if privacy screen is disabled</span></span>|

## <a name="relationships"></a><span data-ttu-id="ae1c0-202">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ae1c0-202">Relationships</span></span>
<span data-ttu-id="ae1c0-203">なし</span><span class="sxs-lookup"><span data-stu-id="ae1c0-203">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ae1c0-204">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ae1c0-204">JSON Representation</span></span>
<span data-ttu-id="ae1c0-205">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ae1c0-205">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.depEnrollmentBaseProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.depEnrollmentBaseProfile",
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
  "privacyPaneDisabled": true
}
```




