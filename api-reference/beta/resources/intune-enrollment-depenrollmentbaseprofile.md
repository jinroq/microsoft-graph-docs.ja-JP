---
title: depEnrollmentBaseProfile リソースの種類
description: DepEnrollmentBaseProfile リソースでは、アップル デバイスの登録プログラム (DEP) の登録プロファイルを表します。 このタイプのプロファイルは、DEP. を使用して対応するデバイスを登録する前に、Apple の DEP のシリアル番号を割り当てる必要があります。
author: tfitzmac
ms.openlocfilehash: 26335fd3d35494b815dd43531ad54b4796dc861c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308373"
---
# <a name="depenrollmentbaseprofile-resource-type"></a><span data-ttu-id="ef346-104">depEnrollmentBaseProfile リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ef346-104">depEnrollmentBaseProfile resource type</span></span>

> <span data-ttu-id="ef346-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ef346-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ef346-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ef346-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ef346-107">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ef346-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ef346-108">DepEnrollmentBaseProfile リソースでは、アップル デバイスの登録プログラム (DEP) の登録プロファイルを表します。</span><span class="sxs-lookup"><span data-stu-id="ef346-108">The DepEnrollmentBaseProfile resource represents an Apple Device Enrollment Program (DEP) enrollment profile.</span></span> <span data-ttu-id="ef346-109">このタイプのプロファイルは、DEP. を使用して対応するデバイスを登録する前に、Apple の DEP のシリアル番号を割り当てる必要があります。</span><span class="sxs-lookup"><span data-stu-id="ef346-109">This type of profile must be assigned to Apple DEP serial numbers before the corresponding devices can enroll via DEP.</span></span>

<span data-ttu-id="ef346-110">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="ef346-110">Inherits from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>

