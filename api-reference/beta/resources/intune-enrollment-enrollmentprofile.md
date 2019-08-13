---
title: しましたリソースの種類
description: しましたリソースは、事前登録を提供する必要がある構成のコレクションを表します。これにより、id が事前にステージングされている特定のデバイスを登録することができます。 事前に展開されたデバイス id は、対応するデバイスの登録時にプロファイルの構成を適用するために、この種類のプロファイルに割り当てられます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 623979d78a43ede047db90f722f4a160fb22f4ad
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327990"
---
# <a name="enrollmentprofile-resource-type"></a><span data-ttu-id="ee4c1-104">しましたリソースの種類</span><span class="sxs-lookup"><span data-stu-id="ee4c1-104">enrollmentProfile resource type</span></span>

> <span data-ttu-id="ee4c1-105">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee4c1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ee4c1-106">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ee4c1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee4c1-107">しましたリソースは、事前登録を提供する必要がある構成のコレクションを表します。これにより、id が事前にステージングされている特定のデバイスを登録することができます。</span><span class="sxs-lookup"><span data-stu-id="ee4c1-107">The enrollmentProfile resource represents a collection of configurations which must be provided pre-enrollment to enable enrolling certain devices whose identities have been pre-staged.</span></span> <span data-ttu-id="ee4c1-108">事前に展開されたデバイス id は、対応するデバイスの登録時にプロファイルの構成を適用するために、この種類のプロファイルに割り当てられます。</span><span class="sxs-lookup"><span data-stu-id="ee4c1-108">Pre-staged device identities are assigned to this type of profile to apply the profile's configurations at enrollment of the corresponding device.</span></span>

