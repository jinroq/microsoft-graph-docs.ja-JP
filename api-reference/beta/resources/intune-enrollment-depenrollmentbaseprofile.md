---
title: depEnrollmentBaseProfile リソースの種類
description: DepEnrollmentBaseProfile リソースは、Apple Device enrollment program (DEP) 登録プロファイルを表します。 この種類のプロファイルは、対応するデバイスが dep を使用して登録できるようになる前に、Apple DEP シリアル番号に割り当てる必要があります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f5ad27470bb09313084feadcf468d83e58964532
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143107"
---
# <a name="depenrollmentbaseprofile-resource-type"></a><span data-ttu-id="ee2c9-104">depEnrollmentBaseProfile リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ee2c9-104">depEnrollmentBaseProfile resource type</span></span>

> <span data-ttu-id="ee2c9-105">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee2c9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ee2c9-106">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ee2c9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee2c9-107">DepEnrollmentBaseProfile リソースは、Apple Device enrollment program (DEP) 登録プロファイルを表します。</span><span class="sxs-lookup"><span data-stu-id="ee2c9-107">The DepEnrollmentBaseProfile resource represents an Apple Device Enrollment Program (DEP) enrollment profile.</span></span> <span data-ttu-id="ee2c9-108">この種類のプロファイルは、対応するデバイスが dep を使用して登録できるようになる前に、Apple DEP シリアル番号に割り当てる必要があります。</span><span class="sxs-lookup"><span data-stu-id="ee2c9-108">This type of profile must be assigned to Apple DEP serial numbers before the corresponding devices can enroll via DEP.</span></span>


<span data-ttu-id="ee2c9-109">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="ee2c9-109">Inherits from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>

