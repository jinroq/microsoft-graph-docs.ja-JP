---
title: androidDeviceOwnerEnrollmentProfile リソースの種類
description: Google のクラウド管理を使用して COSU デバイスを登録するために使われる登録プロファイルです。
ms.openlocfilehash: 0ca468a624f5b1793b09eb6b4d9d9e003cae3ac7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067536"
---
# <a name="androiddeviceownerenrollmentprofile-resource-type"></a><span data-ttu-id="4eaf7-103">androidDeviceOwnerEnrollmentProfile リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4eaf7-103">androidDeviceOwnerEnrollmentProfile resource type</span></span>

> <span data-ttu-id="4eaf7-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4eaf7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4eaf7-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4eaf7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4eaf7-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4eaf7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4eaf7-107">Google のクラウド管理を使用して COSU デバイスを登録するために使われる登録プロファイルです。</span><span class="sxs-lookup"><span data-stu-id="4eaf7-107">Enrollment Profile used to enroll COSU devices using Google's Cloud Management.</span></span>
## <a name="methods"></a><span data-ttu-id="4eaf7-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="4eaf7-108">Methods</span></span>
|<span data-ttu-id="4eaf7-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="4eaf7-109">Method</span></span>|<span data-ttu-id="4eaf7-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4eaf7-110">Return Type</span></span>|<span data-ttu-id="4eaf7-111">説明</span><span class="sxs-lookup"><span data-stu-id="4eaf7-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4eaf7-112">リスト androidDeviceOwnerEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="4eaf7-112">List androidDeviceOwnerEnrollmentProfiles</span></span>](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-list.md)|<span data-ttu-id="4eaf7-113">[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="4eaf7-113">[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) collection</span></span>|<span data-ttu-id="4eaf7-114">[AndroidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="4eaf7-114">List properties and relationships of the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="4eaf7-115">AndroidDeviceOwnerEnrollmentProfile を取得します。</span><span class="sxs-lookup"><span data-stu-id="4eaf7-115">Get androidDeviceOwnerEnrollmentProfile</span></span>](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-get.md)|[<span data-ttu-id="4eaf7-116">androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="4eaf7-116">androidDeviceOwnerEnrollmentProfile</span></span>](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|<span data-ttu-id="4eaf7-117">[AndroidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4eaf7-117">Read properties and relationships of the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="4eaf7-118">AndroidDeviceOwnerEnrollmentProfile を作成します。</span><span class="sxs-lookup"><span data-stu-id="4eaf7-118">Create androidDeviceOwnerEnrollmentProfile</span></span>](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-create.md)|[<span data-ttu-id="4eaf7-119">androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="4eaf7-119">androidDeviceOwnerEnrollmentProfile</span></span>](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|<span data-ttu-id="4eaf7-120">新しい[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="4eaf7-120">Create a new [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="4eaf7-121">AndroidDeviceOwnerEnrollmentProfile を削除します。</span><span class="sxs-lookup"><span data-stu-id="4eaf7-121">Delete androidDeviceOwnerEnrollmentProfile</span></span>](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-delete.md)|<span data-ttu-id="4eaf7-122">なし</span><span class="sxs-lookup"><span data-stu-id="4eaf7-122">None</span></span>|<span data-ttu-id="4eaf7-123">の[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="4eaf7-123">Deletes a [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md).</span></span>|
|[<span data-ttu-id="4eaf7-124">AndroidDeviceOwnerEnrollmentProfile を更新します。</span><span class="sxs-lookup"><span data-stu-id="4eaf7-124">Update androidDeviceOwnerEnrollmentProfile</span></span>](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-update.md)|[<span data-ttu-id="4eaf7-125">androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="4eaf7-125">androidDeviceOwnerEnrollmentProfile</span></span>](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|<span data-ttu-id="4eaf7-126">[AndroidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4eaf7-126">Update the properties of a [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="4eaf7-127">revokeToken action</span><span class="sxs-lookup"><span data-stu-id="4eaf7-127">revokeToken action</span></span>](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-revoketoken.md)|<span data-ttu-id="4eaf7-128">なし</span><span class="sxs-lookup"><span data-stu-id="4eaf7-128">None</span></span>|<span data-ttu-id="4eaf7-129">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="4eaf7-129">Not yet documented</span></span>|
|[<span data-ttu-id="4eaf7-130">createToken action</span><span class="sxs-lookup"><span data-stu-id="4eaf7-130">createToken action</span></span>](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-createtoken.md)|<span data-ttu-id="4eaf7-131">なし</span><span class="sxs-lookup"><span data-stu-id="4eaf7-131">None</span></span>|<span data-ttu-id="4eaf7-132">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="4eaf7-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="4eaf7-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4eaf7-133">Properties</span></span>
|<span data-ttu-id="4eaf7-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4eaf7-134">Property</span></span>|<span data-ttu-id="4eaf7-135">型</span><span class="sxs-lookup"><span data-stu-id="4eaf7-135">Type</span></span>|<span data-ttu-id="4eaf7-136">説明</span><span class="sxs-lookup"><span data-stu-id="4eaf7-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4eaf7-137">accountId</span><span class="sxs-lookup"><span data-stu-id="4eaf7-137">accountId</span></span>|<span data-ttu-id="4eaf7-138">String</span><span class="sxs-lookup"><span data-stu-id="4eaf7-138">String</span></span>|<span data-ttu-id="4eaf7-139">登録プロファイルが属するテナント GUID。</span><span class="sxs-lookup"><span data-stu-id="4eaf7-139">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="4eaf7-140">id</span><span class="sxs-lookup"><span data-stu-id="4eaf7-140">id</span></span>|<span data-ttu-id="4eaf7-141">String</span><span class="sxs-lookup"><span data-stu-id="4eaf7-141">String</span></span>|<span data-ttu-id="4eaf7-142">登録プロファイル用の一意な GUID。</span><span class="sxs-lookup"><span data-stu-id="4eaf7-142">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="4eaf7-143">displayName</span><span class="sxs-lookup"><span data-stu-id="4eaf7-143">displayName</span></span>|<span data-ttu-id="4eaf7-144">String</span><span class="sxs-lookup"><span data-stu-id="4eaf7-144">String</span></span>|<span data-ttu-id="4eaf7-145">登録プロファイルの表示名。</span><span class="sxs-lookup"><span data-stu-id="4eaf7-145">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="4eaf7-146">説明</span><span class="sxs-lookup"><span data-stu-id="4eaf7-146">description</span></span>|<span data-ttu-id="4eaf7-147">String</span><span class="sxs-lookup"><span data-stu-id="4eaf7-147">String</span></span>|<span data-ttu-id="4eaf7-148">登録プロファイルの説明。</span><span class="sxs-lookup"><span data-stu-id="4eaf7-148">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="4eaf7-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4eaf7-149">createdDateTime</span></span>|<span data-ttu-id="4eaf7-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4eaf7-150">DateTimeOffset</span></span>|<span data-ttu-id="4eaf7-151">登録プロファイルが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="4eaf7-151">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="4eaf7-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4eaf7-152">lastModifiedDateTime</span></span>|<span data-ttu-id="4eaf7-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4eaf7-153">DateTimeOffset</span></span>|<span data-ttu-id="4eaf7-154">登録プロファイルが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="4eaf7-154">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="4eaf7-155">tokenValue</span><span class="sxs-lookup"><span data-stu-id="4eaf7-155">tokenValue</span></span>|<span data-ttu-id="4eaf7-156">String</span><span class="sxs-lookup"><span data-stu-id="4eaf7-156">String</span></span>|<span data-ttu-id="4eaf7-157">この登録プロファイル用に最後に作成されたトークンの値。</span><span class="sxs-lookup"><span data-stu-id="4eaf7-157">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="4eaf7-158">tokenCreationDateTime</span><span class="sxs-lookup"><span data-stu-id="4eaf7-158">tokenCreationDateTime</span></span>|<span data-ttu-id="4eaf7-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4eaf7-159">DateTimeOffset</span></span>|<span data-ttu-id="4eaf7-160">直前に作成されたトークンが作成された日時です。</span><span class="sxs-lookup"><span data-stu-id="4eaf7-160">Date time the most recently created token was created.</span></span>|
|<span data-ttu-id="4eaf7-161">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="4eaf7-161">tokenExpirationDateTime</span></span>|<span data-ttu-id="4eaf7-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4eaf7-162">DateTimeOffset</span></span>|<span data-ttu-id="4eaf7-163">最後に作成されたトークンの有効期限が切れる日時。</span><span class="sxs-lookup"><span data-stu-id="4eaf7-163">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="4eaf7-164">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4eaf7-164">enrolledDeviceCount</span></span>|<span data-ttu-id="4eaf7-165">Int32</span><span class="sxs-lookup"><span data-stu-id="4eaf7-165">Int32</span></span>|<span data-ttu-id="4eaf7-166">この登録プロファイルを使用して登録した Android デバイスの合計数。</span><span class="sxs-lookup"><span data-stu-id="4eaf7-166">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="4eaf7-167">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="4eaf7-167">qrCodeContent</span></span>|<span data-ttu-id="4eaf7-168">String</span><span class="sxs-lookup"><span data-stu-id="4eaf7-168">String</span></span>|<span data-ttu-id="4eaf7-169">トークン用の QR コードを生成するために使用された文字列。</span><span class="sxs-lookup"><span data-stu-id="4eaf7-169">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="4eaf7-170">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="4eaf7-170">qrCodeImage</span></span>|[<span data-ttu-id="4eaf7-171">mimeContent</span><span class="sxs-lookup"><span data-stu-id="4eaf7-171">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="4eaf7-172">トークンの QR コードを生成するために使用する文字列。</span><span class="sxs-lookup"><span data-stu-id="4eaf7-172">String used to generate a QR code for the token.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4eaf7-173">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4eaf7-173">Relationships</span></span>
<span data-ttu-id="4eaf7-174">なし</span><span class="sxs-lookup"><span data-stu-id="4eaf7-174">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4eaf7-175">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4eaf7-175">JSON Representation</span></span>
<span data-ttu-id="4eaf7-176">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4eaf7-176">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidDeviceOwnerEnrollmentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerEnrollmentProfile",
  "accountId": "String",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "tokenValue": "String",
  "tokenCreationDateTime": "String (timestamp)",
  "tokenExpirationDateTime": "String (timestamp)",
  "enrolledDeviceCount": 1024,
  "qrCodeContent": "String",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  }
}
```





