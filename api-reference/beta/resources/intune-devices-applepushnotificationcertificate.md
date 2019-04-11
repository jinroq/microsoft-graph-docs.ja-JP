---
title: applePushNotificationCertificate リソースの種類
description: Apple プッシュ通知証明書。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6513e088c07fcc8d3b98b90a52d8d98f9df4a74c
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31784524"
---
# <a name="applepushnotificationcertificate-resource-type"></a><span data-ttu-id="b8faa-103">applePushNotificationCertificate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b8faa-103">applePushNotificationCertificate resource type</span></span>

> <span data-ttu-id="b8faa-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b8faa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8faa-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b8faa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8faa-106">Apple プッシュ通知証明書。</span><span class="sxs-lookup"><span data-stu-id="b8faa-106">Apple push notification certificate.</span></span>

## <a name="methods"></a><span data-ttu-id="b8faa-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="b8faa-107">Methods</span></span>
|<span data-ttu-id="b8faa-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="b8faa-108">Method</span></span>|<span data-ttu-id="b8faa-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b8faa-109">Return Type</span></span>|<span data-ttu-id="b8faa-110">説明</span><span class="sxs-lookup"><span data-stu-id="b8faa-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b8faa-111">applePushNotificationCertificate の取得</span><span class="sxs-lookup"><span data-stu-id="b8faa-111">Get applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-get.md)|[<span data-ttu-id="b8faa-112">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="b8faa-112">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="b8faa-113">[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b8faa-113">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="b8faa-114">applePushNotificationCertificate の更新</span><span class="sxs-lookup"><span data-stu-id="b8faa-114">Update applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-update.md)|[<span data-ttu-id="b8faa-115">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="b8faa-115">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="b8faa-116">[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b8faa-116">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="b8faa-117">downloadApplePushNotificationCertificateSigningRequest 関数</span><span class="sxs-lookup"><span data-stu-id="b8faa-117">downloadApplePushNotificationCertificateSigningRequest function</span></span>](../api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest.md)|<span data-ttu-id="b8faa-118">文字列</span><span class="sxs-lookup"><span data-stu-id="b8faa-118">String</span></span>|<span data-ttu-id="b8faa-119">Apple プッシュ通知の証明書署名要求をダウンロードします</span><span class="sxs-lookup"><span data-stu-id="b8faa-119">Download Apple push notification certificate signing request</span></span>|

## <a name="properties"></a><span data-ttu-id="b8faa-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b8faa-120">Properties</span></span>
|<span data-ttu-id="b8faa-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b8faa-121">Property</span></span>|<span data-ttu-id="b8faa-122">型</span><span class="sxs-lookup"><span data-stu-id="b8faa-122">Type</span></span>|<span data-ttu-id="b8faa-123">説明</span><span class="sxs-lookup"><span data-stu-id="b8faa-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8faa-124">id</span><span class="sxs-lookup"><span data-stu-id="b8faa-124">id</span></span>|<span data-ttu-id="b8faa-125">String</span><span class="sxs-lookup"><span data-stu-id="b8faa-125">String</span></span>|<span data-ttu-id="b8faa-126">証明書の一意識別子</span><span class="sxs-lookup"><span data-stu-id="b8faa-126">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="b8faa-127">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="b8faa-127">appleIdentifier</span></span>|<span data-ttu-id="b8faa-128">文字列</span><span class="sxs-lookup"><span data-stu-id="b8faa-128">String</span></span>|<span data-ttu-id="b8faa-129">MDM プッシュ証明書の作成に使用するアカウントの Apple ID。</span><span class="sxs-lookup"><span data-stu-id="b8faa-129">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="b8faa-130">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="b8faa-130">topicIdentifier</span></span>|<span data-ttu-id="b8faa-131">String</span><span class="sxs-lookup"><span data-stu-id="b8faa-131">String</span></span>|<span data-ttu-id="b8faa-132">トピック ID。</span><span class="sxs-lookup"><span data-stu-id="b8faa-132">Topic Id.</span></span>|
|<span data-ttu-id="b8faa-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b8faa-133">lastModifiedDateTime</span></span>|<span data-ttu-id="b8faa-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8faa-134">DateTimeOffset</span></span>|<span data-ttu-id="b8faa-135">Apple プッシュ通知証明書の最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="b8faa-135">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="b8faa-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="b8faa-136">expirationDateTime</span></span>|<span data-ttu-id="b8faa-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8faa-137">DateTimeOffset</span></span>|<span data-ttu-id="b8faa-138">Apple プッシュ通知証明書の有効期限。</span><span class="sxs-lookup"><span data-stu-id="b8faa-138">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="b8faa-139">certificateuploadstatus</span><span class="sxs-lookup"><span data-stu-id="b8faa-139">certificateUploadStatus</span></span>|<span data-ttu-id="b8faa-140">文字列</span><span class="sxs-lookup"><span data-stu-id="b8faa-140">String</span></span>|<span data-ttu-id="b8faa-141">証明書のアップロード状態。</span><span class="sxs-lookup"><span data-stu-id="b8faa-141">The certificate upload status.</span></span>|
|<span data-ttu-id="b8faa-142">certificateUploadFailureReason</span><span class="sxs-lookup"><span data-stu-id="b8faa-142">certificateUploadFailureReason</span></span>|<span data-ttu-id="b8faa-143">文字列</span><span class="sxs-lookup"><span data-stu-id="b8faa-143">String</span></span>|<span data-ttu-id="b8faa-144">証明書のアップロードが失敗した理由。</span><span class="sxs-lookup"><span data-stu-id="b8faa-144">The reason the certificate upload failed.</span></span>|
|<span data-ttu-id="b8faa-145">certificate</span><span class="sxs-lookup"><span data-stu-id="b8faa-145">certificate</span></span>|<span data-ttu-id="b8faa-146">String</span><span class="sxs-lookup"><span data-stu-id="b8faa-146">String</span></span>|<span data-ttu-id="b8faa-147">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="b8faa-147">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8faa-148">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b8faa-148">Relationships</span></span>
<span data-ttu-id="b8faa-149">なし</span><span class="sxs-lookup"><span data-stu-id="b8faa-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b8faa-150">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b8faa-150">JSON Representation</span></span>
<span data-ttu-id="b8faa-151">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b8faa-151">Here is a JSON representation of the resource.</span></span>
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