## <a name="methods"></a><span data-ttu-id="ee4c1-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="ee4c1-109">Methods</span></span>
|<span data-ttu-id="ee4c1-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="ee4c1-110">Method</span></span>|<span data-ttu-id="ee4c1-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ee4c1-111">Return Type</span></span>|<span data-ttu-id="ee4c1-112">説明</span><span class="sxs-lookup"><span data-stu-id="ee4c1-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ee4c1-113">リスト enrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="ee4c1-113">List enrollmentProfiles</span></span>](../api/intune-enrollment-enrollmentprofile-list.md)|<span data-ttu-id="ee4c1-114">[しました](../resources/intune-enrollment-enrollmentprofile.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ee4c1-114">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) collection</span></span>|<span data-ttu-id="ee4c1-115">[しました](../resources/intune-enrollment-enrollmentprofile.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="ee4c1-115">List properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="ee4c1-116">しましたを取得する</span><span class="sxs-lookup"><span data-stu-id="ee4c1-116">Get enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-get.md)|[<span data-ttu-id="ee4c1-117">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="ee4c1-117">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="ee4c1-118">[しました](../resources/intune-enrollment-enrollmentprofile.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ee4c1-118">Read properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="ee4c1-119">しましたを作成する</span><span class="sxs-lookup"><span data-stu-id="ee4c1-119">Create enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-create.md)|[<span data-ttu-id="ee4c1-120">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="ee4c1-120">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="ee4c1-121">新しい[しました](../resources/intune-enrollment-enrollmentprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="ee4c1-121">Create a new [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="ee4c1-122">しましたの削除</span><span class="sxs-lookup"><span data-stu-id="ee4c1-122">Delete enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-delete.md)|<span data-ttu-id="ee4c1-123">None</span><span class="sxs-lookup"><span data-stu-id="ee4c1-123">None</span></span>|<span data-ttu-id="ee4c1-124">[しました](../resources/intune-enrollment-enrollmentprofile.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="ee4c1-124">Deletes a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span></span>|
|[<span data-ttu-id="ee4c1-125">しましたの更新</span><span class="sxs-lookup"><span data-stu-id="ee4c1-125">Update enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-update.md)|[<span data-ttu-id="ee4c1-126">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="ee4c1-126">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="ee4c1-127">[しました](../resources/intune-enrollment-enrollmentprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ee4c1-127">Update the properties of a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="ee4c1-128">setDefaultProfile アクション</span><span class="sxs-lookup"><span data-stu-id="ee4c1-128">setDefaultProfile action</span></span>](../api/intune-enrollment-enrollmentprofile-setdefaultprofile.md)|<span data-ttu-id="ee4c1-129">なし</span><span class="sxs-lookup"><span data-stu-id="ee4c1-129">None</span></span>|<span data-ttu-id="ee4c1-130">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ee4c1-130">Not yet documented</span></span>|
|[<span data-ttu-id="ee4c1-131">exportMobileConfig 関数</span><span class="sxs-lookup"><span data-stu-id="ee4c1-131">exportMobileConfig function</span></span>](../api/intune-enrollment-enrollmentprofile-exportmobileconfig.md)|<span data-ttu-id="ee4c1-132">String</span><span class="sxs-lookup"><span data-stu-id="ee4c1-132">String</span></span>|<span data-ttu-id="ee4c1-133">モバイル構成をエクスポートします。</span><span class="sxs-lookup"><span data-stu-id="ee4c1-133">Exports the mobile configuration</span></span>|
|[<span data-ttu-id="ee4c1-134">updateDeviceProfileAssignment アクション</span><span class="sxs-lookup"><span data-stu-id="ee4c1-134">updateDeviceProfileAssignment action</span></span>](../api/intune-enrollment-enrollmentprofile-updatedeviceprofileassignment.md)|<span data-ttu-id="ee4c1-135">なし</span><span class="sxs-lookup"><span data-stu-id="ee4c1-135">None</span></span>|<span data-ttu-id="ee4c1-136">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ee4c1-136">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="ee4c1-137">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ee4c1-137">Properties</span></span>
|<span data-ttu-id="ee4c1-138">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ee4c1-138">Property</span></span>|<span data-ttu-id="ee4c1-139">型</span><span class="sxs-lookup"><span data-stu-id="ee4c1-139">Type</span></span>|<span data-ttu-id="ee4c1-140">説明</span><span class="sxs-lookup"><span data-stu-id="ee4c1-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee4c1-141">id</span><span class="sxs-lookup"><span data-stu-id="ee4c1-141">id</span></span>|<span data-ttu-id="ee4c1-142">文字列</span><span class="sxs-lookup"><span data-stu-id="ee4c1-142">String</span></span>|<span data-ttu-id="ee4c1-143">オブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="ee4c1-143">The GUID for the object</span></span>|
|<span data-ttu-id="ee4c1-144">displayName</span><span class="sxs-lookup"><span data-stu-id="ee4c1-144">displayName</span></span>|<span data-ttu-id="ee4c1-145">String</span><span class="sxs-lookup"><span data-stu-id="ee4c1-145">String</span></span>|<span data-ttu-id="ee4c1-146">プロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="ee4c1-146">Name of the profile</span></span>|
|<span data-ttu-id="ee4c1-147">description</span><span class="sxs-lookup"><span data-stu-id="ee4c1-147">description</span></span>|<span data-ttu-id="ee4c1-148">String</span><span class="sxs-lookup"><span data-stu-id="ee4c1-148">String</span></span>|<span data-ttu-id="ee4c1-149">プロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="ee4c1-149">Description of the profile</span></span>|
|<span data-ttu-id="ee4c1-150">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="ee4c1-150">requiresUserAuthentication</span></span>|<span data-ttu-id="ee4c1-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="ee4c1-151">Boolean</span></span>|<span data-ttu-id="ee4c1-152">プロファイルにユーザー認証が必要かどうかを示します</span><span class="sxs-lookup"><span data-stu-id="ee4c1-152">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="ee4c1-153">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="ee4c1-153">configurationEndpointUrl</span></span>|<span data-ttu-id="ee4c1-154">String</span><span class="sxs-lookup"><span data-stu-id="ee4c1-154">String</span></span>|<span data-ttu-id="ee4c1-155">登録に使用する構成エンドポイント url</span><span class="sxs-lookup"><span data-stu-id="ee4c1-155">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="ee4c1-156">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="ee4c1-156">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="ee4c1-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="ee4c1-157">Boolean</span></span>|<span data-ttu-id="ee4c1-158">会社のポータルではなく、Apple セットアップアシスタントを使用して認証することを示します。</span><span class="sxs-lookup"><span data-stu-id="ee4c1-158">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|
|<span data-ttu-id="ee4c1-159">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="ee4c1-159">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="ee4c1-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="ee4c1-160">Boolean</span></span>|<span data-ttu-id="ee4c1-161">セットアップアシスタントの登録済みデバイスで会社のポータルが必要であることを示します。</span><span class="sxs-lookup"><span data-stu-id="ee4c1-161">Indicates that Company Portal is required on setup assistant enrolled devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="ee4c1-162">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ee4c1-162">Relationships</span></span>
<span data-ttu-id="ee4c1-163">なし</span><span class="sxs-lookup"><span data-stu-id="ee4c1-163">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ee4c1-164">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ee4c1-164">JSON Representation</span></span>
<span data-ttu-id="ee4c1-165">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ee4c1-165">Here is a JSON representation of the resource.</span></span>
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



