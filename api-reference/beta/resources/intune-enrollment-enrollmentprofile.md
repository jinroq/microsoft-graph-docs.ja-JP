---
title: enrollmentProfile リソースの種類
description: EnrollmentProfile リソースでは、プレステージされて id が特定のデバイスの登録を有効にするのには事前登録を提供する必要がある構成のコレクションを表します。 ステージング済みのデバイスの id は、対応するデバイスの登録時のプロファイルの構成を適用するのには、このタイプのプロファイルに割り当てられます。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7a7ce4aac1e22610d539419dd6a63d124616b83f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396841"
---
# <a name="enrollmentprofile-resource-type"></a><span data-ttu-id="f2ff7-104">enrollmentProfile リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f2ff7-104">enrollmentProfile resource type</span></span>

> <span data-ttu-id="f2ff7-105">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f2ff7-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f2ff7-106">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f2ff7-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f2ff7-107">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f2ff7-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2ff7-108">EnrollmentProfile リソースでは、プレステージされて id が特定のデバイスの登録を有効にするのには事前登録を提供する必要がある構成のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="f2ff7-108">The enrollmentProfile resource represents a collection of configurations which must be provided pre-enrollment to enable enrolling certain devices whose identities have been pre-staged.</span></span> <span data-ttu-id="f2ff7-109">ステージング済みのデバイスの id は、対応するデバイスの登録時のプロファイルの構成を適用するのには、このタイプのプロファイルに割り当てられます。</span><span class="sxs-lookup"><span data-stu-id="f2ff7-109">Pre-staged device identities are assigned to this type of profile to apply the profile's configurations at enrollment of the corresponding device.</span></span>

