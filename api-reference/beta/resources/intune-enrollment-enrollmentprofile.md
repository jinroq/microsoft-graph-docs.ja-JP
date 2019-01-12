---
title: enrollmentProfile リソースの種類
description: EnrollmentProfile リソースでは、プレステージされて id が特定のデバイスの登録を有効にするのには事前登録を提供する必要がある構成のコレクションを表します。 ステージング済みのデバイスの id は、対応するデバイスの登録時のプロファイルの構成を適用するのには、このタイプのプロファイルに割り当てられます。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: b88745c060e71e32199a96b23f94fa0d3229d451
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935592"
---
# <a name="enrollmentprofile-resource-type"></a><span data-ttu-id="44d42-104">enrollmentProfile リソースの種類</span><span class="sxs-lookup"><span data-stu-id="44d42-104">enrollmentProfile resource type</span></span>

> <span data-ttu-id="44d42-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="44d42-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="44d42-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="44d42-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="44d42-107">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="44d42-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="44d42-108">EnrollmentProfile リソースでは、プレステージされて id が特定のデバイスの登録を有効にするのには事前登録を提供する必要がある構成のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="44d42-108">The enrollmentProfile resource represents a collection of configurations which must be provided pre-enrollment to enable enrolling certain devices whose identities have been pre-staged.</span></span> <span data-ttu-id="44d42-109">ステージング済みのデバイスの id は、対応するデバイスの登録時のプロファイルの構成を適用するのには、このタイプのプロファイルに割り当てられます。</span><span class="sxs-lookup"><span data-stu-id="44d42-109">Pre-staged device identities are assigned to this type of profile to apply the profile's configurations at enrollment of the corresponding device.</span></span>
## <a name="methods"></a><span data-ttu-id="44d42-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="44d42-110">Methods</span></span>
|<span data-ttu-id="44d42-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="44d42-111">Method</span></span>|<span data-ttu-id="44d42-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="44d42-112">Return Type</span></span>|<span data-ttu-id="44d42-113">説明</span><span class="sxs-lookup"><span data-stu-id="44d42-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="44d42-114">リスト enrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="44d42-114">List enrollmentProfiles</span></span>](../api/intune-enrollment-enrollmentprofile-list.md)|<span data-ttu-id="44d42-115">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="44d42-115">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) collection</span></span>|<span data-ttu-id="44d42-116">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="44d42-116">List properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="44d42-117">EnrollmentProfile を取得します。</span><span class="sxs-lookup"><span data-stu-id="44d42-117">Get enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-get.md)|[<span data-ttu-id="44d42-118">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="44d42-118">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="44d42-119">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="44d42-119">Read properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="44d42-120">EnrollmentProfile を作成します。</span><span class="sxs-lookup"><span data-stu-id="44d42-120">Create enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-create.md)|[<span data-ttu-id="44d42-121">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="44d42-121">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="44d42-122">新しい[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="44d42-122">Create a new [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="44d42-123">EnrollmentProfile を削除します。</span><span class="sxs-lookup"><span data-stu-id="44d42-123">Delete enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-delete.md)|<span data-ttu-id="44d42-124">なし</span><span class="sxs-lookup"><span data-stu-id="44d42-124">None</span></span>|<span data-ttu-id="44d42-125">の[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="44d42-125">Deletes a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span></span>|
|[<span data-ttu-id="44d42-126">EnrollmentProfile を更新します。</span><span class="sxs-lookup"><span data-stu-id="44d42-126">Update enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-update.md)|[<span data-ttu-id="44d42-127">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="44d42-127">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="44d42-128">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="44d42-128">Update the properties of a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="44d42-129">setDefaultProfile アクション</span><span class="sxs-lookup"><span data-stu-id="44d42-129">setDefaultProfile action</span></span>](../api/intune-enrollment-enrollmentprofile-setdefaultprofile.md)|<span data-ttu-id="44d42-130">なし</span><span class="sxs-lookup"><span data-stu-id="44d42-130">None</span></span>|<span data-ttu-id="44d42-131">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="44d42-131">Not yet documented</span></span>|
|[<span data-ttu-id="44d42-132">exportMobileConfig 関数</span><span class="sxs-lookup"><span data-stu-id="44d42-132">exportMobileConfig function</span></span>](../api/intune-enrollment-enrollmentprofile-exportmobileconfig.md)|<span data-ttu-id="44d42-133">String</span><span class="sxs-lookup"><span data-stu-id="44d42-133">String</span></span>|<span data-ttu-id="44d42-134">モバイルの構成をエクスポートします。</span><span class="sxs-lookup"><span data-stu-id="44d42-134">Exports the mobile configuration</span></span>|
|[<span data-ttu-id="44d42-135">updateDeviceProfileAssignment アクション</span><span class="sxs-lookup"><span data-stu-id="44d42-135">updateDeviceProfileAssignment action</span></span>](../api/intune-enrollment-enrollmentprofile-updatedeviceprofileassignment.md)|<span data-ttu-id="44d42-136">なし</span><span class="sxs-lookup"><span data-stu-id="44d42-136">None</span></span>|<span data-ttu-id="44d42-137">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="44d42-137">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="44d42-138">プロパティ</span><span class="sxs-lookup"><span data-stu-id="44d42-138">Properties</span></span>
|<span data-ttu-id="44d42-139">プロパティ</span><span class="sxs-lookup"><span data-stu-id="44d42-139">Property</span></span>|<span data-ttu-id="44d42-140">種類</span><span class="sxs-lookup"><span data-stu-id="44d42-140">Type</span></span>|<span data-ttu-id="44d42-141">説明</span><span class="sxs-lookup"><span data-stu-id="44d42-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44d42-142">ID</span><span class="sxs-lookup"><span data-stu-id="44d42-142">id</span></span>|<span data-ttu-id="44d42-143">String</span><span class="sxs-lookup"><span data-stu-id="44d42-143">String</span></span>|<span data-ttu-id="44d42-144">オブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="44d42-144">The GUID for the object</span></span>|
|<span data-ttu-id="44d42-145">displayName</span><span class="sxs-lookup"><span data-stu-id="44d42-145">displayName</span></span>|<span data-ttu-id="44d42-146">String</span><span class="sxs-lookup"><span data-stu-id="44d42-146">String</span></span>|<span data-ttu-id="44d42-147">プロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="44d42-147">Name of the profile</span></span>|
|<span data-ttu-id="44d42-148">説明</span><span class="sxs-lookup"><span data-stu-id="44d42-148">description</span></span>|<span data-ttu-id="44d42-149">String</span><span class="sxs-lookup"><span data-stu-id="44d42-149">String</span></span>|<span data-ttu-id="44d42-150">プロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="44d42-150">Description of the profile</span></span>|
|<span data-ttu-id="44d42-151">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="44d42-151">requiresUserAuthentication</span></span>|<span data-ttu-id="44d42-152">ブール型</span><span class="sxs-lookup"><span data-stu-id="44d42-152">Boolean</span></span>|<span data-ttu-id="44d42-153">プロファイルにユーザー認証が必要なかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="44d42-153">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="44d42-154">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="44d42-154">configurationEndpointUrl</span></span>|<span data-ttu-id="44d42-155">String</span><span class="sxs-lookup"><span data-stu-id="44d42-155">String</span></span>|<span data-ttu-id="44d42-156">登録に使用するエンドポイントの url を構成</span><span class="sxs-lookup"><span data-stu-id="44d42-156">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="44d42-157">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="44d42-157">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="44d42-158">ブール型</span><span class="sxs-lookup"><span data-stu-id="44d42-158">Boolean</span></span>|<span data-ttu-id="44d42-159">アップルらくらく企業ポータルではなくを使用して認証することを示します。</span><span class="sxs-lookup"><span data-stu-id="44d42-159">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|

## <a name="relationships"></a><span data-ttu-id="44d42-160">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="44d42-160">Relationships</span></span>
<span data-ttu-id="44d42-161">なし</span><span class="sxs-lookup"><span data-stu-id="44d42-161">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="44d42-162">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="44d42-162">JSON Representation</span></span>
<span data-ttu-id="44d42-163">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="44d42-163">Here is a JSON representation of the resource.</span></span>
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





