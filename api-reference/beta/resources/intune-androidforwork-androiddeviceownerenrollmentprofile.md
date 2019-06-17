---
title: androidDeviceOwnerEnrollmentProfile リソースの種類
description: Google のクラウド管理を使用して COSU デバイスを登録するために使われる登録プロファイルです。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 92fc907fdc0e50e5d983ac0dbb6f8a122c92641a
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34992893"
---
# <a name="androiddeviceownerenrollmentprofile-resource-type"></a><span data-ttu-id="529de-103">androidDeviceOwnerEnrollmentProfile リソースの種類</span><span class="sxs-lookup"><span data-stu-id="529de-103">androidDeviceOwnerEnrollmentProfile resource type</span></span>

> <span data-ttu-id="529de-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="529de-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="529de-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="529de-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="529de-106">Google のクラウド管理を使用して COSU デバイスを登録するために使われる登録プロファイルです。</span><span class="sxs-lookup"><span data-stu-id="529de-106">Enrollment Profile used to enroll COSU devices using Google's Cloud Management.</span></span>

## <a name="methods"></a><span data-ttu-id="529de-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="529de-107">Methods</span></span>
|<span data-ttu-id="529de-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="529de-108">Method</span></span>|<span data-ttu-id="529de-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="529de-109">Return Type</span></span>|<span data-ttu-id="529de-110">説明</span><span class="sxs-lookup"><span data-stu-id="529de-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="529de-111">リスト androidDeviceOwnerEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="529de-111">List androidDeviceOwnerEnrollmentProfiles</span></span>](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-list.md)|<span data-ttu-id="529de-112">[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="529de-112">[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) collection</span></span>|<span data-ttu-id="529de-113">[AndroidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="529de-113">List properties and relationships of the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="529de-114">AndroidDeviceOwnerEnrollmentProfile を取得する</span><span class="sxs-lookup"><span data-stu-id="529de-114">Get androidDeviceOwnerEnrollmentProfile</span></span>](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-get.md)|[<span data-ttu-id="529de-115">androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="529de-115">androidDeviceOwnerEnrollmentProfile</span></span>](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|<span data-ttu-id="529de-116">[AndroidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="529de-116">Read properties and relationships of the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="529de-117">AndroidDeviceOwnerEnrollmentProfile を作成する</span><span class="sxs-lookup"><span data-stu-id="529de-117">Create androidDeviceOwnerEnrollmentProfile</span></span>](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-create.md)|[<span data-ttu-id="529de-118">androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="529de-118">androidDeviceOwnerEnrollmentProfile</span></span>](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|<span data-ttu-id="529de-119">新しい[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="529de-119">Create a new [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="529de-120">AndroidDeviceOwnerEnrollmentProfile の削除</span><span class="sxs-lookup"><span data-stu-id="529de-120">Delete androidDeviceOwnerEnrollmentProfile</span></span>](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-delete.md)|<span data-ttu-id="529de-121">None</span><span class="sxs-lookup"><span data-stu-id="529de-121">None</span></span>|<span data-ttu-id="529de-122">[AndroidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="529de-122">Deletes a [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md).</span></span>|
|[<span data-ttu-id="529de-123">AndroidDeviceOwnerEnrollmentProfile の更新</span><span class="sxs-lookup"><span data-stu-id="529de-123">Update androidDeviceOwnerEnrollmentProfile</span></span>](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-update.md)|[<span data-ttu-id="529de-124">androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="529de-124">androidDeviceOwnerEnrollmentProfile</span></span>](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|<span data-ttu-id="529de-125">[AndroidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="529de-125">Update the properties of a [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="529de-126">revokeToken action</span><span class="sxs-lookup"><span data-stu-id="529de-126">revokeToken action</span></span>](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-revoketoken.md)|<span data-ttu-id="529de-127">なし</span><span class="sxs-lookup"><span data-stu-id="529de-127">None</span></span>|<span data-ttu-id="529de-128">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="529de-128">Not yet documented</span></span>|
|[<span data-ttu-id="529de-129">createToken action</span><span class="sxs-lookup"><span data-stu-id="529de-129">createToken action</span></span>](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-createtoken.md)|<span data-ttu-id="529de-130">なし</span><span class="sxs-lookup"><span data-stu-id="529de-130">None</span></span>|<span data-ttu-id="529de-131">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="529de-131">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="529de-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="529de-132">Properties</span></span>
|<span data-ttu-id="529de-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="529de-133">Property</span></span>|<span data-ttu-id="529de-134">型</span><span class="sxs-lookup"><span data-stu-id="529de-134">Type</span></span>|<span data-ttu-id="529de-135">説明</span><span class="sxs-lookup"><span data-stu-id="529de-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="529de-136">accountId</span><span class="sxs-lookup"><span data-stu-id="529de-136">accountId</span></span>|<span data-ttu-id="529de-137">String</span><span class="sxs-lookup"><span data-stu-id="529de-137">String</span></span>|<span data-ttu-id="529de-138">登録プロファイルが属するテナント GUID。</span><span class="sxs-lookup"><span data-stu-id="529de-138">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="529de-139">id</span><span class="sxs-lookup"><span data-stu-id="529de-139">id</span></span>|<span data-ttu-id="529de-140">文字列</span><span class="sxs-lookup"><span data-stu-id="529de-140">String</span></span>|<span data-ttu-id="529de-141">登録プロファイルの一意の GUID。</span><span class="sxs-lookup"><span data-stu-id="529de-141">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="529de-142">displayName</span><span class="sxs-lookup"><span data-stu-id="529de-142">displayName</span></span>|<span data-ttu-id="529de-143">String</span><span class="sxs-lookup"><span data-stu-id="529de-143">String</span></span>|<span data-ttu-id="529de-144">登録プロファイルの表示名。</span><span class="sxs-lookup"><span data-stu-id="529de-144">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="529de-145">description</span><span class="sxs-lookup"><span data-stu-id="529de-145">description</span></span>|<span data-ttu-id="529de-146">String</span><span class="sxs-lookup"><span data-stu-id="529de-146">String</span></span>|<span data-ttu-id="529de-147">登録プロファイルの説明。</span><span class="sxs-lookup"><span data-stu-id="529de-147">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="529de-148">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="529de-148">createdDateTime</span></span>|<span data-ttu-id="529de-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="529de-149">DateTimeOffset</span></span>|<span data-ttu-id="529de-150">登録プロファイルが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="529de-150">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="529de-151">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="529de-151">lastModifiedDateTime</span></span>|<span data-ttu-id="529de-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="529de-152">DateTimeOffset</span></span>|<span data-ttu-id="529de-153">登録プロファイルが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="529de-153">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="529de-154">tokenValue</span><span class="sxs-lookup"><span data-stu-id="529de-154">tokenValue</span></span>|<span data-ttu-id="529de-155">String</span><span class="sxs-lookup"><span data-stu-id="529de-155">String</span></span>|<span data-ttu-id="529de-156">この登録プロファイル用に最後に作成されたトークンの値。</span><span class="sxs-lookup"><span data-stu-id="529de-156">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="529de-157">Tokenの日付/時刻</span><span class="sxs-lookup"><span data-stu-id="529de-157">tokenCreationDateTime</span></span>|<span data-ttu-id="529de-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="529de-158">DateTimeOffset</span></span>|<span data-ttu-id="529de-159">最後に作成されたトークンが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="529de-159">Date time the most recently created token was created.</span></span>|
|<span data-ttu-id="529de-160">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="529de-160">tokenExpirationDateTime</span></span>|<span data-ttu-id="529de-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="529de-161">DateTimeOffset</span></span>|<span data-ttu-id="529de-162">最後に作成されたトークンの有効期限が切れる日時。</span><span class="sxs-lookup"><span data-stu-id="529de-162">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="529de-163">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="529de-163">enrolledDeviceCount</span></span>|<span data-ttu-id="529de-164">Int32</span><span class="sxs-lookup"><span data-stu-id="529de-164">Int32</span></span>|<span data-ttu-id="529de-165">この登録プロファイルを使用して登録した Android デバイスの合計数。</span><span class="sxs-lookup"><span data-stu-id="529de-165">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="529de-166">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="529de-166">qrCodeContent</span></span>|<span data-ttu-id="529de-167">String</span><span class="sxs-lookup"><span data-stu-id="529de-167">String</span></span>|<span data-ttu-id="529de-168">トークン用の QR コードを生成するために使用された文字列。</span><span class="sxs-lookup"><span data-stu-id="529de-168">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="529de-169">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="529de-169">qrCodeImage</span></span>|[<span data-ttu-id="529de-170">mimeContent</span><span class="sxs-lookup"><span data-stu-id="529de-170">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="529de-171">トークンの QR コードを生成するために使用する文字列。</span><span class="sxs-lookup"><span data-stu-id="529de-171">String used to generate a QR code for the token.</span></span>|

## <a name="relationships"></a><span data-ttu-id="529de-172">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="529de-172">Relationships</span></span>
<span data-ttu-id="529de-173">なし</span><span class="sxs-lookup"><span data-stu-id="529de-173">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="529de-174">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="529de-174">JSON Representation</span></span>
<span data-ttu-id="529de-175">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="529de-175">Here is a JSON representation of the resource.</span></span>
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





