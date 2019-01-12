---
title: depEnrollmentBaseProfile リソースの種類
description: DepEnrollmentBaseProfile リソースでは、アップル デバイスの登録プログラム (DEP) の登録プロファイルを表します。 このタイプのプロファイルは、DEP. を使用して対応するデバイスを登録する前に、Apple の DEP のシリアル番号を割り当てる必要があります。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9e1383048b08a309ea0ecf60eb1ad07c2636e7e5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937671"
---
# <a name="depenrollmentbaseprofile-resource-type"></a><span data-ttu-id="e64db-104">depEnrollmentBaseProfile リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e64db-104">depEnrollmentBaseProfile resource type</span></span>

> <span data-ttu-id="e64db-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e64db-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e64db-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e64db-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e64db-107">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e64db-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e64db-108">DepEnrollmentBaseProfile リソースでは、アップル デバイスの登録プログラム (DEP) の登録プロファイルを表します。</span><span class="sxs-lookup"><span data-stu-id="e64db-108">The DepEnrollmentBaseProfile resource represents an Apple Device Enrollment Program (DEP) enrollment profile.</span></span> <span data-ttu-id="e64db-109">このタイプのプロファイルは、DEP. を使用して対応するデバイスを登録する前に、Apple の DEP のシリアル番号を割り当てる必要があります。</span><span class="sxs-lookup"><span data-stu-id="e64db-109">This type of profile must be assigned to Apple DEP serial numbers before the corresponding devices can enroll via DEP.</span></span>

<span data-ttu-id="e64db-110">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="e64db-110">Inherits from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>

