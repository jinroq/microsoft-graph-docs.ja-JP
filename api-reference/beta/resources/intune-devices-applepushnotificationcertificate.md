---
title: applePushNotificationCertificate リソースの種類
description: Apple プッシュ通知証明書。
author: tfitzmac
ms.openlocfilehash: 11c03712cc482a882452a9b64867090260863075
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306651"
---
# <a name="applepushnotificationcertificate-resource-type"></a><span data-ttu-id="a276a-103">applePushNotificationCertificate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a276a-103">applePushNotificationCertificate resource type</span></span>

> <span data-ttu-id="a276a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a276a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a276a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a276a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a276a-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a276a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a276a-107">Apple プッシュ通知証明書。</span><span class="sxs-lookup"><span data-stu-id="a276a-107">Apple push notification certificate.</span></span>
## <a name="methods"></a><span data-ttu-id="a276a-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="a276a-108">Methods</span></span>
|<span data-ttu-id="a276a-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="a276a-109">Method</span></span>|<span data-ttu-id="a276a-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a276a-110">Return Type</span></span>|<span data-ttu-id="a276a-111">説明</span><span class="sxs-lookup"><span data-stu-id="a276a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a276a-112">Get applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="a276a-112">Get applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-get.md)|[<span data-ttu-id="a276a-113">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="a276a-113">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="a276a-114">[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a276a-114">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="a276a-115">Update applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="a276a-115">Update applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-update.md)|[<span data-ttu-id="a276a-116">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="a276a-116">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="a276a-117">[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a276a-117">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="a276a-118">downloadApplePushNotificationCertificateSigningRequest 関数</span><span class="sxs-lookup"><span data-stu-id="a276a-118">downloadApplePushNotificationCertificateSigningRequest function</span></span>](../api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest.md)|<span data-ttu-id="a276a-119">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="a276a-119">String</span></span>|<span data-ttu-id="a276a-120">Apple プッシュ通知の証明書署名要求をダウンロードします</span><span class="sxs-lookup"><span data-stu-id="a276a-120">Download Apple push notification certificate signing request</span></span>|

## <a name="properties"></a><span data-ttu-id="a276a-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a276a-121">Properties</span></span>
|<span data-ttu-id="a276a-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a276a-122">Property</span></span>|<span data-ttu-id="a276a-123">種類</span><span class="sxs-lookup"><span data-stu-id="a276a-123">Type</span></span>|<span data-ttu-id="a276a-124">説明</span><span class="sxs-lookup"><span data-stu-id="a276a-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a276a-125">ID</span><span class="sxs-lookup"><span data-stu-id="a276a-125">id</span></span>|<span data-ttu-id="a276a-126">String</span><span class="sxs-lookup"><span data-stu-id="a276a-126">String</span></span>|<span data-ttu-id="a276a-127">証明書の一意識別子</span><span class="sxs-lookup"><span data-stu-id="a276a-127">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="a276a-128">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="a276a-128">appleIdentifier</span></span>|<span data-ttu-id="a276a-129">String</span><span class="sxs-lookup"><span data-stu-id="a276a-129">String</span></span>|<span data-ttu-id="a276a-130">MDM プッシュ証明書の作成に使用するアカウントの Apple ID。</span><span class="sxs-lookup"><span data-stu-id="a276a-130">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="a276a-131">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="a276a-131">topicIdentifier</span></span>|<span data-ttu-id="a276a-132">String</span><span class="sxs-lookup"><span data-stu-id="a276a-132">String</span></span>|<span data-ttu-id="a276a-133">トピック ID。</span><span class="sxs-lookup"><span data-stu-id="a276a-133">Topic Id.</span></span>|
|<span data-ttu-id="a276a-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a276a-134">lastModifiedDateTime</span></span>|<span data-ttu-id="a276a-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a276a-135">DateTimeOffset</span></span>|<span data-ttu-id="a276a-136">Apple プッシュ通知証明書の最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="a276a-136">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="a276a-137">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a276a-137">expirationDateTime</span></span>|<span data-ttu-id="a276a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a276a-138">DateTimeOffset</span></span>|<span data-ttu-id="a276a-139">Apple プッシュ通知証明書の有効期限。</span><span class="sxs-lookup"><span data-stu-id="a276a-139">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="a276a-140">certificateUploadStatus</span><span class="sxs-lookup"><span data-stu-id="a276a-140">certificateUploadStatus</span></span>|<span data-ttu-id="a276a-141">String</span><span class="sxs-lookup"><span data-stu-id="a276a-141">String</span></span>|<span data-ttu-id="a276a-142">証明書のアップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="a276a-142">The certificate upload status.</span></span>|
|<span data-ttu-id="a276a-143">certificateUploadFailureReason</span><span class="sxs-lookup"><span data-stu-id="a276a-143">certificateUploadFailureReason</span></span>|<span data-ttu-id="a276a-144">String</span><span class="sxs-lookup"><span data-stu-id="a276a-144">String</span></span>|<span data-ttu-id="a276a-145">理由の証明書のアップロードに失敗しました。</span><span class="sxs-lookup"><span data-stu-id="a276a-145">The reason the certificate upload failed.</span></span>|
|<span data-ttu-id="a276a-146">証明書</span><span class="sxs-lookup"><span data-stu-id="a276a-146">certificate</span></span>|<span data-ttu-id="a276a-147">String</span><span class="sxs-lookup"><span data-stu-id="a276a-147">String</span></span>|<span data-ttu-id="a276a-148">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="a276a-148">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="a276a-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a276a-149">Relationships</span></span>
<span data-ttu-id="a276a-150">なし</span><span class="sxs-lookup"><span data-stu-id="a276a-150">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a276a-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a276a-151">JSON Representation</span></span>
<span data-ttu-id="a276a-152">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a276a-152">Here is a JSON representation of the resource.</span></span>
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





