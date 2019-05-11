---
title: androidDeviceOwnerEnrollmentProfile リソースの種類
description: Google のクラウド管理を使用して COSU デバイスを登録するために使われる登録プロファイルです。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e4e4fdb5ef4beedc6f253480199f29994bae53f0
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950803"
---
# <a name="androiddeviceownerenrollmentprofile-resource-type"></a><span data-ttu-id="539be-103">androidDeviceOwnerEnrollmentProfile リソースの種類</span><span class="sxs-lookup"><span data-stu-id="539be-103">androidDeviceOwnerEnrollmentProfile resource type</span></span>

> <span data-ttu-id="539be-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="539be-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="539be-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="539be-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="539be-106">Google のクラウド管理を使用して COSU デバイスを登録するために使われる登録プロファイルです。</span><span class="sxs-lookup"><span data-stu-id="539be-106">Enrollment Profile used to enroll COSU devices using Google's Cloud Management.</span></span>

## <a name="methods"></a><span data-ttu-id="539be-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="539be-107">Methods</span></span>
|<span data-ttu-id="539be-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="539be-108">Method</span></span>|<span data-ttu-id="539be-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="539be-109">Return Type</span></span>|<span data-ttu-id="539be-110">説明</span><span class="sxs-lookup"><span data-stu-id="539be-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="539be-111">リスト androidDeviceOwnerEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="539be-111">List androidDeviceOwnerEnrollmentProfiles</span></span>](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-list.md)|<span data-ttu-id="539be-112">[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="539be-112">[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) collection</span></span>|<span data-ttu-id="539be-113">[AndroidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="539be-113">List properties and relationships of the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="539be-114">AndroidDeviceOwnerEnrollmentProfile を取得する</span><span class="sxs-lookup"><span data-stu-id="539be-114">Get androidDeviceOwnerEnrollmentProfile</span></span>](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-get.md)|[<span data-ttu-id="539be-115">androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="539be-115">androidDeviceOwnerEnrollmentProfile</span></span>](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|<span data-ttu-id="539be-116">[AndroidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="539be-116">Read properties and relationships of the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="539be-117">AndroidDeviceOwnerEnrollmentProfile を作成する</span><span class="sxs-lookup"><span data-stu-id="539be-117">Create androidDeviceOwnerEnrollmentProfile</span></span>](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-create.md)|[<span data-ttu-id="539be-118">androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="539be-118">androidDeviceOwnerEnrollmentProfile</span></span>](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|<span data-ttu-id="539be-119">新しい[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="539be-119">Create a new [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="539be-120">AndroidDeviceOwnerEnrollmentProfile の削除</span><span class="sxs-lookup"><span data-stu-id="539be-120">Delete androidDeviceOwnerEnrollmentProfile</span></span>](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-delete.md)|<span data-ttu-id="539be-121">None</span><span class="sxs-lookup"><span data-stu-id="539be-121">None</span></span>|<span data-ttu-id="539be-122">[AndroidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="539be-122">Deletes a [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md).</span></span>|
|[<span data-ttu-id="539be-123">AndroidDeviceOwnerEnrollmentProfile の更新</span><span class="sxs-lookup"><span data-stu-id="539be-123">Update androidDeviceOwnerEnrollmentProfile</span></span>](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-update.md)|[<span data-ttu-id="539be-124">androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="539be-124">androidDeviceOwnerEnrollmentProfile</span></span>](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|<span data-ttu-id="539be-125">[AndroidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="539be-125">Update the properties of a [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="539be-126">revokeToken action</span><span class="sxs-lookup"><span data-stu-id="539be-126">revokeToken action</span></span>](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-revoketoken.md)|<span data-ttu-id="539be-127">なし</span><span class="sxs-lookup"><span data-stu-id="539be-127">None</span></span>|<span data-ttu-id="539be-128">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="539be-128">Not yet documented</span></span>|
|[<span data-ttu-id="539be-129">createToken action</span><span class="sxs-lookup"><span data-stu-id="539be-129">createToken action</span></span>](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-createtoken.md)|<span data-ttu-id="539be-130">なし</span><span class="sxs-lookup"><span data-stu-id="539be-130">None</span></span>|<span data-ttu-id="539be-131">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="539be-131">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="539be-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="539be-132">Properties</span></span>
|<span data-ttu-id="539be-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="539be-133">Property</span></span>|<span data-ttu-id="539be-134">型</span><span class="sxs-lookup"><span data-stu-id="539be-134">Type</span></span>|<span data-ttu-id="539be-135">説明</span><span class="sxs-lookup"><span data-stu-id="539be-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="539be-136">accountId</span><span class="sxs-lookup"><span data-stu-id="539be-136">accountId</span></span>|<span data-ttu-id="539be-137">String</span><span class="sxs-lookup"><span data-stu-id="539be-137">String</span></span>|<span data-ttu-id="539be-138">登録プロファイルが属するテナント GUID。</span><span class="sxs-lookup"><span data-stu-id="539be-138">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="539be-139">id</span><span class="sxs-lookup"><span data-stu-id="539be-139">id</span></span>|<span data-ttu-id="539be-140">文字列</span><span class="sxs-lookup"><span data-stu-id="539be-140">String</span></span>|<span data-ttu-id="539be-141">登録プロファイルの一意の GUID。</span><span class="sxs-lookup"><span data-stu-id="539be-141">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="539be-142">displayName</span><span class="sxs-lookup"><span data-stu-id="539be-142">displayName</span></span>|<span data-ttu-id="539be-143">String</span><span class="sxs-lookup"><span data-stu-id="539be-143">String</span></span>|<span data-ttu-id="539be-144">登録プロファイルの表示名。</span><span class="sxs-lookup"><span data-stu-id="539be-144">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="539be-145">description</span><span class="sxs-lookup"><span data-stu-id="539be-145">description</span></span>|<span data-ttu-id="539be-146">String</span><span class="sxs-lookup"><span data-stu-id="539be-146">String</span></span>|<span data-ttu-id="539be-147">登録プロファイルの説明。</span><span class="sxs-lookup"><span data-stu-id="539be-147">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="539be-148">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="539be-148">createdDateTime</span></span>|<span data-ttu-id="539be-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="539be-149">DateTimeOffset</span></span>|<span data-ttu-id="539be-150">登録プロファイルが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="539be-150">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="539be-151">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="539be-151">lastModifiedDateTime</span></span>|<span data-ttu-id="539be-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="539be-152">DateTimeOffset</span></span>|<span data-ttu-id="539be-153">登録プロファイルが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="539be-153">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="539be-154">tokenValue</span><span class="sxs-lookup"><span data-stu-id="539be-154">tokenValue</span></span>|<span data-ttu-id="539be-155">String</span><span class="sxs-lookup"><span data-stu-id="539be-155">String</span></span>|<span data-ttu-id="539be-156">この登録プロファイル用に最後に作成されたトークンの値。</span><span class="sxs-lookup"><span data-stu-id="539be-156">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="539be-157">Tokenの日付/時刻</span><span class="sxs-lookup"><span data-stu-id="539be-157">tokenCreationDateTime</span></span>|<span data-ttu-id="539be-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="539be-158">DateTimeOffset</span></span>|<span data-ttu-id="539be-159">最後に作成されたトークンが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="539be-159">Date time the most recently created token was created.</span></span>|
|<span data-ttu-id="539be-160">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="539be-160">tokenExpirationDateTime</span></span>|<span data-ttu-id="539be-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="539be-161">DateTimeOffset</span></span>|<span data-ttu-id="539be-162">最後に作成されたトークンの有効期限が切れる日時。</span><span class="sxs-lookup"><span data-stu-id="539be-162">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="539be-163">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="539be-163">enrolledDeviceCount</span></span>|<span data-ttu-id="539be-164">Int32</span><span class="sxs-lookup"><span data-stu-id="539be-164">Int32</span></span>|<span data-ttu-id="539be-165">この登録プロファイルを使用して登録した Android デバイスの合計数。</span><span class="sxs-lookup"><span data-stu-id="539be-165">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="539be-166">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="539be-166">qrCodeContent</span></span>|<span data-ttu-id="539be-167">String</span><span class="sxs-lookup"><span data-stu-id="539be-167">String</span></span>|<span data-ttu-id="539be-168">トークン用の QR コードを生成するために使用された文字列。</span><span class="sxs-lookup"><span data-stu-id="539be-168">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="539be-169">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="539be-169">qrCodeImage</span></span>|[<span data-ttu-id="539be-170">mimeContent</span><span class="sxs-lookup"><span data-stu-id="539be-170">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="539be-171">トークンの QR コードを生成するために使用する文字列。</span><span class="sxs-lookup"><span data-stu-id="539be-171">String used to generate a QR code for the token.</span></span>|

## <a name="relationships"></a><span data-ttu-id="539be-172">関係</span><span class="sxs-lookup"><span data-stu-id="539be-172">Relationships</span></span>
<span data-ttu-id="539be-173">なし</span><span class="sxs-lookup"><span data-stu-id="539be-173">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="539be-174">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="539be-174">JSON Representation</span></span>
<span data-ttu-id="539be-175">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="539be-175">Here is a JSON representation of the resource.</span></span>
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




