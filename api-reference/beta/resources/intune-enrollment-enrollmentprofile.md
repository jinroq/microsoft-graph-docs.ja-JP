---
title: しましたリソースの種類
description: しましたリソースは、事前登録を提供する必要がある構成のコレクションを表します。これにより、id が事前にステージングされている特定のデバイスを登録することができます。 事前に展開されたデバイス id は、対応するデバイスの登録時にプロファイルの構成を適用するために、この種類のプロファイルに割り当てられます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: abc00f27ef65cdddfef30a06bef55a8fa44e488a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573838"
---
# <a name="enrollmentprofile-resource-type"></a><span data-ttu-id="b3992-104">しましたリソースの種類</span><span class="sxs-lookup"><span data-stu-id="b3992-104">enrollmentProfile resource type</span></span>

> <span data-ttu-id="b3992-105">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b3992-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b3992-106">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b3992-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3992-107">しましたリソースは、事前登録を提供する必要がある構成のコレクションを表します。これにより、id が事前にステージングされている特定のデバイスを登録することができます。</span><span class="sxs-lookup"><span data-stu-id="b3992-107">The enrollmentProfile resource represents a collection of configurations which must be provided pre-enrollment to enable enrolling certain devices whose identities have been pre-staged.</span></span> <span data-ttu-id="b3992-108">事前に展開されたデバイス id は、対応するデバイスの登録時にプロファイルの構成を適用するために、この種類のプロファイルに割り当てられます。</span><span class="sxs-lookup"><span data-stu-id="b3992-108">Pre-staged device identities are assigned to this type of profile to apply the profile's configurations at enrollment of the corresponding device.</span></span>

