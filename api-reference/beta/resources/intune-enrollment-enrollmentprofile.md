---
title: enrollmentProfile リソースの種類
description: EnrollmentProfile リソースでは、プレステージされて id が特定のデバイスの登録を有効にするのには事前登録を提供する必要がある構成のコレクションを表します。 ステージング済みのデバイスの id は、対応するデバイスの登録時のプロファイルの構成を適用するのには、このタイプのプロファイルに割り当てられます。
ms.openlocfilehash: 884fee5c6851e79d96cd036294e5e5485d6df66a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070132"
---
# <a name="enrollmentprofile-resource-type"></a><span data-ttu-id="dea95-104">enrollmentProfile リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dea95-104">enrollmentProfile resource type</span></span>

> <span data-ttu-id="dea95-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="dea95-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dea95-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dea95-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dea95-107">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="dea95-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dea95-108">EnrollmentProfile リソースでは、プレステージされて id が特定のデバイスの登録を有効にするのには事前登録を提供する必要がある構成のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="dea95-108">The enrollmentProfile resource represents a collection of configurations which must be provided pre-enrollment to enable enrolling certain devices whose identities have been pre-staged.</span></span> <span data-ttu-id="dea95-109">ステージング済みのデバイスの id は、対応するデバイスの登録時のプロファイルの構成を適用するのには、このタイプのプロファイルに割り当てられます。</span><span class="sxs-lookup"><span data-stu-id="dea95-109">Pre-staged device identities are assigned to this type of profile to apply the profile's configurations at enrollment of the corresponding device.</span></span>
## <a name="methods"></a><span data-ttu-id="dea95-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="dea95-110">Methods</span></span>
|<span data-ttu-id="dea95-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="dea95-111">Method</span></span>|<span data-ttu-id="dea95-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="dea95-112">Return Type</span></span>|<span data-ttu-id="dea95-113">説明</span><span class="sxs-lookup"><span data-stu-id="dea95-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="dea95-114">リスト enrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="dea95-114">List enrollmentProfiles</span></span>](../api/intune-enrollment-enrollmentprofile-list.md)|<span data-ttu-id="dea95-115">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="dea95-115">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) collection</span></span>|<span data-ttu-id="dea95-116">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="dea95-116">List properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="dea95-117">EnrollmentProfile を取得します。</span><span class="sxs-lookup"><span data-stu-id="dea95-117">Get enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-get.md)|[<span data-ttu-id="dea95-118">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="dea95-118">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="dea95-119">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dea95-119">Read properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="dea95-120">EnrollmentProfile を作成します。</span><span class="sxs-lookup"><span data-stu-id="dea95-120">Create enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-create.md)|[<span data-ttu-id="dea95-121">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="dea95-121">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="dea95-122">新しい[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="dea95-122">Create a new [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="dea95-123">EnrollmentProfile を削除します。</span><span class="sxs-lookup"><span data-stu-id="dea95-123">Delete enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-delete.md)|<span data-ttu-id="dea95-124">なし</span><span class="sxs-lookup"><span data-stu-id="dea95-124">None</span></span>|<span data-ttu-id="dea95-125">の[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="dea95-125">Deletes a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span></span>|
|[<span data-ttu-id="dea95-126">EnrollmentProfile を更新します。</span><span class="sxs-lookup"><span data-stu-id="dea95-126">Update enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-update.md)|[<span data-ttu-id="dea95-127">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="dea95-127">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="dea95-128">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="dea95-128">Update the properties of a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="dea95-129">setDefaultProfile アクション</span><span class="sxs-lookup"><span data-stu-id="dea95-129">setDefaultProfile action</span></span>](../api/intune-enrollment-enrollmentprofile-setdefaultprofile.md)|<span data-ttu-id="dea95-130">なし</span><span class="sxs-lookup"><span data-stu-id="dea95-130">None</span></span>|<span data-ttu-id="dea95-131">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="dea95-131">Not yet documented</span></span>|
|[<span data-ttu-id="dea95-132">exportMobileConfig 関数</span><span class="sxs-lookup"><span data-stu-id="dea95-132">exportMobileConfig function</span></span>](../api/intune-enrollment-enrollmentprofile-exportmobileconfig.md)|<span data-ttu-id="dea95-133">String</span><span class="sxs-lookup"><span data-stu-id="dea95-133">String</span></span>|<span data-ttu-id="dea95-134">モバイルの構成をエクスポートします。</span><span class="sxs-lookup"><span data-stu-id="dea95-134">Exports the mobile configuration</span></span>|
|[<span data-ttu-id="dea95-135">updateDeviceProfileAssignment アクション</span><span class="sxs-lookup"><span data-stu-id="dea95-135">updateDeviceProfileAssignment action</span></span>](../api/intune-enrollment-enrollmentprofile-updatedeviceprofileassignment.md)|<span data-ttu-id="dea95-136">なし</span><span class="sxs-lookup"><span data-stu-id="dea95-136">None</span></span>|<span data-ttu-id="dea95-137">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="dea95-137">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="dea95-138">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dea95-138">Properties</span></span>
|<span data-ttu-id="dea95-139">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dea95-139">Property</span></span>|<span data-ttu-id="dea95-140">型</span><span class="sxs-lookup"><span data-stu-id="dea95-140">Type</span></span>|<span data-ttu-id="dea95-141">説明</span><span class="sxs-lookup"><span data-stu-id="dea95-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dea95-142">id</span><span class="sxs-lookup"><span data-stu-id="dea95-142">id</span></span>|<span data-ttu-id="dea95-143">String</span><span class="sxs-lookup"><span data-stu-id="dea95-143">String</span></span>|<span data-ttu-id="dea95-144">オブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="dea95-144">The GUID for the object</span></span>|
|<span data-ttu-id="dea95-145">displayName</span><span class="sxs-lookup"><span data-stu-id="dea95-145">displayName</span></span>|<span data-ttu-id="dea95-146">String</span><span class="sxs-lookup"><span data-stu-id="dea95-146">String</span></span>|<span data-ttu-id="dea95-147">プロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="dea95-147">Name of the profile</span></span>|
|<span data-ttu-id="dea95-148">説明</span><span class="sxs-lookup"><span data-stu-id="dea95-148">description</span></span>|<span data-ttu-id="dea95-149">String</span><span class="sxs-lookup"><span data-stu-id="dea95-149">String</span></span>|<span data-ttu-id="dea95-150">プロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="dea95-150">Description of the profile</span></span>|
|<span data-ttu-id="dea95-151">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="dea95-151">requiresUserAuthentication</span></span>|<span data-ttu-id="dea95-152">ブール値</span><span class="sxs-lookup"><span data-stu-id="dea95-152">Boolean</span></span>|<span data-ttu-id="dea95-153">プロファイルにユーザー認証が必要なかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="dea95-153">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="dea95-154">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="dea95-154">configurationEndpointUrl</span></span>|<span data-ttu-id="dea95-155">String</span><span class="sxs-lookup"><span data-stu-id="dea95-155">String</span></span>|<span data-ttu-id="dea95-156">登録に使用するエンドポイントの url を構成</span><span class="sxs-lookup"><span data-stu-id="dea95-156">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="dea95-157">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="dea95-157">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="dea95-158">ブール値</span><span class="sxs-lookup"><span data-stu-id="dea95-158">Boolean</span></span>|<span data-ttu-id="dea95-159">アップルらくらく企業ポータルではなくを使用して認証することを示します。</span><span class="sxs-lookup"><span data-stu-id="dea95-159">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dea95-160">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="dea95-160">Relationships</span></span>
<span data-ttu-id="dea95-161">なし</span><span class="sxs-lookup"><span data-stu-id="dea95-161">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="dea95-162">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dea95-162">JSON Representation</span></span>
<span data-ttu-id="dea95-163">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="dea95-163">Here is a JSON representation of the resource.</span></span>
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
  "enableAuthenticationViaCompanyPortal": true
}
```





