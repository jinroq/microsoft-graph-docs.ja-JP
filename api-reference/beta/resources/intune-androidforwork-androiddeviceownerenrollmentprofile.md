---
title: androidDeviceOwnerEnrollmentProfile リソースの種類
description: Google のクラウド管理を使用して COSU デバイスを登録するために使われる登録プロファイルです。
localization_priority: Normal
ms.openlocfilehash: 17d8d00fb0c21d9474607e0cc388ce38687af0ce
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841875"
---
# <a name="androiddeviceownerenrollmentprofile-resource-type"></a><span data-ttu-id="1a855-103">androidDeviceOwnerEnrollmentProfile リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1a855-103">androidDeviceOwnerEnrollmentProfile resource type</span></span>

> <span data-ttu-id="1a855-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1a855-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1a855-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1a855-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1a855-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1a855-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1a855-107">Google のクラウド管理を使用して COSU デバイスを登録するために使われる登録プロファイルです。</span><span class="sxs-lookup"><span data-stu-id="1a855-107">Enrollment Profile used to enroll COSU devices using Google's Cloud Management.</span></span>
## <a name="methods"></a><span data-ttu-id="1a855-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="1a855-108">Methods</span></span>
|<span data-ttu-id="1a855-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="1a855-109">Method</span></span>|<span data-ttu-id="1a855-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1a855-110">Return Type</span></span>|<span data-ttu-id="1a855-111">説明</span><span class="sxs-lookup"><span data-stu-id="1a855-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1a855-112">リスト androidDeviceOwnerEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="1a855-112">List androidDeviceOwnerEnrollmentProfiles</span></span>](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-list.md)|<span data-ttu-id="1a855-113">[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1a855-113">[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) collection</span></span>|<span data-ttu-id="1a855-114">[AndroidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="1a855-114">List properties and relationships of the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="1a855-115">AndroidDeviceOwnerEnrollmentProfile を取得します。</span><span class="sxs-lookup"><span data-stu-id="1a855-115">Get androidDeviceOwnerEnrollmentProfile</span></span>](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-get.md)|[<span data-ttu-id="1a855-116">androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="1a855-116">androidDeviceOwnerEnrollmentProfile</span></span>](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|<span data-ttu-id="1a855-117">[AndroidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1a855-117">Read properties and relationships of the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="1a855-118">AndroidDeviceOwnerEnrollmentProfile を作成します。</span><span class="sxs-lookup"><span data-stu-id="1a855-118">Create androidDeviceOwnerEnrollmentProfile</span></span>](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-create.md)|[<span data-ttu-id="1a855-119">androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="1a855-119">androidDeviceOwnerEnrollmentProfile</span></span>](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|<span data-ttu-id="1a855-120">新しい[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="1a855-120">Create a new [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="1a855-121">AndroidDeviceOwnerEnrollmentProfile を削除します。</span><span class="sxs-lookup"><span data-stu-id="1a855-121">Delete androidDeviceOwnerEnrollmentProfile</span></span>](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-delete.md)|<span data-ttu-id="1a855-122">なし</span><span class="sxs-lookup"><span data-stu-id="1a855-122">None</span></span>|<span data-ttu-id="1a855-123">の[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="1a855-123">Deletes a [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md).</span></span>|
|[<span data-ttu-id="1a855-124">AndroidDeviceOwnerEnrollmentProfile を更新します。</span><span class="sxs-lookup"><span data-stu-id="1a855-124">Update androidDeviceOwnerEnrollmentProfile</span></span>](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-update.md)|[<span data-ttu-id="1a855-125">androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="1a855-125">androidDeviceOwnerEnrollmentProfile</span></span>](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|<span data-ttu-id="1a855-126">[AndroidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1a855-126">Update the properties of a [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="1a855-127">revokeToken action</span><span class="sxs-lookup"><span data-stu-id="1a855-127">revokeToken action</span></span>](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-revoketoken.md)|<span data-ttu-id="1a855-128">なし</span><span class="sxs-lookup"><span data-stu-id="1a855-128">None</span></span>|<span data-ttu-id="1a855-129">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="1a855-129">Not yet documented</span></span>|
|[<span data-ttu-id="1a855-130">createToken action</span><span class="sxs-lookup"><span data-stu-id="1a855-130">createToken action</span></span>](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-createtoken.md)|<span data-ttu-id="1a855-131">なし</span><span class="sxs-lookup"><span data-stu-id="1a855-131">None</span></span>|<span data-ttu-id="1a855-132">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="1a855-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="1a855-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1a855-133">Properties</span></span>
|<span data-ttu-id="1a855-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1a855-134">Property</span></span>|<span data-ttu-id="1a855-135">種類</span><span class="sxs-lookup"><span data-stu-id="1a855-135">Type</span></span>|<span data-ttu-id="1a855-136">説明</span><span class="sxs-lookup"><span data-stu-id="1a855-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a855-137">accountId</span><span class="sxs-lookup"><span data-stu-id="1a855-137">accountId</span></span>|<span data-ttu-id="1a855-138">String</span><span class="sxs-lookup"><span data-stu-id="1a855-138">String</span></span>|<span data-ttu-id="1a855-139">登録プロファイルが属するテナント GUID。</span><span class="sxs-lookup"><span data-stu-id="1a855-139">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="1a855-140">id</span><span class="sxs-lookup"><span data-stu-id="1a855-140">id</span></span>|<span data-ttu-id="1a855-141">String</span><span class="sxs-lookup"><span data-stu-id="1a855-141">String</span></span>|<span data-ttu-id="1a855-142">登録プロファイル用の一意な GUID。</span><span class="sxs-lookup"><span data-stu-id="1a855-142">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="1a855-143">displayName</span><span class="sxs-lookup"><span data-stu-id="1a855-143">displayName</span></span>|<span data-ttu-id="1a855-144">String</span><span class="sxs-lookup"><span data-stu-id="1a855-144">String</span></span>|<span data-ttu-id="1a855-145">登録プロファイルの表示名。</span><span class="sxs-lookup"><span data-stu-id="1a855-145">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="1a855-146">説明</span><span class="sxs-lookup"><span data-stu-id="1a855-146">description</span></span>|<span data-ttu-id="1a855-147">String</span><span class="sxs-lookup"><span data-stu-id="1a855-147">String</span></span>|<span data-ttu-id="1a855-148">登録プロファイルの説明。</span><span class="sxs-lookup"><span data-stu-id="1a855-148">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="1a855-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1a855-149">createdDateTime</span></span>|<span data-ttu-id="1a855-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a855-150">DateTimeOffset</span></span>|<span data-ttu-id="1a855-151">登録プロファイルが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="1a855-151">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="1a855-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1a855-152">lastModifiedDateTime</span></span>|<span data-ttu-id="1a855-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a855-153">DateTimeOffset</span></span>|<span data-ttu-id="1a855-154">登録プロファイルが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="1a855-154">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="1a855-155">tokenValue</span><span class="sxs-lookup"><span data-stu-id="1a855-155">tokenValue</span></span>|<span data-ttu-id="1a855-156">String</span><span class="sxs-lookup"><span data-stu-id="1a855-156">String</span></span>|<span data-ttu-id="1a855-157">この登録プロファイル用に最後に作成されたトークンの値。</span><span class="sxs-lookup"><span data-stu-id="1a855-157">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="1a855-158">tokenCreationDateTime</span><span class="sxs-lookup"><span data-stu-id="1a855-158">tokenCreationDateTime</span></span>|<span data-ttu-id="1a855-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a855-159">DateTimeOffset</span></span>|<span data-ttu-id="1a855-160">直前に作成されたトークンが作成された日時です。</span><span class="sxs-lookup"><span data-stu-id="1a855-160">Date time the most recently created token was created.</span></span>|
|<span data-ttu-id="1a855-161">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="1a855-161">tokenExpirationDateTime</span></span>|<span data-ttu-id="1a855-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a855-162">DateTimeOffset</span></span>|<span data-ttu-id="1a855-163">最後に作成されたトークンの有効期限が切れる日時。</span><span class="sxs-lookup"><span data-stu-id="1a855-163">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="1a855-164">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1a855-164">enrolledDeviceCount</span></span>|<span data-ttu-id="1a855-165">Int32</span><span class="sxs-lookup"><span data-stu-id="1a855-165">Int32</span></span>|<span data-ttu-id="1a855-166">この登録プロファイルを使用して登録した Android デバイスの合計数。</span><span class="sxs-lookup"><span data-stu-id="1a855-166">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="1a855-167">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="1a855-167">qrCodeContent</span></span>|<span data-ttu-id="1a855-168">String</span><span class="sxs-lookup"><span data-stu-id="1a855-168">String</span></span>|<span data-ttu-id="1a855-169">トークン用の QR コードを生成するために使用された文字列。</span><span class="sxs-lookup"><span data-stu-id="1a855-169">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="1a855-170">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="1a855-170">qrCodeImage</span></span>|[<span data-ttu-id="1a855-171">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1a855-171">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="1a855-172">トークンの QR コードを生成するために使用する文字列。</span><span class="sxs-lookup"><span data-stu-id="1a855-172">String used to generate a QR code for the token.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a855-173">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1a855-173">Relationships</span></span>
<span data-ttu-id="1a855-174">なし</span><span class="sxs-lookup"><span data-stu-id="1a855-174">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1a855-175">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1a855-175">JSON Representation</span></span>
<span data-ttu-id="1a855-176">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1a855-176">Here is a JSON representation of the resource.</span></span>
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