## <a name="methods"></a><span data-ttu-id="ef346-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="ef346-111">Methods</span></span>
|<span data-ttu-id="ef346-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="ef346-112">Method</span></span>|<span data-ttu-id="ef346-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ef346-113">Return Type</span></span>|<span data-ttu-id="ef346-114">説明</span><span class="sxs-lookup"><span data-stu-id="ef346-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ef346-115">リスト depEnrollmentBaseProfiles</span><span class="sxs-lookup"><span data-stu-id="ef346-115">List depEnrollmentBaseProfiles</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-list.md)|<span data-ttu-id="ef346-116">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ef346-116">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) collection</span></span>|<span data-ttu-id="ef346-117">[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="ef346-117">List properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) objects.</span></span>|
|[<span data-ttu-id="ef346-118">DepEnrollmentBaseProfile を取得します。</span><span class="sxs-lookup"><span data-stu-id="ef346-118">Get depEnrollmentBaseProfile</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-get.md)|[<span data-ttu-id="ef346-119">depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="ef346-119">depEnrollmentBaseProfile</span></span>](../resources/intune-enrollment-depenrollmentbaseprofile.md)|<span data-ttu-id="ef346-120">[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ef346-120">Read properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ef346-121">Properties</span><span class="sxs-lookup"><span data-stu-id="ef346-121">Properties</span></span>
|<span data-ttu-id="ef346-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ef346-122">Property</span></span>|<span data-ttu-id="ef346-123">種類</span><span class="sxs-lookup"><span data-stu-id="ef346-123">Type</span></span>|<span data-ttu-id="ef346-124">説明</span><span class="sxs-lookup"><span data-stu-id="ef346-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef346-125">ID</span><span class="sxs-lookup"><span data-stu-id="ef346-125">id</span></span>|<span data-ttu-id="ef346-126">String</span><span class="sxs-lookup"><span data-stu-id="ef346-126">String</span></span>|<span data-ttu-id="ef346-127">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるオブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="ef346-127">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ef346-128">displayName</span><span class="sxs-lookup"><span data-stu-id="ef346-128">displayName</span></span>|<span data-ttu-id="ef346-129">String</span><span class="sxs-lookup"><span data-stu-id="ef346-129">String</span></span>|<span data-ttu-id="ef346-130">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるプロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="ef346-130">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ef346-131">説明</span><span class="sxs-lookup"><span data-stu-id="ef346-131">description</span></span>|<span data-ttu-id="ef346-132">String</span><span class="sxs-lookup"><span data-stu-id="ef346-132">String</span></span>|<span data-ttu-id="ef346-133">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるプロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="ef346-133">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ef346-134">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="ef346-134">requiresUserAuthentication</span></span>|<span data-ttu-id="ef346-135">ブール型</span><span class="sxs-lookup"><span data-stu-id="ef346-135">Boolean</span></span>|<span data-ttu-id="ef346-136">プロファイルに[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるのユーザー認証が必要なかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="ef346-136">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ef346-137">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="ef346-137">configurationEndpointUrl</span></span>|<span data-ttu-id="ef346-138">String</span><span class="sxs-lookup"><span data-stu-id="ef346-138">String</span></span>|<span data-ttu-id="ef346-139">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から登録の継承を使用するエンドポイントの url を構成</span><span class="sxs-lookup"><span data-stu-id="ef346-139">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ef346-140">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="ef346-140">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="ef346-141">ブール型</span><span class="sxs-lookup"><span data-stu-id="ef346-141">Boolean</span></span>|<span data-ttu-id="ef346-142">アップルらくらく企業ポータルではなくを使用して認証することを示します。</span><span class="sxs-lookup"><span data-stu-id="ef346-142">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="ef346-143">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="ef346-143">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ef346-144">isDefault</span><span class="sxs-lookup"><span data-stu-id="ef346-144">isDefault</span></span>|<span data-ttu-id="ef346-145">ブール型</span><span class="sxs-lookup"><span data-stu-id="ef346-145">Boolean</span></span>|<span data-ttu-id="ef346-146">これは、既定のプロファイルであるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="ef346-146">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="ef346-147">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="ef346-147">supervisedModeEnabled</span></span>|<span data-ttu-id="ef346-148">ブール型</span><span class="sxs-lookup"><span data-stu-id="ef346-148">Boolean</span></span>|<span data-ttu-id="ef346-149">コールを管理モードを有効にする、false それ以外の場合は True です。</span><span class="sxs-lookup"><span data-stu-id="ef346-149">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="ef346-150">参照してくださいhttps://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intuneの追加情報です。</span><span class="sxs-lookup"><span data-stu-id="ef346-150">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="ef346-151">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="ef346-151">supportDepartment</span></span>|<span data-ttu-id="ef346-152">String</span><span class="sxs-lookup"><span data-stu-id="ef346-152">String</span></span>|<span data-ttu-id="ef346-153">サポート部門の情報</span><span class="sxs-lookup"><span data-stu-id="ef346-153">Support department information</span></span>|
|<span data-ttu-id="ef346-154">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="ef346-154">passCodeDisabled</span></span>|<span data-ttu-id="ef346-155">ブール型</span><span class="sxs-lookup"><span data-stu-id="ef346-155">Boolean</span></span>|<span data-ttu-id="ef346-156">パスコードの設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="ef346-156">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="ef346-157">isMandatory</span><span class="sxs-lookup"><span data-stu-id="ef346-157">isMandatory</span></span>|<span data-ttu-id="ef346-158">ブール型</span><span class="sxs-lookup"><span data-stu-id="ef346-158">Boolean</span></span>|<span data-ttu-id="ef346-159">プロファイルが必須かどうかを</span><span class="sxs-lookup"><span data-stu-id="ef346-159">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="ef346-160">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="ef346-160">locationDisabled</span></span>|<span data-ttu-id="ef346-161">ブール型</span><span class="sxs-lookup"><span data-stu-id="ef346-161">Boolean</span></span>|<span data-ttu-id="ef346-162">場所サービス セットアップ] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="ef346-162">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="ef346-163">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="ef346-163">supportPhoneNumber</span></span>|<span data-ttu-id="ef346-164">String</span><span class="sxs-lookup"><span data-stu-id="ef346-164">String</span></span>|<span data-ttu-id="ef346-165">サポート電話番号</span><span class="sxs-lookup"><span data-stu-id="ef346-165">Support phone number</span></span>|
|<span data-ttu-id="ef346-166">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="ef346-166">profileRemovalDisabled</span></span>|<span data-ttu-id="ef346-167">ブール型</span><span class="sxs-lookup"><span data-stu-id="ef346-167">Boolean</span></span>|<span data-ttu-id="ef346-168">プロファイルの削除オプションが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="ef346-168">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="ef346-169">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="ef346-169">restoreBlocked</span></span>|<span data-ttu-id="ef346-170">ブール型</span><span class="sxs-lookup"><span data-stu-id="ef346-170">Boolean</span></span>|<span data-ttu-id="ef346-171">復元の設定] ウィンドウがブロックされていることを示します。</span><span class="sxs-lookup"><span data-stu-id="ef346-171">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="ef346-172">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="ef346-172">appleIdDisabled</span></span>|<span data-ttu-id="ef346-173">ブール型</span><span class="sxs-lookup"><span data-stu-id="ef346-173">Boolean</span></span>|<span data-ttu-id="ef346-174">Apple id の設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="ef346-174">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="ef346-175">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="ef346-175">termsAndConditionsDisabled</span></span>|<span data-ttu-id="ef346-176">ブール型</span><span class="sxs-lookup"><span data-stu-id="ef346-176">Boolean</span></span>|<span data-ttu-id="ef346-177">'条項および条件' の設定ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="ef346-177">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="ef346-178">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="ef346-178">touchIdDisabled</span></span>|<span data-ttu-id="ef346-179">ブール型</span><span class="sxs-lookup"><span data-stu-id="ef346-179">Boolean</span></span>|<span data-ttu-id="ef346-180">タッチ id の設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="ef346-180">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="ef346-181">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="ef346-181">applePayDisabled</span></span>|<span data-ttu-id="ef346-182">ブール型</span><span class="sxs-lookup"><span data-stu-id="ef346-182">Boolean</span></span>|<span data-ttu-id="ef346-183">アップル支払設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="ef346-183">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="ef346-184">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="ef346-184">zoomDisabled</span></span>|<span data-ttu-id="ef346-185">ブール型</span><span class="sxs-lookup"><span data-stu-id="ef346-185">Boolean</span></span>|<span data-ttu-id="ef346-186">ズームの設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="ef346-186">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="ef346-187">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="ef346-187">siriDisabled</span></span>|<span data-ttu-id="ef346-188">ブール型</span><span class="sxs-lookup"><span data-stu-id="ef346-188">Boolean</span></span>|<span data-ttu-id="ef346-189">Siri の設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="ef346-189">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="ef346-190">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="ef346-190">diagnosticsDisabled</span></span>|<span data-ttu-id="ef346-191">ブール型</span><span class="sxs-lookup"><span data-stu-id="ef346-191">Boolean</span></span>|<span data-ttu-id="ef346-192">診断設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="ef346-192">Indicates if diagnostics setup pane is disabled</span></span>|

## <a name="relationships"></a><span data-ttu-id="ef346-193">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ef346-193">Relationships</span></span>
<span data-ttu-id="ef346-194">なし</span><span class="sxs-lookup"><span data-stu-id="ef346-194">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ef346-195">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ef346-195">JSON Representation</span></span>
<span data-ttu-id="ef346-196">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ef346-196">Here is a JSON representation of the resource.</span></span>
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





