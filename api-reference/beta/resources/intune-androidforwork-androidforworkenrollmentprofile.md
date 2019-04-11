---
title: androidForWorkEnrollmentProfile リソース タイプ
description: Google のクラウド管理を使用して COSU デバイスを登録するために使われる登録プロファイルです。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c9f4c7dd24486c4c2d5ea09281008617c97d605f
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31794072"
---
# <a name="androidforworkenrollmentprofile-resource-type"></a><span data-ttu-id="e8d03-103">androidForWorkEnrollmentProfile リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="e8d03-103">androidForWorkEnrollmentProfile resource type</span></span>

> <span data-ttu-id="e8d03-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e8d03-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8d03-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e8d03-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8d03-106">Google のクラウド管理を使用して COSU デバイスを登録するために使われる登録プロファイルです。</span><span class="sxs-lookup"><span data-stu-id="e8d03-106">Enrollment Profile used to enroll COSU devices using Google's Cloud Management.</span></span>

## <a name="methods"></a><span data-ttu-id="e8d03-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="e8d03-107">Methods</span></span>
|<span data-ttu-id="e8d03-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="e8d03-108">Method</span></span>|<span data-ttu-id="e8d03-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e8d03-109">Return Type</span></span>|<span data-ttu-id="e8d03-110">説明</span><span class="sxs-lookup"><span data-stu-id="e8d03-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e8d03-111">androidForWorkEnrollmentProfiles のリスト</span><span class="sxs-lookup"><span data-stu-id="e8d03-111">List androidForWorkEnrollmentProfiles</span></span>](../api/intune-androidforwork-androidforworkenrollmentprofile-list.md)|<span data-ttu-id="e8d03-112">[androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e8d03-112">[androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) collection</span></span>|<span data-ttu-id="e8d03-113">[androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="e8d03-113">List properties and relationships of the [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="e8d03-114">androidForWorkEnrollmentProfile の取得</span><span class="sxs-lookup"><span data-stu-id="e8d03-114">Get androidForWorkEnrollmentProfile</span></span>](../api/intune-androidforwork-androidforworkenrollmentprofile-get.md)|[<span data-ttu-id="e8d03-115">androidForWorkEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="e8d03-115">androidForWorkEnrollmentProfile</span></span>](../resources/intune-androidforwork-androidforworkenrollmentprofile.md)|<span data-ttu-id="e8d03-116">[androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e8d03-116">Read properties and relationships of the [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="e8d03-117">Create androidForWorkEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="e8d03-117">Create androidForWorkEnrollmentProfile</span></span>](../api/intune-androidforwork-androidforworkenrollmentprofile-create.md)|[<span data-ttu-id="e8d03-118">androidForWorkEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="e8d03-118">androidForWorkEnrollmentProfile</span></span>](../resources/intune-androidforwork-androidforworkenrollmentprofile.md)|<span data-ttu-id="e8d03-119">新しい [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="e8d03-119">Create a new [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="e8d03-120">androidForWorkEnrollmentProfile の削除</span><span class="sxs-lookup"><span data-stu-id="e8d03-120">Delete androidForWorkEnrollmentProfile</span></span>](../api/intune-androidforwork-androidforworkenrollmentprofile-delete.md)|<span data-ttu-id="e8d03-121">なし</span><span class="sxs-lookup"><span data-stu-id="e8d03-121">None</span></span>|<span data-ttu-id="e8d03-122">[androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="e8d03-122">Deletes a [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span></span>|
|[<span data-ttu-id="e8d03-123">androidForWorkEnrollmentProfile の更新</span><span class="sxs-lookup"><span data-stu-id="e8d03-123">Update androidForWorkEnrollmentProfile</span></span>](../api/intune-androidforwork-androidforworkenrollmentprofile-update.md)|[<span data-ttu-id="e8d03-124">androidForWorkEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="e8d03-124">androidForWorkEnrollmentProfile</span></span>](../resources/intune-androidforwork-androidforworkenrollmentprofile.md)|<span data-ttu-id="e8d03-125">[androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e8d03-125">Update the properties of a [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="e8d03-126">revokeToken アクション</span><span class="sxs-lookup"><span data-stu-id="e8d03-126">revokeToken action</span></span>](../api/intune-androidforwork-androidforworkenrollmentprofile-revoketoken.md)|<span data-ttu-id="e8d03-127">なし</span><span class="sxs-lookup"><span data-stu-id="e8d03-127">None</span></span>|<span data-ttu-id="e8d03-128">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e8d03-128">Not yet documented</span></span>|
|[<span data-ttu-id="e8d03-129">createToken アクション</span><span class="sxs-lookup"><span data-stu-id="e8d03-129">createToken action</span></span>](../api/intune-androidforwork-androidforworkenrollmentprofile-createtoken.md)|<span data-ttu-id="e8d03-130">なし</span><span class="sxs-lookup"><span data-stu-id="e8d03-130">None</span></span>|<span data-ttu-id="e8d03-131">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e8d03-131">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="e8d03-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e8d03-132">Properties</span></span>
|<span data-ttu-id="e8d03-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e8d03-133">Property</span></span>|<span data-ttu-id="e8d03-134">型</span><span class="sxs-lookup"><span data-stu-id="e8d03-134">Type</span></span>|<span data-ttu-id="e8d03-135">説明</span><span class="sxs-lookup"><span data-stu-id="e8d03-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8d03-136">accountId</span><span class="sxs-lookup"><span data-stu-id="e8d03-136">accountId</span></span>|<span data-ttu-id="e8d03-137">文字列</span><span class="sxs-lookup"><span data-stu-id="e8d03-137">String</span></span>|<span data-ttu-id="e8d03-138">登録プロファイルが属するテナント GUID。</span><span class="sxs-lookup"><span data-stu-id="e8d03-138">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="e8d03-139">id</span><span class="sxs-lookup"><span data-stu-id="e8d03-139">id</span></span>|<span data-ttu-id="e8d03-140">文字列</span><span class="sxs-lookup"><span data-stu-id="e8d03-140">String</span></span>|<span data-ttu-id="e8d03-141">登録プロファイルの一意の GUID。</span><span class="sxs-lookup"><span data-stu-id="e8d03-141">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="e8d03-142">displayName</span><span class="sxs-lookup"><span data-stu-id="e8d03-142">displayName</span></span>|<span data-ttu-id="e8d03-143">String</span><span class="sxs-lookup"><span data-stu-id="e8d03-143">String</span></span>|<span data-ttu-id="e8d03-144">登録プロファイルの表示名。</span><span class="sxs-lookup"><span data-stu-id="e8d03-144">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="e8d03-145">説明</span><span class="sxs-lookup"><span data-stu-id="e8d03-145">description</span></span>|<span data-ttu-id="e8d03-146">String</span><span class="sxs-lookup"><span data-stu-id="e8d03-146">String</span></span>|<span data-ttu-id="e8d03-147">登録プロファイルの説明。</span><span class="sxs-lookup"><span data-stu-id="e8d03-147">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="e8d03-148">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e8d03-148">createdDateTime</span></span>|<span data-ttu-id="e8d03-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8d03-149">DateTimeOffset</span></span>|<span data-ttu-id="e8d03-150">登録プロファイルが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="e8d03-150">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="e8d03-151">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e8d03-151">lastModifiedDateTime</span></span>|<span data-ttu-id="e8d03-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8d03-152">DateTimeOffset</span></span>|<span data-ttu-id="e8d03-153">登録プロファイルが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="e8d03-153">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="e8d03-154">tokenValue</span><span class="sxs-lookup"><span data-stu-id="e8d03-154">tokenValue</span></span>|<span data-ttu-id="e8d03-155">文字列</span><span class="sxs-lookup"><span data-stu-id="e8d03-155">String</span></span>|<span data-ttu-id="e8d03-156">この登録プロファイル用に最後に作成されたトークンの値。</span><span class="sxs-lookup"><span data-stu-id="e8d03-156">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="e8d03-157">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="e8d03-157">tokenExpirationDateTime</span></span>|<span data-ttu-id="e8d03-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8d03-158">DateTimeOffset</span></span>|<span data-ttu-id="e8d03-159">最後に作成されたトークンの有効期限が切れる日時。</span><span class="sxs-lookup"><span data-stu-id="e8d03-159">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="e8d03-160">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e8d03-160">enrolledDeviceCount</span></span>|<span data-ttu-id="e8d03-161">Int32</span><span class="sxs-lookup"><span data-stu-id="e8d03-161">Int32</span></span>|<span data-ttu-id="e8d03-162">この登録プロファイルを使用して登録した Android デバイスの合計数。</span><span class="sxs-lookup"><span data-stu-id="e8d03-162">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="e8d03-163">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="e8d03-163">qrCodeContent</span></span>|<span data-ttu-id="e8d03-164">String</span><span class="sxs-lookup"><span data-stu-id="e8d03-164">String</span></span>|<span data-ttu-id="e8d03-165">トークン用の QR コードを生成するために使用された文字列。</span><span class="sxs-lookup"><span data-stu-id="e8d03-165">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="e8d03-166">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="e8d03-166">qrCodeImage</span></span>|[<span data-ttu-id="e8d03-167">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e8d03-167">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e8d03-168">トークンの QR コードを生成するために使用する文字列。</span><span class="sxs-lookup"><span data-stu-id="e8d03-168">String used to generate a QR code for the token.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e8d03-169">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e8d03-169">Relationships</span></span>
<span data-ttu-id="e8d03-170">なし</span><span class="sxs-lookup"><span data-stu-id="e8d03-170">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e8d03-171">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e8d03-171">JSON Representation</span></span>
<span data-ttu-id="e8d03-172">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e8d03-172">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidForWorkEnrollmentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkEnrollmentProfile",
  "accountId": "String",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "tokenValue": "String",
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





