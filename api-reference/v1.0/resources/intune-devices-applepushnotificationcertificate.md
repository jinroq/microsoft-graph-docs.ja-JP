---
title: applePushNotificationCertificate リソースの種類
description: Apple プッシュ通知証明書。
author: tfitzmac
ms.openlocfilehash: b5be59f1a6318e07fff981fd32ec6461cb530798
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305440"
---
# <a name="applepushnotificationcertificate-resource-type"></a><span data-ttu-id="f8907-103">applePushNotificationCertificate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f8907-103">applePushNotificationCertificate resource type</span></span>

> <span data-ttu-id="f8907-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f8907-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f8907-105">Apple プッシュ通知証明書。</span><span class="sxs-lookup"><span data-stu-id="f8907-105">Apple push notification certificate.</span></span>
## <a name="methods"></a><span data-ttu-id="f8907-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="f8907-106">Methods</span></span>
|<span data-ttu-id="f8907-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="f8907-107">Method</span></span>|<span data-ttu-id="f8907-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f8907-108">Return Type</span></span>|<span data-ttu-id="f8907-109">説明</span><span class="sxs-lookup"><span data-stu-id="f8907-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f8907-110">Get applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="f8907-110">Get applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-get.md)|[<span data-ttu-id="f8907-111">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="f8907-111">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="f8907-112">[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="f8907-112">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="f8907-113">Update applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="f8907-113">Update applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-update.md)|[<span data-ttu-id="f8907-114">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="f8907-114">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="f8907-115">[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f8907-115">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="f8907-116">downloadApplePushNotificationCertificateSigningRequest 関数</span><span class="sxs-lookup"><span data-stu-id="f8907-116">downloadApplePushNotificationCertificateSigningRequest function</span></span>](../api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest.md)|<span data-ttu-id="f8907-117">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f8907-117">String</span></span>|<span data-ttu-id="f8907-118">Apple プッシュ通知の証明書署名要求をダウンロードします</span><span class="sxs-lookup"><span data-stu-id="f8907-118">Download Apple push notification certificate signing request</span></span>|

## <a name="properties"></a><span data-ttu-id="f8907-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f8907-119">Properties</span></span>
|<span data-ttu-id="f8907-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f8907-120">Property</span></span>|<span data-ttu-id="f8907-121">種類</span><span class="sxs-lookup"><span data-stu-id="f8907-121">Type</span></span>|<span data-ttu-id="f8907-122">説明</span><span class="sxs-lookup"><span data-stu-id="f8907-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8907-123">ID</span><span class="sxs-lookup"><span data-stu-id="f8907-123">id</span></span>|<span data-ttu-id="f8907-124">String</span><span class="sxs-lookup"><span data-stu-id="f8907-124">String</span></span>|<span data-ttu-id="f8907-125">証明書の一意識別子</span><span class="sxs-lookup"><span data-stu-id="f8907-125">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="f8907-126">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="f8907-126">appleIdentifier</span></span>|<span data-ttu-id="f8907-127">String</span><span class="sxs-lookup"><span data-stu-id="f8907-127">String</span></span>|<span data-ttu-id="f8907-128">MDM プッシュ証明書の作成に使用するアカウントの Apple ID。</span><span class="sxs-lookup"><span data-stu-id="f8907-128">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="f8907-129">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="f8907-129">topicIdentifier</span></span>|<span data-ttu-id="f8907-130">String</span><span class="sxs-lookup"><span data-stu-id="f8907-130">String</span></span>|<span data-ttu-id="f8907-131">トピック ID。</span><span class="sxs-lookup"><span data-stu-id="f8907-131">Topic Id.</span></span>|
|<span data-ttu-id="f8907-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f8907-132">lastModifiedDateTime</span></span>|<span data-ttu-id="f8907-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8907-133">DateTimeOffset</span></span>|<span data-ttu-id="f8907-134">Apple プッシュ通知証明書の最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="f8907-134">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="f8907-135">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f8907-135">expirationDateTime</span></span>|<span data-ttu-id="f8907-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8907-136">DateTimeOffset</span></span>|<span data-ttu-id="f8907-137">Apple プッシュ通知証明書の有効期限。</span><span class="sxs-lookup"><span data-stu-id="f8907-137">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="f8907-138">証明書</span><span class="sxs-lookup"><span data-stu-id="f8907-138">certificate</span></span>|<span data-ttu-id="f8907-139">String</span><span class="sxs-lookup"><span data-stu-id="f8907-139">String</span></span>|<span data-ttu-id="f8907-140">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="f8907-140">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="f8907-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f8907-141">Relationships</span></span>
<span data-ttu-id="f8907-142">なし</span><span class="sxs-lookup"><span data-stu-id="f8907-142">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f8907-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f8907-143">JSON Representation</span></span>
<span data-ttu-id="f8907-144">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f8907-144">Here is a JSON representation of the resource.</span></span>
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
  "certificate": "String"
}
```



