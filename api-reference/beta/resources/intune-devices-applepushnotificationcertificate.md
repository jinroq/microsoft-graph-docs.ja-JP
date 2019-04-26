---
title: applePushNotificationCertificate リソースの種類
description: Apple プッシュ通知証明書。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6513e088c07fcc8d3b98b90a52d8d98f9df4a74c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32571794"
---
# <a name="applepushnotificationcertificate-resource-type"></a><span data-ttu-id="66283-103">applePushNotificationCertificate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="66283-103">applePushNotificationCertificate resource type</span></span>

> <span data-ttu-id="66283-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="66283-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66283-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="66283-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66283-106">Apple プッシュ通知証明書。</span><span class="sxs-lookup"><span data-stu-id="66283-106">Apple push notification certificate.</span></span>

## <a name="methods"></a><span data-ttu-id="66283-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="66283-107">Methods</span></span>
|<span data-ttu-id="66283-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="66283-108">Method</span></span>|<span data-ttu-id="66283-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="66283-109">Return Type</span></span>|<span data-ttu-id="66283-110">説明</span><span class="sxs-lookup"><span data-stu-id="66283-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="66283-111">Get applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="66283-111">Get applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-get.md)|[<span data-ttu-id="66283-112">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="66283-112">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="66283-113">[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="66283-113">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="66283-114">Update applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="66283-114">Update applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-update.md)|[<span data-ttu-id="66283-115">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="66283-115">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="66283-116">[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="66283-116">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="66283-117">downloadApplePushNotificationCertificateSigningRequest 関数</span><span class="sxs-lookup"><span data-stu-id="66283-117">downloadApplePushNotificationCertificateSigningRequest function</span></span>](../api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest.md)|<span data-ttu-id="66283-118">String</span><span class="sxs-lookup"><span data-stu-id="66283-118">String</span></span>|<span data-ttu-id="66283-119">Apple プッシュ通知の証明書署名要求をダウンロードします</span><span class="sxs-lookup"><span data-stu-id="66283-119">Download Apple push notification certificate signing request</span></span>|

## <a name="properties"></a><span data-ttu-id="66283-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="66283-120">Properties</span></span>
|<span data-ttu-id="66283-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="66283-121">Property</span></span>|<span data-ttu-id="66283-122">型</span><span class="sxs-lookup"><span data-stu-id="66283-122">Type</span></span>|<span data-ttu-id="66283-123">説明</span><span class="sxs-lookup"><span data-stu-id="66283-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66283-124">id</span><span class="sxs-lookup"><span data-stu-id="66283-124">id</span></span>|<span data-ttu-id="66283-125">String</span><span class="sxs-lookup"><span data-stu-id="66283-125">String</span></span>|<span data-ttu-id="66283-126">証明書の一意識別子</span><span class="sxs-lookup"><span data-stu-id="66283-126">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="66283-127">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="66283-127">appleIdentifier</span></span>|<span data-ttu-id="66283-128">String</span><span class="sxs-lookup"><span data-stu-id="66283-128">String</span></span>|<span data-ttu-id="66283-129">MDM プッシュ証明書の作成に使用するアカウントの Apple ID。</span><span class="sxs-lookup"><span data-stu-id="66283-129">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="66283-130">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="66283-130">topicIdentifier</span></span>|<span data-ttu-id="66283-131">String</span><span class="sxs-lookup"><span data-stu-id="66283-131">String</span></span>|<span data-ttu-id="66283-132">トピック ID。</span><span class="sxs-lookup"><span data-stu-id="66283-132">Topic Id.</span></span>|
|<span data-ttu-id="66283-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="66283-133">lastModifiedDateTime</span></span>|<span data-ttu-id="66283-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66283-134">DateTimeOffset</span></span>|<span data-ttu-id="66283-135">Apple プッシュ通知証明書の最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="66283-135">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="66283-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="66283-136">expirationDateTime</span></span>|<span data-ttu-id="66283-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66283-137">DateTimeOffset</span></span>|<span data-ttu-id="66283-138">Apple プッシュ通知証明書の有効期限。</span><span class="sxs-lookup"><span data-stu-id="66283-138">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="66283-139">certificateuploadstatus</span><span class="sxs-lookup"><span data-stu-id="66283-139">certificateUploadStatus</span></span>|<span data-ttu-id="66283-140">String</span><span class="sxs-lookup"><span data-stu-id="66283-140">String</span></span>|<span data-ttu-id="66283-141">証明書のアップロード状態。</span><span class="sxs-lookup"><span data-stu-id="66283-141">The certificate upload status.</span></span>|
|<span data-ttu-id="66283-142">certificateUploadFailureReason</span><span class="sxs-lookup"><span data-stu-id="66283-142">certificateUploadFailureReason</span></span>|<span data-ttu-id="66283-143">String</span><span class="sxs-lookup"><span data-stu-id="66283-143">String</span></span>|<span data-ttu-id="66283-144">証明書のアップロードが失敗した理由。</span><span class="sxs-lookup"><span data-stu-id="66283-144">The reason the certificate upload failed.</span></span>|
|<span data-ttu-id="66283-145">certificate</span><span class="sxs-lookup"><span data-stu-id="66283-145">certificate</span></span>|<span data-ttu-id="66283-146">String</span><span class="sxs-lookup"><span data-stu-id="66283-146">String</span></span>|<span data-ttu-id="66283-147">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="66283-147">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="66283-148">関係</span><span class="sxs-lookup"><span data-stu-id="66283-148">Relationships</span></span>
<span data-ttu-id="66283-149">なし</span><span class="sxs-lookup"><span data-stu-id="66283-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="66283-150">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="66283-150">JSON Representation</span></span>
<span data-ttu-id="66283-151">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="66283-151">Here is a JSON representation of the resource.</span></span>
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