## <a name="methods"></a><span data-ttu-id="e64db-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="e64db-111">Methods</span></span>
|<span data-ttu-id="e64db-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="e64db-112">Method</span></span>|<span data-ttu-id="e64db-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e64db-113">Return Type</span></span>|<span data-ttu-id="e64db-114">説明</span><span class="sxs-lookup"><span data-stu-id="e64db-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e64db-115">リスト depEnrollmentBaseProfiles</span><span class="sxs-lookup"><span data-stu-id="e64db-115">List depEnrollmentBaseProfiles</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-list.md)|<span data-ttu-id="e64db-116">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e64db-116">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) collection</span></span>|<span data-ttu-id="e64db-117">[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="e64db-117">List properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) objects.</span></span>|
|[<span data-ttu-id="e64db-118">DepEnrollmentBaseProfile を取得します。</span><span class="sxs-lookup"><span data-stu-id="e64db-118">Get depEnrollmentBaseProfile</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-get.md)|[<span data-ttu-id="e64db-119">depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="e64db-119">depEnrollmentBaseProfile</span></span>](../resources/intune-enrollment-depenrollmentbaseprofile.md)|<span data-ttu-id="e64db-120">[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e64db-120">Read properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e64db-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e64db-121">Properties</span></span>
|<span data-ttu-id="e64db-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e64db-122">Property</span></span>|<span data-ttu-id="e64db-123">種類</span><span class="sxs-lookup"><span data-stu-id="e64db-123">Type</span></span>|<span data-ttu-id="e64db-124">説明</span><span class="sxs-lookup"><span data-stu-id="e64db-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e64db-125">ID</span><span class="sxs-lookup"><span data-stu-id="e64db-125">id</span></span>|<span data-ttu-id="e64db-126">String</span><span class="sxs-lookup"><span data-stu-id="e64db-126">String</span></span>|<span data-ttu-id="e64db-127">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるオブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="e64db-127">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="e64db-128">displayName</span><span class="sxs-lookup"><span data-stu-id="e64db-128">displayName</span></span>|<span data-ttu-id="e64db-129">String</span><span class="sxs-lookup"><span data-stu-id="e64db-129">String</span></span>|<span data-ttu-id="e64db-130">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるプロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="e64db-130">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="e64db-131">説明</span><span class="sxs-lookup"><span data-stu-id="e64db-131">description</span></span>|<span data-ttu-id="e64db-132">String</span><span class="sxs-lookup"><span data-stu-id="e64db-132">String</span></span>|<span data-ttu-id="e64db-133">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるプロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="e64db-133">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="e64db-134">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="e64db-134">requiresUserAuthentication</span></span>|<span data-ttu-id="e64db-135">ブール型</span><span class="sxs-lookup"><span data-stu-id="e64db-135">Boolean</span></span>|<span data-ttu-id="e64db-136">プロファイルに[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるのユーザー認証が必要なかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="e64db-136">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="e64db-137">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="e64db-137">configurationEndpointUrl</span></span>|<span data-ttu-id="e64db-138">String</span><span class="sxs-lookup"><span data-stu-id="e64db-138">String</span></span>|<span data-ttu-id="e64db-139">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から登録の継承を使用するエンドポイントの url を構成</span><span class="sxs-lookup"><span data-stu-id="e64db-139">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="e64db-140">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="e64db-140">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="e64db-141">ブール型</span><span class="sxs-lookup"><span data-stu-id="e64db-141">Boolean</span></span>|<span data-ttu-id="e64db-142">アップルらくらく企業ポータルではなくを使用して認証することを示します。</span><span class="sxs-lookup"><span data-stu-id="e64db-142">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="e64db-143">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="e64db-143">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="e64db-144">isDefault</span><span class="sxs-lookup"><span data-stu-id="e64db-144">isDefault</span></span>|<span data-ttu-id="e64db-145">ブール型</span><span class="sxs-lookup"><span data-stu-id="e64db-145">Boolean</span></span>|<span data-ttu-id="e64db-146">これは、既定のプロファイルであるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="e64db-146">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="e64db-147">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="e64db-147">supervisedModeEnabled</span></span>|<span data-ttu-id="e64db-148">ブール型</span><span class="sxs-lookup"><span data-stu-id="e64db-148">Boolean</span></span>|<span data-ttu-id="e64db-149">コールを管理モードを有効にする、false それ以外の場合は True です。</span><span class="sxs-lookup"><span data-stu-id="e64db-149">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="e64db-150">参照してくださいhttps://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intuneの追加情報です。</span><span class="sxs-lookup"><span data-stu-id="e64db-150">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="e64db-151">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="e64db-151">supportDepartment</span></span>|<span data-ttu-id="e64db-152">String</span><span class="sxs-lookup"><span data-stu-id="e64db-152">String</span></span>|<span data-ttu-id="e64db-153">サポート部門の情報</span><span class="sxs-lookup"><span data-stu-id="e64db-153">Support department information</span></span>|
|<span data-ttu-id="e64db-154">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="e64db-154">passCodeDisabled</span></span>|<span data-ttu-id="e64db-155">ブール型</span><span class="sxs-lookup"><span data-stu-id="e64db-155">Boolean</span></span>|<span data-ttu-id="e64db-156">パスコードの設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="e64db-156">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="e64db-157">isMandatory</span><span class="sxs-lookup"><span data-stu-id="e64db-157">isMandatory</span></span>|<span data-ttu-id="e64db-158">ブール型</span><span class="sxs-lookup"><span data-stu-id="e64db-158">Boolean</span></span>|<span data-ttu-id="e64db-159">プロファイルが必須かどうかを</span><span class="sxs-lookup"><span data-stu-id="e64db-159">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="e64db-160">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="e64db-160">locationDisabled</span></span>|<span data-ttu-id="e64db-161">ブール型</span><span class="sxs-lookup"><span data-stu-id="e64db-161">Boolean</span></span>|<span data-ttu-id="e64db-162">場所サービス セットアップ] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="e64db-162">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="e64db-163">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="e64db-163">supportPhoneNumber</span></span>|<span data-ttu-id="e64db-164">String</span><span class="sxs-lookup"><span data-stu-id="e64db-164">String</span></span>|<span data-ttu-id="e64db-165">サポート電話番号</span><span class="sxs-lookup"><span data-stu-id="e64db-165">Support phone number</span></span>|
|<span data-ttu-id="e64db-166">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="e64db-166">profileRemovalDisabled</span></span>|<span data-ttu-id="e64db-167">ブール型</span><span class="sxs-lookup"><span data-stu-id="e64db-167">Boolean</span></span>|<span data-ttu-id="e64db-168">プロファイルの削除オプションが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="e64db-168">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="e64db-169">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="e64db-169">restoreBlocked</span></span>|<span data-ttu-id="e64db-170">ブール型</span><span class="sxs-lookup"><span data-stu-id="e64db-170">Boolean</span></span>|<span data-ttu-id="e64db-171">復元の設定] ウィンドウがブロックされていることを示します。</span><span class="sxs-lookup"><span data-stu-id="e64db-171">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="e64db-172">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="e64db-172">appleIdDisabled</span></span>|<span data-ttu-id="e64db-173">ブール型</span><span class="sxs-lookup"><span data-stu-id="e64db-173">Boolean</span></span>|<span data-ttu-id="e64db-174">Apple id の設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="e64db-174">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="e64db-175">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="e64db-175">termsAndConditionsDisabled</span></span>|<span data-ttu-id="e64db-176">ブール型</span><span class="sxs-lookup"><span data-stu-id="e64db-176">Boolean</span></span>|<span data-ttu-id="e64db-177">'条項および条件' の設定ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="e64db-177">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="e64db-178">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="e64db-178">touchIdDisabled</span></span>|<span data-ttu-id="e64db-179">ブール型</span><span class="sxs-lookup"><span data-stu-id="e64db-179">Boolean</span></span>|<span data-ttu-id="e64db-180">タッチ id の設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="e64db-180">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="e64db-181">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="e64db-181">applePayDisabled</span></span>|<span data-ttu-id="e64db-182">ブール型</span><span class="sxs-lookup"><span data-stu-id="e64db-182">Boolean</span></span>|<span data-ttu-id="e64db-183">アップル支払設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="e64db-183">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="e64db-184">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="e64db-184">zoomDisabled</span></span>|<span data-ttu-id="e64db-185">ブール型</span><span class="sxs-lookup"><span data-stu-id="e64db-185">Boolean</span></span>|<span data-ttu-id="e64db-186">ズームの設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="e64db-186">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="e64db-187">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="e64db-187">siriDisabled</span></span>|<span data-ttu-id="e64db-188">ブール型</span><span class="sxs-lookup"><span data-stu-id="e64db-188">Boolean</span></span>|<span data-ttu-id="e64db-189">Siri の設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="e64db-189">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="e64db-190">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="e64db-190">diagnosticsDisabled</span></span>|<span data-ttu-id="e64db-191">ブール型</span><span class="sxs-lookup"><span data-stu-id="e64db-191">Boolean</span></span>|<span data-ttu-id="e64db-192">診断設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="e64db-192">Indicates if diagnostics setup pane is disabled</span></span>|

## <a name="relationships"></a><span data-ttu-id="e64db-193">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e64db-193">Relationships</span></span>
<span data-ttu-id="e64db-194">なし</span><span class="sxs-lookup"><span data-stu-id="e64db-194">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e64db-195">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e64db-195">JSON Representation</span></span>
<span data-ttu-id="e64db-196">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e64db-196">Here is a JSON representation of the resource.</span></span>
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





