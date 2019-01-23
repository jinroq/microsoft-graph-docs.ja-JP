---
title: applePushNotificationCertificate リソースの種類
description: Apple プッシュ通知証明書。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a8a5df851f1826cd3e1e124bf8c2cda89b24da8e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395588"
---
# <a name="applepushnotificationcertificate-resource-type"></a><span data-ttu-id="4a567-103">applePushNotificationCertificate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4a567-103">applePushNotificationCertificate resource type</span></span>

> <span data-ttu-id="4a567-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4a567-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4a567-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4a567-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4a567-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4a567-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a567-107">Apple プッシュ通知証明書。</span><span class="sxs-lookup"><span data-stu-id="4a567-107">Apple push notification certificate.</span></span>

## <a name="methods"></a><span data-ttu-id="4a567-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="4a567-108">Methods</span></span>
|<span data-ttu-id="4a567-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="4a567-109">Method</span></span>|<span data-ttu-id="4a567-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4a567-110">Return Type</span></span>|<span data-ttu-id="4a567-111">説明</span><span class="sxs-lookup"><span data-stu-id="4a567-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4a567-112">Get applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="4a567-112">Get applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-get.md)|[<span data-ttu-id="4a567-113">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="4a567-113">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="4a567-114">[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="4a567-114">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="4a567-115">Update applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="4a567-115">Update applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-update.md)|[<span data-ttu-id="4a567-116">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="4a567-116">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="4a567-117">[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4a567-117">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="4a567-118">downloadApplePushNotificationCertificateSigningRequest 関数</span><span class="sxs-lookup"><span data-stu-id="4a567-118">downloadApplePushNotificationCertificateSigningRequest function</span></span>](../api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest.md)|<span data-ttu-id="4a567-119">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="4a567-119">String</span></span>|<span data-ttu-id="4a567-120">Apple プッシュ通知の証明書署名要求をダウンロードします</span><span class="sxs-lookup"><span data-stu-id="4a567-120">Download Apple push notification certificate signing request</span></span>|

## <a name="properties"></a><span data-ttu-id="4a567-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4a567-121">Properties</span></span>
|<span data-ttu-id="4a567-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4a567-122">Property</span></span>|<span data-ttu-id="4a567-123">型</span><span class="sxs-lookup"><span data-stu-id="4a567-123">Type</span></span>|<span data-ttu-id="4a567-124">説明</span><span class="sxs-lookup"><span data-stu-id="4a567-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a567-125">id</span><span class="sxs-lookup"><span data-stu-id="4a567-125">id</span></span>|<span data-ttu-id="4a567-126">String</span><span class="sxs-lookup"><span data-stu-id="4a567-126">String</span></span>|<span data-ttu-id="4a567-127">証明書の一意識別子</span><span class="sxs-lookup"><span data-stu-id="4a567-127">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="4a567-128">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="4a567-128">appleIdentifier</span></span>|<span data-ttu-id="4a567-129">String</span><span class="sxs-lookup"><span data-stu-id="4a567-129">String</span></span>|<span data-ttu-id="4a567-130">MDM プッシュ証明書の作成に使用するアカウントの Apple ID。</span><span class="sxs-lookup"><span data-stu-id="4a567-130">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="4a567-131">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="4a567-131">topicIdentifier</span></span>|<span data-ttu-id="4a567-132">String</span><span class="sxs-lookup"><span data-stu-id="4a567-132">String</span></span>|<span data-ttu-id="4a567-133">トピック ID。</span><span class="sxs-lookup"><span data-stu-id="4a567-133">Topic Id.</span></span>|
|<span data-ttu-id="4a567-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4a567-134">lastModifiedDateTime</span></span>|<span data-ttu-id="4a567-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a567-135">DateTimeOffset</span></span>|<span data-ttu-id="4a567-136">Apple プッシュ通知証明書の最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="4a567-136">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="4a567-137">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="4a567-137">expirationDateTime</span></span>|<span data-ttu-id="4a567-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a567-138">DateTimeOffset</span></span>|<span data-ttu-id="4a567-139">Apple プッシュ通知証明書の有効期限。</span><span class="sxs-lookup"><span data-stu-id="4a567-139">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="4a567-140">certificateUploadStatus</span><span class="sxs-lookup"><span data-stu-id="4a567-140">certificateUploadStatus</span></span>|<span data-ttu-id="4a567-141">String</span><span class="sxs-lookup"><span data-stu-id="4a567-141">String</span></span>|<span data-ttu-id="4a567-142">証明書のアップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="4a567-142">The certificate upload status.</span></span>|
|<span data-ttu-id="4a567-143">certificateUploadFailureReason</span><span class="sxs-lookup"><span data-stu-id="4a567-143">certificateUploadFailureReason</span></span>|<span data-ttu-id="4a567-144">String</span><span class="sxs-lookup"><span data-stu-id="4a567-144">String</span></span>|<span data-ttu-id="4a567-145">理由の証明書のアップロードに失敗しました。</span><span class="sxs-lookup"><span data-stu-id="4a567-145">The reason the certificate upload failed.</span></span>|
|<span data-ttu-id="4a567-146">証明書</span><span class="sxs-lookup"><span data-stu-id="4a567-146">certificate</span></span>|<span data-ttu-id="4a567-147">String</span><span class="sxs-lookup"><span data-stu-id="4a567-147">String</span></span>|<span data-ttu-id="4a567-148">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="4a567-148">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="4a567-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4a567-149">Relationships</span></span>
<span data-ttu-id="4a567-150">なし</span><span class="sxs-lookup"><span data-stu-id="4a567-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4a567-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4a567-151">JSON Representation</span></span>
<span data-ttu-id="4a567-152">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4a567-152">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.applePushNotificationCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "id": "String (identifier)",
  "appleIdentifier": "String",
  "topicIdentifier": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "certificateUploadStatus": "String",
  "certificateUploadFailureReason": "String",
  "certificate": "String"
}
```




