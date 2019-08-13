---
title: depEnrollmentBaseProfile リソースの種類
description: DepEnrollmentBaseProfile リソースは、Apple Device Enrollment Program (DEP) 登録プロファイルを表します。 この種類のプロファイルは、対応するデバイスが DEP を使用して登録できるようになる前に、Apple DEP シリアル番号に割り当てる必要があります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 611df6a0aff2c2d3c0d6728aa9bbaa443d772a35
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36328068"
---
# <a name="depenrollmentbaseprofile-resource-type"></a><span data-ttu-id="dc0e3-104">depEnrollmentBaseProfile リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dc0e3-104">depEnrollmentBaseProfile resource type</span></span>

> <span data-ttu-id="dc0e3-105">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dc0e3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dc0e3-106">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="dc0e3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc0e3-107">DepEnrollmentBaseProfile リソースは、Apple Device Enrollment Program (DEP) 登録プロファイルを表します。</span><span class="sxs-lookup"><span data-stu-id="dc0e3-107">The DepEnrollmentBaseProfile resource represents an Apple Device Enrollment Program (DEP) enrollment profile.</span></span> <span data-ttu-id="dc0e3-108">この種類のプロファイルは、対応するデバイスが DEP を使用して登録できるようになる前に、Apple DEP シリアル番号に割り当てる必要があります。</span><span class="sxs-lookup"><span data-stu-id="dc0e3-108">This type of profile must be assigned to Apple DEP serial numbers before the corresponding devices can enroll via DEP.</span></span>


<span data-ttu-id="dc0e3-109">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="dc0e3-109">Inherits from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>

