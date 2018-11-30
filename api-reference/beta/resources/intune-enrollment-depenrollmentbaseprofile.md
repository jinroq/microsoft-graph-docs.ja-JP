---
title: depEnrollmentBaseProfile リソースの種類
description: DepEnrollmentBaseProfile リソースでは、アップル デバイスの登録プログラム (DEP) の登録プロファイルを表します。 このタイプのプロファイルは、DEP. を使用して対応するデバイスを登録する前に、Apple の DEP のシリアル番号を割り当てる必要があります。
ms.openlocfilehash: 172e0f0d4ed9b23f8c5a3d5226e24e4ac63b0527
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073260"
---
# <a name="depenrollmentbaseprofile-resource-type"></a><span data-ttu-id="8ba4b-104">depEnrollmentBaseProfile リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8ba4b-104">depEnrollmentBaseProfile resource type</span></span>

> <span data-ttu-id="8ba4b-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8ba4b-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8ba4b-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8ba4b-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8ba4b-107">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8ba4b-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8ba4b-108">DepEnrollmentBaseProfile リソースでは、アップル デバイスの登録プログラム (DEP) の登録プロファイルを表します。</span><span class="sxs-lookup"><span data-stu-id="8ba4b-108">The DepEnrollmentBaseProfile resource represents an Apple Device Enrollment Program (DEP) enrollment profile.</span></span> <span data-ttu-id="8ba4b-109">このタイプのプロファイルは、DEP. を使用して対応するデバイスを登録する前に、Apple の DEP のシリアル番号を割り当てる必要があります。</span><span class="sxs-lookup"><span data-stu-id="8ba4b-109">This type of profile must be assigned to Apple DEP serial numbers before the corresponding devices can enroll via DEP.</span></span>

<span data-ttu-id="8ba4b-110">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="8ba4b-110">Inherits from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>