## <a name="methods"></a><span data-ttu-id="f2ff7-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="f2ff7-110">Methods</span></span>
|<span data-ttu-id="f2ff7-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="f2ff7-111">Method</span></span>|<span data-ttu-id="f2ff7-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f2ff7-112">Return Type</span></span>|<span data-ttu-id="f2ff7-113">説明</span><span class="sxs-lookup"><span data-stu-id="f2ff7-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f2ff7-114">リスト enrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="f2ff7-114">List enrollmentProfiles</span></span>](../api/intune-enrollment-enrollmentprofile-list.md)|<span data-ttu-id="f2ff7-115">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f2ff7-115">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) collection</span></span>|<span data-ttu-id="f2ff7-116">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="f2ff7-116">List properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="f2ff7-117">EnrollmentProfile を取得します。</span><span class="sxs-lookup"><span data-stu-id="f2ff7-117">Get enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-get.md)|[<span data-ttu-id="f2ff7-118">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="f2ff7-118">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="f2ff7-119">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f2ff7-119">Read properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="f2ff7-120">EnrollmentProfile を作成します。</span><span class="sxs-lookup"><span data-stu-id="f2ff7-120">Create enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-create.md)|[<span data-ttu-id="f2ff7-121">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="f2ff7-121">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="f2ff7-122">新しい[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="f2ff7-122">Create a new [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="f2ff7-123">EnrollmentProfile を削除します。</span><span class="sxs-lookup"><span data-stu-id="f2ff7-123">Delete enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-delete.md)|<span data-ttu-id="f2ff7-124">なし</span><span class="sxs-lookup"><span data-stu-id="f2ff7-124">None</span></span>|<span data-ttu-id="f2ff7-125">の[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="f2ff7-125">Deletes a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span></span>|
|[<span data-ttu-id="f2ff7-126">EnrollmentProfile を更新します。</span><span class="sxs-lookup"><span data-stu-id="f2ff7-126">Update enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-update.md)|[<span data-ttu-id="f2ff7-127">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="f2ff7-127">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="f2ff7-128">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f2ff7-128">Update the properties of a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="f2ff7-129">setDefaultProfile アクション</span><span class="sxs-lookup"><span data-stu-id="f2ff7-129">setDefaultProfile action</span></span>](../api/intune-enrollment-enrollmentprofile-setdefaultprofile.md)|<span data-ttu-id="f2ff7-130">なし</span><span class="sxs-lookup"><span data-stu-id="f2ff7-130">None</span></span>|<span data-ttu-id="f2ff7-131">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="f2ff7-131">Not yet documented</span></span>|
|[<span data-ttu-id="f2ff7-132">exportMobileConfig 関数</span><span class="sxs-lookup"><span data-stu-id="f2ff7-132">exportMobileConfig function</span></span>](../api/intune-enrollment-enrollmentprofile-exportmobileconfig.md)|<span data-ttu-id="f2ff7-133">String</span><span class="sxs-lookup"><span data-stu-id="f2ff7-133">String</span></span>|<span data-ttu-id="f2ff7-134">モバイルの構成をエクスポートします。</span><span class="sxs-lookup"><span data-stu-id="f2ff7-134">Exports the mobile configuration</span></span>|
|[<span data-ttu-id="f2ff7-135">updateDeviceProfileAssignment アクション</span><span class="sxs-lookup"><span data-stu-id="f2ff7-135">updateDeviceProfileAssignment action</span></span>](../api/intune-enrollment-enrollmentprofile-updatedeviceprofileassignment.md)|<span data-ttu-id="f2ff7-136">なし</span><span class="sxs-lookup"><span data-stu-id="f2ff7-136">None</span></span>|<span data-ttu-id="f2ff7-137">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="f2ff7-137">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="f2ff7-138">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f2ff7-138">Properties</span></span>
|<span data-ttu-id="f2ff7-139">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f2ff7-139">Property</span></span>|<span data-ttu-id="f2ff7-140">型</span><span class="sxs-lookup"><span data-stu-id="f2ff7-140">Type</span></span>|<span data-ttu-id="f2ff7-141">説明</span><span class="sxs-lookup"><span data-stu-id="f2ff7-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2ff7-142">id</span><span class="sxs-lookup"><span data-stu-id="f2ff7-142">id</span></span>|<span data-ttu-id="f2ff7-143">String</span><span class="sxs-lookup"><span data-stu-id="f2ff7-143">String</span></span>|<span data-ttu-id="f2ff7-144">オブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="f2ff7-144">The GUID for the object</span></span>|
|<span data-ttu-id="f2ff7-145">displayName</span><span class="sxs-lookup"><span data-stu-id="f2ff7-145">displayName</span></span>|<span data-ttu-id="f2ff7-146">String</span><span class="sxs-lookup"><span data-stu-id="f2ff7-146">String</span></span>|<span data-ttu-id="f2ff7-147">プロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="f2ff7-147">Name of the profile</span></span>|
|<span data-ttu-id="f2ff7-148">説明</span><span class="sxs-lookup"><span data-stu-id="f2ff7-148">description</span></span>|<span data-ttu-id="f2ff7-149">String</span><span class="sxs-lookup"><span data-stu-id="f2ff7-149">String</span></span>|<span data-ttu-id="f2ff7-150">プロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="f2ff7-150">Description of the profile</span></span>|
|<span data-ttu-id="f2ff7-151">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="f2ff7-151">requiresUserAuthentication</span></span>|<span data-ttu-id="f2ff7-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="f2ff7-152">Boolean</span></span>|<span data-ttu-id="f2ff7-153">プロファイルにユーザー認証が必要なかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="f2ff7-153">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="f2ff7-154">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="f2ff7-154">configurationEndpointUrl</span></span>|<span data-ttu-id="f2ff7-155">String</span><span class="sxs-lookup"><span data-stu-id="f2ff7-155">String</span></span>|<span data-ttu-id="f2ff7-156">登録に使用するエンドポイントの url を構成</span><span class="sxs-lookup"><span data-stu-id="f2ff7-156">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="f2ff7-157">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="f2ff7-157">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="f2ff7-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="f2ff7-158">Boolean</span></span>|<span data-ttu-id="f2ff7-159">アップルらくらく企業ポータルではなくを使用して認証することを示します。</span><span class="sxs-lookup"><span data-stu-id="f2ff7-159">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|
|<span data-ttu-id="f2ff7-160">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="f2ff7-160">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="f2ff7-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="f2ff7-161">Boolean</span></span>|<span data-ttu-id="f2ff7-162">セットアップ アシスタントが登録されているデバイス上の会社のポータルが必要であることを示します。</span><span class="sxs-lookup"><span data-stu-id="f2ff7-162">Indicates that Company Portal is required on setup assistant enrolled devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="f2ff7-163">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f2ff7-163">Relationships</span></span>
<span data-ttu-id="f2ff7-164">なし</span><span class="sxs-lookup"><span data-stu-id="f2ff7-164">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f2ff7-165">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f2ff7-165">JSON Representation</span></span>
<span data-ttu-id="f2ff7-166">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f2ff7-166">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.enrollmentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.enrollmentProfile",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "String",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true
}
```