## <a name="methods"></a><span data-ttu-id="dc0e3-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="dc0e3-110">Methods</span></span>
|<span data-ttu-id="dc0e3-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="dc0e3-111">Method</span></span>|<span data-ttu-id="dc0e3-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="dc0e3-112">Return Type</span></span>|<span data-ttu-id="dc0e3-113">説明</span><span class="sxs-lookup"><span data-stu-id="dc0e3-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="dc0e3-114">リスト depEnrollmentBaseProfiles</span><span class="sxs-lookup"><span data-stu-id="dc0e3-114">List depEnrollmentBaseProfiles</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-list.md)|<span data-ttu-id="dc0e3-115">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="dc0e3-115">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) collection</span></span>|<span data-ttu-id="dc0e3-116">[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="dc0e3-116">List properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) objects.</span></span>|
|[<span data-ttu-id="dc0e3-117">DepEnrollmentBaseProfile を取得する</span><span class="sxs-lookup"><span data-stu-id="dc0e3-117">Get depEnrollmentBaseProfile</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-get.md)|[<span data-ttu-id="dc0e3-118">depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="dc0e3-118">depEnrollmentBaseProfile</span></span>](../resources/intune-enrollment-depenrollmentbaseprofile.md)|<span data-ttu-id="dc0e3-119">[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="dc0e3-119">Read properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="dc0e3-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dc0e3-120">Properties</span></span>
|<span data-ttu-id="dc0e3-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dc0e3-121">Property</span></span>|<span data-ttu-id="dc0e3-122">型</span><span class="sxs-lookup"><span data-stu-id="dc0e3-122">Type</span></span>|<span data-ttu-id="dc0e3-123">説明</span><span class="sxs-lookup"><span data-stu-id="dc0e3-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc0e3-124">id</span><span class="sxs-lookup"><span data-stu-id="dc0e3-124">id</span></span>|<span data-ttu-id="dc0e3-125">文字列</span><span class="sxs-lookup"><span data-stu-id="dc0e3-125">String</span></span>|<span data-ttu-id="dc0e3-126">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたオブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="dc0e3-126">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="dc0e3-127">displayName</span><span class="sxs-lookup"><span data-stu-id="dc0e3-127">displayName</span></span>|<span data-ttu-id="dc0e3-128">String</span><span class="sxs-lookup"><span data-stu-id="dc0e3-128">String</span></span>|<span data-ttu-id="dc0e3-129">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたプロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="dc0e3-129">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="dc0e3-130">description</span><span class="sxs-lookup"><span data-stu-id="dc0e3-130">description</span></span>|<span data-ttu-id="dc0e3-131">String</span><span class="sxs-lookup"><span data-stu-id="dc0e3-131">String</span></span>|<span data-ttu-id="dc0e3-132">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたプロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="dc0e3-132">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="dc0e3-133">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="dc0e3-133">requiresUserAuthentication</span></span>|<span data-ttu-id="dc0e3-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc0e3-134">Boolean</span></span>|<span data-ttu-id="dc0e3-135">プロファイルが[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承したユーザー認証を必要とするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc0e3-135">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="dc0e3-136">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="dc0e3-136">configurationEndpointUrl</span></span>|<span data-ttu-id="dc0e3-137">String</span><span class="sxs-lookup"><span data-stu-id="dc0e3-137">String</span></span>|<span data-ttu-id="dc0e3-138">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承された登録に使用する構成エンドポイント url</span><span class="sxs-lookup"><span data-stu-id="dc0e3-138">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="dc0e3-139">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="dc0e3-139">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="dc0e3-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc0e3-140">Boolean</span></span>|<span data-ttu-id="dc0e3-141">会社のポータルではなく、Apple セットアップアシスタントを使用して認証することを示します。</span><span class="sxs-lookup"><span data-stu-id="dc0e3-141">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="dc0e3-142">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="dc0e3-142">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="dc0e3-143">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="dc0e3-143">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="dc0e3-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc0e3-144">Boolean</span></span>|<span data-ttu-id="dc0e3-145">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたセットアップアシスタントの登録済みデバイスで、会社のポータルが必要であることを示します。</span><span class="sxs-lookup"><span data-stu-id="dc0e3-145">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="dc0e3-146">isDefault</span><span class="sxs-lookup"><span data-stu-id="dc0e3-146">isDefault</span></span>|<span data-ttu-id="dc0e3-147">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="dc0e3-147">Boolean</span></span>|<span data-ttu-id="dc0e3-148">これが既定のプロファイルであるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="dc0e3-148">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="dc0e3-149">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="dc0e3-149">supervisedModeEnabled</span></span>|<span data-ttu-id="dc0e3-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc0e3-150">Boolean</span></span>|<span data-ttu-id="dc0e3-151">監視モード、有効にする場合は True、それ以外の場合は false。</span><span class="sxs-lookup"><span data-stu-id="dc0e3-151">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="dc0e3-152">詳細https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intuneについては、「」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dc0e3-152">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="dc0e3-153">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="dc0e3-153">supportDepartment</span></span>|<span data-ttu-id="dc0e3-154">String</span><span class="sxs-lookup"><span data-stu-id="dc0e3-154">String</span></span>|<span data-ttu-id="dc0e3-155">サポート部門の情報</span><span class="sxs-lookup"><span data-stu-id="dc0e3-155">Support department information</span></span>|
|<span data-ttu-id="dc0e3-156">Pass Codedisabled</span><span class="sxs-lookup"><span data-stu-id="dc0e3-156">passCodeDisabled</span></span>|<span data-ttu-id="dc0e3-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc0e3-157">Boolean</span></span>|<span data-ttu-id="dc0e3-158">パスコードセットアップウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="dc0e3-158">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="dc0e3-159">isMandatory</span><span class="sxs-lookup"><span data-stu-id="dc0e3-159">isMandatory</span></span>|<span data-ttu-id="dc0e3-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc0e3-160">Boolean</span></span>|<span data-ttu-id="dc0e3-161">プロファイルが必須であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="dc0e3-161">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="dc0e3-162">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="dc0e3-162">locationDisabled</span></span>|<span data-ttu-id="dc0e3-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc0e3-163">Boolean</span></span>|<span data-ttu-id="dc0e3-164">場所サービスの設定ウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="dc0e3-164">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="dc0e3-165">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="dc0e3-165">supportPhoneNumber</span></span>|<span data-ttu-id="dc0e3-166">String</span><span class="sxs-lookup"><span data-stu-id="dc0e3-166">String</span></span>|<span data-ttu-id="dc0e3-167">サポート電話番号</span><span class="sxs-lookup"><span data-stu-id="dc0e3-167">Support phone number</span></span>|
|<span data-ttu-id="dc0e3-168">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="dc0e3-168">profileRemovalDisabled</span></span>|<span data-ttu-id="dc0e3-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc0e3-169">Boolean</span></span>|<span data-ttu-id="dc0e3-170">プロファイルの削除オプションが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="dc0e3-170">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="dc0e3-171">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="dc0e3-171">restoreBlocked</span></span>|<span data-ttu-id="dc0e3-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc0e3-172">Boolean</span></span>|<span data-ttu-id="dc0e3-173">セットアップウィンドウの復元がブロックされているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="dc0e3-173">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="dc0e3-174">りんご Eiddisabled</span><span class="sxs-lookup"><span data-stu-id="dc0e3-174">appleIdDisabled</span></span>|<span data-ttu-id="dc0e3-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc0e3-175">Boolean</span></span>|<span data-ttu-id="dc0e3-176">Apple id のセットアップウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="dc0e3-176">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="dc0e3-177">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="dc0e3-177">termsAndConditionsDisabled</span></span>|<span data-ttu-id="dc0e3-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc0e3-178">Boolean</span></span>|<span data-ttu-id="dc0e3-179">[使用条件] セットアップウィンドウが無効かどうかを示します</span><span class="sxs-lookup"><span data-stu-id="dc0e3-179">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="dc0e3-180">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="dc0e3-180">touchIdDisabled</span></span>|<span data-ttu-id="dc0e3-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc0e3-181">Boolean</span></span>|<span data-ttu-id="dc0e3-182">タッチ id のセットアップウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="dc0e3-182">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="dc0e3-183">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="dc0e3-183">applePayDisabled</span></span>|<span data-ttu-id="dc0e3-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc0e3-184">Boolean</span></span>|<span data-ttu-id="dc0e3-185">Apple の支払い設定ウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="dc0e3-185">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="dc0e3-186">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="dc0e3-186">zoomDisabled</span></span>|<span data-ttu-id="dc0e3-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc0e3-187">Boolean</span></span>|<span data-ttu-id="dc0e3-188">ズーム設定ウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="dc0e3-188">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="dc0e3-189">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="dc0e3-189">siriDisabled</span></span>|<span data-ttu-id="dc0e3-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc0e3-190">Boolean</span></span>|<span data-ttu-id="dc0e3-191">Siri セットアップウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="dc0e3-191">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="dc0e3-192">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="dc0e3-192">diagnosticsDisabled</span></span>|<span data-ttu-id="dc0e3-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc0e3-193">Boolean</span></span>|<span data-ttu-id="dc0e3-194">診断セットアップウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="dc0e3-194">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="dc0e3-195">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="dc0e3-195">displayToneSetupDisabled</span></span>|<span data-ttu-id="dc0e3-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc0e3-196">Boolean</span></span>|<span data-ttu-id="dc0e3-197">Displaytone の設定画面が無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="dc0e3-197">Indicates if displaytone setup screen is disabled</span></span>|
|<span data-ttu-id="dc0e3-198">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="dc0e3-198">privacyPaneDisabled</span></span>|<span data-ttu-id="dc0e3-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc0e3-199">Boolean</span></span>|<span data-ttu-id="dc0e3-200">プライバシー画面が無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="dc0e3-200">Indicates if privacy screen is disabled</span></span>|
|<span data-ttu-id="dc0e3-201">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="dc0e3-201">deviceNameTemplate</span></span>|<span data-ttu-id="dc0e3-202">String</span><span class="sxs-lookup"><span data-stu-id="dc0e3-202">String</span></span>|<span data-ttu-id="dc0e3-203">リテラルまたは名前のパターンを設定します。</span><span class="sxs-lookup"><span data-stu-id="dc0e3-203">Sets a literal or name pattern.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dc0e3-204">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="dc0e3-204">Relationships</span></span>
<span data-ttu-id="dc0e3-205">なし</span><span class="sxs-lookup"><span data-stu-id="dc0e3-205">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dc0e3-206">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dc0e3-206">JSON Representation</span></span>
<span data-ttu-id="dc0e3-207">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="dc0e3-207">Here is a JSON representation of the resource.</span></span>
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
  "privacyPaneDisabled": true,
  "deviceNameTemplate": "String"
}
```