## <a name="methods"></a><span data-ttu-id="8ba4b-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="8ba4b-111">Methods</span></span>
|<span data-ttu-id="8ba4b-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="8ba4b-112">Method</span></span>|<span data-ttu-id="8ba4b-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8ba4b-113">Return Type</span></span>|<span data-ttu-id="8ba4b-114">説明</span><span class="sxs-lookup"><span data-stu-id="8ba4b-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8ba4b-115">リスト depEnrollmentBaseProfiles</span><span class="sxs-lookup"><span data-stu-id="8ba4b-115">List depEnrollmentBaseProfiles</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-list.md)|<span data-ttu-id="8ba4b-116">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="8ba4b-116">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) collection</span></span>|<span data-ttu-id="8ba4b-117">[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="8ba4b-117">List properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) objects.</span></span>|
|[<span data-ttu-id="8ba4b-118">DepEnrollmentBaseProfile を取得します。</span><span class="sxs-lookup"><span data-stu-id="8ba4b-118">Get depEnrollmentBaseProfile</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-get.md)|[<span data-ttu-id="8ba4b-119">depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="8ba4b-119">depEnrollmentBaseProfile</span></span>](../resources/intune-enrollment-depenrollmentbaseprofile.md)|<span data-ttu-id="8ba4b-120">[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8ba4b-120">Read properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8ba4b-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8ba4b-121">Properties</span></span>
|<span data-ttu-id="8ba4b-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8ba4b-122">Property</span></span>|<span data-ttu-id="8ba4b-123">型</span><span class="sxs-lookup"><span data-stu-id="8ba4b-123">Type</span></span>|<span data-ttu-id="8ba4b-124">説明</span><span class="sxs-lookup"><span data-stu-id="8ba4b-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ba4b-125">id</span><span class="sxs-lookup"><span data-stu-id="8ba4b-125">id</span></span>|<span data-ttu-id="8ba4b-126">String</span><span class="sxs-lookup"><span data-stu-id="8ba4b-126">String</span></span>|<span data-ttu-id="8ba4b-127">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるオブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="8ba4b-127">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="8ba4b-128">displayName</span><span class="sxs-lookup"><span data-stu-id="8ba4b-128">displayName</span></span>|<span data-ttu-id="8ba4b-129">String</span><span class="sxs-lookup"><span data-stu-id="8ba4b-129">String</span></span>|<span data-ttu-id="8ba4b-130">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるプロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="8ba4b-130">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="8ba4b-131">説明</span><span class="sxs-lookup"><span data-stu-id="8ba4b-131">description</span></span>|<span data-ttu-id="8ba4b-132">String</span><span class="sxs-lookup"><span data-stu-id="8ba4b-132">String</span></span>|<span data-ttu-id="8ba4b-133">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるプロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="8ba4b-133">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="8ba4b-134">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="8ba4b-134">requiresUserAuthentication</span></span>|<span data-ttu-id="8ba4b-135">ブール値</span><span class="sxs-lookup"><span data-stu-id="8ba4b-135">Boolean</span></span>|<span data-ttu-id="8ba4b-136">プロファイルに[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるのユーザー認証が必要なかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="8ba4b-136">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="8ba4b-137">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="8ba4b-137">configurationEndpointUrl</span></span>|<span data-ttu-id="8ba4b-138">String</span><span class="sxs-lookup"><span data-stu-id="8ba4b-138">String</span></span>|<span data-ttu-id="8ba4b-139">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から登録の継承を使用するエンドポイントの url を構成</span><span class="sxs-lookup"><span data-stu-id="8ba4b-139">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="8ba4b-140">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="8ba4b-140">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="8ba4b-141">ブール値</span><span class="sxs-lookup"><span data-stu-id="8ba4b-141">Boolean</span></span>|<span data-ttu-id="8ba4b-142">アップルらくらく企業ポータルではなくを使用して認証することを示します。</span><span class="sxs-lookup"><span data-stu-id="8ba4b-142">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="8ba4b-143">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="8ba4b-143">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="8ba4b-144">isDefault</span><span class="sxs-lookup"><span data-stu-id="8ba4b-144">isDefault</span></span>|<span data-ttu-id="8ba4b-145">ブール値</span><span class="sxs-lookup"><span data-stu-id="8ba4b-145">Boolean</span></span>|<span data-ttu-id="8ba4b-146">これは、既定のプロファイルであるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="8ba4b-146">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="8ba4b-147">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="8ba4b-147">supervisedModeEnabled</span></span>|<span data-ttu-id="8ba4b-148">ブール値</span><span class="sxs-lookup"><span data-stu-id="8ba4b-148">Boolean</span></span>|<span data-ttu-id="8ba4b-149">コールを管理モードを有効にする、false それ以外の場合は True です。</span><span class="sxs-lookup"><span data-stu-id="8ba4b-149">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="8ba4b-150">参照してくださいhttps://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intuneの追加情報です。</span><span class="sxs-lookup"><span data-stu-id="8ba4b-150">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="8ba4b-151">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="8ba4b-151">supportDepartment</span></span>|<span data-ttu-id="8ba4b-152">String</span><span class="sxs-lookup"><span data-stu-id="8ba4b-152">String</span></span>|<span data-ttu-id="8ba4b-153">サポート部門の情報</span><span class="sxs-lookup"><span data-stu-id="8ba4b-153">Support department information</span></span>|
|<span data-ttu-id="8ba4b-154">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="8ba4b-154">passCodeDisabled</span></span>|<span data-ttu-id="8ba4b-155">ブール値</span><span class="sxs-lookup"><span data-stu-id="8ba4b-155">Boolean</span></span>|<span data-ttu-id="8ba4b-156">パスコードの設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="8ba4b-156">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="8ba4b-157">isMandatory</span><span class="sxs-lookup"><span data-stu-id="8ba4b-157">isMandatory</span></span>|<span data-ttu-id="8ba4b-158">ブール値</span><span class="sxs-lookup"><span data-stu-id="8ba4b-158">Boolean</span></span>|<span data-ttu-id="8ba4b-159">プロファイルが必須かどうかを</span><span class="sxs-lookup"><span data-stu-id="8ba4b-159">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="8ba4b-160">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="8ba4b-160">locationDisabled</span></span>|<span data-ttu-id="8ba4b-161">ブール値</span><span class="sxs-lookup"><span data-stu-id="8ba4b-161">Boolean</span></span>|<span data-ttu-id="8ba4b-162">場所サービス セットアップ] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="8ba4b-162">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="8ba4b-163">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="8ba4b-163">supportPhoneNumber</span></span>|<span data-ttu-id="8ba4b-164">String</span><span class="sxs-lookup"><span data-stu-id="8ba4b-164">String</span></span>|<span data-ttu-id="8ba4b-165">サポート電話番号</span><span class="sxs-lookup"><span data-stu-id="8ba4b-165">Support phone number</span></span>|
|<span data-ttu-id="8ba4b-166">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="8ba4b-166">profileRemovalDisabled</span></span>|<span data-ttu-id="8ba4b-167">ブール値</span><span class="sxs-lookup"><span data-stu-id="8ba4b-167">Boolean</span></span>|<span data-ttu-id="8ba4b-168">プロファイルの削除オプションが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="8ba4b-168">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="8ba4b-169">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="8ba4b-169">restoreBlocked</span></span>|<span data-ttu-id="8ba4b-170">ブール値</span><span class="sxs-lookup"><span data-stu-id="8ba4b-170">Boolean</span></span>|<span data-ttu-id="8ba4b-171">復元の設定] ウィンドウがブロックされていることを示します。</span><span class="sxs-lookup"><span data-stu-id="8ba4b-171">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="8ba4b-172">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="8ba4b-172">appleIdDisabled</span></span>|<span data-ttu-id="8ba4b-173">ブール値</span><span class="sxs-lookup"><span data-stu-id="8ba4b-173">Boolean</span></span>|<span data-ttu-id="8ba4b-174">Apple id の設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="8ba4b-174">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="8ba4b-175">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="8ba4b-175">termsAndConditionsDisabled</span></span>|<span data-ttu-id="8ba4b-176">ブール値</span><span class="sxs-lookup"><span data-stu-id="8ba4b-176">Boolean</span></span>|<span data-ttu-id="8ba4b-177">'条項および条件' の設定ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="8ba4b-177">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="8ba4b-178">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="8ba4b-178">touchIdDisabled</span></span>|<span data-ttu-id="8ba4b-179">ブール値</span><span class="sxs-lookup"><span data-stu-id="8ba4b-179">Boolean</span></span>|<span data-ttu-id="8ba4b-180">タッチ id の設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="8ba4b-180">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="8ba4b-181">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="8ba4b-181">applePayDisabled</span></span>|<span data-ttu-id="8ba4b-182">ブール値</span><span class="sxs-lookup"><span data-stu-id="8ba4b-182">Boolean</span></span>|<span data-ttu-id="8ba4b-183">アップル支払設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="8ba4b-183">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="8ba4b-184">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="8ba4b-184">zoomDisabled</span></span>|<span data-ttu-id="8ba4b-185">ブール値</span><span class="sxs-lookup"><span data-stu-id="8ba4b-185">Boolean</span></span>|<span data-ttu-id="8ba4b-186">ズームの設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="8ba4b-186">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="8ba4b-187">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="8ba4b-187">siriDisabled</span></span>|<span data-ttu-id="8ba4b-188">ブール値</span><span class="sxs-lookup"><span data-stu-id="8ba4b-188">Boolean</span></span>|<span data-ttu-id="8ba4b-189">Siri の設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="8ba4b-189">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="8ba4b-190">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="8ba4b-190">diagnosticsDisabled</span></span>|<span data-ttu-id="8ba4b-191">ブール値</span><span class="sxs-lookup"><span data-stu-id="8ba4b-191">Boolean</span></span>|<span data-ttu-id="8ba4b-192">診断設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="8ba4b-192">Indicates if diagnostics setup pane is disabled</span></span>|

## <a name="relationships"></a><span data-ttu-id="8ba4b-193">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8ba4b-193">Relationships</span></span>
<span data-ttu-id="8ba4b-194">なし</span><span class="sxs-lookup"><span data-stu-id="8ba4b-194">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8ba4b-195">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8ba4b-195">JSON Representation</span></span>
<span data-ttu-id="8ba4b-196">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8ba4b-196">Here is a JSON representation of the resource.</span></span>
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
  "diagnosticsDisabled": true
}
```





