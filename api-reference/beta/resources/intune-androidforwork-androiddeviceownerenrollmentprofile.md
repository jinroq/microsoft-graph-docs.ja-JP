---
title: androidDeviceOwnerEnrollmentProfile リソースの種類
description: Google のクラウド管理を使用して COSU デバイスを登録するために使われる登録プロファイルです。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 53c3f1e26956b1f3cce830b7e7b2fed6a2e3df72
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35737371"
---
# <a name="androiddeviceownerenrollmentprofile-resource-type"></a><span data-ttu-id="de398-103">androidDeviceOwnerEnrollmentProfile リソースの種類</span><span class="sxs-lookup"><span data-stu-id="de398-103">androidDeviceOwnerEnrollmentProfile resource type</span></span>

> <span data-ttu-id="de398-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="de398-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="de398-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="de398-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de398-106">Google のクラウド管理を使用して COSU デバイスを登録するために使われる登録プロファイルです。</span><span class="sxs-lookup"><span data-stu-id="de398-106">Enrollment Profile used to enroll COSU devices using Google's Cloud Management.</span></span>

## <a name="methods"></a><span data-ttu-id="de398-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="de398-107">Methods</span></span>
|<span data-ttu-id="de398-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="de398-108">Method</span></span>|<span data-ttu-id="de398-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="de398-109">Return Type</span></span>|<span data-ttu-id="de398-110">説明</span><span class="sxs-lookup"><span data-stu-id="de398-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="de398-111">リスト androidDeviceOwnerEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="de398-111">List androidDeviceOwnerEnrollmentProfiles</span></span>](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-list.md)|<span data-ttu-id="de398-112">[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="de398-112">[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) collection</span></span>|<span data-ttu-id="de398-113">[AndroidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="de398-113">List properties and relationships of the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="de398-114">AndroidDeviceOwnerEnrollmentProfile を取得する</span><span class="sxs-lookup"><span data-stu-id="de398-114">Get androidDeviceOwnerEnrollmentProfile</span></span>](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-get.md)|[<span data-ttu-id="de398-115">androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="de398-115">androidDeviceOwnerEnrollmentProfile</span></span>](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|<span data-ttu-id="de398-116">[AndroidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="de398-116">Read properties and relationships of the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="de398-117">AndroidDeviceOwnerEnrollmentProfile を作成する</span><span class="sxs-lookup"><span data-stu-id="de398-117">Create androidDeviceOwnerEnrollmentProfile</span></span>](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-create.md)|[<span data-ttu-id="de398-118">androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="de398-118">androidDeviceOwnerEnrollmentProfile</span></span>](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|<span data-ttu-id="de398-119">新しい[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="de398-119">Create a new [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="de398-120">AndroidDeviceOwnerEnrollmentProfile の削除</span><span class="sxs-lookup"><span data-stu-id="de398-120">Delete androidDeviceOwnerEnrollmentProfile</span></span>](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-delete.md)|<span data-ttu-id="de398-121">None</span><span class="sxs-lookup"><span data-stu-id="de398-121">None</span></span>|<span data-ttu-id="de398-122">[AndroidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="de398-122">Deletes a [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md).</span></span>|
|[<span data-ttu-id="de398-123">AndroidDeviceOwnerEnrollmentProfile の更新</span><span class="sxs-lookup"><span data-stu-id="de398-123">Update androidDeviceOwnerEnrollmentProfile</span></span>](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-update.md)|[<span data-ttu-id="de398-124">androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="de398-124">androidDeviceOwnerEnrollmentProfile</span></span>](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|<span data-ttu-id="de398-125">[AndroidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="de398-125">Update the properties of a [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="de398-126">revokeToken action</span><span class="sxs-lookup"><span data-stu-id="de398-126">revokeToken action</span></span>](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-revoketoken.md)|<span data-ttu-id="de398-127">なし</span><span class="sxs-lookup"><span data-stu-id="de398-127">None</span></span>|<span data-ttu-id="de398-128">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="de398-128">Not yet documented</span></span>|
|[<span data-ttu-id="de398-129">createToken action</span><span class="sxs-lookup"><span data-stu-id="de398-129">createToken action</span></span>](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-createtoken.md)|<span data-ttu-id="de398-130">なし</span><span class="sxs-lookup"><span data-stu-id="de398-130">None</span></span>|<span data-ttu-id="de398-131">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="de398-131">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="de398-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="de398-132">Properties</span></span>
|<span data-ttu-id="de398-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="de398-133">Property</span></span>|<span data-ttu-id="de398-134">型</span><span class="sxs-lookup"><span data-stu-id="de398-134">Type</span></span>|<span data-ttu-id="de398-135">説明</span><span class="sxs-lookup"><span data-stu-id="de398-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de398-136">accountId</span><span class="sxs-lookup"><span data-stu-id="de398-136">accountId</span></span>|<span data-ttu-id="de398-137">String</span><span class="sxs-lookup"><span data-stu-id="de398-137">String</span></span>|<span data-ttu-id="de398-138">登録プロファイルが属するテナント GUID。</span><span class="sxs-lookup"><span data-stu-id="de398-138">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="de398-139">id</span><span class="sxs-lookup"><span data-stu-id="de398-139">id</span></span>|<span data-ttu-id="de398-140">文字列</span><span class="sxs-lookup"><span data-stu-id="de398-140">String</span></span>|<span data-ttu-id="de398-141">登録プロファイルの一意の GUID。</span><span class="sxs-lookup"><span data-stu-id="de398-141">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="de398-142">displayName</span><span class="sxs-lookup"><span data-stu-id="de398-142">displayName</span></span>|<span data-ttu-id="de398-143">String</span><span class="sxs-lookup"><span data-stu-id="de398-143">String</span></span>|<span data-ttu-id="de398-144">登録プロファイルの表示名。</span><span class="sxs-lookup"><span data-stu-id="de398-144">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="de398-145">description</span><span class="sxs-lookup"><span data-stu-id="de398-145">description</span></span>|<span data-ttu-id="de398-146">String</span><span class="sxs-lookup"><span data-stu-id="de398-146">String</span></span>|<span data-ttu-id="de398-147">登録プロファイルの説明。</span><span class="sxs-lookup"><span data-stu-id="de398-147">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="de398-148">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="de398-148">createdDateTime</span></span>|<span data-ttu-id="de398-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de398-149">DateTimeOffset</span></span>|<span data-ttu-id="de398-150">登録プロファイルが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="de398-150">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="de398-151">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="de398-151">lastModifiedDateTime</span></span>|<span data-ttu-id="de398-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de398-152">DateTimeOffset</span></span>|<span data-ttu-id="de398-153">登録プロファイルが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="de398-153">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="de398-154">tokenValue</span><span class="sxs-lookup"><span data-stu-id="de398-154">tokenValue</span></span>|<span data-ttu-id="de398-155">String</span><span class="sxs-lookup"><span data-stu-id="de398-155">String</span></span>|<span data-ttu-id="de398-156">この登録プロファイル用に最後に作成されたトークンの値。</span><span class="sxs-lookup"><span data-stu-id="de398-156">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="de398-157">Tokenの日付/時刻</span><span class="sxs-lookup"><span data-stu-id="de398-157">tokenCreationDateTime</span></span>|<span data-ttu-id="de398-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de398-158">DateTimeOffset</span></span>|<span data-ttu-id="de398-159">最後に作成されたトークンが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="de398-159">Date time the most recently created token was created.</span></span>|
|<span data-ttu-id="de398-160">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="de398-160">tokenExpirationDateTime</span></span>|<span data-ttu-id="de398-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de398-161">DateTimeOffset</span></span>|<span data-ttu-id="de398-162">最後に作成されたトークンの有効期限が切れる日時。</span><span class="sxs-lookup"><span data-stu-id="de398-162">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="de398-163">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="de398-163">enrolledDeviceCount</span></span>|<span data-ttu-id="de398-164">Int32</span><span class="sxs-lookup"><span data-stu-id="de398-164">Int32</span></span>|<span data-ttu-id="de398-165">この登録プロファイルを使用して登録した Android デバイスの合計数。</span><span class="sxs-lookup"><span data-stu-id="de398-165">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="de398-166">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="de398-166">qrCodeContent</span></span>|<span data-ttu-id="de398-167">String</span><span class="sxs-lookup"><span data-stu-id="de398-167">String</span></span>|<span data-ttu-id="de398-168">トークンの QR コードを生成するために使用する文字列。</span><span class="sxs-lookup"><span data-stu-id="de398-168">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="de398-169">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="de398-169">qrCodeImage</span></span>|[<span data-ttu-id="de398-170">mimeContent</span><span class="sxs-lookup"><span data-stu-id="de398-170">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="de398-171">トークンの QR コードを生成するために使用する文字列。</span><span class="sxs-lookup"><span data-stu-id="de398-171">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="de398-172">scopeTags</span><span class="sxs-lookup"><span data-stu-id="de398-172">scopeTags</span></span>|<span data-ttu-id="de398-173">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="de398-173">String collection</span></span>|<span data-ttu-id="de398-174">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="de398-174">List of Scope Tags for this Entity instance.</span></span>|

## <a name="relationships"></a><span data-ttu-id="de398-175">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="de398-175">Relationships</span></span>
<span data-ttu-id="de398-176">なし</span><span class="sxs-lookup"><span data-stu-id="de398-176">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="de398-177">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="de398-177">JSON Representation</span></span>
<span data-ttu-id="de398-178">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="de398-178">Here is a JSON representation of the resource.</span></span>
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
  },
  "scopeTags": [
    "String"
  ]
}
```