## <a name="methods"></a><span data-ttu-id="b3992-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="b3992-109">Methods</span></span>
|<span data-ttu-id="b3992-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="b3992-110">Method</span></span>|<span data-ttu-id="b3992-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b3992-111">Return Type</span></span>|<span data-ttu-id="b3992-112">説明</span><span class="sxs-lookup"><span data-stu-id="b3992-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b3992-113">リスト enrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="b3992-113">List enrollmentProfiles</span></span>](../api/intune-enrollment-enrollmentprofile-list.md)|<span data-ttu-id="b3992-114">[しました](../resources/intune-enrollment-enrollmentprofile.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b3992-114">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) collection</span></span>|<span data-ttu-id="b3992-115">[しました](../resources/intune-enrollment-enrollmentprofile.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="b3992-115">List properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="b3992-116">しましたを取得する</span><span class="sxs-lookup"><span data-stu-id="b3992-116">Get enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-get.md)|[<span data-ttu-id="b3992-117">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="b3992-117">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="b3992-118">[しました](../resources/intune-enrollment-enrollmentprofile.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b3992-118">Read properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="b3992-119">しましたを作成する</span><span class="sxs-lookup"><span data-stu-id="b3992-119">Create enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-create.md)|[<span data-ttu-id="b3992-120">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="b3992-120">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="b3992-121">新しい[しました](../resources/intune-enrollment-enrollmentprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="b3992-121">Create a new [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="b3992-122">しましたの削除</span><span class="sxs-lookup"><span data-stu-id="b3992-122">Delete enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-delete.md)|<span data-ttu-id="b3992-123">なし</span><span class="sxs-lookup"><span data-stu-id="b3992-123">None</span></span>|<span data-ttu-id="b3992-124">[しました](../resources/intune-enrollment-enrollmentprofile.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="b3992-124">Deletes a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span></span>|
|[<span data-ttu-id="b3992-125">しましたの更新</span><span class="sxs-lookup"><span data-stu-id="b3992-125">Update enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-update.md)|[<span data-ttu-id="b3992-126">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="b3992-126">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="b3992-127">[しました](../resources/intune-enrollment-enrollmentprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b3992-127">Update the properties of a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="b3992-128">setDefaultProfile アクション</span><span class="sxs-lookup"><span data-stu-id="b3992-128">setDefaultProfile action</span></span>](../api/intune-enrollment-enrollmentprofile-setdefaultprofile.md)|<span data-ttu-id="b3992-129">なし</span><span class="sxs-lookup"><span data-stu-id="b3992-129">None</span></span>|<span data-ttu-id="b3992-130">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="b3992-130">Not yet documented</span></span>|
|[<span data-ttu-id="b3992-131">exportmobileconfig 関数</span><span class="sxs-lookup"><span data-stu-id="b3992-131">exportMobileConfig function</span></span>](../api/intune-enrollment-enrollmentprofile-exportmobileconfig.md)|<span data-ttu-id="b3992-132">String</span><span class="sxs-lookup"><span data-stu-id="b3992-132">String</span></span>|<span data-ttu-id="b3992-133">モバイル構成をエクスポートします。</span><span class="sxs-lookup"><span data-stu-id="b3992-133">Exports the mobile configuration</span></span>|
|[<span data-ttu-id="b3992-134">updateDeviceProfileAssignment アクション</span><span class="sxs-lookup"><span data-stu-id="b3992-134">updateDeviceProfileAssignment action</span></span>](../api/intune-enrollment-enrollmentprofile-updatedeviceprofileassignment.md)|<span data-ttu-id="b3992-135">なし</span><span class="sxs-lookup"><span data-stu-id="b3992-135">None</span></span>|<span data-ttu-id="b3992-136">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="b3992-136">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="b3992-137">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b3992-137">Properties</span></span>
|<span data-ttu-id="b3992-138">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b3992-138">Property</span></span>|<span data-ttu-id="b3992-139">型</span><span class="sxs-lookup"><span data-stu-id="b3992-139">Type</span></span>|<span data-ttu-id="b3992-140">説明</span><span class="sxs-lookup"><span data-stu-id="b3992-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3992-141">id</span><span class="sxs-lookup"><span data-stu-id="b3992-141">id</span></span>|<span data-ttu-id="b3992-142">String</span><span class="sxs-lookup"><span data-stu-id="b3992-142">String</span></span>|<span data-ttu-id="b3992-143">オブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="b3992-143">The GUID for the object</span></span>|
|<span data-ttu-id="b3992-144">displayName</span><span class="sxs-lookup"><span data-stu-id="b3992-144">displayName</span></span>|<span data-ttu-id="b3992-145">String</span><span class="sxs-lookup"><span data-stu-id="b3992-145">String</span></span>|<span data-ttu-id="b3992-146">プロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="b3992-146">Name of the profile</span></span>|
|<span data-ttu-id="b3992-147">説明</span><span class="sxs-lookup"><span data-stu-id="b3992-147">description</span></span>|<span data-ttu-id="b3992-148">String</span><span class="sxs-lookup"><span data-stu-id="b3992-148">String</span></span>|<span data-ttu-id="b3992-149">プロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="b3992-149">Description of the profile</span></span>|
|<span data-ttu-id="b3992-150">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="b3992-150">requiresUserAuthentication</span></span>|<span data-ttu-id="b3992-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3992-151">Boolean</span></span>|<span data-ttu-id="b3992-152">プロファイルにユーザー認証が必要かどうかを示します</span><span class="sxs-lookup"><span data-stu-id="b3992-152">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="b3992-153">configurationendpointurl</span><span class="sxs-lookup"><span data-stu-id="b3992-153">configurationEndpointUrl</span></span>|<span data-ttu-id="b3992-154">String</span><span class="sxs-lookup"><span data-stu-id="b3992-154">String</span></span>|<span data-ttu-id="b3992-155">登録に使用する構成エンドポイント url</span><span class="sxs-lookup"><span data-stu-id="b3992-155">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="b3992-156">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="b3992-156">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="b3992-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3992-157">Boolean</span></span>|<span data-ttu-id="b3992-158">会社のポータルではなく、Apple セットアップアシスタントを使用して認証することを示します。</span><span class="sxs-lookup"><span data-stu-id="b3992-158">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|
|<span data-ttu-id="b3992-159">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="b3992-159">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="b3992-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3992-160">Boolean</span></span>|<span data-ttu-id="b3992-161">セットアップアシスタントの登録済みデバイスで会社のポータルが必要であることを示します。</span><span class="sxs-lookup"><span data-stu-id="b3992-161">Indicates that Company Portal is required on setup assistant enrolled devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="b3992-162">関係</span><span class="sxs-lookup"><span data-stu-id="b3992-162">Relationships</span></span>
<span data-ttu-id="b3992-163">なし</span><span class="sxs-lookup"><span data-stu-id="b3992-163">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b3992-164">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b3992-164">JSON Representation</span></span>
<span data-ttu-id="b3992-165">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b3992-165">Here is a JSON representation of the resource.</span></span>
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