## <a name="methods"></a><span data-ttu-id="ee2c9-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="ee2c9-110">Methods</span></span>
|<span data-ttu-id="ee2c9-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="ee2c9-111">Method</span></span>|<span data-ttu-id="ee2c9-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ee2c9-112">Return Type</span></span>|<span data-ttu-id="ee2c9-113">説明</span><span class="sxs-lookup"><span data-stu-id="ee2c9-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ee2c9-114">リスト depEnrollmentBaseProfiles</span><span class="sxs-lookup"><span data-stu-id="ee2c9-114">List depEnrollmentBaseProfiles</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-list.md)|<span data-ttu-id="ee2c9-115">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ee2c9-115">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) collection</span></span>|<span data-ttu-id="ee2c9-116">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="ee2c9-116">List properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) objects.</span></span>|
|[<span data-ttu-id="ee2c9-117">depEnrollmentBaseProfile を取得する</span><span class="sxs-lookup"><span data-stu-id="ee2c9-117">Get depEnrollmentBaseProfile</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-get.md)|[<span data-ttu-id="ee2c9-118">depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="ee2c9-118">depEnrollmentBaseProfile</span></span>](../resources/intune-enrollment-depenrollmentbaseprofile.md)|<span data-ttu-id="ee2c9-119">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ee2c9-119">Read properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ee2c9-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ee2c9-120">Properties</span></span>
|<span data-ttu-id="ee2c9-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ee2c9-121">Property</span></span>|<span data-ttu-id="ee2c9-122">型</span><span class="sxs-lookup"><span data-stu-id="ee2c9-122">Type</span></span>|<span data-ttu-id="ee2c9-123">説明</span><span class="sxs-lookup"><span data-stu-id="ee2c9-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee2c9-124">id</span><span class="sxs-lookup"><span data-stu-id="ee2c9-124">id</span></span>|<span data-ttu-id="ee2c9-125">文字列</span><span class="sxs-lookup"><span data-stu-id="ee2c9-125">String</span></span>|<span data-ttu-id="ee2c9-126">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたオブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="ee2c9-126">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ee2c9-127">displayName</span><span class="sxs-lookup"><span data-stu-id="ee2c9-127">displayName</span></span>|<span data-ttu-id="ee2c9-128">String</span><span class="sxs-lookup"><span data-stu-id="ee2c9-128">String</span></span>|<span data-ttu-id="ee2c9-129">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたプロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="ee2c9-129">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ee2c9-130">説明</span><span class="sxs-lookup"><span data-stu-id="ee2c9-130">description</span></span>|<span data-ttu-id="ee2c9-131">String</span><span class="sxs-lookup"><span data-stu-id="ee2c9-131">String</span></span>|<span data-ttu-id="ee2c9-132">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたプロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="ee2c9-132">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ee2c9-133">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="ee2c9-133">requiresUserAuthentication</span></span>|<span data-ttu-id="ee2c9-134">ブール値</span><span class="sxs-lookup"><span data-stu-id="ee2c9-134">Boolean</span></span>|<span data-ttu-id="ee2c9-135">プロファイルが[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承したユーザー認証を必要とするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ee2c9-135">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ee2c9-136">configurationendpointurl</span><span class="sxs-lookup"><span data-stu-id="ee2c9-136">configurationEndpointUrl</span></span>|<span data-ttu-id="ee2c9-137">String</span><span class="sxs-lookup"><span data-stu-id="ee2c9-137">String</span></span>|<span data-ttu-id="ee2c9-138">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承された登録に使用する構成エンドポイント url</span><span class="sxs-lookup"><span data-stu-id="ee2c9-138">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ee2c9-139">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="ee2c9-139">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="ee2c9-140">ブール値</span><span class="sxs-lookup"><span data-stu-id="ee2c9-140">Boolean</span></span>|<span data-ttu-id="ee2c9-141">会社のポータルではなく、Apple セットアップアシスタントを使用して認証することを示します。</span><span class="sxs-lookup"><span data-stu-id="ee2c9-141">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="ee2c9-142">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="ee2c9-142">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ee2c9-143">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="ee2c9-143">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="ee2c9-144">ブール値</span><span class="sxs-lookup"><span data-stu-id="ee2c9-144">Boolean</span></span>|<span data-ttu-id="ee2c9-145">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたセットアップアシスタントの登録済みデバイスで、会社のポータルが必要であることを示します。</span><span class="sxs-lookup"><span data-stu-id="ee2c9-145">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ee2c9-146">isDefault</span><span class="sxs-lookup"><span data-stu-id="ee2c9-146">isDefault</span></span>|<span data-ttu-id="ee2c9-147">ブール値</span><span class="sxs-lookup"><span data-stu-id="ee2c9-147">Boolean</span></span>|<span data-ttu-id="ee2c9-148">これが既定のプロファイルであるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="ee2c9-148">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="ee2c9-149">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="ee2c9-149">supervisedModeEnabled</span></span>|<span data-ttu-id="ee2c9-150">ブール値</span><span class="sxs-lookup"><span data-stu-id="ee2c9-150">Boolean</span></span>|<span data-ttu-id="ee2c9-151">監視モード、有効にする場合は True、それ以外の場合は false。</span><span class="sxs-lookup"><span data-stu-id="ee2c9-151">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="ee2c9-152">詳細https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intuneについては、「」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ee2c9-152">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="ee2c9-153">supportdepartment</span><span class="sxs-lookup"><span data-stu-id="ee2c9-153">supportDepartment</span></span>|<span data-ttu-id="ee2c9-154">String</span><span class="sxs-lookup"><span data-stu-id="ee2c9-154">String</span></span>|<span data-ttu-id="ee2c9-155">サポート部門の情報</span><span class="sxs-lookup"><span data-stu-id="ee2c9-155">Support department information</span></span>|
|<span data-ttu-id="ee2c9-156">pass codedisabled</span><span class="sxs-lookup"><span data-stu-id="ee2c9-156">passCodeDisabled</span></span>|<span data-ttu-id="ee2c9-157">ブール値</span><span class="sxs-lookup"><span data-stu-id="ee2c9-157">Boolean</span></span>|<span data-ttu-id="ee2c9-158">パスコードセットアップウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="ee2c9-158">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="ee2c9-159">ismandatory</span><span class="sxs-lookup"><span data-stu-id="ee2c9-159">isMandatory</span></span>|<span data-ttu-id="ee2c9-160">ブール値</span><span class="sxs-lookup"><span data-stu-id="ee2c9-160">Boolean</span></span>|<span data-ttu-id="ee2c9-161">プロファイルが必須であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="ee2c9-161">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="ee2c9-162">locationdisabled</span><span class="sxs-lookup"><span data-stu-id="ee2c9-162">locationDisabled</span></span>|<span data-ttu-id="ee2c9-163">ブール値</span><span class="sxs-lookup"><span data-stu-id="ee2c9-163">Boolean</span></span>|<span data-ttu-id="ee2c9-164">場所サービスの設定ウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="ee2c9-164">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="ee2c9-165">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="ee2c9-165">supportPhoneNumber</span></span>|<span data-ttu-id="ee2c9-166">String</span><span class="sxs-lookup"><span data-stu-id="ee2c9-166">String</span></span>|<span data-ttu-id="ee2c9-167">サポート電話番号</span><span class="sxs-lookup"><span data-stu-id="ee2c9-167">Support phone number</span></span>|
|<span data-ttu-id="ee2c9-168">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="ee2c9-168">profileRemovalDisabled</span></span>|<span data-ttu-id="ee2c9-169">ブール値</span><span class="sxs-lookup"><span data-stu-id="ee2c9-169">Boolean</span></span>|<span data-ttu-id="ee2c9-170">プロファイルの削除オプションが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="ee2c9-170">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="ee2c9-171">restoreblocked</span><span class="sxs-lookup"><span data-stu-id="ee2c9-171">restoreBlocked</span></span>|<span data-ttu-id="ee2c9-172">ブール値</span><span class="sxs-lookup"><span data-stu-id="ee2c9-172">Boolean</span></span>|<span data-ttu-id="ee2c9-173">セットアップウィンドウの復元がブロックされているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="ee2c9-173">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="ee2c9-174">りんご eiddisabled</span><span class="sxs-lookup"><span data-stu-id="ee2c9-174">appleIdDisabled</span></span>|<span data-ttu-id="ee2c9-175">ブール値</span><span class="sxs-lookup"><span data-stu-id="ee2c9-175">Boolean</span></span>|<span data-ttu-id="ee2c9-176">Apple id のセットアップウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="ee2c9-176">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="ee2c9-177">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="ee2c9-177">termsAndConditionsDisabled</span></span>|<span data-ttu-id="ee2c9-178">ブール値</span><span class="sxs-lookup"><span data-stu-id="ee2c9-178">Boolean</span></span>|<span data-ttu-id="ee2c9-179">[使用条件] セットアップウィンドウが無効かどうかを示します</span><span class="sxs-lookup"><span data-stu-id="ee2c9-179">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="ee2c9-180">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="ee2c9-180">touchIdDisabled</span></span>|<span data-ttu-id="ee2c9-181">ブール値</span><span class="sxs-lookup"><span data-stu-id="ee2c9-181">Boolean</span></span>|<span data-ttu-id="ee2c9-182">タッチ id のセットアップウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="ee2c9-182">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="ee2c9-183">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="ee2c9-183">applePayDisabled</span></span>|<span data-ttu-id="ee2c9-184">ブール値</span><span class="sxs-lookup"><span data-stu-id="ee2c9-184">Boolean</span></span>|<span data-ttu-id="ee2c9-185">Apple の支払い設定ウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="ee2c9-185">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="ee2c9-186">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="ee2c9-186">zoomDisabled</span></span>|<span data-ttu-id="ee2c9-187">ブール値</span><span class="sxs-lookup"><span data-stu-id="ee2c9-187">Boolean</span></span>|<span data-ttu-id="ee2c9-188">ズーム設定ウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="ee2c9-188">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="ee2c9-189">siridisabled</span><span class="sxs-lookup"><span data-stu-id="ee2c9-189">siriDisabled</span></span>|<span data-ttu-id="ee2c9-190">ブール値</span><span class="sxs-lookup"><span data-stu-id="ee2c9-190">Boolean</span></span>|<span data-ttu-id="ee2c9-191">siri セットアップウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="ee2c9-191">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="ee2c9-192">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="ee2c9-192">diagnosticsDisabled</span></span>|<span data-ttu-id="ee2c9-193">ブール値</span><span class="sxs-lookup"><span data-stu-id="ee2c9-193">Boolean</span></span>|<span data-ttu-id="ee2c9-194">診断セットアップウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="ee2c9-194">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="ee2c9-195">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="ee2c9-195">displayToneSetupDisabled</span></span>|<span data-ttu-id="ee2c9-196">ブール値</span><span class="sxs-lookup"><span data-stu-id="ee2c9-196">Boolean</span></span>|<span data-ttu-id="ee2c9-197">displaytone の設定画面が無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="ee2c9-197">Indicates if displaytone setup screen is disabled</span></span>|
|<span data-ttu-id="ee2c9-198">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="ee2c9-198">privacyPaneDisabled</span></span>|<span data-ttu-id="ee2c9-199">ブール値</span><span class="sxs-lookup"><span data-stu-id="ee2c9-199">Boolean</span></span>|<span data-ttu-id="ee2c9-200">プライバシー画面が無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="ee2c9-200">Indicates if privacy screen is disabled</span></span>|

## <a name="relationships"></a><span data-ttu-id="ee2c9-201">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ee2c9-201">Relationships</span></span>
<span data-ttu-id="ee2c9-202">なし</span><span class="sxs-lookup"><span data-stu-id="ee2c9-202">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ee2c9-203">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ee2c9-203">JSON Representation</span></span>
<span data-ttu-id="ee2c9-204">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ee2c9-204">Here is a JSON representation of the resource.</span></span>
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




